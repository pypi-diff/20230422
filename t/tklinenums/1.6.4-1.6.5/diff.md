# Comparing `tmp/tklinenums-1.6.4.tar.gz` & `tmp/tklinenums-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.6.4.tar", last modified: Sat Apr 22 01:22:08 2023, max compression
+gzip compressed data, was "tklinenums-1.6.5.tar", last modified: Sat Apr 22 19:07:28 2023, max compression
```

## Comparing `tklinenums-1.6.4.tar` & `tklinenums-1.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:22:08.842734 tklinenums-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-22 01:22:08.842734 tklinenums-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-22 01:21:48.000000 tklinenums-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 01:21:48.000000 tklinenums-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 01:22:08.842734 tklinenums-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-22 01:21:48.000000 tklinenums-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:22:08.842734 tklinenums-1.6.4/tklinenums/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 01:21:48.000000 tklinenums-1.6.4/tklinenums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-04-22 01:21:48.000000 tklinenums-1.6.4/tklinenums/tklinenums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 01:22:08.842734 tklinenums-1.6.4/tklinenums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 01:22:08.000000 tklinenums-1.6.4/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:07:28.629502 tklinenums-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-22 19:07:28.629502 tklinenums-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-22 19:07:08.000000 tklinenums-1.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 19:07:08.000000 tklinenums-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:07:28.629502 tklinenums-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-22 19:07:08.000000 tklinenums-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:07:28.629502 tklinenums-1.6.5/tklinenums/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:07:08.000000 tklinenums-1.6.5/tklinenums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-22 19:07:08.000000 tklinenums-1.6.5/tklinenums/tklinenums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:07:28.629502 tklinenums-1.6.5/tklinenums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.6.4/PKG-INFO` & `tklinenums-1.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.4
+Version: 1.6.5
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
 <h1 align="center">TkLineNums</h1>
 
 > **Note**
-> If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or `sudo apt-get install python-tk`. Linux machines have plenty of variations for installation as is documented [here](https://www.geeksforgeeks.org/how-to-install-tkinter-on-linux/#:~:text=For%20Debian%2Dbased%20Linux%3A).
+> If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or with the distro package manager on Linux as documented [here](https://tecadmin.net/how-to-install-python-tkinter-on-linux/).
 
 ## Description
 `TkLineNums` is a simple line numbering widget for Python's `tkinter` GUI library. It is directly connects to a `Text` widget and even supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features of the `TkLineNums` widget:
```

### Comparing `tklinenums-1.6.4/README.md` & `tklinenums-1.6.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">TkLineNums</h1>
 
 > **Note**
-> If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or `sudo apt-get install python-tk`. Linux machines have plenty of variations for installation as is documented [here](https://www.geeksforgeeks.org/how-to-install-tkinter-on-linux/#:~:text=For%20Debian%2Dbased%20Linux%3A).
+> If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or with the distro package manager on Linux as documented [here](https://tecadmin.net/how-to-install-python-tkinter-on-linux/).
 
 ## Description
 `TkLineNums` is a simple line numbering widget for Python's `tkinter` GUI library. It is directly connects to a `Text` widget and even supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features of the `TkLineNums` widget:
```

### Comparing `tklinenums-1.6.4/tklinenums/tklinenums.py` & `tklinenums-1.6.5/tklinenums/tklinenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.bind("<Button-1>", self.click_see, add=True)
         self.bind("<ButtonRelease-1>", self.unclick, add=True)
         self.bind("<Double-Button-1>", self.double_click, add=True)
         self.bind("<Button1-Motion>", self.drag, add=True)
         self.bind("<Button1-Leave>", self.auto_scroll, add=True)
 
         # Set the yscrollcommand of the text widget to redraw the widget
-        text["yscrollcommand"] = self.redraw
+        editor["yscrollcommand"] = self.redraw
 
     def redraw(self, *args) -> None:
         """Redraws the widget"""
         # Resize the widget based on the number of lines in the editor
         self.resize()
 
         # Delete all the old line numbers
@@ -229,15 +229,15 @@
         ) <= 1000 else self.config(width=temp_font.measure(f" {end} "))
 
     def set_to_ttk_style(self) -> None:
         """Sets the widget to the ttk style"""
 
         # Set the background and foreground to the ttk style
         self["bg"] = self.tk.eval("ttk::style lookup TLineNumbers -background")
-        self["fg"] = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
+        self.foreground = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
 
     def reload(self) -> None:
         """Reloads the widget"""
         self.set_to_ttk_style()
         self.redraw()
```

### Comparing `tklinenums-1.6.4/tklinenums.egg-info/PKG-INFO` & `tklinenums-1.6.5/tklinenums.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.4
+Version: 1.6.5
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
 <h1 align="center">TkLineNums</h1>
 
 > **Note**
-> If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or `sudo apt-get install python-tk`. Linux machines have plenty of variations for installation as is documented [here](https://www.geeksforgeeks.org/how-to-install-tkinter-on-linux/#:~:text=For%20Debian%2Dbased%20Linux%3A).
+> If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or with the distro package manager on Linux as documented [here](https://tecadmin.net/how-to-install-python-tkinter-on-linux/).
 
 ## Description
 `TkLineNums` is a simple line numbering widget for Python's `tkinter` GUI library. It is directly connects to a `Text` widget and even supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features of the `TkLineNums` widget:
```

