# Comparing `tmp/drummachine-0.0.2.tar.gz` & `tmp/drummachine-0.1.3.tar.gz`

## Comparing `drummachine-0.0.2.tar` & `drummachine-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 drummachine-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 drummachine-0.0.2/demos/audio.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 drummachine-0.0.2/demos/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drummachine-0.0.2/src/drummachine/__init__.py
--rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 drummachine-0.0.2/src/drummachine/__main__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 drummachine-0.0.2/src/drummachine/waveforms.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 drummachine-0.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 drummachine-0.0.2/LICENSE
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 drummachine-0.0.2/README.md
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 drummachine-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 drummachine-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 drummachine-0.1.3/MANIFEST.in
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 drummachine-0.1.3/demos/audio.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 drummachine-0.1.3/demos/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drummachine-0.1.3/src/drummachine/__init__.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 drummachine-0.1.3/src/drummachine/__main__.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 drummachine-0.1.3/src/drummachine/waveforms.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 drummachine-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 drummachine-0.1.3/LICENSE
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 drummachine-0.1.3/README.md
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 drummachine-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 drummachine-0.1.3/PKG-INFO
```

### Comparing `drummachine-0.0.2/demos/audio.py` & `drummachine-0.1.3/demos/audio.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.2/demos/ui.py` & `drummachine-0.1.3/demos/ui.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.2/src/drummachine/__main__.py` & `drummachine-0.1.3/src/drummachine/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             if m >= maxy - 1 or n >= maxx - 1:
                 continue
             stdscr.addstr(m, n, ui_grid[m, n], curses.color_pair(instr_color_idx[cidx]) if curses.has_colors() else curses.A_BOLD)
 
     return ui_grid, ui_map
 
 def process_key_press(stdscr, i, j, ui_grid, ui_map, icon, on_indices, tempo_delta_samples = 100):
-    global n_subdiv_samples
+    global n_subdiv_samples, sound_on
     key = stdscr.getch()
     i, j = get_arrow_key_input(key, i, j, ui_map)
     i, j = limit_arrow_key_input(i, j, ui_grid.shape[0]-icon.shape[0], ui_grid.shape[1]-icon.shape[1])
     if key == ord(' '):
         if ui_map[i, j] in on_indices:
             sound_on[np.unravel_index(ui_map[i, j]-1, sound_on.shape)] = 0
             on_indices.remove(ui_map[i, j])
@@ -130,38 +130,45 @@
             on_indices.add(ui_map[i, j])
     elif key == ord('='):
         n_subdiv_samples -= tempo_delta_samples
         if n_subdiv_samples <= 0:
             n_subdiv_samples += 2*tempo_delta_samples
     elif key == ord('-'):
         n_subdiv_samples += tempo_delta_samples
+    elif key == ord('r'):
+        sound_on = np.random.randint(low=0, high=2, size=(n_instruments, single_instrument_layout.count(1)))
     return i, j
 
 def get_indices():
     idx_i, row_idx = 1, 0
     indices = set()
     for row in sound_on:
         indices.update(np.where(row == 1)[0] + idx_i + row_idx)
         row_idx += len(row)
     return indices
 
+def display_help(stdscr, y0):
+    stdscr.addstr(y0 + 1, 0, 'MOVE CURSOR: ← / ↑ / → / ↓')
+    stdscr.addstr(y0 + 2, 0, '(DE)ACTIVATE SOUND: <spacebar>')
+    stdscr.addstr(y0 + 3, 0, 'CHANGE TEMPO: + / -')
+    stdscr.addstr(y0 + 4, 0, 'RANDOM BEAT: R')
+    stdscr.addstr(y0 + 5, 0, 'EXIT: CTRL + C')
+
 def build_ui(stdscr):
     i, j = 0, 0
     icon = get_icon()
-    on_indices = get_indices()
     threading.Thread(target=play_audio).start()
+
     while True:
