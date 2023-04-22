# Comparing `tmp/drummachine-0.0.1.tar.gz` & `tmp/drummachine-0.0.2.tar.gz`

## Comparing `drummachine-0.0.1.tar` & `drummachine-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 drummachine-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 drummachine-0.0.1/demos/audio.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 drummachine-0.0.1/demos/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drummachine-0.0.1/src/drummachine/__init__.py
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 drummachine-0.0.1/src/drummachine/__main__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 drummachine-0.0.1/src/drummachine/waveforms.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 drummachine-0.0.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 drummachine-0.0.1/LICENSE
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 drummachine-0.0.1/README.md
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 drummachine-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 drummachine-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 drummachine-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 drummachine-0.0.2/demos/audio.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 drummachine-0.0.2/demos/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drummachine-0.0.2/src/drummachine/__init__.py
+-rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 drummachine-0.0.2/src/drummachine/__main__.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 drummachine-0.0.2/src/drummachine/waveforms.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 drummachine-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 drummachine-0.0.2/LICENSE
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 drummachine-0.0.2/README.md
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 drummachine-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 drummachine-0.0.2/PKG-INFO
```

### Comparing `drummachine-0.0.1/demos/audio.py` & `drummachine-0.0.2/demos/audio.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.1/demos/ui.py` & `drummachine-0.0.2/demos/ui.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.1/src/drummachine/__main__.py` & `drummachine-0.0.2/src/drummachine/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,25 @@
 
 def play_audio():
     with stream:
         while True:
             if stream.stopped:
                 break
 
+def get_samplerate():
+    output_device = sd.query_devices(kind='output')
+    try:
+        return output_device['default_samplerate']
+    except TypeError:
+        print('no output device available, terminating...')
+        sys.exit(0)
+    except KeyError:
+        print('no default samplerate available, terminating...')
+        sys.exit(0)
+
 def init_colors(stdscr=None):
     curses.use_default_colors()
     for i in range(0, curses.COLORS):
         curses.init_pair(i + 1, i, -1)
     if stdscr:
         stdscr.nodelay(False)
         for i in range(0, 255):
@@ -206,15 +217,15 @@
 single_instrument_layout = n_beats * [1, 1, 1, 1, 0, 0, 0, 0]
 layout = np.vstack([single_instrument_layout for _ in range(n_instruments)])
 #sound_on = np.zeros((n_instruments, single_instrument_layout.count(1)), dtype=int)
 sound_on = np.random.randint(low=0, high=2, size=(n_instruments, single_instrument_layout.count(1)))
 
 gain = 0.01
 n_channels = 2
-samplerate = sd.query_devices('output')['default_samplerate']
+samplerate = get_samplerate()
 stream = sd.OutputStream(channels=n_channels, callback=callback, samplerate=samplerate)
 
 n_subdiv_samples = int(samplerate // 8) # 120 BPM, 16th note subdiv
 waveforms = [
     wfs.get_kick(),
     wfs.get_snare(Fs=samplerate),
     wfs.get_hihat(),
```

### Comparing `drummachine-0.0.1/src/drummachine/waveforms.py` & `drummachine-0.0.2/src/drummachine/waveforms.py`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.1/LICENSE` & `drummachine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drummachine-0.0.1/pyproject.toml` & `drummachine-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "drummachine"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Guitar Dan", email="guitardanuk@gmail.com" },
 ]
 description = "A drum machine package for sequencing waveforms using numpy, curses and the sounddevice module."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drummachine-0.0.1/PKG-INFO` & `drummachine-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drummachine
-Version: 0.0.1
+Version: 0.0.2
 Summary: A drum machine package for sequencing waveforms using numpy, curses and the sounddevice module.
 Project-URL: Homepage, https://github.com/guitardan/realtime-audio
 Project-URL: Bug Tracker, https://github.com/guitardan/realtime-audio/issues
 Author-email: Guitar Dan <guitardanuk@gmail.com>
 License-File: LICENSE
 Keywords: audio,drums,music
 Classifier: Environment :: Console :: Curses
```

