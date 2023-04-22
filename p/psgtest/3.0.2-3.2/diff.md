# Comparing `tmp/psgtest-3.0.2.tar.gz` & `tmp/psgtest-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psgtest-3.0.2.tar", last modified: Fri Apr 21 11:21:40 2023, max compression
+gzip compressed data, was "dist\psgtest-3.2.tar", last modified: Sat Apr 22 14:35:21 2023, max compression
```

## Comparing `psgtest-3.0.2.tar` & `psgtest-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:21:40.000000 psgtest-3.0.2/
--rw-rw-rw-   0        0        0     8172 2023-04-21 11:21:40.000000 psgtest-3.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 11:21:40.000000 psgtest-3.0.2/psgtest/
--rw-rw-rw-   0        0        0    39473 2023-04-21 11:20:24.000000 psgtest-3.0.2/psgtest/psgtest.py
--rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-3.0.2/psgtest/psgtest_icon.ico
--rw-rw-rw-   0        0        0    20186 2021-10-30 20:48:11.000000 psgtest-3.0.2/psgtest/psgtest_icon.png
--rw-rw-rw-   0        0        0       23 2021-11-12 18:21:37.000000 psgtest-3.0.2/psgtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:21:40.000000 psgtest-3.0.2/psgtest.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     8172 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       27 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0      295 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 11:21:39.000000 psgtest-3.0.2/psgtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6056 2023-04-21 10:47:58.000000 psgtest-3.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 11:21:40.000000 psgtest-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1483 2023-04-21 11:21:17.000000 psgtest-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:35:21.000000 psgtest-3.2/
+-rw-rw-rw-   0        0        0     8368 2023-04-22 14:35:21.000000 psgtest-3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest/
+-rw-rw-rw-   0        0        0    40591 2023-04-22 14:27:57.000000 psgtest-3.2/psgtest/psgtest.py
+-rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-3.2/psgtest/psgtest_icon.ico
+-rw-rw-rw-   0        0        0    20186 2021-10-30 20:48:11.000000 psgtest-3.2/psgtest/psgtest_icon.png
+-rw-rw-rw-   0        0        0       23 2021-11-12 18:21:37.000000 psgtest-3.2/psgtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     8368 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      295 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6206 2023-04-22 14:29:57.000000 psgtest-3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:35:21.000000 psgtest-3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1481 2023-04-22 14:29:57.000000 psgtest-3.2/setup.py
```

### Comparing `psgtest-3.0.2/PKG-INFO` & `psgtest-3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 3.0.2
+Version: 3.2
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
           <img src="https://raw.githubusercontent.com/PySimpleGUI/PySimpleGUI/master/images/for_readme/Logo%20with%20text%20for%20GitHub%20Top.png" alt="Python GUIs for Humans">
           <h2 align="center">psgtest</h2>
           <h2 align="center">Simple Python Testing</h2>
         </p>
         
         Run your Python programs using the interpreter version of your choice, and display the output in a GUI window.
         