+        on_indices = get_indices()
         ui_grid, ui_map = draw_grid(stdscr, icon, on_indices, i, j)
         i, j = process_key_press(stdscr, i, j, ui_grid, ui_map, icon, on_indices)
 
         #debug_print(stdscr, sound_on, ui_grid.shape[0] + 5)
-        stdscr.addstr(ui_grid.shape[0] + 1, 0, '(DE)ACTIVATE SOUND: <spacebar>')
-        stdscr.addstr(ui_grid.shape[0] + 2, 0, 'MOVE CURSOR: ← / ↑ / → / ↓')
-        stdscr.addstr(ui_grid.shape[0] + 3, 0, 'CHANGE TEMPO: + / -')
-        stdscr.addstr(ui_grid.shape[0] + 4, 0, 'EXIT: CTRL + C')
+        display_help(stdscr, ui_grid.shape[0])
         stdscr.refresh() # stdscr.erase() # stdscr.clear()
 
 def get_superposition():
     out = np.zeros((sound_on.shape[0], n_subdiv_samples*sound_on.shape[1]))
     for m in range(sound_on.shape[0]):
         for n in range(sound_on.shape[1]):
             if sound_on[m, n] == 1:
@@ -187,15 +194,18 @@
     except KeyError:
         print('no default samplerate available, terminating...')
         sys.exit(0)
 
 def init_colors(stdscr=None):
     curses.use_default_colors()
     for i in range(0, curses.COLORS):
-        curses.init_pair(i + 1, i, -1)
+        try:
+            curses.init_pair(i + 1, i, -1)
+        except ValueError:
+            break
     if stdscr:
         stdscr.nodelay(False)
         for i in range(0, 255):
             stdscr.addstr(f'{i} ', curses.color_pair(i))
         stdscr.getch()
         stdscr.nodelay(True)
         stdscr.erase()
@@ -212,16 +222,15 @@
     except ValueError: # extreme tempo changes
         outdata[:] = np.zeros((frames,1))
 
 n_instruments, n_beats = 4, 4
 instr_color_idx = [14, 4, 11, 7]
 single_instrument_layout = n_beats * [1, 1, 1, 1, 0, 0, 0, 0]
 layout = np.vstack([single_instrument_layout for _ in range(n_instruments)])
-#sound_on = np.zeros((n_instruments, single_instrument_layout.count(1)), dtype=int)
-sound_on = np.random.randint(low=0, high=2, size=(n_instruments, single_instrument_layout.count(1)))
+sound_on = np.zeros((n_instruments, single_instrument_layout.count(1)), dtype=int)
 
 gain = 0.01
 n_channels = 2
 samplerate = get_samplerate()
 stream = sd.OutputStream(channels=n_channels, callback=callback, samplerate=samplerate)
 
 n_subdiv_samples = int(samplerate // 8) # 120 BPM, 16th note subdiv
```

### Comparing `drummachine-0.0.2/src/drummachine/waveforms.py` & `drummachine-0.1.3/src/drummachine/waveforms.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.2/LICENSE` & `drummachine-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.2/pyproject.toml` & `drummachine-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "drummachine"
-version = "0.0.2"
+version = "0.1.3"
 authors = [
   { name="Guitar Dan", email="guitardanuk@gmail.com" },
 ]
 description = "A drum machine package for sequencing waveforms using numpy, curses and the sounddevice module."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drummachine-0.0.2/PKG-INFO` & `drummachine-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drummachine
-Version: 0.0.2
+Version: 0.1.3
 Summary: A drum machine package for sequencing waveforms using numpy, curses and the sounddevice module.
 Project-URL: Homepage, https://github.com/guitardan/realtime-audio
 Project-URL: Bug Tracker, https://github.com/guitardan/realtime-audio/issues
 Author-email: Guitar Dan <guitardanuk@gmail.com>
 License-File: LICENSE
 Keywords: audio,drums,music
 Classifier: Environment :: Console :: Curses
```