-        ![example](https://raw.githubusercontent.com/PySimpleGUI/psgtest/main/images_for_readme/psgtest_example.gif?token=ALAGMY7OEDZBCYVS7LEZP33BRUQGC)
+        ![psgtest 3 0](https://user-images.githubusercontent.com/46163555/233642958-730f19f0-43a9-4bea-833e-9524c2d770ff.gif)
+        
         
         ## Installation
         
         ### Old-school Straight Pip
         
         pip install psgtest
         
@@ -82,20 +83,25 @@
         You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
         
         Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
         
         
         ## Release Notes
         
+        ### 3.2   22-Apr-2023
+        
+        - Added piped output for regression testing
+        - Added cleanup of processes when exiting. If any processes are running, they will be killed.
+        
         ### 3.0   21-Apr-2023
         
-        Greatly expanded the Regression test features
-        Made regression multi-threaded
-        Added testing across all Python interpreters
-        Removed direct calls to Python Thread module and using only PySimpleGUI supplied calls
+        - Greatly expanded the Regression test features
+        - Made regression multi-threaded
+        - Added testing across all Python interpreters
+        - Removed direct calls to Python Thread module and using only PySimpleGUI supplied calls
         
         
         ### 1.13.0
         
         * Run all Interpreters feature added
         
         ### 1.12.0
```

### Comparing `psgtest-3.0.2/psgtest/psgtest.py` & `psgtest-3.2/psgtest/psgtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,40 @@
 import sys
 import subprocess
 import PySimpleGUI as sg
 import time
 import psutil
 import signal
 
-version = '3.0'
+version = '3.2'
 
 """
                              dP                       dP   
                              88                       88   
 88d888b. .d8888b. .d8888b. d8888P .d8888b. .d8888b. d8888P 
 88'  `88 Y8ooooo. 88'  `88   88   88ooood8 Y8ooooo.   88   
 88.  .88       88 88.  .88   88   88.  ...       88   88   
 88Y888P' `88888P' `8888P88   dP   `88888P' `88888P'   dP   
 88                     .88                                 
 dP                 d8888P
 
 
 3.0 21-Apr-2023 - Expanded regression tests. Now works correctly. Added ability to run across all interpreters. Made regression threaded.
+3.1 21-Apr-2023 - Removed "Edit Me" button. Instead you should use the right-click Edit Me that is standard in PySimpleGUI utilities
+3.2 23-Apr-2023 - Added piped output for Regression Tests - now creates tabs for tests when running regression and will keep open any that fail
+                  Added cleaning up of all potentially running processes upon exit. Makes quitting with lots of tests running MUCH easier since don't have to manually kill them
 
     Copyright 2021, 2022, 2023 PySimpleGUI
 """
 
 
 DEFAULT_OUTPUT_SIZE = (80,5)
 file_list_dict = {}
+sp_to_mline_dict = {}
+sp_to_filename = {}
 
 '''
 M""MMMMM""MM          dP                               MM""""""""`M                                     
 M  MMMMM  MM          88                               MM  mmmmmmmM                                     
 M         `M .d8888b. 88 88d888b. .d8888b. 88d888b.    M'      MMMM dP    dP 88d888b. .d8888b. .d8888b. 
 M  MMMMM  MM 88ooood8 88 88'  `88 88ooood8 88'  `88    MM  MMMMMMMM 88    88 88'  `88 88'  `"" Y8ooooo. 
 M  MMMMM  MM 88.  ... 88 88.  .88 88.  ... 88          MM  MMMMMMMM 88.  .88 88    88 88.  ...       88 
@@ -140,29 +145,32 @@
 MMMM  MMMM 88d888b. 88d888b. .d8888b. .d8888b. .d888b88 
 MMMM  MMMM 88'  `88 88'  `88 88ooood8 88'  `88 88'  `88 
 MMMM  MMMM 88    88 88       88.  ... 88.  .88 88.  .88 
 MMMM  MMMM dP    dP dP       `88888P' `88888P8 `88888P8 
 MMMMMMMMMM
 '''
 
-def the_thread(window: sg.Window, sp: subprocess.Popen):
+def piped_output_thread(window: sg.Window, sp: subprocess.Popen, regression=False):
     """
     The thread that's used to run the subprocess so that the GUI can continue and the stdout/stderror is collected
 
     :param window:
     :param sp:
     :return:
     """
 
     window.write_event_value('-THREAD-', (sp, '===THEAD STARTING==='))
     window.write_event_value('-THREAD-', (sp, '----- STDOUT & STDERR Follows ----'))
     for line in sp.stdout:
         oline = line.decode().rstrip()
         window.write_event_value('-THREAD-', (sp, oline))
-    window.write_event_value('-THREAD-', (sp, '===THEAD DONE==='))
+    if regression:
+        window.write_event_value('-THREAD-', (sp, '===THEAD DONE REGRESSION==='))
+    else:
+        window.write_event_value('-THREAD-', (sp, '===THEAD DONE==='))
 
 
 
 
 '''
 MM"""""""`YM                                                       
 MM  mmmmm  M                                                       
@@ -235,21 +243,17 @@
 MMMM  MMMM `88888P' `88888P'   dP   `88888P' 
 MMMMMMMMMM
 '''
 
 
 
 
-def regression_thread(window:sg.Window, program_list, block_size, iterations, kill_after=None, interpreter_path=None):
-    # tcprint(window, f'Regression starting.  window = {window}\n' +
-    #       f'program_list = {program_list}\n' +
-    #       f'block_size = {block_size}\n' +
-    #       f'iterations = {iterations}\n' +
-    #       f'kill_after = {kill_after}\n' +
-    #       f'interpreter = {interpreter_path}')
+def regression_thread(window:sg.Window, program_list, block_size, iterations, kill_after=None, interpreter_path=None, pipe_output=False):
+    global sp_to_mline_dict, sp_to_filename
+
     tcprint(window , f"-------- Start Regression using {interpreter_path} --------", colors='white on green')
     block_count = 0
     if interpreter_path is not None:
         interpreter_paths = [interpreter_path, ]
     else:
         interpreter_paths = []
         for interpreter in interpreter_dict.values():
@@ -258,15 +262,28 @@
                 interpreter_paths.append(ipath)
     for interpreter_path in interpreter_paths:
         tcprint(window, f'Testing interpreter {interpreter_path}', colors='white on blue')
         for iteration in range(iterations):
             tcprint(window, f'Starting Iteration Number {iteration}', 'white on red')
             for file, file_to_run in get_next_program(program_list):
                 tcprint(window, f'Starting {file_to_run}', 'white on purple')
-                sp = sg.execute_command_subprocess(interpreter_path, f'"{file_to_run}"', pipe_output=True)
+                sp = sg.execute_command_subprocess(interpreter_path, f'"{file_to_run}"', pipe_output=pipe_output)
+                if pipe_output:
+                    sp_to_filename[sp] = file
+                    mline_key = f'{file}-MLINE-'
+                    if mline_key not in sp_to_mline_dict.values():
+                        tab = make_output_tab(file, mline_key, file)
+                        window['-TABGROUP-'].add_tab(tab)
+                    else:
+                        if not window[file].visible:
+                            window[file].update(visible=True)
+                    sp_to_mline_dict[sp] = mline_key
+                    window[file].select()
+                    window.start_thread(lambda: piped_output_thread(window, sp, regression=True), '-PIPE THREAD DONE-')
+
                 if kill_after is not None:
                     window.timer_start(kill_after * 1000, ('-TIMER THREAD-', sp), repeating=False)
                     if (block_count+1) % block_size == 0:
                         time.sleep(kill_after)
                 block_count += 1
     tcprint(window , f"-------- DONE WITH REGRESSION TEST -------", colors='white on green')
 
@@ -452,15 +469,15 @@
         [sg.Multiline(
             size=(sg.user_settings_get_entry('-output width-', DEFAULT_OUTPUT_SIZE[0]), sg.user_settings_get_entry('-output height-', DEFAULT_OUTPUT_SIZE[1])),
             write_only=True, key='-ML-', reroute_stdout=False, reroute_stderr=False, echo_stdout_stderr=False, reroute_cprint=True, auto_refresh=True,
             expand_x=True, expand_y=True, font=sg.user_settings_get_entry('-output font-', 'Courier 10'))],
         [sg.B('Copy To Clipboard', key=('-COPY-', '-ML-')), sg.B('Clear', k=('-CLEAR-', '-ML-'))]]
 
     bottom_right = [
-        [sg.Button('Edit Me (this program)'), sg.B('Settings'), sg.Button('Exit')],
+        [sg.B('Settings'), sg.Button('Exit')],
         [sg.T('psgtest ver ' + version + '   PySimpleGUI ver ' + sg.version.split(' ')[0] + '  tkinter ver ' + sg.tclversion_detailed, font='Default 8', pad=(0, 0))],
         [sg.T('Python ver ' + sys.version, font='Default 8', pad=(0, 0))]]
 
     # tab1 = sg.Tab('Output',old_right_col, k='-TAB1-',  expand_x=True, expand_y=True)
     tab1 = sg.Tab('Output', output_tab_layout, k='-TAB1-', )
 
     tab_group = sg.TabGroup([[tab1, ]], k='-TABGROUP-', expand_x=True, expand_y=True, font='_ 8', tab_location='topleft')
@@ -468,16 +485,14 @@
 
     right_col = [[tab_group]] + bottom_right
     choose_folder_at_top = sg.pin(sg.Column([[sg.T('Click settings to set top of your tree or choose a previously chosen folder'),
                                               sg.Combo(sorted(sg.user_settings_get_entry('-folder names-', [])),
                                                        default_value=sg.user_settings_get_entry('-test script folder-', ''), size=(50, 30), key='-FOLDERNAME-',
                                                        enable_events=True, readonly=True)]], pad=(0, 0), k='-FOLDER CHOOSE-', expand_x=True, expand_y=True))
 
-    # interpreter_list = sorted(list(interpreter_dict.keys()))
-    # interpreter_keys = sorted(list(interpreter_dict.values()))
     interpreter_list = []
     for key, value in interpreter_dict.items():
         if sg.user_settings_get_entry(value, ''):
             interpreter_list.append(key)
 
     interpreter_list = sorted(interpreter_list)
     if len(interpreter_list) == 0:  # no interpreters found in settings file, so set one using the currently running version of Python
@@ -535,15 +550,15 @@
 '''
 
 def main():
     """
     The main program that contains the event loop.
     It will call the make_window function to create the window.
     """
-    global file_list_dict
+    global file_list_dict, sp_to_mline_dict, sp_to_filename
 
 
 
     def start_batch(list_of_programs, interpreter=None):
         if interpreter is None:
             current_interpreter = sg.user_settings_get_entry('-current interpreter-')
             if current_interpreter != values['-INTERPRETER TOP-']:
@@ -579,16 +594,15 @@
                 if not window[file].visible:
                     window[file].update(visible=True)
             sp_to_mline_dict[sp] = mline_key
             window[file].select()
             # Let a thread handle getting all the output so that the rest of the GUI keep running
 
             if pipe_output:
-                window.start_thread(lambda: the_thread(window, sp), '-PIPE THREAD DONE-')
-                # threading.Thread(target=the_thread, args=(window, sp), daemon=True).start()
+                window.start_thread(lambda: piped_output_thread(window, sp), '-PIPE THREAD DONE-')
                 if values['-REGRESSION KILL-']:
                     try:
                         seconds = float(values['-REGRESSION SECONDS-'])
                     except:
                         seconds = 15
                     window.timer_start(seconds*1000, ('-TIMER THREAD-',  sp), repeating=False)
 
@@ -604,16 +618,14 @@
             sg.user_settings_delete_filename(filename='psgtest.json')
             sg.popup_auto_close('Settings file deleted... please restart the program')
             exit()
         else:
             sg.popup_auto_close('Cancelling operation... See what you can do about the problem...')
             exit()
     window['-FILTER NUMBER-'].update(f'{len(file_list)} files')
-    sp_to_mline_dict = {}
-    sp_to_filename = {}
     counter = 0
     dont_close_tab = {}
     regression_programs = []
     try:
         while True:
             event, values = window.read()
             # print(event, values)
@@ -733,28 +745,35 @@
                 else:
                     regression_programs = values['-DEMO LIST-']
                 # start the first batch
                 if values['-REGRESSION KILL-']:
                     kill_after = int(values['-REGRESSION SECONDS-'])
                 else:
                     kill_after = None
-                window.start_thread(lambda: regression_thread(window, regression_programs, int(values['-REGRESSION BLOCK SIZE-']), int(values['-STRESS RUNS-']), kill_after,  sg.user_settings_get_entry('-interpreter path-', '')), '-DONE-')
+                window.start_thread(lambda: regression_thread(window, regression_programs, int(values['-REGRESSION BLOCK SIZE-']), int(values['-STRESS RUNS-']), kill_after,  sg.user_settings_get_entry('-interpreter path-', ''), values['-SHOW OUTPUT-']), '-DONE-')
             elif event == 'Run Regression All Interpreters':
                 if values['-SINGLE FILE-']:
                     regression_programs = [values['-SINGLE FILE-'],]
                 else:
                     regression_programs = values['-DEMO LIST-']
                 # start the first batch
                 if values['-REGRESSION KILL-']:
                     kill_after = int(values['-REGRESSION SECONDS-'])
                 else:
                     kill_after = None
-                window.start_thread(lambda: regression_thread(window, regression_programs, int(values['-REGRESSION BLOCK SIZE-']), int(values['-STRESS RUNS-']), kill_after,  None), '-DONE-')
+                window.start_thread(lambda: regression_thread(window, regression_programs, int(values['-REGRESSION BLOCK SIZE-']), int(values['-STRESS RUNS-']), kill_after,  None, values['-SHOW OUTPUT-']), '-DONE-')
     except Exception as e:
         sg.Print('WHOA!  Exception in the main event loop', e, wait=True)
+        sg.popup_error_with_traceback('Exception in event loop', e)
+
+    # clean up any tests that are still running
+    for sp in sp_to_filename.keys():
+        print(f'Clean-up killing {sp.pid}')
+        kill_proc_tree(sp.pid)
+
     window.close()
 
 
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `psgtest-3.0.2/psgtest/psgtest_icon.ico` & `psgtest-3.2/psgtest/psgtest_icon.ico`

 * *Files identical despite different names*

### Comparing `psgtest-3.0.2/psgtest/psgtest_icon.png` & `psgtest-3.2/psgtest/psgtest_icon.png`

 * *Files identical despite different names*

### Comparing `psgtest-3.0.2/psgtest.egg-info/PKG-INFO` & `psgtest-3.2/psgtest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 3.0.2
+Version: 3.2
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
           <img src="https://raw.githubusercontent.com/PySimpleGUI/PySimpleGUI/master/images/for_readme/Logo%20with%20text%20for%20GitHub%20Top.png" alt="Python GUIs for Humans">
           <h2 align="center">psgtest</h2>
           <h2 align="center">Simple Python Testing</h2>
         </p>
         
         Run your Python programs using the interpreter version of your choice, and display the output in a GUI window.
         
-        ![example](https://raw.githubusercontent.com/PySimpleGUI/psgtest/main/images_for_readme/psgtest_example.gif?token=ALAGMY7OEDZBCYVS7LEZP33BRUQGC)
+        ![psgtest 3 0](https://user-images.githubusercontent.com/46163555/233642958-730f19f0-43a9-4bea-833e-9524c2d770ff.gif)
+        
         
         ## Installation
         
         ### Old-school Straight Pip
         
         pip install psgtest
         
@@ -82,20 +83,25 @@
         You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
         
         Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
         
         
         ## Release Notes
         
+        ### 3.2   22-Apr-2023
+        
+        - Added piped output for regression testing
+        - Added cleanup of processes when exiting. If any processes are running, they will be killed.
+        
         ### 3.0   21-Apr-2023
         
-        Greatly expanded the Regression test features
-        Made regression multi-threaded
-        Added testing across all Python interpreters
-        Removed direct calls to Python Thread module and using only PySimpleGUI supplied calls
+        - Greatly expanded the Regression test features
+        - Made regression multi-threaded
+        - Added testing across all Python interpreters
+        - Removed direct calls to Python Thread module and using only PySimpleGUI supplied calls
         
         
         ### 1.13.0
         
         * Run all Interpreters feature added
         
         ### 1.12.0
```

### Comparing `psgtest-3.0.2/README.md` & `psgtest-3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,16 @@
   <img src="https://raw.githubusercontent.com/PySimpleGUI/PySimpleGUI/master/images/for_readme/Logo%20with%20text%20for%20GitHub%20Top.png" alt="Python GUIs for Humans">
   <h2 align="center">psgtest</h2>
   <h2 align="center">Simple Python Testing</h2>
 </p>
 
 Run your Python programs using the interpreter version of your choice, and display the output in a GUI window.
 
-![example](https://raw.githubusercontent.com/PySimpleGUI/psgtest/main/images_for_readme/psgtest_example.gif?token=ALAGMY7OEDZBCYVS7LEZP33BRUQGC)
+![psgtest 3 0](https://user-images.githubusercontent.com/46163555/233642958-730f19f0-43a9-4bea-833e-9524c2d770ff.gif)
+
 
 ## Installation
 
 ### Old-school Straight Pip
 
 pip install psgtest
 
@@ -74,20 +75,25 @@
 You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
 
 Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
 
 
 ## Release Notes
 
+### 3.2   22-Apr-2023
+
+- Added piped output for regression testing
+- Added cleanup of processes when exiting. If any processes are running, they will be killed.
+
 ### 3.0   21-Apr-2023
 
-Greatly expanded the Regression test features
-Made regression multi-threaded
-Added testing across all Python interpreters
-Removed direct calls to Python Thread module and using only PySimpleGUI supplied calls
+- Greatly expanded the Regression test features
+- Made regression multi-threaded
+- Added testing across all Python interpreters
+- Removed direct calls to Python Thread module and using only PySimpleGUI supplied calls
 
 
 ### 1.13.0
 
 * Run all Interpreters feature added
 
 ### 1.12.0
```

### Comparing `psgtest-3.0.2/setup.py` & `psgtest-3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             return f.read()
     except IOError:
         return ''
 
 
 setuptools.setup(
     name="psgtest",
-    version="3.0.2",
+    version="3.2",
     author="PySimpleGUI",
     author_email="PySimpleGUI@PySimpleGUI.org",
     description="Run your Python programs, capture the output, using your choice of interpreters",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/PySimpleGUI/psgtest",
     packages=['psgtest'],
```

