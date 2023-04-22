# Comparing `tmp/tksheet-5.6.8.tar.gz` & `tmp/tksheet-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-5.6.8.tar", last modified: Thu Apr  6 11:14:57 2023, max compression
+gzip compressed data, was "tksheet-6.0.0.tar", last modified: Sat Apr 22 18:12:28 2023, max compression
```

## Comparing `tksheet-5.6.8.tar` & `tksheet-6.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 11:14:57.345203 tksheet-5.6.8/
--rw-rw-rw-   0        0        0     1087 2023-03-26 15:09:51.000000 tksheet-5.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2172 2023-04-06 11:14:57.345203 tksheet-5.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     1522 2023-04-02 17:10:11.000000 tksheet-5.6.8/README.md
--rw-rw-rw-   0        0        0       86 2023-04-06 11:14:57.345203 tksheet-5.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-03 13:47:11.000000 tksheet-5.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 11:14:57.329577 tksheet-5.6.8/tksheet/
--rw-rw-rw-   0        0        0      317 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/__init__.py
--rw-rw-rw-   0        0        0   146851 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0    96382 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0   314198 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    11669 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0    96245 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5666 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    51924 2023-04-06 07:31:37.000000 tksheet-5.6.8/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-04-06 11:14:57.345203 tksheet-5.6.8/tksheet.egg-info/
--rw-rw-rw-   0        0        0     2172 2023-04-06 11:14:57.000000 tksheet-5.6.8/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-06 11:14:57.000000 tksheet-5.6.8/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 11:14:57.000000 tksheet-5.6.8/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 11:14:57.000000 tksheet-5.6.8/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 18:12:28.041739 tksheet-6.0.0/
+-rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2882 2023-04-22 18:12:28.041739 tksheet-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2232 2023-04-18 08:24:22.000000 tksheet-6.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-22 18:12:28.041739 tksheet-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-04-06 11:16:22.000000 tksheet-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:12:28.026112 tksheet-6.0.0/tksheet/
+-rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.0/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   154985 2023-04-22 17:48:29.000000 tksheet-6.0.0/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   100042 2023-04-22 17:24:51.000000 tksheet-6.0.0/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0    10066 2023-04-22 08:55:16.000000 tksheet-6.0.0/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   326370 2023-04-22 16:43:14.000000 tksheet-6.0.0/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12894 2023-04-21 17:11:16.000000 tksheet-6.0.0/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0    99701 2023-04-22 17:25:19.000000 tksheet-6.0.0/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5642 2023-04-20 08:50:10.000000 tksheet-6.0.0/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    52264 2023-04-22 08:42:39.000000 tksheet-6.0.0/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:12:28.041739 tksheet-6.0.0/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     2882 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 18:12:28.000000 tksheet-6.0.0/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-5.6.8/PKG-INFO` & `tksheet-6.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,47 @@
-Metadata-Version: 2.1
-Name: tksheet
-Version: 5.6.8
-Summary: Tkinter table / sheet widget
-Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/5.6.8.tar.gz
-Author: ragardner
-Author-email: github@ragardner.simplelogin.com
-License: MIT
-Keywords: tkinter,table,widget,sheet,grid,tk
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+# **tksheet** [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
-# tksheet [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
+## **Python tkinter table widget**
 
+----
 
-Python tkinter table widget
-
-```
+```python
+#To install using pip
 pip install tksheet
-```
-```
+
+#To update using pip
 pip install tksheet --upgrade
 ```
 
-### Help
- - [Documentation](https://github.com/ragardner/tksheet/wiki)
- - [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-
-### Features
- - Display and modify tabular data
- - Stores its display data as a Python list of lists, sublists being rows
- - Runs smoothly even with millions of rows/columns
- - Edit cells directly
- - Drag and drop columns and rows
- - Multiple line headers and rows
- - Expand row heights and column widths
- - Change fonts and font size
- - Change any colors in the sheet
- - Create an unlimited number of high performance dropdown and check boxes
- - Left `"w"`, Center `"center"` or Right `"e"` text alignment
- - Cell values can be any class with a `str` method
+## **Help**
+----
+- [Documentation](https://github.com/ragardner/tksheet/wiki)
+- [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
+- [Questions](https://github.com/ragardner/tksheet/wiki#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki#contributing).
+
+## **Features**
+----
+- Display and modify tabular data
+- Stores its display data as a Python list of lists, sublists being rows
+- Runs smoothly even with millions of rows/columns
+- Edit cells directly
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
+- Drag and drop columns and rows
+- Multiple line header and index cells
+- Expand row heights and column widths
+- Change fonts and font size (not for individual cells)
+- Change any colors in the sheet
+- Create an unlimited number of high performance dropdown and check boxes
+- Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
-### Light Blue Theme
+### **light blue theme**
+----
 
 ![alt text](https://i.imgur.com/ojU3IQi.jpeg)
 
-### Dark Theme
+### **black theme**
+----
 
-![alt text](https://i.imgur.com/JeF9vJe.jpeg)
+![alt text](https://i.imgur.com/JeF9vJe.jpeg)
```

### Comparing `tksheet-5.6.8/setup.py` & `tksheet-6.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '5.6.8',
+  version = '6.0.0',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/5.6.8.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.0.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet.py` & `tksheet-6.0.0/tksheet/_tksheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ._tksheet_vars import *
+from ._tksheet_formatters import *
 from ._tksheet_other_classes import *
 from ._tksheet_top_left_rectangle import *
 from ._tksheet_column_headers import *
 from ._tksheet_row_index import *
 from ._tksheet_main_table import *
 
 from collections import deque
@@ -22,22 +23,25 @@
                  show_y_scrollbar: bool = True,
                  width: int = None,
                  height: int = None,
                  headers: list = None,
                  header: list = None,
                  default_header: str = "letters", #letters, numbers or both
                  default_row_index: str = "numbers", #letters, numbers or both
+                 to_clipboard_delimiter = "\t",
+                 to_clipboard_quotechar = '"',
+                 to_clipboard_lineterminator = "\n",
+                 from_clipboard_delimiters = ["\t"],
                  show_default_header_for_empty: bool = True,
                  show_default_index_for_empty: bool = True,
                  page_up_down_select_row: bool = True,
                  expand_sheet_if_paste_too_big: bool = False,
                  paste_insert_column_limit: int = None,
                  paste_insert_row_limit: int = None,
                  show_dropdown_borders: bool = False,
-                 ctrl_keys_over_dropdowns_enabled: bool = False,
                  arrow_key_down_right_scroll_page: bool = False,
                  enable_edit_cell_auto_resize: bool = True,
                  edit_cell_validation: bool = True,
                  data_reference: list = None,
                  data: list = None,
                  startup_select: tuple = None, #either (start row, end row, "rows"), (start column, end column, "rows") or (cells start row, cells start column, cells end row, cells end column, "cells")
                  startup_focus: bool = True,
@@ -185,22 +189,25 @@
                             show_header = show_header,
                             enable_edit_cell_auto_resize = enable_edit_cell_auto_resize,
                             edit_cell_validation = edit_cell_validation,
                             page_up_down_select_row = page_up_down_select_row,
                             expand_sheet_if_paste_too_big = expand_sheet_if_paste_too_big,
                             paste_insert_column_limit = paste_insert_column_limit,
                             paste_insert_row_limit = paste_insert_row_limit,
-                            ctrl_keys_over_dropdowns_enabled = ctrl_keys_over_dropdowns_enabled,
                             show_dropdown_borders = show_dropdown_borders,
                             arrow_key_down_right_scroll_page = arrow_key_down_right_scroll_page,
                             display_selected_fg_over_highlights = display_selected_fg_over_highlights,
                             show_vertical_grid = show_vertical_grid,
                             show_horizontal_grid = show_horizontal_grid,
                             column_width = column_width,
                             row_height = row_height,
+                            to_clipboard_delimiter = to_clipboard_delimiter,
+                            to_clipboard_quotechar = to_clipboard_quotechar,
+                            to_clipboard_lineterminator = to_clipboard_lineterminator,
+                            from_clipboard_delimiters = from_clipboard_delimiters,
                             column_headers_canvas = self.CH,
                             row_index_canvas = self.RI,
                             headers = headers,
                             header = header,
                             header_height = header_height,
                             data_reference = data if data_reference is None else data_reference,
                             total_cols = total_columns,
@@ -864,15 +871,15 @@
         if canvas_positions:
             if any(x - z < self.MT.min_cw or not isinstance(x, int) or isinstance(x, bool) for z, x in zip(islice(column_widths, 0, None), islice(column_widths, 1, None))):
                 return False
         elif not canvas_positions:
             if any(z < self.MT.min_cw or not isinstance(z, int) or isinstance(z, bool) for z in column_widths):
                 return False
         return True
-            
+
     def default_row_height(self, height = None):
         if height is not None:
             self.MT.default_rh = (height if isinstance(height, str) else "pixels", height if isinstance(height, int) else self.MT.GetLinesHeight(int(height)))
         return self.MT.default_rh[1]
 
     def default_header_height(self, height = None):
         if height is not None:
@@ -912,31 +919,32 @@
     def delete_row(self, idx = 0, deselect_all = False, redraw = True):
         self.delete_rows(rows = {idx}, deselect_all = deselect_all, redraw = redraw)
 
     def delete_rows(self, rows: set = set(), deselect_all = False, redraw = True):
         if deselect_all:
             self.deselect("all", redraw = False)
         if isinstance(rows, set):
-            _rows = rows
+            to_del = rows
         else:
-            _rows = set(rows)
-        self.MT.data[:] = [row for r, row in enumerate(self.MT.data) if r not in _rows]
-        rhs = tuple(int(b - a) for a, b in zip(self.MT.row_positions, islice(self.MT.row_positions, 1, len(self.MT.row_positions))))
+            to_del = set(rows)
+        if not to_del:
+            return
+        self.MT.data[:] = [row for r, row in enumerate(self.MT.data) if r not in to_del]
         if self.MT.all_rows_displayed:
-            self.set_row_heights(row_heights = tuple(h for r, h in enumerate(rhs) if r not in _rows))
+            self.set_row_heights(row_heights = (h for r, h in enumerate(int(b - a) for a, b in zip(self.MT.row_positions, islice(self.MT.row_positions, 1, len(self.MT.row_positions)))) if r not in to_del))
         else:
             dispset = set(self.MT.displayed_rows)
             heights_to_del = {i for i, r in enumerate(to_bis) if r in dispset}
             if heights_to_del:
-                self.set_row_heights(row_heights = tuple(h for r, h in enumerate(rhs) if r not in heights_to_del))
-            self.MT.displayed_rows = [r for r in self.MT.displayed_rows if r not in _rows]
-        to_bis = sorted(_rows)
-        self.MT.cell_options = {(r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r), c): v for (r, c), v in self.MT.cell_options.items() if r not in _rows}
-        self.MT.row_options = {r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v for r, v in self.MT.row_options.items() if r not in _rows}
-        self.RI.cell_options = {r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v for r, v in self.RI.cell_options.items() if r not in _rows}
+                self.set_row_heights(row_heights = (h for r, h in enumerate(int(b - a) for a, b in zip(self.MT.row_positions, islice(self.MT.row_positions, 1, len(self.MT.row_positions)))) if r not in heights_to_del))
+            self.MT.displayed_rows = [r for r in self.MT.displayed_rows if r not in to_del]
+        to_bis = sorted(to_del)
+        self.MT.cell_options = {(r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r), c): v for (r, c), v in self.MT.cell_options.items() if r not in to_del}
+        self.MT.row_options = {r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v for r, v in self.MT.row_options.items() if r not in to_del}
+        self.RI.cell_options = {r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v for r, v in self.RI.cell_options.items() if r not in to_del}
         self.set_refresh_timer(redraw)
 
     def insert_row_position(self, idx = "end", height = None, deselect_all = False, redraw = False):
         self.MT.insert_row_position(idx = idx,
                                     height = height,
                                     deselect_all = deselect_all)
         if redraw:
@@ -1020,24 +1028,26 @@
     def delete_columns(self, columns: set = set(), deselect_all = False, redraw = True):
         if deselect_all:
             self.deselect("all", redraw = False)
         if isinstance(columns, set):
             to_del = columns
         else:
             to_del = set(columns)
+        if not to_del:
+            return
         self.MT.data[:] = [[e for c, e in enumerate(r) if c not in to_del] for r in self.MT.data]
         to_bis = sorted(to_del)
-        cws = tuple(int(b - a) for a, b in zip(self.MT.col_positions, islice(self.MT.col_positions, 1, len(self.MT.col_positions))))
+        cws = tuple()
         if self.MT.all_columns_displayed:
-            self.set_column_widths(column_widths = tuple(w for c, w in enumerate(cws) if c not in to_del))
+            self.set_column_widths(column_widths = (w for c, w in enumerate(int(b - a) for a, b in zip(self.MT.col_positions, islice(self.MT.col_positions, 1, len(self.MT.col_positions)))) if c not in to_del))
         else:
             dispset = set(self.MT.displayed_columns)
             widths_to_del = {i for i, c in enumerate(to_bis) if c in dispset}
             if widths_to_del:
-                self.set_column_widths(column_widths = tuple(w for c, w in enumerate(cws) if c not in widths_to_del))
+                self.set_column_widths(column_widths = (w for c, w in enumerate(int(b - a) for a, b in zip(self.MT.col_positions, islice(self.MT.col_positions, 1, len(self.MT.col_positions)))) if c not in widths_to_del))
             self.MT.displayed_columns = [c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c) for c in self.MT.displayed_columns if c not in to_del]
         self.MT.cell_options = {(r, c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c)): v for (r, c), v in self.MT.cell_options.items() if c not in to_del}
         self.MT.col_options = {c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c): v for c, v in self.MT.col_options.items() if c not in to_del}
         self.CH.cell_options = {c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c): v for c, v in self.CH.cell_options.items() if c not in to_del}
         self.set_refresh_timer(redraw)
 
     def insert_column_position(self, idx = "end", width = None, deselect_all = False, redraw = False):
@@ -1679,20 +1689,26 @@
 
     def header_font(self, newfont = None):
         self.MT.header_font(newfont)
 
     def set_options(self,
                     redraw = True,
                     **kwargs):
+        if 'to_clipboard_delimiter' in kwargs:
+            self.MT.to_clipboard_delimiter = kwargs['to_clipboard_delimiter']
+        if 'to_clipboard_quotechar' in kwargs:
+            self.MT.to_clipboard_quotechar = kwargs['to_clipboard_quotechar']
+        if 'to_clipboard_lineterminator' in kwargs:
+            self.MT.to_clipboard_lineterminator = kwargs['to_clipboard_lineterminator']
+        if 'from_clipboard_delimiters' in kwargs:
+            self.MT.from_clipboard_delimiters = kwargs['from_clipboard_delimiters']
         if 'show_dropdown_borders' in kwargs:
             self.MT.show_dropdown_borders = kwargs['show_dropdown_borders']
         if 'edit_cell_validation' in kwargs:
             self.MT.edit_cell_validation = kwargs['edit_cell_validation']
-        if 'ctrl_keys_over_dropdowns_enabled' in kwargs:
-            self.MT.ctrl_keys_over_dropdowns_enabled = kwargs['ctrl_keys_over_dropdowns_enabled']
         if 'show_default_header_for_empty' in kwargs:
             self.CH.show_default_header_for_empty = kwargs['show_default_header_for_empty']
         if 'show_default_index_for_empty' in kwargs:
             self.RI.show_default_index_for_empty = kwargs['show_default_index_for_empty']
         if 'selected_rows_to_end_of_window' in kwargs:
             self.MT.selected_rows_to_end_of_window = kwargs['selected_rows_to_end_of_window']
         if 'horizontal_grid_to_end_of_window' in kwargs:
@@ -1766,15 +1782,15 @@
         if 'table_selected_columns_border_fg' in kwargs:
             self.MT.table_selected_columns_border_fg = kwargs['table_selected_columns_border_fg']
         if 'table_selected_columns_bg' in kwargs:
             self.MT.table_selected_columns_bg = kwargs['table_selected_columns_bg']
         if 'table_selected_columns_fg' in kwargs:
             self.MT.table_selected_columns_fg = kwargs['table_selected_columns_fg']
         if 'default_header' in kwargs:
-            self.CH.default_hdr = kwargs['default_header'].lower()
+            self.CH.default_header = kwargs['default_header'].lower()
         if 'default_row_index' in kwargs:
             self.RI.default_index = kwargs['default_row_index'].lower()
         if 'max_colwidth' in kwargs:
             self.CH.max_cw = float(kwargs['max_colwidth'])
         if 'max_row_height' in kwargs:
             self.RI.max_rh = float(kwargs['max_row_height'])
         if 'max_header_height' in kwargs:
@@ -1872,15 +1888,136 @@
                              redraw = redraw)
             self.config(bg = theme_dark_green['table_bg'])
         elif theme.lower() == "black":
             self.set_options(**theme_black,
                              redraw = redraw)
             self.config(bg = theme_black['table_bg'])
         self.MT.recreate_all_selection_boxes()
-            
+
+    def get_header_data(self, c, get_displayed = False):
+        return self.CH.get_cell_data(datacn = c, get_displayed = get_displayed)
+
+    def get_index_data(self, r, get_displayed = False):
+        return self.RI.get_cell_data(datarn = r, get_displayed = get_displayed)
+
+    def get_sheet_data(self, 
+                       get_displayed = False, 
+                       get_header = False,
+                       get_index = False,
+                       get_header_displayed = True,
+                       get_index_displayed = True,
+                       only_rows = None,
+                       only_columns = None,
+                       **kwargs):
+        if only_rows is not None:
+            if isinstance(only_rows, int):
+                only_rows = (only_rows, )
+            elif not is_iterable(only_rows):
+                raise ValueError(f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}")
+        if only_columns is not None:
+            if isinstance(only_columns, int):
+                only_columns = (only_columns, )
+            elif not is_iterable(only_columns):
+                raise ValueError(f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}")
+        if get_header:
+            maxlen = len(self.MT._headers) if isinstance(self.MT._headers, (list, tuple)) else 0
+            data = []
+            for rn in only_rows if only_rows is not None else range(len(self.MT.data)):
+                r = self.get_row_data(rn, get_displayed = get_displayed, only_columns = only_columns)
+                if len(r) > maxlen:
+                    maxlen = len(r)
+                if get_index:
+                    data.append([self.get_index_data(rn, get_displayed = get_index_displayed)] + r)
+                else:
+                    data.append(r)
+            iterable = only_columns if only_columns is not None else range(maxlen)
+            if get_index:
+                return [[""] + [self.get_header_data(cn, get_displayed = get_header_displayed) for cn in iterable]] + data
+            else:
+                return [[self.get_header_data(cn, get_displayed = get_header_displayed) for cn in iterable]] + data
+        elif not get_header:
+            iterable = only_rows if only_rows is not None else range(len(self.MT.data))
+            return [self.get_row_data(rn,
+                                      get_displayed = get_displayed,
+                                      get_index = get_index,
+                                      get_index_displayed = get_index_displayed,
+                                      only_columns = only_columns)
+                    for rn in iterable]
+    
+    def get_cell_data(self, r, c, get_displayed = False, **kwargs):
+        return self.MT.get_cell_data(r, c, get_displayed)
+
+    def get_row_data(self, r, get_displayed = False, get_index = False, get_index_displayed = True, only_columns = None, **kwargs):
+        if only_columns is not None:
+            if isinstance(only_columns, int):
+                only_columns = (only_columns, )
+            elif not is_iterable(only_columns):
+                raise ValueError(f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}")
+        if r >= self.MT.total_data_rows():
+            raise IndexError(f"Row #{r} is out of range.")
+        if r >= len(self.MT.data):
+            total_data_cols = self.MT.total_data_cols()
+            self.MT.data.extend([list(repeat("", total_data_cols)) for i in range((r + 1) - len(self.MT.data))])
+        iterable = only_columns if only_columns is not None else range(len(self.MT.data[r]))
+        if get_index:
+            return ([self.get_index_data(r, get_displayed = get_index_displayed)] +
+                    [self.MT.get_cell_data(r, c, get_displayed = get_displayed) for c in iterable])
+        else:
+            return [self.MT.get_cell_data(r, c, get_displayed = get_displayed) for c in iterable]
+
+    def get_column_data(self, c, get_displayed = False, get_header = False, get_header_displayed = True, only_rows = None, **kwargs):
+        if only_rows is not None:
+            if isinstance(only_rows, int):
+                only_rows = (only_rows, )
+            elif not is_iterable(only_rows):
+                raise ValueError(f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}")
+        iterable = only_rows if only_rows is not None else range(len(self.MT.data))
+        return (([self.get_header_data(c, get_displayed = get_header_displayed)] if get_header else []) + 
+                [self.MT.get_cell_data(r, c, get_displayed = get_displayed) for r in iterable])
+
+    def yield_sheet_rows(self,
+                         get_displayed = False, 
+                         get_header = False,
+                         get_index = False,
+                         get_index_displayed = True,
+                         get_header_displayed = True,
+                         only_rows = None,
+                         only_columns = None,
+                         **kwargs):
+        if only_rows is not None:
+            if isinstance(only_rows, int):
+                only_rows = (only_rows, )
+            elif not is_iterable(only_rows):
+                raise ValueError(f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}")
+        if only_columns is not None:
+            if isinstance(only_columns, int):
+                only_columns = (only_columns, )
+            elif not is_iterable(only_columns):
+                raise ValueError(f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}")
+        if get_header:
+            maxlen = self.MT.total_data_cols()
+            iterable = only_columns if only_columns is not None else range(maxlen)
+            yield ([""] if get_index else []) + [self.get_header_data(c, get_displayed = get_header_displayed) for c in iterable]
+        iterable = only_rows if only_rows is not None else range(len(self.MT.data))
+        yield from  (self.get_row_data(r,
+                                       get_displayed = get_displayed,
+                                       get_index = get_index,
+                                       get_index_displayed = get_index_displayed,
+                                       only_columns = only_columns) 
+                        for r in iterable)
+
+    @property
+    def data(self):
+        return self.MT.data
+        
+    def formatted(self, r, c):
+        if (r, c) in self.MT.cell_options and 'format' in self.MT.cell_options[(r, c)]:
+            return True
+        return False
+    
     def data_reference(self,
                        newdataref = None,
                        reset_col_positions = True,
                        reset_row_positions = True,
                        redraw = False):
         return self.MT.data_reference(newdataref,
                                       reset_col_positions,
@@ -1889,144 +2026,80 @@
 
     def set_sheet_data(self,
                        data = [[]],
                        reset_col_positions = True,
                        reset_row_positions = True,
                        redraw = True,
                        verify = False,
-                       reset_highlights = False):
-        if verify:
-            if not isinstance(data, list) or not all(isinstance(row, list) for row in data):
-                raise ValueError("Data argument must be a list of lists, sublists being rows")
+                       reset_highlights = False,
+                       keep_formatting = True):
+        if verify and (not isinstance(data, list) or not all(isinstance(row, list) for row in data)):
+            raise ValueError("Data argument must be a list of lists, sublists being rows")
         if reset_highlights:
             self.dehighlight_all()
         return self.MT.data_reference(data,
                                       reset_col_positions,
                                       reset_row_positions,
                                       redraw,
-                                      return_id = False)
-
-    def get_sheet_data(self, return_copy = False, get_header = False, get_index = False):
-        if return_copy:
-            if get_header and get_index:
-                index_limit = len(self.MT._row_index)
-                return [[""] + self.MT._headers.copy()] + [[f"{self.MT._row_index[rn]}"] + r.copy() if rn < index_limit else [""] + r.copy() for rn, r in enumerate(self.MT.data)]
-            elif get_header and not get_index:
-                return [self.MT._headers.copy()] + [r.copy() for r in self.MT.data]
-            elif get_index and not get_header:
-                index_limit = len(self.MT._row_index)
-                return [[f"{self.MT._row_index[rn]}"] + r.copy() if rn < index_limit else [""] + r.copy() for rn, r in enumerate(self.MT.data)]
-            elif not get_index and not get_header:
-                return [r.copy() for r in self.MT.data]
-        else:
-            if get_header and get_index:
-                index_limit = len(self.MT._row_index)
-                return [[""] + self.MT._headers] + [[self.MT._row_index[rn]] + r if rn < index_limit else [""] + r for rn, r in enumerate(self.MT.data)]
-            elif get_header and not get_index:
-                return [self.MT._headers] + self.MT.data
-            elif get_index and not get_header:
-                index_limit = len(self.MT._row_index)
-                return [[self.MT._row_index[rn]] + r if rn < index_limit else [""] + r for rn, r in enumerate(self.MT.data)]
-            elif not get_index and not get_header:
-                return self.MT.data
+                                      return_id = False,
+                                      keep_formatting = keep_formatting)
 
-    @property
-    def data(self):
-        return self.MT.data
+    def set_cell_data(self, r, c, value = "", redraw = False, keep_formatting = True):
+        if not keep_formatting:
+            self.MT.delete_cell_format(r, c, clear_values = False)
+        self.MT.set_cell_data(r, c, value)
+        if redraw:
+            self.set_refresh_timer()
             
-    def yield_sheet_rows(self, get_header = False, get_index = False):
-        if get_header:
-            if get_index:
-                yield [""] + [self.get_n2a(c, self.CH.default_hdr) for c in range(len(max(self.MT.data, key = len)))] if isinstance(self.MT._headers, int) or not self.MT._headers else self.MT._headers
-            else:
-                yield [self.get_n2a(c, self.CH.default_hdr) for c in range(len(max(self.MT.data, key = len)))] if isinstance(self.MT._headers, int) or not self.MT._headers else self.MT._headers
-        if get_index:
-            if isinstance(self.MT._row_index, int) or not self.MT._row_index:
-                for rn, r in enumerate(self.MT.data):
-                    yield [self.get_n2a(rn, self.RI.default_index)] + r
-            else:
-                index_limit = len(self.MT._row_index)
-                for rn, r in enumerate(self.MT.data):
-                    yield [self.MT._row_index[rn]] + r if rn < index_limit else [""] + r
-        else:
-            yield from self.MT.data
-                
-    def get_n2a(self, n = 0, _type = "numbers"):
-        if _type == "letters":
-            return num2alpha(n)
-        elif _type == "numbers":
-            return f"{n + 1}"
-        else:
-            return f"{num2alpha(n)} {n + 1}"
-
-    def get_cell_data(self, r, c, return_copy = True):
-        if return_copy:
-            try:
-                return f"{self.MT.data[r][c]}"
-            except:
-                return None
-        else:
-            try:
-                return self.MT.data[r][c]
-            except:
-                return None
-
-    def get_row_data(self, r, return_copy = True):
-        if return_copy:
-            try:
-                return tuple(f"{e}" for e in self.MT.data[r])
-            except:
-                return None
-        else:
-            try:
-                return self.MT.data[r]
-            except:
-                return None
-
-    def get_column_data(self, c, return_copy = True):
-        res = []
-        if return_copy:
-            for r in self.MT.data:
-                try:
-                    res.append(f"{r[c]}")
-                except:
-                    continue
-            return tuple(res)
+    def set_row_data(self, r, values = tuple(), add_columns = True, redraw = False, keep_formatting = True):
+        if r >= len(self.MT.data):
+            raise Exception("Row number is out of range")
+        if not keep_formatting:
+            self.MT.delete_row_format(r, clear_values = False)
+        maxidx = len(self.MT.data[r]) - 1
+        if not values:
+            self.MT.data[r][:] = list(repeat("", len(self.MT.data[r])))
+        if add_columns:
+            for c, v in enumerate(values):
+                if c > maxidx:
+                    self.MT.data[r].append(v)
+                    if self.MT.all_columns_displayed and c >= len(self.MT.col_positions) - 1:
+                        self.MT.insert_col_position("end")
+                else:
+                    self.set_cell_data(r = r, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         else:
-            for r in self.MT.data:
-                try:
-                    res.append(r[c])
-                except:
-                    continue
-            return res
-
-    def set_cell_data(self, r, c, value = "", set_copy = True, redraw = False):
-        self.MT.data[r][c] = f"{value}" if set_copy else value
+            for c, v in enumerate(values):
+                if c > maxidx:
+                    self.MT.data[r].append(v)
+                else:
+                    self.set_cell_data(r = r, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         self.set_refresh_timer(redraw)
 
-    def set_column_data(self, c, values = tuple(), add_rows = True, redraw = False):
+    def set_column_data(self, c, values = tuple(), add_rows = True, redraw = False, keep_formatting = True):
+        if not keep_formatting:
+            self.MT.delete_column_format(c, clear_values = False)
         if add_rows:
             maxidx = len(self.MT.data) - 1
             total_cols = None
             height = self.MT.default_rh[1]
             for rn, v in enumerate(values):
                 if rn > maxidx:
                     if total_cols is None:
                         total_cols = self.MT.total_data_cols()
                     self.MT.data.append(list(repeat("", total_cols)))
                     self.MT.insert_row_position("end", height = height)
                     maxidx += 1
-                if c > len(self.MT.data[rn]) - 1:
+                if c >= len(self.MT.data[rn]):
                     self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
-                self.MT.data[rn][c] = v
+                self.set_cell_data(r = rn, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         else:
             for rn, v in enumerate(values):
-                if c > len(self.MT.data[rn]) - 1:
+                if c >= len(self.MT.data[rn]):
                     self.MT.data[rn].extend(list(repeat("", c - len(self.MT.data[rn]))))
-                self.MT.data[rn][c] = v
+                self.set_cell_data(r = rn, c = c, value = v, redraw = False, keep_formatting = keep_formatting)
         self.set_refresh_timer(redraw)
 
     def insert_column(self,
                       values = None, 
                       idx = "end", 
                       width = None, 
                       deselect_all = False, 
@@ -2121,36 +2194,14 @@
         if isinstance(idx, int):
             num_add = len(data)
             self.MT.cell_options = {(rn, cn if cn < idx else cn + num_add): t2 for (rn, cn), t2 in self.MT.cell_options.items()}
             self.MT.col_options = {cn if cn < idx else cn + num_add: t for cn, t in self.MT.col_options.items()}
             self.CH.cell_options = {cn if cn < idx else cn + num_add: t for cn, t in self.CH.cell_options.items()}
         self.set_refresh_timer(redraw)
 
-    def set_row_data(self, r, values = tuple(), add_columns = True, redraw = False):
-        if len(self.MT.data) - 1 < r:
-            raise Exception("Row number is out of range")
-        maxidx = len(self.MT.data[r]) - 1
-        if not values:
-            self.MT.data[r][:] = list(repeat("", len(self.MT.data[r])))
-        if add_columns:
-            for c, v in enumerate(values):
-                if c > maxidx:
-                    self.MT.data[r].append(v)
-                    if self.MT.all_columns_displayed and c >= len(self.MT.col_positions) - 1:
-                        self.MT.insert_col_position("end")
-                else:
-                    self.MT.data[r][c] = v
-        else:
-            for c, v in enumerate(values):
-                if c > maxidx:
-                    self.MT.data[r].append(v)
-                else:
-                    self.MT.data[r][c] = v
-        self.set_refresh_timer(redraw)
-
     def insert_row(self, values = None, idx = "end", height = None, deselect_all = False, add_columns = False,
                    redraw = False):
         self.MT.insert_row_position(idx = idx,
                                     height = height,
                                     deselect_all = deselect_all)
         total_cols = None
         if values is None:
@@ -2220,20 +2271,23 @@
             self.MT.row_options = {rn if rn < idx else rn + num_add: t for rn, t in self.MT.row_options.items()}
             self.RI.cell_options = {rn if rn < idx else rn + num_add: t for rn, t in self.RI.cell_options.items()}
         self.set_refresh_timer(redraw)
 
     def sheet_data_dimensions(self, total_rows = None, total_columns = None):
         self.MT.data_dimensions(total_rows, total_columns)
 
-    def get_total_rows(self):
-        return len(self.MT.data)
+    def get_total_rows(self, include_index = False):
+        return self.MT.total_data_rows(include_index = include_index)
+
+    def get_total_columns(self, include_header = False):
+        return self.MT.total_data_cols(include_header = include_header)
 
     def equalize_data_row_lengths(self):
         return self.MT.equalize_data_row_lengths()
-                    
+
     def display_columns(self,
                         columns = None,
                         all_columns_displayed = None,
                         reset_col_positions = True,
                         refresh = False,
                         redraw = False,
                         deselect_all = True):
@@ -2284,29 +2338,22 @@
     def create_header_checkbox(self,
                                c,
                                checked = False,
                                state = "normal",
                                redraw = False,
                                check_function = None,
                                text = ""):
+        _kwargs = {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
         if isinstance(c, str) and c.lower() == "all":
             for c_ in range(self.MT.total_data_cols()):
-                self.CH.create_checkbox(c = c_,
-                                        checked = checked,
-                                        state = state,
-                                        redraw = redraw,
-                                        check_function = check_function,
-                                        text = text)
-        else:
-            self.CH.create_checkbox(c = c,
-                                    checked = checked,
-                                    state = state,
-                                    redraw = redraw,
-                                    check_function = check_function,
-                                    text = text)
+                self.CH.create_checkbox(datacn = c_,
+                                        **_kwargs)
+        else:
+            self.CH.create_checkbox(datacn = c,
+                                    **_kwargs)
 
     def click_header_checkbox(self,
                               c,
                               checked = None):
         if c in self.CH.cell_options and 'checkbox' in self.CH.cell_options[c]:
             if not type(self.MT._headers[c]) == bool:
                 if checked is None:
@@ -2346,29 +2393,22 @@
     def create_index_checkbox(self,
                               r,
                               checked = False,
                               state = "normal",
                               redraw = False,
                               check_function = None,
                               text = ""):
+        _kwargs = {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(self.MT.total_data_rows()):
-                self.RI.create_checkbox(r = r_,
-                                        checked = checked,
-                                        state = state,
-                                        redraw = redraw,
-                                        check_function = check_function,
-                                        text = text)
-        else:
-            self.RI.create_checkbox(r = r,
-                                    checked = checked,
-                                    state = state,
-                                    redraw = redraw,
-                                    check_function = check_function,
-                                    text = text)
+                self.RI.create_checkbox(datarn = r_,
+                                        **_kwargs)
+        else:
+            self.RI.create_checkbox(datarn = r,
+                                    **_kwargs)
 
     def click_index_checkbox(self,
                              r,
                              checked = None):
         if r in self.RI.cell_options and 'checkbox' in self.RI.cell_options[r]:
             if not type(self.MT._row_index[r]) == bool:
                 if checked is None:
@@ -2409,51 +2449,36 @@
                         r,
                         c,
                         checked = False,
                         state = "normal",
                         redraw = False,
                         check_function = None,
                         text = ""):
+        _kwargs = {'checked': checked, 'state': state, 'redraw': redraw, 'check_function': check_function, 'text': text}
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
-                self.MT.create_checkbox(r = r_,
-                                        c = c,
-                                        checked = checked,
-                                        state = state,
-                                        redraw = redraw,
-                                        check_function = check_function,
-                                        text = text)
+                self.MT.create_checkbox(datarn = r_,
+                                        datacn = c,
+                                        **_kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
-                self.MT.create_checkbox(r = r,
-                                        c = c_,
-                                        checked = checked,
-                                        state = state,
-                                        redraw = redraw,
-                                        check_function = check_function,
-                                        text = text)
+                self.MT.create_checkbox(datarn = r,
+                                        datacn = c_,
+                                        **_kwargs)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
-                    self.MT.create_checkbox(r = r_,
-                                            c = c_,
-                                            checked = checked,
-                                            state = state,
-                                            redraw = redraw,
-                                            check_function = check_function,
-                                            text = text)
-        else:
-            self.MT.create_checkbox(r = r,
-                                    c = c,
-                                    checked = checked,
-                                    state = state,
-                                    redraw = redraw,
-                                    check_function = check_function,
-                                    text = text)
+                    self.MT.create_checkbox(datarn = r_,
+                                            datacn = c_,
+                                            **_kwargs)
+        else:
+            self.MT.create_checkbox(datarn = r,
+                                    datacn = c,
+                                    **_kwargs)
 
     def click_checkbox(self,
                        r,
                        c,
                        checked = None):
         if (r, c) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(r, c)]:
             if not type(self.MT.data[r][c]) == bool:
@@ -2495,40 +2520,35 @@
         if check_function != "":
             self.MT.cell_options[(r, c)]['checkbox']['check_function'] = check_function
         if state and state.lower() in ("normal", "disabled"):
             self.MT.cell_options[(r, c)]['checkbox']['state'] = state
         if text is not None:
             self.MT.cell_options[(r, c)]['checkbox']['text'] = text
         return {**self.MT.cell_options[(r, c)]['checkbox'], 'checked': self.MT.data[r][c]}
-    
+
     def create_header_dropdown(self,
                                c = 0,
                                values = [],
                                set_value = None,
-                               state = "readonly",
+                               state = "normal",
                                redraw = False,
                                selection_function = None,
-                               modified_function = None):
+                               modified_function = None,
+                               search_function = dropdown_search_function,
+                               validate_input = True,
+                               text = None):
+        _kwargs = {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
+                   'modified_function': modified_function, 'search_function': dropdown_search_function, 'validate_input': validate_input, 'text': text}
         if isinstance(c, str) and c.lower() == "all":
             for c_ in range(self.MT.total_data_cols()):
-                self.CH.create_dropdown(c = c_,
-                                        values = values,
-                                        set_value = set_value,
-                                        state = state,
-                                        redraw = redraw,
-                                        selection_function = selection_function,
-                                        modified_function = modified_function)
-        else:
-            self.CH.create_dropdown(c = c,
-                                    values = values,
-                                    set_value = set_value,
-                                    state = state,
-                                    redraw = redraw,
-                                    selection_function = selection_function,
-                                    modified_function = modified_function)
+                self.CH.create_dropdown(datacn = c_,
+                                        **_kwargs)
+        else:
+            self.CH.create_dropdown(datacn = c,
+                                    **_kwargs)
 
     def get_header_dropdown_value(self, c):
         if 'dropdown' in self.CH.cell_options[c]:
             return self.MT._headers[c]
 
     def get_header_dropdown_values(self, c = 0):
         return self.CH.cell_options[c]['dropdown']['values']
@@ -2536,70 +2556,65 @@
     def header_dropdown_functions(self, c, selection_function = "", modified_function = ""):
         if selection_function != "":
             self.CH.cell_options[c]['dropdown']['select_function'] = selection_function
         if modified_function != "":
             self.CH.cell_options[c]['dropdown']['modified_function'] = modified_function
         return self.CH.cell_options[c]['dropdown']['select_function'], self.CH.cell_options[c]['dropdown']['modified_function']
 
-    def set_header_dropdown_values(self, c = 0, set_existing_dropdown = False, values = [], displayed = None):
+    def set_header_dropdown_values(self, c = 0, set_existing_dropdown = False, values = [], set_value = None):
         if set_existing_dropdown:
             if self.CH.existing_dropdown_window is not None:
                 c_ = self.CH.existing_dropdown_window.c
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             c_ = c
         self.CH.cell_options[c_]['dropdown']['values'] = values
         if self.CH.cell_options[c_]['dropdown']['window'] != "no dropdown open":
             self.CH.cell_options[c_]['dropdown']['window'].values(values)
-        if displayed is not None:
-            self.MT.headers(newheaders = displayed, index = c_)
+        if set_value is not None:
+            self.MT.headers(newheaders = set_value, index = c_)
 
     def delete_header_dropdown(self, c = 0):
         if c == "all":
             for c_ in self.CH.cell_options:
                 if 'dropdown' in self.CH.cell_options[c_]:
                     self.CH.delete_dropdown(c_)
         else:
             self.CH.delete_dropdown(c)
 
     def get_header_dropdowns(self):
         return {k: v['dropdown'] for k, v in self.CH.cell_options.items() if 'dropdown' in v}
     
     def open_header_dropdown(self, c):
-        self.CH.display_dropdown_window(c)
+        self.CH.open_dropdown_window(c)
 
     def close_header_dropdown(self, c):
-        self.CH.hide_dropdown_window(c)
+        self.CH.close_dropdown_window(c)
         
     def create_index_dropdown(self,
                               r = 0,
                               values = [],
                               set_value = None,
-                              state = "readonly",
+                              state = "normal",
                               redraw = False,
                               selection_function = None,
-                              modified_function = None):
+                              modified_function = None,
+                              search_function = dropdown_search_function,
+                              validate_input = True,
+                              text = None):
+        _kwargs = {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
+                   'modified_function': modified_function, 'search_function': dropdown_search_function, 'validate_input': validate_input, 'text': text}
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(self.MT.total_data_rows()):
-                self.RI.create_dropdown(r = r_,
-                                        values = values,
-                                        set_value = set_value,
-                                        state = state,
-                                        redraw = redraw,
-                                        selection_function = selection_function,
-                                        modified_function = modified_function)
-        else:
-            self.RI.create_dropdown(r = r,
-                                    values = values,
-                                    set_value = set_value,
-                                    state = state,
-                                    redraw = redraw,
-                                    selection_function = selection_function,
-                                    modified_function = modified_function)
+                self.RI.create_dropdown(datarn = r_,
+                                        **_kwargs)
+        else:
+            self.RI.create_dropdown(datarn = r,
+                                    **_kwargs)
 
     def get_index_dropdown_value(self, r):
         if 'dropdown' in self.RI.cell_options[r]:
             return self.MT._row_index[r]
 
     def get_index_dropdown_values(self, r = 0):
         return self.RI.cell_options[r]['dropdown']['values']
@@ -2607,127 +2622,111 @@
     def index_dropdown_functions(self, r, selection_function = "", modified_function = ""):
         if selection_function != "":
             self.RI.cell_options[r]['dropdown']['select_function'] = selection_function
         if modified_function != "":
             self.RI.cell_options[r]['dropdown']['modified_function'] = modified_function
         return self.RI.cell_options[r]['dropdown']['select_function'], self.RI.cell_options[r]['dropdown']['modified_function']
 
-    def set_index_dropdown_values(self, r = 0, set_existing_dropdown = False, values = [], displayed = None):
+    def set_index_dropdown_values(self, r = 0, set_existing_dropdown = False, values = [], set_value = None):
         if set_existing_dropdown:
             if self.RI.existing_dropdown_window is not None:
                 r_ = self.RI.existing_dropdown_window.r
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             r_ = r
         self.RI.cell_options[r_]['dropdown']['values'] = values
         if self.RI.cell_options[r_]['dropdown']['window'] != "no dropdown open":
             self.RI.cell_options[r_]['dropdown']['window'].values(values)
-        if displayed is not None:
-            self.MT.row_index(newindex = displayed, index = r_)
+        if set_value is not None:
+            self.MT.row_index(newindex = set_value, index = r_)
 
     def delete_index_dropdown(self, r = 0):
         if r == "all":
             for r_ in self.RI.cell_options:
                 if 'dropdown' in self.RI.cell_options[r_]:
                     self.RI.delete_dropdown(r_)
         else:
             self.RI.delete_dropdown(r)
 
     def get_index_dropdowns(self):
         return {k: v['dropdown'] for k, v in self.RI.cell_options.items() if 'dropdown' in v}
     
     def open_index_dropdown(self, r):
-        self.RI.display_dropdown_window(r)
+        self.RI.open_dropdown_window(r)
 
     def close_index_dropdown(self, r):
-        self.RI.hide_dropdown_window(r)
+        self.RI.close_dropdown_window(r)
 
     def create_dropdown(self,
                         r = 0,
                         c = 0,
                         values = [],
                         set_value = None,
-                        state = "readonly",
+                        state = "normal",
                         redraw = False,
                         selection_function = None,
-                        modified_function = None):
+                        modified_function = None,
+                        search_function = dropdown_search_function,
+                        validate_input = True,
+                        text = None):
+        _kwargs = {'values': values, 'set_value': set_value, 'state': state, 'redraw': redraw, 'selection_function': selection_function,
+                   'modified_function': modified_function, 'search_function': dropdown_search_function, 'validate_input': validate_input, 'text': text}
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
-                self.MT.create_dropdown(r = r_,
-                                        c = c,
-                                        values = values,
-                                        set_value = set_value,
-                                        state = state,
-                                        redraw = redraw,
-                                        selection_function = selection_function,
-                                        modified_function = modified_function)
+                self.MT.create_dropdown(datarn = r_,
+                                        datacn = c,
+                                        **_kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
-                self.MT.create_dropdown(r = r,
-                                        c = c_,
-                                        values = values,
-                                        set_value = set_value,
-                                        state = state,
-                                        redraw = redraw,
-                                        selection_function = selection_function,
-                                        modified_function = modified_function)
+                self.MT.create_dropdown(datarn = r,
+                                        datacn = c_,
+                                        **_kwargs)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
-                    self.MT.create_dropdown(r = r_,
-                                            c = c_,
-                                            values = values,
-                                            set_value = set_value,
-                                            state = state,
-                                            redraw = redraw,
-                                            selection_function = selection_function,
-                                            modified_function = modified_function)
-        
-        else:
-            self.MT.create_dropdown(r = r,
-                                    c = c,
-                                    values = values,
-                                    set_value = set_value,
-                                    state = state,
-                                    redraw = redraw,
-                                    selection_function = selection_function,
-                                    modified_function = modified_function)
+                    self.MT.create_dropdown(datarn = r_,
+                                            datacn = c_,
+                                            **_kwargs)
+        else:
+            self.MT.create_dropdown(datarn = r,
+                                    datacn = c,
+                                    **_kwargs)
 
     def get_dropdown_value(self, r, c):
         return self.get_cell_data(r, c)
 
     def get_dropdown_values(self, r = 0, c = 0):
         return self.MT.cell_options[(r, c)]['dropdown']['values']
 
     def dropdown_functions(self, r, c, selection_function = "", modified_function = ""):
         if selection_function != "":
             self.MT.cell_options[(r, c)]['dropdown']['select_function'] = selection_function
         if modified_function != "":
             self.MT.cell_options[(r, c)]['dropdown']['modified_function'] = modified_function
         return self.MT.cell_options[(r, c)]['dropdown']['select_function'], self.MT.cell_options[(r, c)]['dropdown']['modified_function']
 
-    def set_dropdown_values(self, r = 0, c = 0, set_existing_dropdown = False, values = [], displayed = None):
+    def set_dropdown_values(self, r = 0, c = 0, set_existing_dropdown = False, values = [], set_value = None):
         if set_existing_dropdown:
             if self.MT.existing_dropdown_window is not None:
                 r_ = self.MT.existing_dropdown_window.r
                 c_ = self.MT.existing_dropdown_window.c
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             r_ = r
             c_ = c
         self.MT.cell_options[(r_, c_)]['dropdown']['values'] = values
         if self.MT.cell_options[(r_, c_)]['dropdown']['window'] != "no dropdown open":
             self.MT.cell_options[(r_, c_)]['dropdown']['window'].values(values)
-        if displayed is not None:
-            self.set_cell_data(r_, c_, displayed)
+        if set_value is not None:
+            self.set_cell_data(r_, c_, set_value)
             if self.MT.cell_options[(r_, c_)]['dropdown']['window'] != "no dropdown open" and self.MT.text_editor_loc is not None and self.MT.text_editor is not None:
-                self.MT.text_editor.set_text(displayed)
+                self.MT.text_editor.set_text(set_value)
 
     def delete_dropdown(self, r = 0, c = 0):
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_, c_ in self.MT.cell_options:
                 if 'dropdown' in self.MT.cell_options[(r_, c)]:
                     self.MT.delete_dropdown(r_, c)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
@@ -2741,18 +2740,136 @@
         else:
             self.MT.delete_dropdown(r, c)
 
     def get_dropdowns(self):
         return {k: v['dropdown'] for k, v in self.MT.cell_options.items() if 'dropdown' in v}
 
     def open_dropdown(self, r, c):
-        self.MT.display_dropdown_window(r, c)
+        self.MT.open_dropdown_window(r, c)
 
     def close_dropdown(self, r, c):
-        self.MT.hide_dropdown_window(r, c)
+        self.MT.close_dropdown_window(r, c)
+
+    def reapply_formatting(self):
+        self.MT.reapply_formatting()
+        
+    def reapply_formatting(self):
+        self.MT.reapply_formatting()
+        
+    def delete_all_formatting(self, clear_values = False):
+        self.MT.delete_all_formatting(clear_values = clear_values)
+
+    def format_cell(self,
+                    r,
+                    c,
+                    formatter_options = {},
+                    formatter_class = None,
+                    redraw = True,
+                    **kwargs,
+                    ):
+        if isinstance(r, str) and r.lower() == 'all' and isinstance(c, int):
+            for r_ in range(self.MT.total_data_rows()):
+                self.MT.format_cell(datarn = r_,
+                                    datacn = c, 
+                                    **{'formatter': formatter_class, **formatter_options, **kwargs})
+        elif isinstance(c, str) and c.lower() == 'all' and isinstance(r, int):
+            for c_ in range(self.MT.total_data_cols()):
+                self.MT.format_cell(datarn = r,
+                                    datacn = c_, 
+                                    **{'formatter': formatter_class, **formatter_options, **kwargs})
+        elif isinstance(r, str) and r.lower() == 'all' and isinstance(c, str) and c.lower() == 'all':
+            for r_ in range(self.MT.total_data_rows()):
+                for c_ in range(self.MT.total_data_cols()):
+                    self.MT.format_cell(datarn = r_,
+                                        datacn = c_, 
+                                        **{'formatter': formatter_class, **formatter_options, **kwargs})
+        else:
+            self.MT.format_cell(datarn = r,
+                                datacn = c, 
+                                **{'formatter': formatter_class, **formatter_options, **kwargs})
+        self.set_refresh_timer(redraw)
+
+    def delete_cell_format(self,
+                           r = "all",
+                           c = "all",
+                           clear_values = False,
+                           ):
+        if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
+            for r_, c_ in self.MT.cell_options:
+                if 'format' in self.MT.cell_options[(r_, c)]:
+                    self.MT.delete_cell_format(r_, c, clear_values = clear_values)
+        elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
+            for r_, c_ in self.MT.cell_options:
+                if 'format' in self.MT.cell_options[(r, c_)]:
+                    self.MT.delete_cell_format(r, c_, clear_values = clear_values)
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
+            for r_, c_ in self.MT.cell_options:
+                if 'format' in self.MT.cell_options[(r_, c_)]:
+                    self.MT.delete_cell_format(r_, c_, clear_values = clear_values)
+        else:
+            self.MT.delete_cell_format(r, c, clear_values = clear_values)
+
+    def format_row(self,
+                   r,
+                   formatter_options = {},
+                   formatter_class = None,
+                   redraw = True,
+                   **kwargs,
+                   ):
+        if isinstance(r, str) and r.lower() == "all":
+            for r_ in range(len(self.MT.data)):
+                self.MT.format_column(r_, **{'formatter': formatter_class, **formatter_options, **kwargs})
+        elif is_iterable(r):
+            for r_ in r:
+                self.MT.format_row(r_, **{'formatter': formatter_class, **formatter_options, **kwargs})
+        else:
+            self.MT.format_row(r, **{'formatter': formatter_class, **formatter_options, **kwargs})
+        self.set_refresh_timer(redraw)
+
+    def delete_row_format(self, r = "all", clear_values = False):
+        if is_iterable(r):
+            for r_ in r:
+                self.MT.delete_row_format(r_, clear_values = clear_values)
+        else:
+            self.MT.delete_row_format(r, clear_values = clear_values)
+
+    def format_column(self,
+                      c,
+                      formatter_options = {},
+                      formatter_class = None,
+                      redraw = True,
+                      **kwargs,
+                      ):
+        if isinstance(c, str) and c.lower() == "all":
+            for c_ in range(self.MT.total_data_cols()):
+                self.MT.format_column(c_, **{'formatter': formatter_class, **formatter_options, **kwargs})
+        elif is_iterable(c):
+            for c_ in c:
+                self.MT.format_column(c_, **{'formatter': formatter_class, **formatter_options, **kwargs})
+        else:
+            self.MT.format_column(c, **{'formatter': formatter_class, **formatter_options, **kwargs})
+        self.set_refresh_timer(redraw)
+
+    def delete_column_format(self, c = "all", clear_values = False):
+        if is_iterable(c):
+            for c_ in c:
+                self.MT.delete_column_format(c_, clear_values = clear_values)
+        else:
+            self.MT.delete_column_format(c, clear_values = clear_values)
+
+    def format_sheet(self, 
+                     formatter_options = {},
+                     formatter_class = None,
+                     redraw = True,
+                     **kwargs):
+        self.MT.format_sheet(**{'formatter': formatter_class, **formatter_options, **kwargs})
+        self.set_refresh_timer(redraw)
+        
+    def delete_sheet_format(self, clear_values = False):
+        self.MT.delete_sheet_format(clear_values = clear_values)
 
 
 class Sheet_Dropdown(Sheet):
     def __init__(self,
                  parent,
                  r,
                  c,
@@ -2762,15 +2879,17 @@
                  colors = {'bg': theme_light_blue['popup_menu_bg'],
                            'fg': theme_light_blue['popup_menu_fg'],
                            'highlight_bg': theme_light_blue['popup_menu_highlight_bg'],
                            'highlight_fg': theme_light_blue['popup_menu_highlight_fg']},
                  outline_color = theme_light_blue['table_fg'],
                  outline_thickness = 2,
                  values = [],
-                 hide_dropdown_window = None,
+                 close_dropdown_window = None,
+                 modified_function = None,
+                 search_function = dropdown_search_function,
                  arrowkey_RIGHT = None,
                  arrowkey_LEFT = None,
                  align = "w",
                  # False for using r, c "r" for r "c" for c
                  single_index = False):
         Sheet.__init__(self,
                        parent = parent,
@@ -2795,15 +2914,17 @@
                        table_selected_rows_fg = colors['highlight_fg'],
                        width = width,
                        height = height,
                        font = font if font else get_font(),
                        table_fg = colors['fg'],
                        table_bg = colors['bg'])
         self.parent = parent
-        self.hide_dropdown_window = hide_dropdown_window
+        self.close_dropdown_window = close_dropdown_window
+        self.modified_function = modified_function
+        self.search_function = search_function
         self.arrowkey_RIGHT = arrowkey_RIGHT
         self.arrowkey_LEFT = arrowkey_LEFT
         self.h_ = height
         self.w_ = width
         self.r = r
         self.c = c
         self.row = -1
@@ -2832,14 +2953,26 @@
 
     def arrowkey_DOWN(self, event = None):
         self.deselect("all")
         if len(self.MT.data) - 1 > self.row:
             self.row += 1
         self.see(self.row, 0, redraw = False)
         self.select_row(self.row)
+        
+    def search_and_see(self, event = None):
+        if self.modified_function is not None:
+            self.modified_function(event)
+        if self.search_function is not None:
+            rn = self.search_function(search_for = fr"{event.value}".lower(), 
+                                      data = self.MT.data)
+            if rn is not None:
+                self.row = rn
+                self.deselect("all")
+                self.see(self.row, 0, redraw = False)
+                self.select_row(self.row)
 
     def mouse_motion(self, event = None):
         self.row = self.identify_row(event, exclude_index = True, allow_end = False)
         self.deselect("all")
         if self.row is not None:
             self.select_row(self.row)
             
@@ -2857,22 +2990,22 @@
                 row = None
             else:
                 row = next(iter(row))
         else:
             row = self.identify_row(event, exclude_index = True, allow_end = False)
         if self.single_index:
             if row is None:
-                self.hide_dropdown_window(self.r if self.single_index == "r" else self.c)
+                self.close_dropdown_window(self.r if self.single_index == "r" else self.c)
             else:
-                self.hide_dropdown_window(self.r if self.single_index == "r" else self.c, self.get_cell_data(row, 0))
+                self.close_dropdown_window(self.r if self.single_index == "r" else self.c, self.get_cell_data(row, 0))
         else:
             if row is None:
-                self.hide_dropdown_window(self.r, self.c)
+                self.close_dropdown_window(self.r, self.c)
             else:
-                self.hide_dropdown_window(self.r, self.c, self.get_cell_data(row, 0))
+                self.close_dropdown_window(self.r, self.c, self.get_cell_data(row, 0))
 
     def values(self, values = [], redraw = True):
         self.set_sheet_data([[v] for v in values],
                             reset_col_positions = False,
                             reset_row_positions = False,
                             redraw = False,
                             verify = False)
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet_column_headers.py` & `tksheet-6.0.0/tksheet/_tksheet_row_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,248 +1,230 @@
 from ._tksheet_vars import *
+from ._tksheet_formatters import *
 from ._tksheet_other_classes import *
 
 from itertools import islice, accumulate, chain, cycle, repeat
 from collections import defaultdict
 from math import floor, ceil
 import bisect
 import pickle
 import tkinter as tk
 import zlib
 
 
-class ColumnHeaders(tk.Canvas):
+class RowIndex(tk.Canvas):
     def __init__(self,
                  *args,
                  **kwargs):
         tk.Canvas.__init__(self,
                            kwargs['parentframe'],
-                           background = kwargs['header_bg'],
+                           background = kwargs['index_bg'],
                            highlightthickness = 0)
         self.parentframe = kwargs['parentframe']
-        self.current_height = None    # is set from within MainTable() __init__ or from Sheet parameters
         self.MT = None         # is set from within MainTable() __init__
-        self.RI = None    # is set from within MainTable() __init__
+        self.CH = None      # is set from within MainTable() __init__
         self.TL = None                # is set from within TopLeftRectangle() __init__
         self.extra_begin_edit_cell_func = None
         self.extra_end_edit_cell_func = None
         self.text_editor = None
         self.text_editor_id = None
         self.text_editor_loc = None
-        self.centre_alignment_text_mod_indexes = (slice(1, None), slice(None, -1))
-        self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
-        self.grid_cyctup = ("st", "end")
-        self.grid_cyc = cycle(self.grid_cyctup)
         self.b1_pressed_loc = None
         self.existing_dropdown_canvas_id = None
         self.existing_dropdown_window = None
         self.closed_dropdown = None
+        self.centre_alignment_text_mod_indexes = (slice(1, None), slice(None, -1))
+        self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
+        self.grid_cyctup = ("st", "end")
+        self.grid_cyc = cycle(self.grid_cyctup)
         self.being_drawn_rect = None
         self.extra_motion_func = None
         self.extra_b1_press_func = None
         self.extra_b1_motion_func = None
         self.extra_b1_release_func = None
-        self.extra_double_b1_func = None
-        self.ch_extra_begin_drag_drop_func = None
-        self.ch_extra_end_drag_drop_func = None
         self.extra_rc_func = None
         self.selection_binding_func = None
         self.shift_selection_binding_func = None
         self.drag_selection_binding_func = None
-        self.column_width_resize_func = None
+        self.ri_extra_begin_drag_drop_func = None
+        self.ri_extra_end_drag_drop_func = None
+        self.extra_double_b1_func = None
+        self.row_height_resize_func = None
+        self.new_row_width = 0
+        self.cell_options = {}
+        self.drag_and_drop_enabled = False
+        self.dragged_row = None
         self.width_resizing_enabled = False
         self.height_resizing_enabled = False
         self.double_click_resizing_enabled = False
-        self.col_selection_enabled = False
-        self.drag_and_drop_enabled = False
-        self.rc_delete_col_enabled = False
-        self.rc_insert_col_enabled = False
-        self.hide_columns_enabled = False
+        self.row_selection_enabled = False
+        self.rc_insert_row_enabled = False
+        self.rc_delete_row_enabled = False
         self.edit_cell_enabled = False
-        self.dragged_col = None
-        self.visible_col_dividers = {}
-        self.col_height_resize_bbox = tuple()
-        self.cell_options = {}
+        self.visible_row_dividers = {}
+        self.row_width_resize_bbox = tuple()
         self.rsz_w = None
         self.rsz_h = None
-        self.new_col_height = 0
-        self.lines_start_at = 0
         self.currently_resizing_width = False
         self.currently_resizing_height = False
-        self.ch_rc_popup_menu = None
+        self.ri_rc_popup_menu = None
         
         self.disp_text = defaultdict(set)
         self.disp_high = defaultdict(set)
         self.disp_grid = {}
         self.disp_fill_sels = {}
+        self.disp_bord_sels = {}
         self.disp_resize_lines = {}
         self.disp_dropdown = {}
         self.disp_checkbox = {}
         self.hidd_text = defaultdict(set)
         self.hidd_high = defaultdict(set)
         self.hidd_grid = {}
         self.hidd_fill_sels = {}
+        self.hidd_bord_sels = {}
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
         
-        self.column_drag_and_drop_perform = kwargs['column_drag_and_drop_perform']
-        self.default_hdr = kwargs['default_header'].lower()
-        self.max_cw = float(kwargs['max_colwidth'])
-        self.max_header_height = float(kwargs['max_header_height'])
-        self.header_bg = kwargs['header_bg']
-        self.header_fg = kwargs['header_fg']
-        self.header_grid_fg = kwargs['header_grid_fg']
-        self.header_border_fg = kwargs['header_border_fg']
-        self.header_selected_cells_bg = kwargs['header_selected_cells_bg']
-        self.header_selected_cells_fg = kwargs['header_selected_cells_fg']
-        self.header_selected_columns_bg = kwargs['header_selected_columns_bg']
-        self.header_selected_columns_fg = kwargs['header_selected_columns_fg']
-        self.header_hidden_columns_expander_bg = kwargs['header_hidden_columns_expander_bg']
-        self.show_default_header_for_empty = kwargs['show_default_header_for_empty']
+        self.row_drag_and_drop_perform = kwargs['row_drag_and_drop_perform']
+        if kwargs['row_index_width'] is None:
+            self.set_width(70)
+            self.default_width = 70
+        else:
+            self.set_width(kwargs['row_index_width'])
+            self.default_width = kwargs['row_index_width']
+        self.max_rh = float(kwargs['max_rh'])
+        self.max_row_width = float(kwargs['max_row_width'])
+        self.index_fg = kwargs['index_fg']
+        self.index_grid_fg = kwargs['index_grid_fg']
+        self.index_border_fg = kwargs['index_border_fg']
+        self.index_selected_cells_bg = kwargs['index_selected_cells_bg']
+        self.index_selected_cells_fg = kwargs['index_selected_cells_fg']
+        self.index_selected_rows_bg = kwargs['index_selected_rows_bg']
+        self.index_selected_rows_fg = kwargs['index_selected_rows_fg']
+        self.index_hidden_rows_expander_bg = kwargs['index_hidden_rows_expander_bg']
+        self.index_bg = kwargs['index_bg']
         self.drag_and_drop_bg = kwargs['drag_and_drop_bg']
         self.resizing_line_fg = kwargs['resizing_line_fg']
-        self.align = kwargs['header_align']
+        self.align = kwargs['row_index_align']
+        self.show_default_index_for_empty = kwargs['show_default_index_for_empty']
+        self.auto_resize_width = kwargs['auto_resize_width']
+        self.default_index = kwargs['default_row_index'].lower()
         self.basic_bindings()
-        
+
     def basic_bindings(self, enable = True):
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
             self.bind(get_rc_binding(), self.rc)
-            self.bind("<MouseWheel>", self.mousewheel)
         else:
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
             self.unbind(get_rc_binding())
-            self.unbind("<MouseWheel>")
-            
-    def mousewheel(self, event = None):
-        maxlines = 0
-        if isinstance(self.MT._headers, int):
-            if len(self.MT.data) > self.MT._headers:
-                maxlines = max(len(e.rstrip().split("\n")) if isinstance(e, str) else len(f"{e}".rstrip().split("\n")) for e in self.MT.data[self.MT._headers])
-        elif self.MT._headers:
-            maxlines = max(len(e.rstrip().split("\n")) if isinstance(e, str) else len(f"{e}".rstrip().split("\n")) for e in self.MT._headers)
-        if maxlines == 1:
-            maxlines = 0
-        if self.lines_start_at > maxlines:
-            self.lines_start_at = maxlines
-        if (event.delta < 0 or event.num == 5) and self.lines_start_at < maxlines:
-            self.lines_start_at += 1
-        elif (event.delta >= 0 or event.num == 4) and self.lines_start_at > 0:
-            self.lines_start_at -= 1
-        self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = False)
 
-    def set_height(self, new_height, set_TL = False):
-        self.current_height = new_height
+    def set_width(self, new_width, set_TL = False):
+        self.current_width = new_width
         try:
-            self.config(height = new_height)
+            self.config(width = new_width)
         except:
             return
         if set_TL:
-            self.TL.set_dimensions(new_h = new_height)
+            self.TL.set_dimensions(new_w = new_width)
 
     def enable_bindings(self, binding):
-        if binding == "column_width_resize":
+        if binding == "row_width_resize":
             self.width_resizing_enabled = True
-        if binding == "column_height_resize":
+        elif binding == "row_height_resize":
             self.height_resizing_enabled = True
-        if binding == "double_click_column_resize":
+        elif binding == "double_click_row_resize":
             self.double_click_resizing_enabled = True
-        if binding == "column_select":
-            self.col_selection_enabled = True
-        if binding == "drag_and_drop":
+        elif binding == "row_select":
+            self.row_selection_enabled = True
+        elif binding == "drag_and_drop":
             self.drag_and_drop_enabled = True
-        if binding == "hide_columns":
-            self.hide_columns_enabled = True
-
+        
     def disable_bindings(self, binding):
-        if binding == "column_width_resize":
+        if binding == "row_width_resize":
             self.width_resizing_enabled = False
-        if binding == "column_height_resize":
+        elif binding == "row_height_resize":
             self.height_resizing_enabled = False
-        if binding == "double_click_column_resize":
+        elif binding == "double_click_row_resize":
             self.double_click_resizing_enabled = False
-        if binding == "column_select":
-            self.col_selection_enabled = False
-        if binding == "drag_and_drop":
+        elif binding == "row_select":
+            self.row_selection_enabled = False
+        elif binding == "drag_and_drop":
             self.drag_and_drop_enabled = False
-        if binding == "hide_columns":
-            self.hide_columns_enabled = False
 
-    def check_mouse_position_width_resizers(self, x, y):
-        for c, (x1, y1, x2, y2) in self.visible_col_dividers.items():
+    def check_mouse_position_height_resizers(self, x, y):
+        for r, (x1, y1, x2, y2) in self.visible_row_dividers.items():
             if (x >= x1 and
                 y >= y1 and
                 x <= x2 and
                 y <= y2):
-                return c
+                return r
 
     def rc(self, event):
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
-        if self.MT.identify_col(x = event.x, allow_end = False) is None:
+        if self.MT.identify_row(y = event.y, allow_end = False) is None:
             self.MT.deselect("all")
             if self.MT.rc_popup_menus_enabled:
                 popup_menu = self.MT.empty_rc_popup_menu
-        elif self.col_selection_enabled and not self.currently_resizing_width and not self.currently_resizing_height:
-            c = self.MT.identify_col(x = event.x)
-            if c < len(self.MT.col_positions) - 1:
-                if self.MT.col_selected(c):
+        elif self.row_selection_enabled and not self.currently_resizing_width and not self.currently_resizing_height:
+            r = self.MT.identify_row(y = event.y)
+            if r < len(self.MT.row_positions) - 1:
+                if self.MT.row_selected(r):
                     if self.MT.rc_popup_menus_enabled:
-                        popup_menu = self.ch_rc_popup_menu
+                        popup_menu = self.ri_rc_popup_menu
                 else:
                     if self.MT.single_selection_enabled and self.MT.rc_select_enabled:
-                        self.select_col(c, redraw = True)
+                        self.select_row(r, redraw = True)
                     elif self.MT.toggle_selection_enabled and self.MT.rc_select_enabled:
-                        self.toggle_select_col(c, redraw = True)
+                        self.toggle_select_row(r, redraw = True)
                     if self.MT.rc_popup_menus_enabled:
-                        popup_menu = self.ch_rc_popup_menu
+                        popup_menu = self.ri_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def shift_b1_press(self, event):
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.mouseclick_outside_editor_or_dropdown()
-        x = event.x
-        c = self.MT.identify_col(x = x)
-        if self.drag_and_drop_enabled or self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
-            if c < len(self.MT.col_positions) - 1:
-                c_selected = self.MT.col_selected(c)
-                if not c_selected and self.col_selection_enabled:
-                    c = int(c)
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        y = event.y
+        r = self.MT.identify_row(y = y)
+        if self.drag_and_drop_enabled or self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            if r < len(self.MT.row_positions) - 1:
+                r_selected = self.MT.row_selected(r)
+                if not r_selected and self.row_selection_enabled:
+                    r = int(r)
                     currently_selected = self.MT.currently_selected()
-                    if currently_selected and currently_selected.type_ == "column":
-                        min_c = int(currently_selected[1])
+                    if currently_selected and currently_selected.type_ == "row":
+                        min_r = int(currently_selected.row)
                         self.MT.delete_selection_rects(delete_current = False)
-                        if c > min_c:
-                            self.MT.create_selected(0, min_c, len(self.MT.row_positions) - 1, c + 1, "columns")
-                            func_event = tuple(range(min_c, c + 1))
-                        elif c < min_c:
-                            self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, min_c + 1, "columns")
-                            func_event = tuple(range(c, min_c + 1))
+                        if r > min_r:
+                            self.MT.create_selected(min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+                            func_event = tuple(range(min_r, r + 1))
+                        elif r < min_r:
+                            self.MT.create_selected(r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows")
+                            func_event = tuple(range(r, min_r + 1))
                     else:
-                        self.select_col(c)
-                        func_event = (c, )
+                        self.select_row(r)
+                        func_event = (r, )
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.shift_selection_binding_func is not None:
-                        self.shift_selection_binding_func(SelectionBoxEvent("shift_select_columns", func_event))
-                elif c_selected:
-                    self.dragged_col = c
+                        self.shift_selection_binding_func(SelectionBoxEvent("shift_select_rows", func_event))
+                elif r_selected:
+                    self.dragged_row = r
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
                 self.itemconfig(t, width = width, fill = fill, tag = tag)
@@ -263,582 +245,641 @@
 
     def mouse_motion(self, event):
         if not self.currently_resizing_height and not self.currently_resizing_width:
             x = self.canvasx(event.x)
             y = self.canvasy(event.y)
             mouse_over_resize = False
             mouse_over_selected = False
-            if self.width_resizing_enabled:
-                c = self.check_mouse_position_width_resizers(x, y)
-                if c is not None:
-                    self.rsz_w, mouse_over_resize = c, True
-                    self.config(cursor = "sb_h_double_arrow")
-                else:
-                    self.rsz_w = None
             if self.height_resizing_enabled and not mouse_over_resize:
+                r = self.check_mouse_position_height_resizers(x, y)
+                if r is not None:
+                    self.config(cursor = "sb_v_double_arrow")
+                    self.rsz_h = r
+                    mouse_over_resize = True
+                else:
+                    self.rsz_h = None
+            if self.width_resizing_enabled and not mouse_over_resize:
                 try:
-                    x1, y1, x2, y2 = self.col_height_resize_bbox[0], self.col_height_resize_bbox[1], self.col_height_resize_bbox[2], self.col_height_resize_bbox[3]
+                    x1, y1, x2, y2 = self.row_width_resize_bbox[0], self.row_width_resize_bbox[1], self.row_width_resize_bbox[2], self.row_width_resize_bbox[3]
                     if x >= x1 and y >= y1 and x <= x2 and y <= y2:
-                        self.config(cursor = "sb_v_double_arrow")
-                        self.rsz_h = True
+                        self.config(cursor = "sb_h_double_arrow")
+                        self.rsz_w = True
                         mouse_over_resize = True
                     else:
-                        self.rsz_h = None
+                        self.rsz_w = None
                 except:
-                    self.rsz_h = None
+                    self.rsz_w = None
             if not mouse_over_resize:
-                if self.MT.col_selected(self.MT.identify_col(event, allow_end = False)):
+                if self.MT.row_selected(self.MT.identify_row(event, allow_end = False)):
                     self.config(cursor = "hand2")
                     mouse_over_selected = True
             if not mouse_over_resize and not mouse_over_selected:
                 self.MT.reset_mouse_motion_creations()
         if self.extra_motion_func is not None:
             self.extra_motion_func(event)
 
     def double_b1(self, event = None):
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
-        if self.double_click_resizing_enabled and self.width_resizing_enabled and self.rsz_w is not None and not self.currently_resizing_width:
-            col = self.rsz_w - 1
-            old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
-            new_width = self.set_col_width(col)
+        if self.double_click_resizing_enabled and self.height_resizing_enabled and self.rsz_h is not None and not self.currently_resizing_height:
+            row = self.rsz_h - 1
+            old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
+            new_height = self.set_row_height(row)
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-            if self.column_width_resize_func is not None and old_width != new_width:
-                self.column_width_resize_func(ResizeEvent("column_width_resize", col, old_width, new_width))
-        elif self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
-            c = self.MT.identify_col(x = event.x)
-            if c < len(self.MT.col_positions) - 1:
+            if self.row_height_resize_func is not None and old_height != new_height:
+                self.row_height_resize_func(ResizeEvent("row_height_resize", row, old_height, new_height))
+        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
+            self.set_width_of_index_to_text()
+        elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            r = self.MT.identify_row(y = event.y)
+            if r < len(self.MT.row_positions) - 1:
                 if self.MT.single_selection_enabled:
-                    self.select_col(c, redraw = True)
+                    self.select_row(r, redraw = True)
                 elif self.MT.toggle_selection_enabled:
-                    self.toggle_select_col(c, redraw = True)
-                dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                if ((dcol in self.cell_options and 'checkbox' in self.cell_options[dcol]) or
-                    (dcol in self.cell_options and 'dropdown' in self.cell_options[dcol]) or
+                    self.toggle_select_row(r, redraw = True)
+                datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+                if ((datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]) or
+                    (datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]) or
                     self.edit_cell_enabled):
                     self.open_cell(event)
-        self.rsz_w = None
+        self.rsz_h = None
         self.mouse_motion(event)
         if self.extra_double_b1_func is not None:
             self.extra_double_b1_func(event)
         
     def b1_press(self, event = None):
         self.MT.unbind("<MouseWheel>")
         self.focus_set()
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown()
+        self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = self.canvasx(event.x)
         y = self.canvasy(event.y)
-        c = self.MT.identify_col(x = event.x)
-        self.b1_pressed_loc = c
-        if self.check_mouse_position_width_resizers(x, y) is None:
+        r = self.MT.identify_row(y = event.y)
+        self.b1_pressed_loc = r
+        if self.check_mouse_position_height_resizers(x, y) is None:
+            self.rsz_h = None
+        if not x >= self.row_width_resize_bbox[0] and y >= self.row_width_resize_bbox[1] and x <= self.row_width_resize_bbox[2] and y <= self.row_width_resize_bbox[3]:
             self.rsz_w = None
-        if self.width_resizing_enabled and self.rsz_w is not None:
+        if self.height_resizing_enabled and self.rsz_h is not None:
+            self.currently_resizing_height = True
+            y = self.MT.row_positions[self.rsz_h]
+            line2y = self.MT.row_positions[self.rsz_h - 1]
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+            self.create_resize_line(0, y, self.current_width, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+            self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+            self.create_resize_line(0, line2y, self.current_width, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
+            self.MT.create_resize_line(x1, line2y, x2, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
+        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
             self.currently_resizing_width = True
-            x = self.MT.col_positions[self.rsz_w]
-            line2x = self.MT.col_positions[self.rsz_w - 1]
-            self.create_resize_line(x, 0, x, self.current_height, width = 1, fill = self.resizing_line_fg, tag = "rwl")
-            self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
-            self.create_resize_line(line2x, 0, line2x, self.current_height,width = 1, fill = self.resizing_line_fg, tag = "rwl2")
-            self.MT.create_resize_line(line2x, y1, line2x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl2")
-        elif self.height_resizing_enabled and self.rsz_w is None and self.rsz_h is not None:
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-            self.currently_resizing_height = True
-            y = event.y
-            if y < self.MT.hdr_min_rh:
-                y = int(self.MT.hdr_min_rh)
-            self.new_col_height = y
-            self.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
-        elif self.MT.identify_col(x = event.x, allow_end = False) is None:
+            x = int(event.x)
+            if x < self.MT.min_cw:
+                x = int(self.MT.min_cw)
+            self.new_row_width = x
+            self.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+        elif self.MT.identify_row(y = event.y, allow_end = False) is None:
             self.MT.deselect("all")
-        elif self.col_selection_enabled and self.rsz_w is None and self.rsz_h is None:
-            if c < len(self.MT.col_positions) - 1:
-                if self.MT.col_selected(c):
-                    dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                    if ((dcol in self.cell_options and 'dropdown' in self.cell_options[dcol] and x < self.MT.col_positions[c + 1] and x > self.MT.col_positions[c + 1] - self.MT.hdr_txt_h - 4) or
-                        (dcol in self.cell_options and 'checkbox' in self.cell_options[dcol] and x < self.MT.col_positions[c] + self.MT.hdr_txt_h + 5)) and event.y < self.MT.hdr_txt_h + 5:
+        elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            r = self.MT.identify_row(y = event.y)
+            if r < len(self.MT.row_positions) - 1:
+                if self.MT.row_selected(r):
+                    datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+                    if ((datarn in self.cell_options and 'dropdown' in self.cell_options[datarn] and event.x < self.current_width and event.x > self.current_width - self.MT.txt_h - 4) or
+                        (datarn in self.cell_options and 'checkbox' in self.cell_options[datarn] and event.x < self.current_width + self.MT.txt_h + 5)) and y < self.MT.row_positions[r] + self.MT.txt_h + 5:
                         pass
                     else:
-                        self.dragged_col = c
+                        self.dragged_row = r
                 else:
-                    self.being_drawn_rect = (0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
+                    self.being_drawn_rect = (r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
                     if self.MT.single_selection_enabled:
-                        self.select_col(c, redraw = True)
+                        self.select_row(r, redraw = True)
                     elif self.MT.toggle_selection_enabled:
-                        self.toggle_select_col(c, redraw = True)
+                        self.toggle_select_row(r, redraw = True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
     
     def b1_motion(self, event):
-        x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-        if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
-            x = self.canvasx(event.x)
-            size = x - self.MT.col_positions[self.rsz_w - 1]
-            if size >= self.MT.min_cw and size < self.max_cw:
+        x1,y1,x2,y2 = self.MT.get_canvas_visible_area()
+        if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
+            y = self.canvasy(event.y)
+            size = y - self.MT.row_positions[self.rsz_h - 1]
+            if size >= self.MT.min_rh and size < self.max_rh:
                 self.delete_resize_lines()
                 self.MT.delete_resize_lines()
-                line2x = self.MT.col_positions[self.rsz_w - 1]
-                self.create_resize_line(x, 0, x, self.current_height, width = 1, fill = self.resizing_line_fg, tag = "rwl")
-                self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
-                self.create_resize_line(line2x, 0, line2x, self.current_height,width = 1, fill = self.resizing_line_fg, tag = "rwl2")
-                self.MT.create_resize_line(line2x, y1, line2x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl2")
-        elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
-            evy = event.y
+                line2y = self.MT.row_positions[self.rsz_h - 1]
+                self.create_resize_line(0, y, self.current_width, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+                self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+                self.create_resize_line(0, line2y, self.current_width, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
+                self.MT.create_resize_line(x1, line2y, x2, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
+        elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
+            evx = event.x
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            if evy > self.current_height:
-                y = self.MT.canvasy(evy - self.current_height)
-                if evy > self.max_header_height:
-                    evy = int(self.max_header_height)
-                    y = self.MT.canvasy(evy - self.current_height)
-                self.new_col_height = evy
-                self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+            if evx > self.current_width:
+                x = self.MT.canvasx(evx - self.current_width)
+                if evx > self.max_row_width:
+                    evx = int(self.max_row_width)
+                    x = self.MT.canvasx(evx - self.current_width)
+                self.new_row_width = evx
+                self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
             else:
-                y = evy
-                if y < self.MT.hdr_min_rh:
-                    y = int(self.MT.hdr_min_rh)
-                self.new_col_height = y
-                self.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
-        elif self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
-            x = self.canvasx(event.x)
-            if x > 0 and x < self.MT.col_positions[-1]:
-                x = event.x
-                wend = self.winfo_width()
-                xcheck = self.xview()
-                if x >= wend - 0 and len(xcheck) > 1 and xcheck[1] < 1:
-                    if x >= wend + 15:
-                        self.MT.xview_scroll(2, "units")
-                        self.xview_scroll(2, "units")
+                x = evx
+                if x < self.MT.min_cw:
+                    x = int(self.MT.min_cw)
+                self.new_row_width = x
+                self.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+        if self.drag_and_drop_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None and self.MT.anything_selected(exclude_cells = True, exclude_columns = True):
+            y = self.canvasy(event.y)
+            if y > 0 and y < self.MT.row_positions[-1]:
+                y = event.y
+                hend = self.winfo_height()
+                ycheck = self.yview()
+                if y >= hend - 0 and len(ycheck) > 1 and ycheck[1] < 1:
+                    if y >= hend + 15:
+                        self.MT.yview_scroll(2, "units")
+                        self.yview_scroll(2, "units")
                     else:
-                        self.MT.xview_scroll(1, "units")
-                        self.xview_scroll(1, "units")
-                    self.check_xview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_header = True)
-                elif x <= 0 and len(xcheck) > 1 and xcheck[0] > 0:
-                    if x >= -15:
-                        self.MT.xview_scroll(-1, "units")
-                        self.xview_scroll(-1, "units")
+                        self.MT.yview_scroll(1, "units")
+                        self.yview_scroll(1, "units")
+                    self.check_yview()
+                    self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
+                elif y <= 0 and len(ycheck) > 1 and ycheck[0] > 0:
+                    if y >= -15:
+                        self.MT.yview_scroll(-1, "units")
+                        self.yview_scroll(-1, "units")
                     else:
-                        self.MT.xview_scroll(-2, "units")
-                        self.xview_scroll(-2, "units")
-                    self.check_xview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_header = True)
-                col = self.MT.identify_col(x = event.x)
-                sels = self.MT.get_selected_cols()
+                        self.MT.yview_scroll(-2, "units")
+                        self.yview_scroll(-2, "units")
+                    self.check_yview()
+                    self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
+                row = self.MT.identify_row(y = event.y)
+                sels = self.MT.get_selected_rows()
                 selsmin = min(sels)
-                if col in sels:
-                    xpos = self.MT.col_positions[selsmin]
+                if row in sels:
+                    ypos = self.MT.row_positions[selsmin]
                 else:
-                    if col < selsmin:
-                        xpos = self.MT.col_positions[col]
+                    if row < selsmin:
+                        ypos = self.MT.row_positions[row]
                     else:
-                        xpos = self.MT.col_positions[col + 1]
+                        ypos = self.MT.row_positions[row + 1]
                 self.delete_resize_lines()
                 self.MT.delete_resize_lines()
-                self.create_resize_line(xpos, 0, xpos, self.current_height, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
-                self.MT.create_resize_line(xpos, y1, xpos, y2, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
-        elif self.MT.drag_selection_enabled and self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+                self.create_resize_line(0, ypos, self.current_width, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+                self.MT.create_resize_line(x1, ypos, x2, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+        elif self.MT.drag_selection_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             need_redraw = False
-            end_col = self.MT.identify_col(x = event.x)
+            end_row = self.MT.identify_row(y = event.y)
             currently_selected = self.MT.currently_selected()
-            if end_col < len(self.MT.col_positions) - 1 and currently_selected:
-                if currently_selected.type_ == "column":
-                    start_col = currently_selected[1]
-                    if end_col >= start_col:
-                        rect = (0, start_col, len(self.MT.row_positions) - 1, end_col + 1, "columns")
-                        func_event = tuple(range(start_col, end_col + 1))
-                    elif end_col < start_col:
-                        rect = (0, end_col, len(self.MT.row_positions) - 1, start_col + 1, "columns")
-                        func_event = tuple(range(end_col, start_col + 1))
+            if end_row < len(self.MT.row_positions) - 1 and currently_selected:
+                if currently_selected.type_ == "row":
+                    start_row = currently_selected.row
+                    if end_row >= start_row:
+                        rect = (start_row, 0, end_row + 1, len(self.MT.col_positions) - 1, "rows")
+                        func_event = tuple(range(start_row, end_row + 1))
+                    elif end_row < start_row:
+                        rect = (end_row, 0, start_row + 1, len(self.MT.col_positions) - 1, "rows")
+                        func_event = tuple(range(end_row, start_row + 1))
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         self.MT.delete_selection_rects(delete_current = False)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
-                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
-                xcheck = self.xview()
-                if event.x > self.winfo_width() and len(xcheck) > 1 and xcheck[1] < 1:
-                    try:
-                        self.MT.xview_scroll(1, "units")
-                        self.xview_scroll(1, "units")
-                    except:
-                        pass
-                    self.check_xview()
-                    need_redraw = True
-                elif event.x < 0 and self.canvasx(self.winfo_width()) > 0 and xcheck and xcheck[0] > 0:
-                    try:
-                        self.xview_scroll(-1, "units")
-                        self.MT.xview_scroll(-1, "units")
-                    except:
-                        pass
-                    self.check_xview()
-                    need_redraw = True
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
+            ycheck = self.yview()
+            if event.y > self.winfo_height() and len(ycheck) > 1 and ycheck[1] < 1:
+                try:
+                    self.MT.yview_scroll(1, "units")
+                    self.yview_scroll(1, "units")
+                except:
+                    pass
+                self.check_yview()
+                need_redraw = True
+            elif event.y < 0 and self.canvasy(self.winfo_height()) > 0 and ycheck and ycheck[0] > 0:
+                try:
+                    self.yview_scroll(-1, "units")
+                    self.MT.yview_scroll(-1, "units")
+                except:
+                    pass
+                self.check_yview()
+                need_redraw = True
             if need_redraw:
-                self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False)
+                self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
 
-    def check_xview(self):
-        xcheck = self.xview()
-        if xcheck and xcheck[0] < 0:
-            self.MT.set_xviews("moveto", 0)
-        elif len(xcheck) > 1 and xcheck[1] > 1:
-            self.MT.set_xviews("moveto", 1)
+    def check_yview(self):
+        ycheck = self.yview()
+        if ycheck and ycheck[0] < 0:
+            self.MT.set_yviews("moveto", 0)
+        if len(ycheck) > 1 and ycheck[1] > 1:
+            self.MT.set_yviews("moveto", 1)
             
     def b1_release(self, event = None):
         if self.being_drawn_rect is not None:
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.MT.create_selected(*to_sel)
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
-        if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
-            self.currently_resizing_width = False
-            new_col_pos = int(self.coords("rwl")[0])
+        if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
+            self.currently_resizing_height = False
+            new_row_pos = int(self.coords("rhl")[1])
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
-            size = new_col_pos - self.MT.col_positions[self.rsz_w - 1]
-            if size < self.MT.min_cw:
-                new_col_pos = ceil(self.MT.col_positions[self.rsz_w - 1] + self.MT.min_cw)
-            elif size > self.max_cw:
-                new_col_pos = floor(self.MT.col_positions[self.rsz_w - 1] + self.max_cw)
-            increment = new_col_pos - self.MT.col_positions[self.rsz_w]
-            self.MT.col_positions[self.rsz_w + 1:] = [e + increment for e in islice(self.MT.col_positions, self.rsz_w + 1, len(self.MT.col_positions))]
-            self.MT.col_positions[self.rsz_w] = new_col_pos
-            new_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
+            old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
+            size = new_row_pos - self.MT.row_positions[self.rsz_h - 1]
+            if size < self.MT.min_rh:
+                new_row_pos = ceil(self.MT.row_positions[self.rsz_h - 1] + self.MT.min_rh)
+            elif size > self.max_rh:
+                new_row_pos = floor(self.MT.row_positions[self.rsz_h - 1] + self.max_rh)
+            increment = new_row_pos - self.MT.row_positions[self.rsz_h]
+            self.MT.row_positions[self.rsz_h + 1:] = [e + increment for e in islice(self.MT.row_positions, self.rsz_h + 1, len(self.MT.row_positions))]
+            self.MT.row_positions[self.rsz_h] = new_row_pos
+            new_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             self.MT.recreate_all_selection_boxes()
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-            if self.column_width_resize_func is not None and old_width != new_width:
-                self.column_width_resize_func(ResizeEvent("column_width_resize", self.rsz_w - 1, old_width, new_width))
-        elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
-            self.currently_resizing_height = False
+            if self.row_height_resize_func is not None and old_height != new_height:
+                self.row_height_resize_func(ResizeEvent("row_height_resize", self.rsz_h - 1, old_height, new_height))
+        elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
+            self.currently_resizing_width = False
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            self.set_height(self.new_col_height,set_TL = True)
+            self.set_width(self.new_row_width, set_TL = True)
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-        elif self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
+        if self.drag_and_drop_enabled and self.MT.anything_selected(exclude_cells = True, exclude_columns = True) and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None:
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            x = event.x
-            c = self.MT.identify_col(x = x)
-            orig_selected = self.MT.get_selected_cols()
-            if c != self.dragged_col and c is not None and c not in orig_selected and len(orig_selected) != len(self.MT.col_positions) - 1:
+            y = event.y
+            r = self.MT.identify_row(y = y)
+            orig_selected = self.MT.get_selected_rows()
+            if r != self.dragged_row and r is not None and r not in orig_selected and len(orig_selected) != (len(self.MT.row_positions) - 1):
                 orig_selected = sorted(orig_selected)
                 if len(orig_selected) > 1:
-                    start_idx = bisect.bisect_left(orig_selected, self.dragged_col)
+                    orig_min = orig_selected[0]
+                    orig_max = orig_selected[1]
+                    start_idx = bisect.bisect_left(orig_selected, self.dragged_row)
                     forward_gap = get_index_of_gap_in_sorted_integer_seq_forward(orig_selected, start_idx)
                     reverse_gap = get_index_of_gap_in_sorted_integer_seq_reverse(orig_selected, start_idx)
                     if forward_gap is not None:
                         orig_selected[:] = orig_selected[:forward_gap]
                     if reverse_gap is not None:
                         orig_selected[:] = orig_selected[reverse_gap:]
                 rm1start = orig_selected[0]
-                totalcols = len(orig_selected)
+                totalrows = len(orig_selected)
                 extra_func_success = True
-                if c >= len(self.MT.col_positions) - 1:
-                    c -= 1
-                if self.ch_extra_begin_drag_drop_func is not None:
+                if r >= len(self.MT.row_positions) - 1:
+                    r -= 1
+                if self.ri_extra_begin_drag_drop_func is not None:
                     try:
-                        self.ch_extra_begin_drag_drop_func(BeginDragDropEvent("begin_column_header_drag_drop", tuple(orig_selected), int(c)))
+                        self.ri_extra_begin_drag_drop_func(BeginDragDropEvent("begin_row_index_drag_drop", tuple(orig_selected), int(r)))
                     except:
                         extra_func_success = False
                 if extra_func_success:
-                    new_selected, dispset = self.MT.move_columns_adjust_options_dict(c,
-                                                                                     rm1start, 
-                                                                                     totalcols,
-                                                                                     move_data = self.column_drag_and_drop_perform)
+                    new_selected, dispset = self.MT.move_rows_adjust_options_dict(r, 
+                                                                                  rm1start, totalrows, move_data = self.row_drag_and_drop_perform)
                     if self.MT.undo_enabled:
-                        self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_cols",                 #0
-                                                                                int(orig_selected[0]),  #1
-                                                                                int(new_selected[0]),        #2
-                                                                                int(new_selected[-1]),       #3
-                                                                                sorted(orig_selected),  #4
-                                                                                dispset))))                  #5
+                        self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_rows",
+                                                                                min(orig_selected),
+                                                                                new_selected[0],
+                                                                                new_selected[-1],
+                                                                                sorted(orig_selected)))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-                    if self.ch_extra_end_drag_drop_func is not None:
-                        self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", tuple(orig_selected), new_selected, int(c)))
+                    if self.ri_extra_end_drag_drop_func is not None:
+                        self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", tuple(orig_selected), new_selected, int(r)))
+                        
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
-            c = self.MT.identify_col(x = event.x)
-            if c is not None and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
-                dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                canvasx = self.canvasx(event.x)
-                if ((dcol in self.cell_options and 'dropdown' in self.cell_options[dcol] and canvasx < self.MT.col_positions[c + 1] and canvasx > self.MT.col_positions[c + 1] - self.MT.hdr_txt_h - 4) or
-                    (dcol in self.cell_options and 'checkbox' in self.cell_options[dcol] and canvasx < self.MT.col_positions[c] + self.MT.hdr_txt_h + 5)):
-                    if event.y < self.MT.hdr_txt_h + 5:
-                        self.open_cell(event)
+            r = self.MT.identify_row(y = event.y)
+            if r is not None and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
+                datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+                if (self.canvasy(event.y) < self.MT.row_positions[r] + self.MT.txt_h and
+                    (
+                     (datarn in self.cell_options and 
+                      'dropdown' in self.cell_options[datarn] and 
+                      event.x < self.current_width and 
+                      event.x > self.current_width - self.MT.txt_h - 4) 
+                    or
+                     (datarn in self.cell_options and 
+                      'checkbox' in self.cell_options[datarn] and
+                      event.x < self.MT.txt_h + 5)
+                     )
+                ):
+                    self.open_cell(event)
             else:
-                self.mouseclick_outside_editor_or_dropdown()
+                self.mouseclick_outside_editor_or_dropdown_all_canvases()
             self.b1_pressed_loc = None
-            self.closed_dropdown = None
-        self.dragged_col = None
+            self.closed_dropdown = None    
+        self.dragged_row = None
         self.currently_resizing_width = False
         self.currently_resizing_height = False
         self.rsz_w = None
         self.rsz_h = None
         self.mouse_motion(event)
         if self.extra_b1_release_func is not None:
             self.extra_b1_release_func(event)
             
-    def readonly_header(self, columns = [], readonly = True):
-        if isinstance(columns, int):
-            columns_ = [columns]
+    def readonly_index(self, rows = [], readonly = True):
+        if isinstance(rows, int):
+            rows_ = [rows]
         else:
-            columns_ = columns
+            rows_ = rows
         if not readonly:
-            for c in columns_:
-                if c in self.cell_options and 'readonly' in self.cell_options[c]:
-                    del self.cell_options[c]['readonly']
-        else:
-            for c in columns_:
-                if c not in self.cell_options:
-                    self.cell_options[c] = {}
-                self.cell_options[c]['readonly'] = True
+            for r in rows_:
+                if r in self.cell_options and 'readonly' in self.cell_options[r]:
+                    del self.cell_options[r]['readonly']
+        else:
+            for r in rows_:
+                if r not in self.cell_options:
+                    self.cell_options[r] = {}
+                self.cell_options[r]['readonly'] = True
 
-    def highlight_cells(self, c = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
+    def highlight_cells(self, r = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
         if bg is None and fg is None:
             return
         if cells and not isinstance(cells, int):
             iterable = cells
         elif isinstance(cells, int):
             iterable = (cells, )
         else:
-            iterable = (c, )
-        for c_ in iterable:
-            if c_ not in self.cell_options:
-                self.cell_options[c_] = {}
-            if 'highlight' in self.cell_options[c_] and not overwrite:
-                self.cell_options[c_]['highlight'] = (self.cell_options[c_]['highlight'][0] if bg is None else bg,
-                                                      self.cell_options[c_]['highlight'][1] if fg is None else fg)
+            iterable = (r, )
+        for r_ in iterable:
+            if r_ not in self.cell_options:
+                self.cell_options[r_] = {}
+            if 'highlight' in self.cell_options[r_] and not overwrite:
+                self.cell_options[r_]['highlight'] = (self.cell_options[r_]['highlight'][0] if bg is None else bg,
+                                                        self.cell_options[r_]['highlight'][1] if fg is None else fg)
             else:
-                self.cell_options[c_]['highlight'] = (bg, fg)
+                self.cell_options[r_]['highlight'] = (bg, fg)
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(True, False)
+            self.MT.main_table_redraw_grid_and_text(False, True)
 
-    def select_col(self, c, redraw = False, keep_other_selections = False):
+    def select_row(self, r, redraw = False, keep_other_selections = False):
         ignore_keep = False
         if keep_other_selections:
-            if self.MT.col_selected(c):
-                self.MT.create_current(0, c, type_ = "column", inside = True)
+            if self.MT.row_selected(r):
+                self.MT.create_current(r, 0, type_ = "row", inside = True)
             else:
                 ignore_keep = True
         if ignore_keep or not keep_other_selections:
             self.MT.delete_selection_rects()
-            self.MT.create_current(0, c, type_ = "column", inside = True)
-            self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
+            self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+            self.MT.create_current(r, 0, type_ = "row", inside = True)
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
-            self.selection_binding_func(SelectColumnEvent("select_column", int(c)))
+            self.selection_binding_func(SelectRowEvent("select_row", int(r)))
 
-    def toggle_select_col(self, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
+    def toggle_select_row(self, row, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
-            if self.MT.col_selected(column):
-                self.MT.deselect(c = column, redraw = redraw)
+            if self.MT.row_selected(row):
+                self.MT.deselect(r = row, redraw = redraw)
             else:
-                self.add_selection(c = column, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+                self.add_selection(r = row, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
         else:
-            if self.MT.col_selected(column):
-                self.MT.deselect(c = column, redraw = redraw)
+            if self.MT.row_selected(row):
+                self.MT.deselect(r = row, redraw = redraw)
             else:
-                self.select_col(column, redraw = redraw)
+                self.select_row(row, redraw = redraw)
 
-    def add_selection(self, c, redraw = False, run_binding_func = True, set_as_current = True):
-        c = int(c)
+    def add_selection(self, r, redraw = False, run_binding_func = True, set_as_current = True):
+        r = int(r)
         if set_as_current:
             create_new_sel = False
             current = self.MT.get_tags_of_current()
             if current:
                 if current[0] == "Current_Outside":
                     create_new_sel = True
-            self.MT.create_current(0, c, type_ = "column", inside = True)
+            self.MT.create_current(r, 0, type_ = "row", inside = True)
             if create_new_sel:
                 r1, c1, r2, c2 = tuple(int(e) for e in current[1].split("_") if e)
                 self.MT.create_selected(r1, c1, r2, c2, current[2] + "s")
-        self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
+        self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+            self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
-            self.selection_binding_func(("select_column", int(c)))
+            self.selection_binding_func(("select_row", int(r)))
 
-    def set_col_width(self, col, width = None, only_set_if_too_small = False, displayed_only = False, recreate = True, return_new_width = False):
-        if col < 0:
-            return
-        qconf = self.MT.txt_measure_canvas.itemconfig
-        qbbox = self.MT.txt_measure_canvas.bbox
-        qtxtm = self.MT.txt_measure_canvas_text
-        qtxth = self.MT.txt_h
-        qclop = self.MT.cell_options
-        qfont = self.MT._font
-        if width is None:
-            w = self.MT.min_cw
-            hw = self.MT.min_cw
-            if displayed_only:
-                x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                start_row, end_row = self.MT.get_visible_rows(y1, y2)
-            else:
-                start_row, end_row = 0, None
+    def set_row_height(self, row, height = None, only_set_if_too_small = False, recreate = True, return_new_height = False, displayed_only = False):
+        r_norm = row + 1
+        r_extra = row + 2
+        min_rh = self.MT.min_rh
+        datarn = row if self.MT.all_rows_displayed else self.MT.displayed_rows[row]
+        if height is None:
             if self.MT.all_columns_displayed:
-                data_col = col
+                if displayed_only:
+                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+                    start_col, end_col = self.MT.get_visible_columns(x1, x2)
+                else:
+                    start_col, end_col = 0, len(self.MT.data[row]) if self.MT.data else 0
+                iterable = range(start_col, end_col)
             else:
-                data_col = self.MT.displayed_columns[col]
-            # header
-            if data_col in self.cell_options and 'checkbox' in self.cell_options[data_col]:
-                qconf(qtxtm, text = self.cell_options[data_col]['checkbox']['text'], font = self.MT._hdr_font)
-                b = qbbox(qtxtm)
-                hw = b[2] - b[0] + 7 + self.MT.hdr_txt_h
-            else:
-                txt = ""
-                if isinstance(self.MT._headers, int) or len(self.MT._headers) - 1 >= data_col:
-                    if isinstance(self.MT._headers, int):
-                        txt = self.MT.data[self.MT._headers][data_col]
+                if displayed_only:
+                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+                    start_col, end_col = self.MT.get_visible_columns(x1, x2)
+                else:
+                    start_col, end_col = 0, len(self.MT.displayed_columns)
+                iterable = self.MT.displayed_columns[start_col:end_col]
+            new_height = int(min_rh)
+            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+                txt = self.cell_options[datarn]['checkbox']['text']
+            else:
+                txt = self.get_valid_cell_data_as_str(datarn, fix = False)
+            if txt:
+                h = self.MT.GetTextHeight(txt) + 5
+            else:
+                h = min_rh
+            if h < min_rh:
+                h = int(min_rh)
+            elif h > self.max_rh:
+                h = int(self.max_rh)
+            if h > new_height:
+                new_height = h
+            if self.MT.data:
+                for cn in iterable:
+                    if (datarn, cn) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(datarn, cn)]:
+                        txt = self.MT.cell_options[(datarn, cn)]['checkbox']['text']
                     else:
-                        txt = self.MT._headers[data_col]
-                    if txt or (data_col in self.cell_options and 'dropdown' in self.cell_options[data_col]):
-                        qconf(qtxtm, text = txt, font = self.MT._hdr_font)
-                        b = qbbox(qtxtm)
-                        if data_col in self.cell_options and 'dropdown' in self.cell_options[data_col]:
-                            hw = b[2] - b[0] + 7 + self.MT.hdr_txt_h
-                        else:
-                            hw = b[2] - b[0] + 7
-                if not isinstance(self.MT._headers, int) and ((not txt and self.show_default_header_for_empty) or len(self.MT._headers) < data_col):
-                    if self.default_hdr == "letters":
-                        hw = self.MT.GetHdrTextWidth(num2alpha(data_col)) + 7
-                    elif self.default_hdr == "numbers":
-                        hw = self.MT.GetHdrTextWidth(f"{data_col + 1}") + 7
+                        txt = self.MT.get_valid_cell_data_as_str(datarn, cn, get_displayed = True)
+                    if txt:
+                        h = self.MT.GetTextHeight(txt) + 5
                     else:
-                        hw = self.MT.GetHdrTextWidth(f"{data_col + 1} {num2alpha(data_col)}") + 7
-            # table
-            for rn, r in enumerate(islice(self.MT.data, start_row, end_row), start_row):
-                if (rn, data_col) in qclop and 'checkbox' in qclop[(rn, data_col)]:
-                    qconf(qtxtm, text = qclop[(rn, data_col)]['checkbox']['text'], font = qfont)
-                    b = qbbox(qtxtm)
-                    tw = qtxth + 7 + b[2] - b[0]
-                    if tw > w:
-                        w = tw
+                        h = min_rh
+                    if h < min_rh:
+                        h = int(min_rh)
+                    elif h > self.max_rh:
+                        h = int(self.max_rh)
+                    if h > new_height:
+                        new_height = h
+        else:
+            new_height = int(height)
+        if new_height < min_rh:
+            new_height = int(min_rh)
+        elif new_height > self.max_rh:
+            new_height = int(self.max_rh)
+        if only_set_if_too_small and new_height <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
+            return self.MT.row_positions[row + 1] - self.MT.row_positions[row]
+        if not return_new_height:
+            new_row_pos = self.MT.row_positions[row] + new_height
+            increment = new_row_pos - self.MT.row_positions[r_norm]
+            self.MT.row_positions[r_extra:] = [e + increment for e in islice(self.MT.row_positions, r_extra, len(self.MT.row_positions))]
+            self.MT.row_positions[r_norm] = new_row_pos
+            if recreate:
+                self.MT.recreate_all_selection_boxes()
+        return new_height
+
+    def set_width_of_index_to_text(self, recreate = True):
+        if not self.MT._row_index and isinstance(self.MT._row_index, list):
+            return
+        qconf = self.MT.txt_measure_canvas.itemconfig
+        qbbox = self.MT.txt_measure_canvas.bbox
+        qtxtm = self.MT.txt_measure_canvas_text
+        new_width = int(self.MT.min_cw)
+        if isinstance(self.MT._row_index, list):
+            for rn, row in enumerate(self.MT._row_index):
+                if rn in self.cell_options and 'checkbox' in self.cell_options[rn]:
+                    txt = self.cell_options[rn]['checkbox']['text']
                 else:
                     try:
-                        if isinstance(r[data_col], str):
-                            txt = r[data_col]
+                        if isinstance(row, str):
+                            txt = row
                         else:
-                            txt = f"{r[data_col]}"
+                            txt = f"{row}"
                     except:
-                        continue
-                    if txt:
-                        qconf(qtxtm, text = txt, font = qfont)
-                        b = qbbox(qtxtm)
-                        tw = b[2] - b[0] + qtxth + 7 if (rn, data_col) in qclop and 'dropdown' in qclop[(rn, data_col)] else b[2] - b[0] + 7
-                        if tw > w:
-                            w = tw
-            if w > hw:
-                new_width = w
-            else:
-                new_width = hw
-        else:
-            new_width = int(width)
-        if new_width <= self.MT.min_cw:
-            new_width = int(self.MT.min_cw)
-        elif new_width > self.max_cw:
-            new_width = int(self.max_cw)
-        if only_set_if_too_small:
-            if new_width <= self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
-                return self.MT.col_positions[col + 1] - self.MT.col_positions[col]
-        if not return_new_width:
-            new_col_pos = self.MT.col_positions[col] + new_width
-            increment = new_col_pos - self.MT.col_positions[col + 1]
-            self.MT.col_positions[col + 2:] = [e + increment for e in islice(self.MT.col_positions, col + 2, len(self.MT.col_positions))]
-            self.MT.col_positions[col + 1] = new_col_pos
-            if recreate:
-                self.MT.recreate_all_selection_boxes()
-        return new_width
+                        txt = ""
+                if txt:
+                    qconf(qtxtm, text = txt)
+                    b = qbbox(qtxtm)
+                    w = b[2] - b[0] + 10
+                else:
+                    w = self.default_width
+                if w < self.MT.min_cw:
+                    w = int(self.MT.min_cw)
+                elif w > self.max_row_width:
+                    w = int(self.max_row_width)
+                if rn in self.cell_options and 'checkbox' in self.cell_options[rn]:
+                    w += self.MT.txt_h + 6
+                elif rn in self.cell_options and 'dropdown' in self.cell_options[rn]:
+                    w += self.MT.txt_h + 4
+                if w > new_width:
+                    new_width = w
+        elif isinstance(self.MT._row_index, int):
+            c = self.MT._row_index
+            for rn, row in enumerate(self.MT.data):
+                if (rn, c) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(rn, c)]:
+                    txt = self.MT.cell_options[(rn, c)]['checkbox']['text']
+                else:
+                    txt = self.MT.get_valid_cell_data_as_str(rn, c, get_displayed = True)
+                if txt:
+                    qconf(qtxtm, text = txt)
+                    b = qbbox(qtxtm)
+                    w = b[2] - b[0] + 10
+                else:
+                    w = self.default_width
+                if w < self.MT.min_cw:
+                    w = int(self.MT.min_cw)
+                elif w > self.max_row_width:
+                    w = int(self.max_row_width)
+                if w > new_width:
+                    new_width = w
+        if new_width == self.MT.min_cw:
+            new_width = self.MT.min_cw + 10
+        self.set_width(new_width, set_TL = True)
+        if recreate:
+            self.MT.recreate_all_selection_boxes()
+        self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
 
-    def set_width_of_all_cols(self, width = None, only_set_if_too_small = False, recreate = True):
-        if width is None:
-            if self.MT.all_columns_displayed:
-                iterable = range(self.MT.total_data_cols())
-            else:
-                iterable = range(len(self.MT.displayed_columns))
-            self.MT.col_positions = list(accumulate(chain([0], (self.set_col_width(cn, only_set_if_too_small = only_set_if_too_small, recreate = False, return_new_width = True) for cn in iterable))))
-        elif width is not None:
-            if self.MT.all_columns_displayed:
-                self.MT.col_positions = list(accumulate(chain([0], (width for cn in range(self.MT.total_data_cols())))))
-            else:
-                self.MT.col_positions = list(accumulate(chain([0], (width for cn in range(len(self.MT.displayed_columns))))))
+    def set_height_of_all_rows(self, height = None, only_set_if_too_small = False, recreate = True):
+        if height is None:
+            self.MT.row_positions = list(accumulate(chain([0], (self.set_row_height(rn, only_set_if_too_small = only_set_if_too_small, recreate = False, return_new_height = True) for rn in range(len(self.MT.data))))))
+        else:
+            self.MT.row_positions = list(accumulate(chain([0], (height for r in range(len(self.MT.data))))))
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
-    def align_cells(self, columns = [], align = "global"):
-        if isinstance(columns, int):
-            cols = [columns]
+    def align_cells(self, rows = [], align = "global"):
+        if isinstance(rows, int):
+            rows = [rows]
         else:
-            cols = columns
+            rows = rows
         if align == "global":
-            for c in cols:
-                if c in self.cell_options and 'align' in self.cell_options[c]:
-                    del self.cell_options[c]['align']
-        else:
-            for c in cols:
-                if c not in self.cell_options:
-                    self.cell_options[c] = {}
-                self.cell_options[c]['align'] = align
+            for r in rows:
+                if r in self.cell_options and 'align' in self.cell_options[r]:
+                    del self.cell_options[r]['align']
+        else:
+            for r in rows:
+                if r not in self.cell_options:
+                    self.cell_options[r] = {}
+                self.cell_options[r]['align'] = align
+
+    def auto_set_index_width(self, end_row):
+        if not self.MT._row_index and not isinstance(self.MT._row_index, int) and self.auto_resize_width:
+            if self.default_index == "letters":
+                new_w = self.MT.GetTextWidth(f"{num2alpha(end_row)}") + 20
+                if self.current_width - new_w > 15 or new_w - self.current_width > 5:
+                    self.set_width(new_w, set_TL = True)
+                    return True
+            elif self.default_index == "numbers":
+                new_w = self.MT.GetTextWidth(f"{end_row}") + 20
+                if self.current_width - new_w > 15 or new_w - self.current_width > 5:
+                    self.set_width(new_w, set_TL = True)
+                    return True
+            elif self.default_index == "both":
+                new_w = self.MT.GetTextWidth(f"{end_row + 1} {num2alpha(end_row)}") + 20
+                if self.current_width - new_w > 15 or new_w - self.current_width > 5:
+                    self.set_width(new_w, set_TL = True)
+                    return True
+        return False
 
-    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, hlcol):
+    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, hlrow):
         redrawn = False
-        if hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol] and c in actual_selected_cols:
-            if self.cell_options[hlcol]['highlight'][0] is not None:
-                c_1 = self.cell_options[hlcol]['highlight'][0] if self.cell_options[hlcol]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[hlcol]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1,
-                                                0,
-                                                sc,
-                                                self.current_height - 1,
+        if r in self.cell_options and 'highlight' in self.cell_options[r] and r in actual_selected_rows:
+            if self.cell_options[r]['highlight'][0] is not None:
+                c_1 = self.cell_options[r]['highlight'][0] if self.cell_options[r]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[r]['highlight'][0]]
+                redrawn = self.redraw_highlight(0,
+                                                fr + 1,
+                                                self.current_width - 1,
+                                                sr,
                                                 fill = (f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"),
-                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "",
-                                                tag = "hi")
-            fill = self.header_selected_columns_fg if self.cell_options[hlcol]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[hlcol]['highlight'][1]
-        elif hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol] and (c in selected_cols or selected_rows):
-            if self.cell_options[hlcol]['highlight'][0] is not None:
-                c_1 = self.cell_options[hlcol]['highlight'][0] if self.cell_options[hlcol]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[hlcol]['highlight'][0]]
-                redrawn = self.redraw_highlight(fc + 1,
-                                                0,
-                                                sc,
-                                                self.current_height - 1,
+                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "",
+                                                tag = "s")
+            fill = self.index_selected_rows_fg if self.cell_options[r]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[r]['highlight'][1]
+        elif r in self.cell_options and 'highlight' in self.cell_options[r] and (r in selected_rows or selected_cols):
+            if self.cell_options[r]['highlight'][0] is not None:
+                c_1 = self.cell_options[r]['highlight'][0] if self.cell_options[r]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[r]['highlight'][0]]
+                redrawn = self.redraw_highlight(0,
+                                                fr + 1,
+                                                self.current_width - 1,
+                                                sr,
                                                 fill = (f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"),
-                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "", 
-                                                tag = "hi")
-            fill = self.header_selected_cells_fg if self.cell_options[hlcol]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[hlcol]['highlight'][1]
-        elif c in actual_selected_cols:
-            fill = self.header_selected_columns_fg
-        elif c in selected_cols or selected_rows:
-            fill = self.header_selected_cells_fg
-        elif hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol]:
-            if self.cell_options[hlcol]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1,
-                                                0, 
-                                                sc, 
-                                                self.current_height - 1, 
-                                                fill = self.cell_options[hlcol]['highlight'][0], 
-                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "", 
-                                                tag = "hi")
-            fill = self.header_fg if self.cell_options[hlcol]['highlight'][1] is None else self.cell_options[hlcol]['highlight'][1]
+                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "",
+                                                tag = "s")
+            fill = self.index_selected_cells_fg if self.cell_options[r]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[r]['highlight'][1]
+        elif r in actual_selected_rows:
+            fill = self.index_selected_rows_fg
+        elif r in selected_rows or selected_cols:
+            fill = self.index_selected_cells_fg
+        elif r in self.cell_options and 'highlight' in self.cell_options[r]:
+            if self.cell_options[r]['highlight'][0] is not None:
+                redrawn = self.redraw_highlight(0, 
+                                                fr + 1, 
+                                                self.current_width - 1, 
+                                                sr,
+                                                fill = self.cell_options[r]['highlight'][0], 
+                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "", 
+                                                tag = "s")
+            fill = self.index_fg if self.cell_options[r]['highlight'][1] is None else self.cell_options[r]['highlight'][1]
         else:
-            fill = self.header_fg
+            fill = self.index_fg
         return fill, redrawn
-            
+
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
-        coords = (x1 - 1 if outline else x1,
-                  y1 - 1 if outline else y1,
-                  x2, 
-                  y2)
+        coords = (x1, y1, x2, y2)
         k = None
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
             if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
@@ -865,45 +906,45 @@
         
         if k is not None and not self.hidd_high[k]:
             del self.hidd_high[k]
 
         self.disp_high[config].add(DrawnItem(iid = iid, showing = 1))
         return True
 
-    def redraw_gridline(self,points, fill, width, tag):
+    def redraw_gridline(self, points, fill, width, tag):
         if self.hidd_grid:
             t, sh = self.hidd_grid.popitem()
             self.coords(t, points)
             if sh:
-                self.itemconfig(t, fill = fill, width = width, tag = tag, capstyle = tk.BUTT, joinstyle = tk.ROUND)
+                self.itemconfig(t, fill = fill, width = width, tag = tag)
             else:
-                self.itemconfig(t, fill = fill, width = width, tag = tag, capstyle = tk.BUTT, joinstyle = tk.ROUND, state = "normal")
+                self.itemconfig(t, fill = fill, width = width, tag = tag, state = "normal")
             self.disp_grid[t] = True
         else:
             self.disp_grid[self.create_line(points, fill = fill, width = width, tag = tag)] = True
             
     def redraw_dropdown(self, x1, y1, x2, y2, fill, outline, tag, draw_outline = True, draw_arrow = True, dd_is_open = False):
         if draw_outline and self.MT.show_dropdown_borders:
-            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.header_fg, tag = tag)
+            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.index_fg, tag = tag)
         if draw_arrow:
-            topysub = floor(self.MT.hdr_half_txt_h / 2)
-            mid_y = y1 + floor(self.MT.hdr_min_rh / 2)
-            if mid_y + topysub + 1 >= y1 + self.MT.hdr_txt_h - 1:
+            topysub = floor(self.MT.half_txt_h / 2)
+            mid_y = y1 + floor(self.MT.min_rh / 2)
+            if mid_y + topysub + 1 >= y1 + self.MT.txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
                 ty2 = mid_y - topysub + 3 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
             else:
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 2
                 ty2 = mid_y - topysub + 2 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 2
-            tx1 = x2 - self.MT.hdr_txt_h + 1
-            tx2 = x2 - self.MT.hdr_half_txt_h - 1
+            tx1 = x2 - self.MT.txt_h + 1
+            tx2 = x2 - self.MT.half_txt_h - 1
             tx3 = x2 - 3
             if tx2 - tx1 > tx3 - tx2:
                 tx1 += (tx2 - tx1) - (tx3 - tx2)
             elif tx2 - tx1 < tx3 - tx2:
                 tx1 -= (tx3 - tx2) - (tx2 - tx1)
             points = (tx1, ty1, tx2, ty2, tx3, ty3)
             if self.hidd_dropdown:
@@ -914,15 +955,15 @@
                 else:
                     self.itemconfig(t, fill = fill, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_line(points, fill = fill, width = 2, capstyle = tk.ROUND, joinstyle = tk.ROUND, tag = tag)
             self.disp_dropdown[t] = True
             
-    def redraw_checkbox(self, dcol, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
+    def redraw_checkbox(self, r, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
         points = self.MT.get_checkbox_points(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill = outline, outline = fill)
             else:
@@ -946,19 +987,22 @@
                 else:
                     self.itemconfig(t, fill = fill, outline = outline, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill = fill, outline = outline, tag = tag, smooth = True)
             self.disp_checkbox[t] = True
 
-    def redraw_grid_and_text(self, last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, selected_cols, selected_rows, actual_selected_cols):
-        self.configure(scrollregion = (0,
-                                       0,
-                                       last_col_line_pos + self.MT.empty_horizontal,
-                                       self.current_height))
+    def redraw_grid_and_text(self, last_row_line_pos, scrollpos_top, y_stop, start_row, end_row, scrollpos_bot, selected_rows, selected_cols, actual_selected_rows, row_pos_exists):
+        try:
+            self.configure(scrollregion = (0,
+                                           0,
+                                           self.current_width,
+                                           last_row_line_pos + self.MT.empty_vertical))
+        except:
+            return
         for k, v in self.disp_text.items():
             if k in self.hidd_text:
                 self.hidd_text[k] = self.hidd_text[k] | self.disp_text[k]
             else:
                 self.hidd_text[k] = v
         self.disp_text = defaultdict(set)
         for k, v in self.disp_high.items():
@@ -969,137 +1013,134 @@
         self.disp_high = defaultdict(set)
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
         self.disp_dropdown = {}
         self.hidd_checkbox.update(self.disp_checkbox)
         self.disp_checkbox = {}
-        self.visible_col_dividers = {}
-        self.col_height_resize_bbox = (scrollpos_left, self.current_height - 2, x_stop, self.current_height)
-        draw_x = self.MT.col_positions[start_col]
-        yend = self.current_height - 5
-        if self.MT.show_vertical_grid or self.width_resizing_enabled:
+        self.visible_row_dividers = {}
+        draw_y = self.MT.row_positions[start_row]
+        xend = self.current_width - 6
+        self.row_width_resize_bbox = (self.current_width - 2, scrollpos_top, self.current_width, scrollpos_bot)
+        if (self.MT.show_horizontal_grid or self.height_resizing_enabled) and row_pos_exists:
             self.grid_cyc = cycle(self.grid_cyctup)
-            points = []
-            for c in range(start_col + 1, end_col):
-                draw_x = self.MT.col_positions[c]
-                if self.width_resizing_enabled:
-                    self.visible_col_dividers[c] = (draw_x - 2, 1, draw_x + 2, yend)
+            points = [self.current_width - 1, y_stop - 1, 
+                      self.current_width - 1, scrollpos_top - 1,
+                      -1, scrollpos_top - 1]
+            for r in range(start_row + 1, end_row):
+                draw_y = self.MT.row_positions[r]
+                if self.height_resizing_enabled:
+                    self.visible_row_dividers[r] = (1, draw_y - 2, xend, draw_y + 2)
                 st_or_end = next(self.grid_cyc)
                 if st_or_end == "st":
-                    points.extend([draw_x, -1,
-                                   draw_x, self.current_height,
-                                   self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x, self.current_height])
+                    points.extend([-1, draw_y,
+                                   self.current_width, draw_y,
+                                   self.current_width, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
                 elif st_or_end == "end":
-                    points.extend([draw_x, self.current_height,
-                                   draw_x, -1,
-                                   self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x, -1])
+                    points.extend([self.current_width, draw_y,
+                                   -1, draw_y,
+                                   -1, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
                 if points:
-                    self.redraw_gridline(points = points, fill = self.header_grid_fg, width = 1, tag = "v")
-        self.redraw_gridline(points = (draw_x, 0, draw_x, self.current_height), fill = self.header_grid_fg, width = 1, tag = "fv")
-        self.redraw_gridline(points = (scrollpos_left, self.current_height - 1, x_stop, self.current_height - 1), fill = self.header_border_fg, width = 1, tag = "h")
-        top = self.canvasy(0)
-        c_2 = self.header_selected_cells_bg if self.header_selected_cells_bg.startswith("#") else Color_Map_[self.header_selected_cells_bg]
-        c_3 = self.header_selected_columns_bg if self.header_selected_columns_bg.startswith("#") else Color_Map_[self.header_selected_columns_bg]
-        font = self.MT._hdr_font
-        for c in range(start_col, end_col - 1):
-            draw_y = self.MT.hdr_fl_ins
-            cleftgridln = self.MT.col_positions[c]
-            crightgridln = self.MT.col_positions[c + 1]
-            if self.MT.all_columns_displayed:
-                dcol = c
+                    self.redraw_gridline(points = points, fill = self.index_grid_fg, width = 1, tag = "h")
+        scrollpos_bot_add2 = scrollpos_bot + 2
+        c_2 = self.index_selected_cells_bg if self.index_selected_cells_bg.startswith("#") else Color_Map_[self.index_selected_cells_bg]
+        c_3 = self.index_selected_rows_bg if self.index_selected_rows_bg.startswith("#") else Color_Map_[self.index_selected_rows_bg]
+        font = self.MT._font
+        for r in range(start_row, end_row - 1):
+            rtopgridln = self.MT.row_positions[r]
+            rbotgridln = self.MT.row_positions[r + 1]
+            if rbotgridln - rtopgridln < self.MT.txt_h:
+                continue
+            if rbotgridln > scrollpos_bot_add2:
+                rbotgridln = scrollpos_bot_add2
+            if self.MT.all_rows_displayed:
+                datarn = r
             else:
-                dcol = self.MT.displayed_columns[c]
-            fill, dd_drawn = self.redraw_highlight_get_text_fg(cleftgridln, crightgridln, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, dcol)
-
-            if dcol in self.cell_options and 'align' in self.cell_options[dcol]:
-                align = self.cell_options[dcol]['align']
+                datarn = self.MT.displayed_rows[r]
+            fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, datarn)
+            
+            if r in self.cell_options and 'align' in self.cell_options[r]:
+                align = self.cell_options[r]['align']
             else:
                 align = self.align
                 
             if align == "w":
-                draw_x = cleftgridln + 3
-                if dcol in self.cell_options and 'dropdown' in self.cell_options[dcol]:
-                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
-                    self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1, 
+                draw_x = 3
+                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
+                    mw = self.current_width - self.MT.txt_h - 2
+                    self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[dcol]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
                 else:
-                    mw = crightgridln - cleftgridln - 1
+                    mw = self.current_width - 2
 
             elif align == "e":
-                if dcol in self.cell_options and 'dropdown' in self.cell_options[dcol]:
-                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
-                    draw_x = crightgridln - 5 - self.MT.hdr_txt_h
-                    self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1,
+                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
+                    mw = self.current_width - self.MT.txt_h - 2
+                    draw_x = self.current_width - 5 - self.MT.txt_h
+                    self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[dcol]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
                 else:
-                    mw = crightgridln - cleftgridln - 1
-                    draw_x = crightgridln - 3
+                    mw = self.current_width - 2
+                    draw_x = self.current_width - 3
 
             elif align == "center":
-                #stop = cleftgridln + 5
-                if dcol in self.cell_options and 'dropdown' in self.cell_options[dcol]:
-                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
-                    draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.MT.hdr_txt_h) / 2)
-                    self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1, 
+                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
+                    mw = self.current_width - self.MT.txt_h - 2
+                    draw_x = ceil((self.current_width - self.MT.txt_h) / 2)
+                    self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[dcol]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
                 else:
-                    mw = crightgridln - cleftgridln - 1
-                    draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
+                    mw = self.current_width - 1
+                    draw_x = floor(self.current_width / 2)
 
-            if dcol in self.cell_options and 'checkbox' in self.cell_options[dcol]:
-                if mw > self.MT.hdr_txt_h + 2:
-                    box_w = self.MT.hdr_txt_h + 1
+            if r in self.cell_options and 'checkbox' in self.cell_options[r]:
+                if mw > + 2:
+                    box_w = self.MT.txt_h + 1
                     mw -= box_w
                     if align == "w":
                         draw_x += box_w + 1
                     elif align == "center":
                         draw_x += ceil(box_w / 2) + 1
                         mw -= 1
                     else:
                         mw -= 3
                     try:
-                        draw_check = self.MT._headers[dcol] if isinstance(self.MT._headers, (list, tuple)) else self.MT.data[self.MT._headers][dcol]
+                        draw_check = self.MT._row_index[r] if isinstance(self.MT._row_index, (list, tuple)) else self.MT.data[r][self.MT._row_index]
                     except:
                         draw_check = False
-                    self.redraw_checkbox(dcol,
-                                         cleftgridln + 2,
+                    self.redraw_checkbox(r,
                                          2,
-                                         cleftgridln + self.MT.hdr_txt_h + 3,
-                                         self.MT.hdr_txt_h + 3,
-                                         fill = fill if self.cell_options[dcol]['checkbox']['state'] == "normal" else self.header_grid_fg,
+                                         rtopgridln + 2,
+                                         self.MT.txt_h + 3,
+                                         rtopgridln + self.MT.txt_h + 3,
+                                         fill = fill if self.cell_options[r]['checkbox']['state'] == "normal" else self.index_grid_fg,
                                          outline = "",
-                                         tag = "cb", 
+                                         tag = "cb",
                                          draw_check = draw_check)
-
-            try:
-                if dcol in self.cell_options and 'checkbox' in self.cell_options[dcol]:
-                    lns = self.cell_options[dcol]['checkbox']['text'].split("\n") if isinstance(self.cell_options[dcol]['checkbox']['text'], str) else f"{self.cell_options[dcol]['checkbox']['text']}".split("\n")
-                elif isinstance(self.MT._headers, int):
-                    lns = self.MT.data[self.MT._headers][dcol].split("\n") if isinstance(self.MT.data[self.MT._headers][dcol], str) else f"{self.MT.data[self.MT._headers][dcol]}".split("\n")
-                else:
-                    lns = self.MT._headers[dcol].split("\n") if isinstance(self.MT._headers[dcol], str) else f"{self.MT._headers[dcol]}".split("\n")
-                got_hdr = True
-            except:
-                got_hdr = False
-            if not got_hdr or (lns == [""] and self.show_default_header_for_empty):
-                if self.default_hdr == "letters":
-                    lns = (num2alpha(dcol), )
-                elif self.default_hdr == "numbers":
-                    lns = (f"{dcol + 1}", )
+            if r in self.cell_options and 'checkbox' in self.cell_options[r]:
+                lns = self.cell_options[r]['checkbox']['text'].split("\n") if isinstance(self.cell_options[r]['checkbox']['text'], str) else f"{self.cell_options[r]['checkbox']['text']}".split("\n")
+            else:
+                lns = self.get_valid_cell_data_as_str(r, fix = False).split("\n")
+            if lns == [""]:
+                if self.show_default_index_for_empty:
+                    lns = (get_n2a(r, self.default_index), )
                 else:
-                    lns = (f"{dcol + 1} {num2alpha(dcol)}", )
-            if mw > self.MT.hdr_txt_w and not ((align == "w" and (draw_x > x_stop)) or
-                                               (align == "e" and (draw_x > x_stop)) or
-                                               (align == "center" and (cleftgridln + 5 > x_stop))):
-                for txt in islice(lns, self.lines_start_at if self.lines_start_at < len(lns) else len(lns) - 1, None):
-                    if draw_y > top:
+                    continue
+            draw_y = rtopgridln + self.MT.fl_ins
+            if mw > 5:
+                draw_y = rtopgridln + self.MT.fl_ins
+                start_ln = int((scrollpos_top - rtopgridln) / self.MT.xtra_lines_increment)
+                if start_ln < 0:
+                    start_ln = 0
+                draw_y += start_ln * self.MT.xtra_lines_increment
+                if draw_y + self.MT.half_txt_h - 1 <= rbotgridln and len(lns) > start_ln:
+                    for txt in islice(lns, start_ln, None):
                         config = TextCfg(txt, fill, font, align)
                         k = None
                         if config in self.hidd_text:
                             k = config
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
                             if (int(cc1) == int(draw_x) and
@@ -1126,283 +1167,253 @@
                             else:
                                 self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align, state = "normal")
                         if k is not None and not self.hidd_text[k]:
                             del self.hidd_text[k]
                         wd = self.bbox(iid)
                         wd = wd[2] - wd[0]
                         if wd > mw:
-                            if align == "w":
+                            if align == "w" and datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
                                 txt = txt[:int(len(txt) * (mw / wd))]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[:-1]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
-                            elif align == "e":
+                            elif align == "e" and datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
                                 txt = txt[len(txt) - int(len(txt) * (mw / wd)):]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[1:]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
-                            elif align == "center":
-                                self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
+                            elif align == "center" and ((datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]) or (datarn in self.cell_options and 'dropdown' in self.cell_options[datarn])):
                                 tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
                                 txt = txt[tmod - 1:-tmod]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
+                                self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[next(self.c_align_cyc)]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
                                 self.coords(iid, draw_x, draw_y)
-                            self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = 1))
+                            self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
                         else:
-                            self.disp_text[config].add(DrawnItem(iid = iid, showing = 1))
-                    draw_y += self.MT.hdr_xtra_lines_increment
-                    if draw_y - 1 > self.current_height:
-                        break
+                            self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
+                        draw_y += self.MT.xtra_lines_increment
+                        if draw_y + self.MT.half_txt_h - 1 > rbotgridln:
+                            break
         self.tag_raise("t")
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
                     self.hidd_text[cfg].discard(namedtup)
-                    self.hidd_text[cfg].add(namedtup._replace(showing = 0))
+                    self.hidd_text[cfg].add(namedtup._replace(showing = False))
         for cfg, set_ in self.hidd_high.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
                     self.hidd_high[cfg].discard(namedtup)
-                    self.hidd_high[cfg].add(namedtup._replace(showing = 0))
+                    self.hidd_high[cfg].add(namedtup._replace(showing = False))
         for t, sh in self.hidd_grid.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_grid[t] = False
         for t, sh in self.hidd_dropdown.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_dropdown[t] = False
         for t, sh in self.hidd_checkbox.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_checkbox[t] = False
                 
     def open_cell(self, event = None, ignore_existing_editor = False):
-        if not self.MT.anything_selected()  or (not ignore_existing_editor and self.text_editor_id is not None):
+        if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
-        x1 = int(currently_selected[1])
-        dcol = x1 if self.MT.all_columns_displayed else self.MT.displayed_columns[x1]
-        if dcol in self.cell_options and 'readonly' in self.cell_options[dcol]:
+        r = int(currently_selected[0])
+        datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        if datarn in self.cell_options and 'readonly' in self.cell_options[datarn]:
             return
-        elif dcol in self.cell_options and ('dropdown' in self.cell_options[dcol] or 'checkbox' in self.cell_options[dcol]):
+        elif datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 'checkbox' in self.cell_options[datarn]):
             if self.MT.event_opens_dropdown_or_checkbox(event):
-                if 'dropdown' in self.cell_options[dcol]:
-                    self.display_dropdown_window(x1, event = event)
-                elif 'checkbox' in self.cell_options[dcol]:
-                    self._click_checkbox(x1, dcol)
+                if 'dropdown' in self.cell_options[datarn]:
+                    self.open_dropdown_window(r, event = event)
+                elif 'checkbox' in self.cell_options[datarn]:
+                    self._click_checkbox(r, datarn)
         elif self.edit_cell_enabled:
-            self.edit_cell_(event, c = x1, dropdown = False)
+            self.edit_cell_(event, r = r, dropdown = False)
 
-    # c is displayed col
-    def edit_cell_(self, event = None, c = None, dropdown = False):
+    # r is displayed row
+    def edit_cell_(self, event = None, r = None, dropdown = False):
         text = None
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, 'keysym') and event.keysym == 'Return':
                     extra_func_key = "Return"
                 elif hasattr(event, 'keysym') and event.keysym == 'F2':
                     extra_func_key = "F2"
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            if isinstance(self.MT._headers, list):
-                if len(self.MT._headers) <= dcol:
-                    self.MT._headers.extend(list(repeat("", dcol - len(self.MT._headers) + 1)))
-                text = f"{self.MT._headers[dcol]}"
-            elif isinstance(self.MT._headers, int):
-                try:
-                    text = f"{self.MT.data[self.MT._headers][dcol]}"
-                except:
-                    text = ""
-            
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+            text = self.get_cell_data(datarn, redirect_int = True)
         elif event is not None and ((hasattr(event, 'keysym') and event.keysym == 'BackSpace') or
-                                  event.keycode in (8, 855638143)
-                                  ):
+                                    event.keycode in (8, 855638143)):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and ((hasattr(event, "char") and event.char.isalpha()) or
                                     (hasattr(event, "char") and event.char.isdigit()) or
                                     (hasattr(event, "char") and event.char in symbols_set)):
             extra_func_key = event.char
             text = event.char
         else:
             return False
-        self.text_editor_loc = c
+        self.text_editor_loc = r
         if self.extra_begin_edit_cell_func is not None:
             try:
-                text = self.extra_begin_edit_cell_func(EditHeaderEvent(c, extra_func_key, text, "begin_edit_header"))
+                text = self.extra_begin_edit_cell_func(EditIndexEvent(r, extra_func_key, text, "begin_edit_index"))
             except:
                 return False
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
-            if self.height_resizing_enabled:
-                self.set_current_height_to_cell(dcol)
-            self.set_col_width_run_binding(c)
-        self.select_col(c = c, keep_other_selections = True)
-        self.create_text_editor(c = c, text = text, set_data_ref_on_destroy = True, dropdown = dropdown)
+            self.set_row_height_run_binding(r)
+        self.select_row(r = r, keep_other_selections = True, redraw = not dropdown)
+        self.create_text_editor(r = r, text = text, set_data_on_close = True, dropdown = dropdown)
         return True
     
     # displayed indexes
-    def get_cell_align(self, c):
-        dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if dcol in self.cell_options and 'align' in self.cell_options[dcol]:
-            align = self.cell_options[dcol]['align']
+    def get_cell_align(self, r):
+        datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        if datarn in self.cell_options and 'align' in self.cell_options[datarn]:
+            align = self.cell_options[datarn]['align']
         else:
             align = self.align
         return align
 
-    # c is displayed col
+    # r is displayed row
     def create_text_editor(self,
-                           c = 0,
+                           r = 0,
                            text = None,
                            state = "normal",
                            see = True,
-                           set_data_ref_on_destroy = False,
+                           set_data_on_close = False,
                            binding = None,
                            dropdown = False):
-        if c == self.text_editor_loc and self.text_editor is not None:
+        if r == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
-            has_redrawn = self.MT.see(r = 0, c = c, keep_yscroll = True, check_cell_visibility = True)
+            has_redrawn = self.MT.see(r = r, c = 0, keep_yscroll = True, check_cell_visibility = True)
             if not has_redrawn:
                 self.MT.refresh()
-        self.text_editor_loc = c
-        x = self.MT.col_positions[c] + 1
-        y = 0
-        w = self.MT.col_positions[c + 1] - x
-        h = self.current_height + 1
-        dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+        self.text_editor_loc = r
+        x = 0
+        y = self.MT.row_positions[r] + 1
+        w = self.current_width + 1
+        h = self.MT.row_positions[r + 1] - y
+        datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if text is None:
-            if isinstance(self.MT._headers, list):
-                if len(self.MT._headers) <= dcol:
-                    self.MT._headers.extend(list(repeat("", dcol - len(self.MT._headers) + 1)))
-                text = f"{self.MT._headers[dcol]}"
-            elif isinstance(self.MT._headers, int):
-                try:
-                    text = f"{self.MT.data[self.MT._headers][dcol]}"
-                except:
-                    text = ""
-        #bg, fg = self.get_widget_bg_fg(dcol)
-        bg, fg = self.header_bg, self.header_fg
+            text = self.get_valid_cell_data_as_str(datarn)
+        bg, fg = self.index_bg, self.index_fg
         self.text_editor = TextEditor(self,
                                       text = text,
-                                      font = self.MT._hdr_font,
+                                      font = self.MT._font,
                                       state = state,
                                       width = w,
                                       height = h,
                                       border_color = self.MT.table_selected_cells_border_fg,
                                       show_border = False,
                                       bg = bg,
                                       fg = fg,
                                       popup_menu_font = self.MT.popup_menu_font,
                                       popup_menu_fg = self.MT.popup_menu_fg,
                                       popup_menu_bg = self.MT.popup_menu_bg,
                                       popup_menu_highlight_bg = self.MT.popup_menu_highlight_bg,
                                       popup_menu_highlight_fg = self.MT.popup_menu_highlight_fg,
                                       binding = binding,
-                                      align = self.get_cell_align(c),
-                                      c = c,
-                                      newline_binding = self.text_editor_has_wrapped)
+                                      align = self.get_cell_align(r),
+                                      r = r,
+                                      newline_binding = self.text_editor_newline_binding)
         self.text_editor.update_idletasks()
         self.text_editor_id = self.create_window((x, y), window = self.text_editor, anchor = "nw")
         if not dropdown:
             self.text_editor.textedit.focus_set()
             self.text_editor.scroll_to_bottom()
-        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(c = c))
+        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(r = r))
         if USER_OS == 'darwin':
-            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(c = c))
+            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(r = r))
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.textedit.bind(key, func)
         if binding is not None:
-            self.text_editor.textedit.bind("<Tab>", lambda x: binding((c, "Tab")))
-            self.text_editor.textedit.bind("<Return>", lambda x: binding((c, "Return")))
-            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((c, "FocusOut")))
-            self.text_editor.textedit.bind("<Escape>", lambda x: binding((c, "Escape")))
-        elif binding is None and set_data_ref_on_destroy:
-            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((c, "Tab")))
-            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((c, "Return")))
+            self.text_editor.textedit.bind("<Tab>", lambda x: binding((r, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: binding((r, "Return")))
+            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, "Escape")))
+        elif binding is None and set_data_on_close:
+            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, "Return")))
             if not dropdown:
-                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((c, "FocusOut")))
-            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((c, "Escape")))
+                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, "Escape")))
         else:
             self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
-    
-    # displayed indexes                            #just here to receive text editor arg
-    def text_editor_has_wrapped(self, r = 0, c = 0, check_lines = None):
-        if self.width_resizing_enabled:
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            curr_width = self.text_editor.winfo_width()
-            new_width = curr_width + (self.MT.hdr_txt_h * 2)
-            if new_width != curr_width:
-                self.text_editor.config(width = new_width)
-                self.set_col_width_run_binding(c, width = new_width, only_set_if_too_small = False)
-                if dcol in self.cell_options and 'dropdown' in self.cell_options[dcol]:
-                    self.itemconfig(self.cell_options[dcol]['dropdown']['canvas_id'],
-                                    width = new_width)
-                    self.cell_options[dcol]['dropdown']['window'].update_idletasks()
-                    self.cell_options[dcol]['dropdown']['window']._reselect()
-                self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = True)
-    
-    # displayed indexes
+            
     def text_editor_newline_binding(self, r = 0, c = 0, event = None, check_lines = True):
         if self.height_resizing_enabled:
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             curr_height = self.text_editor.winfo_height()
-            if not check_lines or self.MT.GetHdrLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
-                new_height = curr_height + self.MT.hdr_xtra_lines_increment
-                space_bot = self.MT.get_space_bot(0)
+            if not check_lines or self.MT.GetLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
+                new_height = curr_height + self.MT.xtra_lines_increment
+                space_bot = self.MT.get_space_bot(r)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
+                    self.set_row_height(datarn, new_height)
+                    self.MT.refresh()
                     self.text_editor.config(height = new_height)
-                    self.set_height(new_height, set_TL = True)
-                    if dcol in self.cell_options and 'dropdown' in self.cell_options[dcol]:
-                        win_h, anchor = self.get_dropdown_height_anchor(dcol, new_height)
-                        self.coords(self.cell_options[dcol]['dropdown']['canvas_id'],
-                                    self.MT.col_positions[c], new_height - 1)
-                        self.itemconfig(self.cell_options[dcol]['dropdown']['canvas_id'],
-                                        anchor = anchor, height = win_h)
+                    if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+                        text_editor_h = self.text_editor.winfo_height()
+                        win_h, anchor = self.get_dropdown_height_anchor(datarn, text_editor_h)
+                        if anchor == "nw":
+                            self.coords(self.cell_options[datarn]['dropdown']['canvas_id'],
+                                        self.MT.col_positions[c], self.MT.row_positions[r] + text_editor_h - 1)
+                            self.itemconfig(self.cell_options[datarn]['dropdown']['canvas_id'],
+                                            anchor = anchor, height = win_h)
+                        elif anchor == "sw":
+                            self.coords(self.cell_options[datarn]['dropdown']['canvas_id'],
+                                        self.MT.col_positions[c], self.MT.row_positions[r])
+                            self.itemconfig(self.cell_options[datarn]['dropdown']['canvas_id'],
+                                            anchor = anchor, height = win_h)
             
     def bind_cell_edit(self, enable = True):
         if enable:
             self.edit_cell_enabled = True
         else:
             self.edit_cell_enabled = False
 
-    def bind_text_editor_destroy(self, binding, c):
-        self.text_editor.textedit.bind("<Return>", lambda x: binding((c, "Return")))
-        self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((c, "FocusOut")))
-        self.text_editor.textedit.bind("<Escape>", lambda x: binding((c, "Escape")))
+    def bind_text_editor_destroy(self, binding, r):
+        self.text_editor.textedit.bind("<Return>", lambda x: binding((r, "Return")))
+        self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, "FocusOut")))
+        self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, "Escape")))
         self.text_editor.textedit.focus_set()
 
     def destroy_text_editor(self, event = None):
         if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
-            self.extra_end_edit_cell_func(EditHeaderEvent(int(self.text_editor_loc), "Escape", None, "escape_edit_header"))
+            self.extra_end_edit_cell_func(EditHeaderEvent(int(self.text_editor_loc), "Escape", None, "escape_edit_index"))
         self.text_editor_loc = None
         try:
             self.delete(self.text_editor_id)
         except:
             pass
         try:
             self.text_editor.destroy()
@@ -1415,294 +1426,374 @@
         try:
             self.text_editor_id = None
         except:
             pass
         if event is not None and len(event) >= 3 and "Escape" in event:
             self.focus_set()
 
-    # c is displayed col
-    def close_text_editor(self, editor_info = None, c = None, set_data_ref_on_destroy = True, event = None, destroy = True, move_down = True, redraw = True, recreate = True):
+    # r is displayed row
+    def close_text_editor(self, editor_info = None, r = None, set_data_on_close = True, event = None, destroy = True, move_down = True, redraw = True, recreate = True):
         if self.focus_get() is None and editor_info:
-            return
+            return "break"
         if editor_info is not None and len(editor_info) >= 2 and editor_info[1] == "Escape":
             self.destroy_text_editor("Escape")
-            self.hide_dropdown_window(c)
-            return
+            self.close_dropdown_window(r)
+            return "break"
         if self.text_editor is not None:
             self.text_editor_value = self.text_editor.get()
         if destroy:
             self.destroy_text_editor()
-        if set_data_ref_on_destroy:
-            if c is None and editor_info is not None and len(editor_info) >= 2:
-                c = editor_info[0]
-            if self.extra_end_edit_cell_func is None:
-                self._set_cell_data(c, dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c], value = self.text_editor_value)
-            elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation:
-                self._set_cell_data(c, dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c], value = self.text_editor_value)
-                self.extra_end_edit_cell_func(EditHeaderEvent(c, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_header"))
+        if set_data_on_close:
+            if r is None and editor_info is not None and len(editor_info) >= 2:
+                r = editor_info[0]
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(datarn, self.text_editor_value):
+                self.set_cell_data_undo(r, datarn = datarn, value = self.text_editor_value, check_input_valid = False)
+            elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation and self.input_valid_for_cell(datarn, self.text_editor_value):
+                self.set_cell_data_undo(r, datarn = datarn, value = self.text_editor_value, check_input_valid = False)
+                self.extra_end_edit_cell_func(EditIndexEvent(r, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_index"))
             elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
-                validation = self.extra_end_edit_cell_func(EditHeaderEvent(c, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_header"))
+                validation = self.extra_end_edit_cell_func(EditIndexEvent(r, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_index"))
                 if validation is not None:
                     self.text_editor_value = validation
-                    self._set_cell_data(c, dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c], value = self.text_editor_value)
+                    if self.input_valid_for_cell(datarn, self.text_editor_value):
+                        self.set_cell_data_undo(r, datarn = datarn, value = self.text_editor_value, check_input_valid = False)
         if move_down:
             pass
-        self.hide_dropdown_window(c)
+        self.close_dropdown_window(r)
         if recreate:
             self.MT.recreate_all_selection_boxes()
         if redraw:
             self.MT.refresh()
         if editor_info is not None and len(editor_info) >= 2 and editor_info[1] != "FocusOut":
             self.focus_set()
         return "break"
-    
+
     #internal event use
-    def _set_cell_data(self, c = 0, dcol = None, value = "", cell_resize = True, undo = True, redraw = True):
-        if dcol is None:
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if isinstance(self.MT._headers, list):
-            if len(self.MT._headers) <= dcol:
-                self.MT._headers.extend(list(repeat("", dcol - len(self.MT._headers) + 1)))
-            if self.MT.undo_enabled and undo:
-                if self.MT._headers[dcol] != value:
-                    self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_header",
-                                                                           {dcol: self.MT._headers[dcol]},
-                                                                           (((0, c, len(self.MT.row_positions) - 1, c + 1), "columns"), ),
-                                                                           self.MT.currently_selected()))))
-            self.MT._headers[dcol] = value
-        elif isinstance(self.MT._headers, int):
-            self.MT._set_cell_data(r = self.MT._headers, c = c, dcol = dcol, value = value, undo = True)
+    def set_cell_data_undo(self, r = 0, datarn = None, value = "", cell_resize = True, undo = True, redraw = True, check_input_valid = True):
+        if datarn is None:
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        if isinstance(self.MT._row_index, int):
+            self.MT.set_cell_data_undo(r = r, c = self.MT._row_index, datarn = datarn, value = value, undo = True)
+        else:
+            self.fix_index(datarn)
+            if not check_input_valid or self.input_valid_for_cell(datarn, value):
+                if self.MT.undo_enabled and undo:
+                    self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_index",
+                                                                            {datarn: self.MT._row_index[datarn]},
+                                                                            (((r, 0, r + 1, len(self.MT.col_positions) - 1), "rows"), ),
+                                                                            self.MT.currently_selected()))))
+                self.set_cell_data(datarn = datarn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
-            if self.height_resizing_enabled:
-                self.set_current_height_to_cell(dcol)
-            self.set_col_width_run_binding(c)
+            self.set_row_height_run_binding(r, only_set_if_too_small = False)
         if redraw:
             self.MT.refresh()
+
+    def set_cell_data(self, datarn = None, value = ""):
+        if isinstance(self.MT._row_index, int):
+            self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
+        else:
+            self.fix_index(datarn)
+            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+                self.MT._row_index[datarn] = to_bool(value)
+            else:
+                self.MT._row_index[datarn] = value
+            
+    def input_valid_for_cell(self, datarn, value):
+        if datarn in self.cell_options:
+            if 'readonly' in self.cell_options[datarn]:
+                return False
+            if 'checkbox' in self.cell_options[datarn]:
+                return is_bool_like(value)
+        if self.cell_equal_to(datarn, value):
+            return False
+        if (datarn in self.cell_options and 
+            'dropdown' in self.cell_options[datarn] and 
+            self.cell_options[datarn]['dropdown']['validate_input'] and 
+            value not in self.cell_options[datarn]['dropdown']['values']):
+            return False
         return True
     
-    # displayed indexes
-    def set_col_width_run_binding(self, c, width = None, only_set_if_too_small = True):
-        old_width = self.MT.col_positions[c + 1] - self.MT.col_positions[c]
-        new_width = self.set_col_width(c, width = width, only_set_if_too_small = only_set_if_too_small)
-        if self.column_width_resize_func is not None and old_width != new_width:
-            self.column_width_resize_func(ResizeEvent("column_width_resize", c, old_width, new_width))
+    def cell_equal_to(self, datarn, value):
+        self.fix_index(datarn)
+        if isinstance(self.MT._row_index, list):
+            if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+                try:
+                    return to_bool(self.MT._row_index[datarn]) == to_bool(value)
+                except:
+                    return False
+            return self.MT._row_index[datarn] == value
+        elif isinstance(self.MT._row_index, int):
+            return self.MT.cell_equal_to(datarn, self.MT._row_index, value)
+            
+    def get_cell_data(self, datarn, get_displayed = False, redirect_int = False):
+        if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None and get_displayed:
+            return self.cell_options[datarn]['dropdown']['text']
+        if redirect_int and isinstance(self.MT._row_index, int):
+            return self.MT.get_cell_data(datarn, self.MT._row_index, none_to_empty_str = True)
+        if isinstance(self.MT._row_index, int) or not self.MT._row_index or datarn >= len(self.MT._row_index) or not self.MT._row_index[datarn]:
+            if get_displayed and self.show_default_index_for_empty:
+                return get_n2a(datarn, self.default_index)
+            else:
+                return ""
+        return self.MT._row_index[datarn]
+            
+    def get_valid_cell_data_as_str(self, datarn, fix = True) -> str:
+        if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn] and self.cell_options[datarn]['dropdown']['text'] is not None:
+            return f"{self.cell_options[datarn]['dropdown']['text']}"
+        if isinstance(self.MT._row_index, int):
+            return self.MT.get_valid_cell_data_as_str(datarn, self.MT._row_index, get_displayed = True)
+        if fix:
+            self.fix_index(datarn)
+        try:
+            return f"{self.MT._row_index[datarn]}"
+        except:
+            return ""
+            
+    def fix_index(self, datarn = None):
+        if isinstance(self.MT._row_index, int):
+            return
+        if isinstance(self.MT._row_index, float):
+            self.MT._row_index = int(self.MT._row_index)
+            return
+        if not isinstance(self.MT._row_index, list):
+            try:
+                self.MT._row_index = list(self.MT._row_index)
+            except:
+                self.MT._row_index = []
+        if isinstance(datarn, int) and datarn >= len(self.MT._row_index):
+            self.MT._row_index.extend(list(repeat("", datarn - len(self.MT._row_index) + 1)))
+            
+    def set_row_height_run_binding(self, r, only_set_if_too_small = True):
+        old_height = self.MT.row_positions[r + 1] - self.MT.row_positions[r]
+        new_height = self.set_row_height(r, only_set_if_too_small = only_set_if_too_small)
+        if self.row_height_resize_func is not None and old_height != new_height:
+            self.row_height_resize_func(ResizeEvent("row_height_resize", r, old_height, new_height))
 
     #internal event use
-    def _click_checkbox(self, c, dcol = None, undo = True, redraw = True):
-        if dcol is None:
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if self.cell_options[dcol]['checkbox']['state'] == "normal":
-            if isinstance(self.MT._headers, list):
-                self._set_cell_data(c, dcol = dcol, value = not self.MT._headers[dcol] if type(self.MT._headers[dcol]) == bool else False, cell_resize = False)
-            elif isinstance(self.MT._headers, int):
-                self._set_cell_data(c, dcol = dcol, value = not self.MT.data[self.MT._headers][dcol] if type(self.MT.data[self.MT._headers][dcol]) == bool else False, cell_resize = False)
-            if self.cell_options[dcol]['checkbox']['check_function'] is not None:
-                self.cell_options[dcol]['checkbox']['check_function']((0, c, "HeaderCheckboxClicked", f"{self.MT._headers[dcol] if isinstance(self.MT._headers, list) else self.MT.data[self.MT._headers][dcol]}"))
+    def _click_checkbox(self, r, datarn = None, undo = True, redraw = True):
+        if datarn is None:
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        if self.cell_options[datarn]['checkbox']['state'] == "normal":
+            if isinstance(self.MT._row_index, list):
+                value = not self.MT._row_index[datarn] if type(self.MT._row_index[datarn]) == bool else False
+            elif isinstance(self.MT._row_index, int):
+                value = not self.MT.data[self.MT._row_index][datarn] if type(self.MT.data[self.MT._row_index][datarn]) == bool else False
+            else:
+                value = False
+            self.set_cell_data_undo(r, 
+                                    datarn = datarn, 
+                                    value = value, 
+                                    cell_resize = False)
+            if self.cell_options[datarn]['checkbox']['check_function'] is not None:
+                self.cell_options[datarn]['checkbox']['check_function']((r,
+                                                                         0, 
+                                                                         "IndexCheckboxClicked",
+                                                                         self.MT._row_index[datarn] if isinstance(self.MT._row_index, list) else self.MT.get_cell_data(datarn, self.MT._row_index)))
             if self.extra_end_edit_cell_func is not None:
-                self.extra_end_edit_cell_func(EditHeaderEvent(c, "Return", f"{self.MT._headers[dcol] if isinstance(self.MT._headers, list) else self.MT.data[self.MT._headers][dcol]}", "end_edit_header"))
+                self.extra_end_edit_cell_func(EditIndexEvent(r, 
+                                                             "Return",
+                                                             self.MT._row_index[datarn] if isinstance(self.MT._row_index, list) else self.MT.get_cell_data(datarn, self.MT._row_index), 
+                                                             "end_edit_index"))
         if redraw:
             self.MT.refresh()
 
-    def create_checkbox(self, c = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
-        if c in self.cell_options and any(x in self.cell_options[c] for x in ('dropdown', 'checkbox')):
-            self.delete_dropdown_and_checkbox(c)
-        self._set_cell_data(dcol = c, value = checked, cell_resize = False, undo = False) # only works because cell_resize and undo are false else needs c arg
-        if c not in self.cell_options:
-            self.cell_options[c] = {}
-        self.cell_options[c]['checkbox'] = {'check_function': check_function,
-                                            'state': state,
-                                            'text': text}
+    def create_checkbox(self, datarn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
+        if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 
+                                            'checkbox' in self.cell_options[datarn]):
+            self.delete_dropdown_and_checkbox(datarn)
+        self.set_cell_data(datarn = datarn, 
+                            value = checked)
+        if datarn not in self.cell_options:
+            self.cell_options[datarn] = {}
+        self.cell_options[datarn]['checkbox'] = {'check_function': check_function,
+                                                 'state': state,
+                                                 'text': text}
         if redraw:
             self.MT.refresh()
 
-    def create_dropdown(self, c = 0, values = [], set_value = None, state = "readonly", redraw = True, selection_function = None, modified_function = None):
-        if c in self.cell_options and any(x in self.cell_options[c] for x in ('dropdown', 'checkbox')):
-            self.delete_dropdown_and_checkbox(c)
-        self._set_cell_data(dcol = c, value = set_value if set_value is not None else values[0] if values else "", cell_resize = False, undo = False) # only works because cell_resize and undo are false else needs c arg
-        if c not in self.cell_options:
-            self.cell_options[c] = {}
-        self.cell_options[c]['dropdown'] = {'values': values,
-                                            'align': "w",
-                                            'window': "no dropdown open",
-                                            'canvas_id': "no dropdown open",
-                                            'select_function': selection_function,
-                                            'modified_function': modified_function,
-                                            'state': state}
+    def create_dropdown(self, 
+                        datarn = 0, 
+                        values = [], set_value = None, 
+                        state = "normal", redraw = True, 
+                        selection_function = None, modified_function = None,
+                        search_function = dropdown_search_function, validate_input = True, text = None):
+        if datarn in self.cell_options and ('dropdown' in self.cell_options[datarn] or 
+                                            'checkbox' in self.cell_options[datarn]):
+            self.delete_dropdown_and_checkbox(datarn)
+        self.set_cell_data(datarn = datarn, 
+                            value = set_value if set_value is not None else values[0] if values else "")
+        if datarn not in self.cell_options:
+            self.cell_options[datarn] = {}
+        self.cell_options[datarn]['dropdown'] = {'values': values,
+                                                 'window': "no dropdown open",
+                                                 'canvas_id': "no dropdown open",
+                                                 'select_function': selection_function,
+                                                 'modified_function': modified_function,
+                                                 'search_function': search_function,
+                                                 'validate_input': validate_input,
+                                                 'text': text,
+                                                 'state': state}
         if redraw:
             self.MT.refresh()
-            
-    def get_widget_bg_fg(self, c):
-        bg = self.header_bg
-        fg = self.header_fg
-        if c in self.cell_options and 'highlight' in self.cell_options[c]:
-            if self.cell_options[c]['highlight'][0] is not None:
-                bg = self.cell_options[c]['highlight'][0]
-            if self.cell_options[c]['highlight'][1] is not None:
-                fg = self.cell_options[c]['highlight'][1]
-        return bg, fg
-
-    def get_dropdown_height_anchor(self, dcol, text_editor_h = None):
+    
+    def get_dropdown_height_anchor(self, datarn, text_editor_h = None):
         win_h = 5
-        for i, v in enumerate(self.cell_options[dcol]['dropdown']['values']):
+        for i, v in enumerate(self.cell_options[datarn]['dropdown']['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
-                win_h += self.MT.hdr_fl_ins + (v_numlines * self.MT.hdr_xtra_lines_increment) + 5 # end of cell
+                win_h += self.MT.fl_ins + (v_numlines * self.MT.xtra_lines_increment) + 5 # end of cell
             else:
-                win_h += self.MT.hdr_min_rh
+                win_h += self.MT.min_rh
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.MT.get_space_bot(0, text_editor_h)
         win_h2 = int(win_h)
         if win_h > space_bot:
             win_h = space_bot - 1
-        if win_h < self.MT.hdr_txt_h + 5:
-            win_h = self.MT.hdr_txt_h + 5
+        if win_h < self.MT.txt_h + 5:
+            win_h = self.MT.txt_h + 5
         elif win_h > win_h2:
             win_h = win_h2
         return win_h, "nw"
-    
-    # data indexes
-    def set_current_height_to_cell(self, dcol):
-        x = self.MT.txt_measure_canvas.create_text(0,
-                                                   0,
-                                                   text = self.MT.data[self.MT._headers][dcol] if isinstance(self.MT._headers, int) else self.MT._headers[dcol],
-                                                   font = self.MT._hdr_font)
-        b = self.MT.txt_measure_canvas.bbox(x)
-        self.MT.txt_measure_canvas.delete(x)
-        new_height = b[3] - b[1] + 5
-        space_bot = self.MT.get_space_bot(0)
-        if new_height > space_bot:
-            new_height = space_bot
-        self.set_height(new_height, set_TL = True)
             
-    # c is displayed col
-    def display_dropdown_window(self, c, dcol = None, event = None):
+    # r is displayed row
+    def open_dropdown_window(self, r, datarn = None, event = None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
-        if dcol is None:
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-        if self.cell_options[dcol]['dropdown']['state'] == "normal":
-            if not self.edit_cell_(c = c, dropdown = True, event = event):
+        if datarn is None:
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        if self.cell_options[datarn]['dropdown']['state'] == "normal":
+            if not self.edit_cell_(r = r, dropdown = True, event = event):
                 return
-        win_h, anchor = self.get_dropdown_height_anchor(dcol)
+        win_h, anchor = self.get_dropdown_height_anchor(datarn)
         window = self.MT.parentframe.dropdown_class(self.MT.winfo_toplevel(),
+                                                    r,
                                                     0,
-                                                    c,
-                                                    width = self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1,
+                                                    width = self.current_width,
                                                     height = win_h,
-                                                    font = self.MT._hdr_font,
+                                                    font = self.MT._font,
                                                     colors = {'bg': self.MT.popup_menu_bg, 
                                                               'fg': self.MT.popup_menu_fg, 
                                                               'highlight_bg': self.MT.popup_menu_highlight_bg,
                                                               'highlight_fg': self.MT.popup_menu_highlight_fg},
                                                     outline_color = self.MT.popup_menu_fg,
-                                                    values = self.cell_options[dcol]['dropdown']['values'],
-                                                    hide_dropdown_window = self.hide_dropdown_window,
+                                                    values = self.cell_options[datarn]['dropdown']['values'],
+                                                    close_dropdown_window = self.close_dropdown_window,
+                                                    search_function = self.cell_options[datarn]['dropdown']['search_function'],
                                                     arrowkey_RIGHT = self.MT.arrowkey_RIGHT,
                                                     arrowkey_LEFT = self.MT.arrowkey_LEFT,
-                                                    align = self.cell_options[dcol]['dropdown']['align'],
-                                                    single_index = "c")
-        ypos = self.current_height - 1
-        self.cell_options[dcol]['dropdown']['canvas_id'] = self.create_window((self.MT.col_positions[c], ypos),
+                                                    align = "w",
+                                                    single_index = "r")
+        ypos = self.MT.row_positions[r + 1]
+        self.cell_options[datarn]['dropdown']['canvas_id'] = self.create_window((0, ypos),
                                                                                window = window,
                                                                                anchor = anchor)
-        if self.cell_options[dcol]['dropdown']['state'] == "normal":
-            if self.cell_options[dcol]['dropdown']['modified_function'] is not None:
-                self.text_editor.textedit.bind("<<TextModified>>", self.cell_options[dcol]['dropdown']['modified_function'])
+        if self.cell_options[datarn]['dropdown']['state'] == "normal":
+            self.text_editor.textedit.bind("<<TextModified>>", 
+                                           lambda x: window.search_and_see(DropDownModifiedEvent("IndexComboboxModified", r, 0, self.text_editor.get())))
+            if self.cell_options[datarn]['dropdown']['modified_function'] is not None:
+                window.modified_function = self.cell_options[datarn]['dropdown']['modified_function']
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
                 self.after(2, self.text_editor.scroll_to_bottom())
             except:
                 return
             redraw = False
         else:
-            window.bind("<FocusOut>", lambda x: self.hide_dropdown_window(c))
+            window.bind("<FocusOut>", lambda x: self.close_dropdown_window(r))
             self.update_idletasks()
             window.focus_set()
             redraw = True
         self.existing_dropdown_window = window
-        self.cell_options[dcol]['dropdown']['window'] = window
-        self.existing_dropdown_canvas_id = self.cell_options[dcol]['dropdown']['canvas_id']
+        self.cell_options[datarn]['dropdown']['window'] = window
+        self.existing_dropdown_canvas_id = self.cell_options[datarn]['dropdown']['canvas_id']
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = False)
+            self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True, redraw_table = False)
             
-    # c is displayed col
-    def hide_dropdown_window(self, c = None, selection = None, redraw = True):
-        if c is not None and selection is not None:
-            dcol = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            if self.cell_options[dcol]['dropdown']['select_function'] is not None: # user has specified a selection function
-                self.cell_options[dcol]['dropdown']['select_function'](EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
+    # r is displayed row
+    def close_dropdown_window(self, r = None, selection = None, redraw = True):
+        if r is not None and selection is not None:
+            datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+            if self.cell_options[datarn]['dropdown']['select_function'] is not None: # user has specified a selection function
+                self.cell_options[datarn]['dropdown']['select_function'](EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
             if self.extra_end_edit_cell_func is None:
-                self._set_cell_data(c, dcol = dcol, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(r, datarn = datarn, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
-                validation = self.extra_end_edit_cell_func(EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
+                validation = self.extra_end_edit_cell_func(EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
                 if validation is not None:
                     selection = validation
-                self._set_cell_data(c, dcol = dcol, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(r, datarn = datarn, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation:
-                self._set_cell_data(c, dcol = dcol, value = selection, redraw = not redraw)
-                self.extra_end_edit_cell_func(EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
+                self.set_cell_data_undo(r, datarn = datarn, value = selection, redraw = not redraw)
+                self.extra_end_edit_cell_func(EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
             self.focus_set()
             self.MT.recreate_all_selection_boxes()
         self.destroy_text_editor("Escape")
-        self.destroy_opened_dropdown_window(c)
+        self.destroy_opened_dropdown_window(r)
         if redraw:
             self.MT.refresh()
+            
+    def get_existing_dropdown_coords(self):
+        if self.existing_dropdown_window is not None:
+            return int(self.existing_dropdown_window.r)
+        return None
         
     def mouseclick_outside_editor_or_dropdown(self):
-        if self.existing_dropdown_window is not None:
-            closed_dd_coords = int(self.existing_dropdown_window.c)
-        else:
-            closed_dd_coords = None
+        closed_dd_coords = self.get_existing_dropdown_coords()
         if self.text_editor_loc is not None and self.text_editor is not None:
             self.close_text_editor(editor_info = (self.text_editor_loc, "ButtonPress-1"))
         else:
             self.destroy_text_editor("Escape")
-        if closed_dd_coords:
+        if closed_dd_coords is not None:
             self.destroy_opened_dropdown_window(closed_dd_coords) #displayed coords not data, necessary for b1 function
         return closed_dd_coords
-            
-    # function can receive two None args
-    def destroy_opened_dropdown_window(self, c = None, dcol = None):
-        if c is not None or dcol is not None:
-            if dcol is None:
-                dcol_ = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+    
+    def mouseclick_outside_editor_or_dropdown_all_canvases(self):
+        self.CH.mouseclick_outside_editor_or_dropdown()
+        self.MT.mouseclick_outside_editor_or_dropdown()
+        return self.mouseclick_outside_editor_or_dropdown()
+
+    # r is displayed row, function can have two None args
+    def destroy_opened_dropdown_window(self, r = None, datarn = None):
+        if r is None and datarn is None and self.existing_dropdown_window is not None:
+            r = self.get_existing_dropdown_coords()
+        if r is not None or datarn is not None:
+            if datarn is None:
+                datarn_ = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             else:
-                dcol_ = dcol
+                datarn_ = r
         else:
-            dcol_ = None
+            datarn_ = None
         try:
             self.delete(self.existing_dropdown_canvas_id)
         except:
             pass
         self.existing_dropdown_canvas_id = None
         try:
             self.existing_dropdown_window.destroy()
         except:
             pass
-        self.existing_dropdown_window = None
-        if dcol_ in self.cell_options and 'dropdown' in self.cell_options[dcol_]:
-            self.cell_options[dcol_]['dropdown']['canvas_id'] = "no dropdown open"
-            self.cell_options[dcol_]['dropdown']['window'] = "no dropdown open"
+        if datarn_ in self.cell_options and 'dropdown' in self.cell_options[datarn_]:
+            self.cell_options[datarn_]['dropdown']['canvas_id'] = "no dropdown open"
+            self.cell_options[datarn_]['dropdown']['window'] = "no dropdown open"
             try:
-                self.delete(self.cell_options[dcol_]['dropdown']['canvas_id'])
+                self.delete(self.cell_options[datarn_]['dropdown']['canvas_id'])
             except:
                 pass
-            
-    # c is dcol
-    def delete_dropdown(self, c):
-        self.destroy_opened_dropdown_window(dcol = c)
-        if c in self.cell_options and 'dropdown' in self.cell_options[c]:
-            del self.cell_options[c]['dropdown']
-            
-    # c is dcol
-    def delete_checkbox(self, c):
-        if c in self.cell_options and 'checkbox' in self.cell_options[c]:
-            del self.cell_options[c]['checkbox']
-
-    # c is dcol
-    def delete_dropdown_and_checkbox(self, c):
-        self.delete_dropdown(dcol = c)
-        self.delete_checkbox(c)
+        self.existing_dropdown_window = None
+
+    def delete_dropdown(self, datarn):
+        self.destroy_opened_dropdown_window(datarn = datarn)
+        if datarn in self.cell_options and 'dropdown' in self.cell_options[datarn]:
+            del self.cell_options[datarn]['dropdown']
+
+    def delete_checkbox(self, datarn):
+        if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
+            del self.cell_options[datarn]['checkbox']
+
+    def delete_dropdown_and_checkbox(self, datarn):
+        self.delete_dropdown(datarn)
+        self.delete_checkbox(datarn)
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet_main_table.py` & `tksheet-6.0.0/tksheet/_tksheet_main_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from ._tksheet_vars import *
+from ._tksheet_formatters import *
 from ._tksheet_other_classes import *
 
 from collections import defaultdict, deque
 from itertools import islice, repeat, accumulate, chain, product, cycle
 from math import floor, ceil
 from tkinter import TclError
 import bisect
-import csv as csv_module
+import csv as csv
 import io
 import pickle
 import tkinter as tk
+from typing import Union, Any, Type, Callable
 import zlib
 
 
 class MainTable(tk.Canvas):
     def __init__(self,
                  *args,
                  **kwargs):
@@ -50,35 +52,48 @@
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
 
         self.cell_options = {}
         self.col_options = {}
         self.row_options = {}
+        self.sheet_options = {}
 
         """
         cell options dict looks like:
         {(row int, column int): {'dropdown': {'values': values,
                                               'window': "no dropdown open",
                                               'select_function': selection_function,
                                               'keypress_function': keypress_function,
                                               'state': state},
                                  'highlight: (bg, fg),
                                  'align': "e",
-                                 'readonly': True}
+                                 'readonly': True,
+                                 'format': {}
+                                }
         """
-
+        self.arrowkey_binding_functions = {"tab": self.tab_key,
+                                           "up": self.arrowkey_UP, 
+                                           "right": self.arrowkey_RIGHT,
+                                           "down": self.arrowkey_DOWN, 
+                                           "left": self.arrowkey_LEFT,
+                                           "prior": self.page_UP, 
+                                           "next": self.page_DOWN}
         self.extra_table_rc_menu_funcs = {}
         self.extra_index_rc_menu_funcs = {}
         self.extra_header_rc_menu_funcs = {}
         self.extra_empty_space_rc_menu_funcs = {}
 
         self.max_undos = kwargs['max_undos']
         self.undo_storage = deque(maxlen = kwargs['max_undos'])
 
+        self.to_clipboard_delimiter = kwargs['to_clipboard_delimiter']
+        self.to_clipboard_quotechar = kwargs['to_clipboard_quotechar']
+        self.to_clipboard_lineterminator = kwargs['to_clipboard_lineterminator']
+        self.from_clipboard_delimiters = kwargs['from_clipboard_delimiters'] if isinstance(kwargs['from_clipboard_delimiters'], str) else "".join(kwargs['from_clipboard_delimiters'])
         self.page_up_down_select_row = kwargs['page_up_down_select_row']
         self.expand_sheet_if_paste_too_big = kwargs['expand_sheet_if_paste_too_big']
         self.paste_insert_column_limit = kwargs['paste_insert_column_limit']
         self.paste_insert_row_limit = kwargs['paste_insert_row_limit']
         self.arrow_key_down_right_scroll_page = kwargs['arrow_key_down_right_scroll_page']
         self.cell_auto_resize_enabled = kwargs['enable_edit_cell_auto_resize']
         self.edit_cell_validation = kwargs['edit_cell_validation']
@@ -138,19 +153,17 @@
         self.deselection_binding_func = None
         self.drag_selection_binding_func = None
         self.shift_selection_binding_func = None
         self.select_all_binding_func = None
 
         self.single_selection_enabled = False
         self.toggle_selection_enabled = False # with this mode every left click adds the cell to selected cells
-        self.ctrl_keys_over_dropdowns_enabled = kwargs['ctrl_keys_over_dropdowns_enabled']
         self.show_dropdown_borders = kwargs['show_dropdown_borders']
         self.drag_selection_enabled = False
         self.select_all_enabled = False
-        self.arrowkeys_enabled = False
         self.undo_enabled = False
         self.cut_enabled = False
         self.copy_enabled = False
         self.paste_enabled = False
         self.delete_key_enabled = False
         self.rc_select_enabled = False
         self.rc_delete_column_enabled = False
@@ -360,15 +373,19 @@
                 boxes[tuple(int(e) for e in self.gettags(item)[1].split("_") if e)] = "rows"
             return boxes
 
     def ctrl_c(self, event = None):
         currently_selected = self.currently_selected()
         if currently_selected:
             s = io.StringIO()
-            writer = csv_module.writer(s, dialect = csv_module.excel_tab, lineterminator = "\n")
+            writer = csv.writer(s,
+                                dialect = csv.excel_tab, 
+                                delimiter = self.to_clipboard_delimiter,
+                                quotechar = self.to_clipboard_quotechar,
+                                lineterminator = self.to_clipboard_lineterminator)
             rows = []
             if currently_selected.type_ in ("cell", "column"):
                 boxes, maxrows = self.get_ctrl_x_c_boxes()
                 if self.extra_begin_ctrl_c_func is not None:
                     try:
                         self.extra_begin_ctrl_c_func(CtrlKeyEvent("begin_ctrl_c", boxes, currently_selected, tuple()))
                     except:
@@ -376,153 +393,121 @@
                 for rn in range(maxrows):
                     row = []
                     for r1, c1, r2, c2 in boxes:
                         if r2 - r1 < maxrows:
                             continue
                         data_ref_rn = r1 + rn
                         for c in range(c1, c2):
-                            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                            try:
-                                row.append(self.data[data_ref_rn][dcol])
-                            except:
-                                row.append("")
+                            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                            row.append(self.get_cell_clipboard(data_ref_rn, datacn))
                     writer.writerow(row)
                     rows.append(row)
             else:
                 boxes = self.get_ctrl_x_c_boxes()
                 if self.extra_begin_ctrl_c_func is not None:
                     try:
                         self.extra_begin_ctrl_c_func(CtrlKeyEvent("begin_ctrl_c", boxes, currently_selected, tuple()))
                     except:
                         return
                 for r1, c1, r2, c2 in boxes:
                     for rn in range(r2 - r1):
                         row = []
                         data_ref_rn = r1 + rn
                         for c in range(c1, c2):
-                            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                            try:
-                                row.append(self.data[data_ref_rn][dcol])
-                            except:
-                                row.append("")
+                            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                            row.append(self.get_cell_clipboard(data_ref_rn, datacn))
                         writer.writerow(row)
                         rows.append(row)
             for r1, c1, r2, c2 in boxes:
                 self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
             self.clipboard_clear()
             self.clipboard_append(s.getvalue())
             self.update_idletasks()
             if self.extra_end_ctrl_c_func is not None:
                 self.extra_end_ctrl_c_func(CtrlKeyEvent("end_ctrl_c", boxes, currently_selected, rows))
             
     def ctrl_x(self, event = None):
-        if self.anything_selected():
-            undo_storage = {}
-            s = io.StringIO()
-            writer = csv_module.writer(s, dialect = csv_module.excel_tab, lineterminator = "\n")
-            currently_selected = self.currently_selected()
-            rows = []
-            if currently_selected.type_ in ("cell", "column"):
-                boxes, maxrows = self.get_ctrl_x_c_boxes()
-                if self.extra_begin_ctrl_x_func is not None:
-                    try:
-                        self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
-                    except:
-                        return
-                for rn in range(maxrows):
+        if not self.anything_selected():
+            return
+        undo_storage = {}
+        s = io.StringIO()
+        writer = csv.writer(s,
+                            dialect = csv.excel_tab, 
+                            delimiter = self.to_clipboard_delimiter,
+                            quotechar = self.to_clipboard_quotechar,
+                            lineterminator = self.to_clipboard_lineterminator)
+        currently_selected = self.currently_selected()
+        rows = []
+        changes = 0
+        if currently_selected.type_ in ("cell", "column"):
+            boxes, maxrows = self.get_ctrl_x_c_boxes()
+            if self.extra_begin_ctrl_x_func is not None:
+                try:
+                    self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
+                except:
+                    return
+            for rn in range(maxrows):
+                row = []
+                for r1, c1, r2, c2 in boxes:
+                    if r2 - r1 < maxrows:
+                        continue
+                    data_ref_rn = r1 + rn
+                    for c in range(c1, c2):
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                        row.append(self.get_cell_clipboard(data_ref_rn, datacn))
+                writer.writerow(row)
+                rows.append(row)
+            for rn in range(maxrows):
+                for r1, c1, r2, c2 in boxes:
+                    if r2 - r1 < maxrows:
+                        continue
+                    data_ref_rn = r1 + rn
+                    for c in range(c1, c2):
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                        if self.input_valid_for_cell(data_ref_rn, datacn, ""):
+                            if self.undo_enabled:
+                                undo_storage[(data_ref_rn, datacn)] = self.get_cell_data(data_ref_rn, datacn)
+                            self.set_cell_data(data_ref_rn, datacn, "")
+                            changes += 1
+        else:
+            boxes = self.get_ctrl_x_c_boxes()
+            if self.extra_begin_ctrl_x_func is not None:
+                try:
+                    self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
+                except:
+                    return
+            for r1, c1, r2, c2 in boxes:
+                for rn in range(r2 - r1):
                     row = []
-                    for r1, c1, r2, c2 in boxes:
-                        if r2 - r1 < maxrows:
-                            continue
-                        data_ref_rn = r1 + rn
-                        for c in range(c1, c2):
-                            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                            try:
-                                sx = f"{self.data[data_ref_rn][dcol]}"
-                                row.append(sx)
-                                if self.undo_enabled:
-                                    undo_storage[(data_ref_rn, dcol)] = sx
-                            except:
-                                row.append("")
+                    data_ref_rn = r1 + rn
+                    for c in range(c1, c2):
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                        row.append(self.get_cell_data(data_ref_rn, datacn))
                     writer.writerow(row)
                     rows.append(row)
-                for rn in range(maxrows):
-                    for r1, c1, r2, c2 in boxes:
-                        if r2 - r1 < maxrows:
-                            continue
-                        data_ref_rn = r1 + rn
-                        if data_ref_rn in self.row_options and 'readonly' in self.row_options[data_ref_rn]:
-                            continue
-                        for c in range(c1, c2):
-                            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                            if (
-                                ((data_ref_rn, dcol) in self.cell_options and ('readonly' in self.cell_options[(data_ref_rn, dcol)] or 'checkbox' in self.cell_options[(data_ref_rn, dcol)])) or
-                                (dcol in self.col_options and 'readonly' in self.col_options[dcol]) or
-                                (not self.ctrl_keys_over_dropdowns_enabled and 
-                                (data_ref_rn, dcol) in self.cell_options and 
-                                'dropdown' in self.cell_options[(data_ref_rn, dcol)] and
-                                "" not in self.cell_options[(data_ref_rn, dcol)]['dropdown']['values'])
-                                ):
-                                continue
-                            try:
-                                self.data[data_ref_rn][dcol] = ""
-                            except:
-                                continue
-            else:
-                boxes = self.get_ctrl_x_c_boxes()
-                if self.extra_begin_ctrl_x_func is not None:
-                    try:
-                        self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
-                    except:
-                        return
-                for r1, c1, r2, c2 in boxes:
-                    for rn in range(r2 - r1):
-                        row = []
-                        data_ref_rn = r1 + rn
-                        for c in range(c1, c2):
-                            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                            try:
-                                sx = f"{self.data[data_ref_rn][dcol]}"
-                                row.append(sx)
-                                if self.undo_enabled:
-                                    undo_storage[(data_ref_rn, dcol)] = sx
-                            except:
-                                row.append("")
-                        writer.writerow(row)
-                        rows.append(row)
-                for r1, c1, r2, c2 in boxes:
-                    for rn in range(r2 - r1):
-                        data_ref_rn = r1 + rn
-                        if data_ref_rn in self.row_options and 'readonly' in self.row_options[data_ref_rn]:
-                            continue
-                        for c in range(c1, c2):
-                            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                            if (
-                                ((data_ref_rn, dcol) in self.cell_options and ('readonly' in self.cell_options[(data_ref_rn, dcol)] or 'checkbox' in self.cell_options[(data_ref_rn, dcol)])) or
-                                (dcol in self.col_options and 'readonly' in self.col_options[dcol]) or
-                                (not self.ctrl_keys_over_dropdowns_enabled and 
-                                (data_ref_rn, dcol) in self.cell_options and 
-                                'dropdown' in self.cell_options[(data_ref_rn, dcol)] and
-                                "" not in self.cell_options[(data_ref_rn, dcol)]['dropdown']['values'])
-                                ):
-                                continue
-                            try:
-                                self.data[data_ref_rn][dcol] = ""
-                            except:
-                                continue
-            if self.undo_enabled:
-                self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
-            self.clipboard_clear()
-            self.clipboard_append(s.getvalue())
-            self.update_idletasks()
-            self.refresh()
             for r1, c1, r2, c2 in boxes:
-                self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
-            if self.extra_end_ctrl_x_func is not None:
-                self.extra_end_ctrl_x_func(CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows))
+                for rn in range(r2 - r1):
+                    data_ref_rn = r1 + rn
+                    for c in range(c1, c2):
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                        if self.input_valid_for_cell(data_ref_rn, datacn, ""):
+                            if self.undo_enabled:
+                                undo_storage[(data_ref_rn, datacn)] = self.get_cell_data(data_ref_rn, datacn)
+                            self.set_cell_data(data_ref_rn, datacn, "")
+                            changes += 1
+        if changes and self.undo_enabled:
+            self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
+        self.clipboard_clear()
+        self.clipboard_append(s.getvalue())
+        self.update_idletasks()
+        self.refresh()
+        for r1, c1, r2, c2 in boxes:
+            self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
+        if self.extra_end_ctrl_x_func is not None:
+            self.extra_end_ctrl_x_func(CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows))
 
     def find_last_selected_box_with_current(self, currently_selected):
         if currently_selected.type_ in ("cell", "column"):
             boxes, maxrows = self.get_ctrl_x_c_boxes()
         else:
             boxes = self.get_ctrl_x_c_boxes()
         for (r1, c1, r2, c2), type_ in boxes.items():
@@ -536,44 +521,49 @@
         return (currently_selected.row, currently_selected.column, currently_selected.row + 1, currently_selected.column + 1)
 
     def ctrl_v(self, event = None):
         if not self.expand_sheet_if_paste_too_big and (len(self.col_positions) == 1 or len(self.row_positions) == 1):
             return
         currently_selected = self.currently_selected()
         if currently_selected:
-            y1 = currently_selected[0]
-            x1 = currently_selected[1]
+            selected_r = currently_selected[0]
+            selected_c = currently_selected[1]
         elif not currently_selected and not self.expand_sheet_if_paste_too_big:
             return
         else:
             if not self.data:
-                x1, y1 = 0, 0
+                selected_c, selected_r = 0, 0
             else:
                 if len(self.col_positions) == 1 and len(self.row_positions) > 1:
-                    x1, y1 = 0, len(self.row_positions) - 1
+                    selected_c, selected_r = 0, len(self.row_positions) - 1
                 elif len(self.row_positions) == 1 and len(self.col_positions) > 1:
-                    x1, y1 = len(self.col_positions) - 1, 0
+                    selected_c, selected_r = len(self.col_positions) - 1, 0
                 elif len(self.row_positions) > 1 and len(self.col_positions) > 1:
-                    x1, y1 = 0, len(self.row_positions) - 1
+                    selected_c, selected_r = 0, len(self.row_positions) - 1
         try:
             data = self.clipboard_get()
         except:
             return
-        data = list(csv_module.reader(io.StringIO(data), delimiter = "\t", quotechar = '"', skipinitialspace = True))
+        try:
+            dialect = csv.Sniffer().sniff(data, delimiters = self.from_clipboard_delimiters)
+        except:
+            dialect = csv.excel_tab
+        data = list(csv.reader(io.StringIO(data),
+                               dialect = dialect, 
+                               skipinitialspace = True))
         if not data:
             return
         numcols = len(max(data, key = len))
         numrows = len(data)
         for rn, r in enumerate(data):
             if len(r) < numcols:
                 data[rn].extend(list(repeat("", numcols - len(r))))
         lastbox_r1, lastbox_c1, lastbox_r2, lastbox_c2 = self.find_last_selected_box_with_current(currently_selected)
         lastbox_numrows = lastbox_r2 - lastbox_r1
         lastbox_numcols = lastbox_c2 - lastbox_c1
-        
         if lastbox_numrows > numrows and lastbox_numrows % numrows == 0:
             nd = []
             for times in range(int(lastbox_numrows / numrows)):
                 nd.extend([r.copy() for r in data])
             data.extend(nd)
             numrows *= int(lastbox_numrows / numrows)
         if lastbox_numcols > numcols and lastbox_numcols % numcols == 0:
@@ -581,125 +571,103 @@
                 for times in range(int(lastbox_numcols / numcols)):
                     data[rn].extend(r.copy())
             numcols *= int(lastbox_numcols / numcols)
         undo_storage = {}
         if self.expand_sheet_if_paste_too_big:
             added_rows = 0
             added_cols = 0
-            if x1 + numcols > len(self.col_positions) - 1:
-                added_cols = x1 + numcols - len(self.col_positions) + 1
+            if selected_c + numcols > len(self.col_positions) - 1:
+                added_cols = selected_c + numcols - len(self.col_positions) + 1
                 if isinstance(self.paste_insert_column_limit, int) and self.paste_insert_column_limit < len(self.col_positions) - 1 + added_cols:
                     added_cols = self.paste_insert_column_limit - len(self.col_positions) - 1
                 if added_cols > 0:
                     self.insert_col_positions(widths = int(added_cols))
                 if not self.all_columns_displayed:
                     total_data_cols = self.total_data_cols()
                     self.displayed_columns.extend(list(range(total_data_cols, total_data_cols + added_cols)))
-            if y1 + numrows > len(self.row_positions) - 1:
-                added_rows = y1 + numrows - len(self.row_positions) + 1
+            if selected_r + numrows > len(self.row_positions) - 1:
+                added_rows = selected_r + numrows - len(self.row_positions) + 1
                 if isinstance(self.paste_insert_row_limit, int) and self.paste_insert_row_limit < len(self.row_positions) - 1 + added_rows:
                     added_rows = self.paste_insert_row_limit - len(self.row_positions) - 1
                 if added_rows > 0:
                     self.insert_row_positions(heights = int(added_rows))
             added_rows_cols = (added_rows, added_cols)
         else:
             added_rows_cols = (0, 0)
-        if x1 + numcols > len(self.col_positions) - 1:
-            numcols = len(self.col_positions) - 1 - x1
-        if y1 + numrows > len(self.row_positions) - 1:
-            numrows = len(self.row_positions) - 1 - y1
+        if selected_c + numcols > len(self.col_positions) - 1:
+            numcols = len(self.col_positions) - 1 - selected_c
+        if selected_r + numrows > len(self.row_positions) - 1:
+            numrows = len(self.row_positions) - 1 - selected_r
         if self.extra_begin_ctrl_v_func is not None or self.extra_end_ctrl_v_func is not None:
-            rows = [[data[ndr][ndc] for ndc, c in enumerate(range(x1, x1 + numcols))] for ndr, r in enumerate(range(y1, y1 + numrows))]
+            rows = [[data[ndr][ndc] for ndc, c in enumerate(range(selected_c, selected_c + numcols))] for ndr, r in enumerate(range(selected_r, selected_r + numrows))]
         if self.extra_begin_ctrl_v_func is not None:
             try:
                 self.extra_begin_ctrl_v_func(PasteEvent("begin_ctrl_v", currently_selected, rows))
             except:
                 return
-        for ndr, r in enumerate(range(y1, y1 + numrows)):
-            for ndc, c in enumerate(range(x1, x1 + numcols)):
-                dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                if r > len(self.data) - 1:
-                    self.data.extend([list(repeat("", c + 1)) for r in range((r + 1) - len(self.data))])
-                elif c > len(self.data[r]) - 1:
-                    self.data[r].extend(list(repeat("", (c + 1) - len(self.data[r]))))
-                if (
-                    ((r, dcol) in self.cell_options and 'readonly' in self.cell_options[(r, dcol)]) or
-                    ((r, dcol) in self.cell_options and 'checkbox' in self.cell_options[(r, dcol)]) or
-                    (dcol in self.col_options and 'readonly' in self.col_options[dcol]) or
-                    (r in self.row_options and 'readonly' in self.row_options[r]) or
-                    # if pasting not allowed in dropdowns and paste value isn't in dropdown values
-                    (not self.ctrl_keys_over_dropdowns_enabled and 
-                     (r, dcol) in self.cell_options and 
-                     'dropdown' in self.cell_options[(r, dcol)] and
-                     data[ndr][ndc] not in self.cell_options[(r, dcol)]['dropdown']['values'])
-                    ):
-                    continue
-                if self.undo_enabled:
-                    undo_storage[(r, dcol)] = f"{self.data[r][dcol]}"
-                self.data[r][dcol] = data[ndr][ndc]
+        changes = 0
+        for ndr, r in enumerate(range(selected_r, selected_r + numrows)):
+            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+            for ndc, c in enumerate(range(selected_c, selected_c + numcols)):
+                datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                if self.input_valid_for_cell(datarn, datacn, data[ndr][ndc]):
+                    if self.undo_enabled:
+                        undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
+                    self.set_cell_data(datarn, datacn, data[ndr][ndc])
+                    changes += 1
         if self.expand_sheet_if_paste_too_big and self.undo_enabled:
             self.equalize_data_row_lengths()
         self.deselect("all")
-        if self.undo_enabled:
+        if changes and self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells_paste",
                                                                  undo_storage,
-                                                                 (((y1, x1, y1 + numrows, x1 + numcols), "cells"), ), # boxes
+                                                                 (((selected_r, selected_c, selected_r + numrows, selected_c + numcols), "cells"), ), # boxes
                                                                  currently_selected,
                                                                  added_rows_cols))))
-        self.create_selected(y1, x1, y1 + numrows, x1 + numcols, "cells")
-        self.create_current(y1, x1, type_ = "cell", inside = True if numrows > 1 or numcols > 1 else False)
-        self.see(r = y1, c = x1, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
+        self.create_selected(selected_r, selected_c, selected_r + numrows, selected_c + numcols, "cells")
+        self.create_current(selected_r, selected_c, type_ = "cell", inside = True if numrows > 1 or numcols > 1 else False)
+        self.see(r = selected_r, c = selected_c, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
         self.refresh()
         if self.extra_end_ctrl_v_func is not None:
             self.extra_end_ctrl_v_func(PasteEvent("end_ctrl_v", currently_selected, rows))
 
     def delete_key(self, event = None):
         if self.anything_selected():
             currently_selected = self.currently_selected()
             undo_storage = {}
-            boxes = []
+            boxes = {}
             for item in chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside")):
                 alltags = self.gettags(item)
                 box = tuple(int(e) for e in alltags[1].split("_") if e)
                 if alltags[0] in ("CellSelectFill", "Current_Outside"):
-                    boxes.append((box, "cells"))
+                    boxes[box] = "cells"
                 elif alltags[0] == "ColSelectFill":
-                    boxes.append((box, "columns"))
+                    boxes[box] = "columns"
                 elif alltags[0] == "RowSelectFill":
-                    boxes.append((box, "rows"))
+                    boxes[box] = "rows"
             if self.extra_begin_delete_key_func is not None:
                 try:
                     self.extra_begin_delete_key_func(CtrlKeyEvent("begin_delete_key", boxes, currently_selected, tuple()))
                 except:
                     return
-            for (r1, c1, r2, c2), _ in boxes:
+            changes = 0
+            for r1, c1, r2, c2 in boxes:
                 for r in range(r1, r2):
+                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                     for c in range(c1, c2):
-                        dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                        if (
-                            ((r, dcol) in self.cell_options and ('readonly' in self.cell_options[(r, dcol)] or 'checkbox' in self.cell_options[(r, dcol)])) or
-                            # if del key not allowed in dropdowns and empty string isn't in dropdown values
-                            (not self.ctrl_keys_over_dropdowns_enabled and 
-                            (r, dcol) in self.cell_options and 
-                            'dropdown' in self.cell_options[(r, dcol)] and
-                            "" not in self.cell_options[(r, dcol)]['dropdown']['values']) or
-                            (dcol in self.col_options and 'readonly' in self.col_options[dcol]) or
-                            (r in self.row_options and 'readonly' in self.row_options[r])
-                            ):
-                            continue
-                        try:
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                        if self.input_valid_for_cell(datarn, datacn, ""):
                             if self.undo_enabled:
-                                undo_storage[(r, dcol)] = f"{self.data[r][dcol]}"
-                            self.data[r][dcol] = ""
-                        except:
-                            continue
+                                undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
+                            self.set_cell_data(datarn, datacn, "")
+                            changes += 1
             if self.extra_end_delete_key_func is not None:
                 self.extra_end_delete_key_func(CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage))
-            if self.undo_enabled:
-                self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, boxes, currently_selected))))
+            if changes and self.undo_enabled:
+                self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
             self.refresh()
             
     def move_columns_adjust_options_dict(self, col, to_move_min, num_cols, move_data = True, create_selections = True):
         c = int(col)
         to_move_max = to_move_min + num_cols
         to_del = to_move_max + num_cols
         orig_selected = list(range(to_move_min, to_move_min + num_cols))
@@ -918,209 +886,198 @@
                 newrowsdct[k] if k in newrowsdct else
                 k - num_rows if k < r and k > to_move_min else
                 k: v for k, v in self.row_options.items()
             }
         return new_selected, {}
 
     def ctrl_z(self, event = None):
-        if self.undo_storage:
-            if not isinstance(self.undo_storage[-1], (tuple, dict)):
-                undo_storage = pickle.loads(zlib.decompress(self.undo_storage[-1]))
-            else:
-                undo_storage = self.undo_storage[-1]
-            self.deselect("all")
-            if self.extra_begin_ctrl_z_func is not None:
-                try:
-                    self.extra_begin_ctrl_z_func(UndoEvent("begin_ctrl_z", undo_storage[0], undo_storage))
-                except:
-                    return
-            self.undo_storage.pop()
-            if undo_storage[0] in ("edit_header", ):
-                for c, v in undo_storage[1].items():
-                    self._headers[c] = v
-                for box in undo_storage[2]:
-                    r1, c1, r2, c2 = box[0]
-                    if not self.expand_sheet_if_paste_too_big:
-                        self.create_selected(r1, c1, r2, c2, box[1])
-                self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
-                
-            if undo_storage[0] in ("edit_index", ):
-                for r, v in undo_storage[1].items():
-                    self._row_index[r] = v
-                for box in undo_storage[2]:
-                    r1, c1, r2, c2 = box[0]
-                    if not self.expand_sheet_if_paste_too_big:
-                        self.create_selected(r1, c1, r2, c2, box[1])
-                self.create_current(0, undo_storage[3][1], type_ = "row", inside = True)
-                            
-            if undo_storage[0] in ("edit_cells", "edit_cells_paste"):
-                for (r, c), v in undo_storage[1].items():
-                    self.data[r][c] = v
-                start_row = float("inf")
-                start_col = float("inf")
-                for box in undo_storage[2]:
-                    r1, c1, r2, c2 = box[0]
-                    if not self.expand_sheet_if_paste_too_big:
-                        self.create_selected(r1, c1, r2, c2, box[1])
-                    if r1 < start_row:
-                        start_row = r1
-                    if c1 < start_col:
-                        start_col = c1
-                if undo_storage[0] == "edit_cells_paste" and self.expand_sheet_if_paste_too_big:
-                    if undo_storage[4][0] > 0:
-                        self.del_row_positions(len(self.row_positions) - 1 - undo_storage[4][0], undo_storage[4][0])
-                        self.data[:] = self.data[:-undo_storage[4][0]]
-                    if undo_storage[4][1] > 0:
-                        quick_added_cols = undo_storage[4][1]
-                        self.del_col_positions(len(self.col_positions) - 1 - quick_added_cols, quick_added_cols)
-                        for rn in range(len(self.data)):
-                            self.data[rn][:] = self.data[rn][:-quick_added_cols]
-                        if not self.all_columns_displayed:
-                            self.displayed_columns[:] = self.displayed_columns[:-quick_added_cols]
-                if undo_storage[3]:
-                    if isinstance(undo_storage[3][0], int):
-                        self.create_current(undo_storage[3][0], undo_storage[3][1], type_ = "cell", inside = True if self.cell_selected(undo_storage[3][0], undo_storage[3][1]) else False)
-                    elif undo_storage[3][0] == "column":
-                        self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
-                    elif undo_storage[3][0] == "row":
-                        self.create_current(undo_storage[3][1], 0, type_ = "row", inside = True)
-                elif start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
-                    self.create_current(start_row, start_col, type_ = "cell", inside = True if self.cell_selected(start_row, start_col) else False)
-                if start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
-                    self.see(r = start_row, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
-            
-            elif undo_storage[0] == "move_cols":
-                c = undo_storage[1]
-                to_move_min = undo_storage[2]
-                totalcols = len(undo_storage[4])
-                if to_move_min < c:
-                    c += totalcols - 1
-                self.move_columns_adjust_options_dict(c, to_move_min, totalcols)
+        if not self.undo_storage:
+            return
+        if not isinstance(self.undo_storage[-1], (tuple, dict)):
+            undo_storage = pickle.loads(zlib.decompress(self.undo_storage[-1]))
+        else:
+            undo_storage = self.undo_storage[-1]
+        self.deselect("all")
+        if self.extra_begin_ctrl_z_func is not None:
+            try:
+                self.extra_begin_ctrl_z_func(UndoEvent("begin_ctrl_z", undo_storage[0], undo_storage))
+            except:
+                return
+        self.undo_storage.pop()
+        if undo_storage[0] in ("edit_header", ):
+            for c, v in undo_storage[1].items():
+                self._headers[c] = v
+            for box in undo_storage[2]:
+                r1, c1, r2, c2 = box[0]
+                if not self.expand_sheet_if_paste_too_big:
+                    self.create_selected(r1, c1, r2, c2, box[1])
+            self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
             
-            elif undo_storage[0] == "move_rows":
-                rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
-                r = undo_storage[1]
-                to_move_min = undo_storage[2]
-                totalrows = len(undo_storage[4])
-                if to_move_min < r:
-                    r += totalrows - 1
-                self.move_rows_adjust_options_dict(r, to_move_min, totalrows)
+        if undo_storage[0] in ("edit_index", ):
+            for r, v in undo_storage[1].items():
+                self._row_index[r] = v
+            for box in undo_storage[2]:
+                r1, c1, r2, c2 = box[0]
+                if not self.expand_sheet_if_paste_too_big:
+                    self.create_selected(r1, c1, r2, c2, box[1])
+            self.create_current(0, undo_storage[3][1], type_ = "row", inside = True)
                         
-            elif undo_storage[0] == "insert_row":
-                self.data[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
-                try:
-                    self._row_index[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
-                except:
-                    pass
-                self.del_row_positions(undo_storage[1]['sheet_row_num'],
-                                       undo_storage[1]['numrows'],
-                                       deselect_all = False)
-                for r in range(undo_storage[1]['sheet_row_num'],
-                               undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']):
-                    if r in self.row_options:
-                        del self.row_options[r]
-                    if r in self.RI.cell_options:
-                        del self.RI.cell_options[r]
-                numrows = undo_storage[1]['numrows']
-                idx = undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']
-                self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
-                self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
-                self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
-                if len(self.row_positions) > 1:
-                    start_row = undo_storage[1]['sheet_row_num'] if undo_storage[1]['sheet_row_num'] < len(self.row_positions) - 1 else undo_storage[1]['sheet_row_num'] - 1
-                    self.RI.select_row(start_row)
-                    self.see(r = start_row, c = 0, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
+        if undo_storage[0] in ("edit_cells", "edit_cells_paste"):
+            for (datarn, datacn), v in undo_storage[1].items():
+                self.set_cell_data(datarn, datacn, v)
+            start_row = float("inf")
+            start_col = float("inf")
+            for box in undo_storage[2]:
+                r1, c1, r2, c2 = box[0]
+                if not self.expand_sheet_if_paste_too_big:
+                    self.create_selected(r1, c1, r2, c2, box[1])
+                if r1 < start_row:
+                    start_row = r1
+                if c1 < start_col:
+                    start_col = c1
+            if undo_storage[0] == "edit_cells_paste" and self.expand_sheet_if_paste_too_big:
+                if undo_storage[4][0] > 0:
+                    self.del_row_positions(len(self.row_positions) - 1 - undo_storage[4][0], undo_storage[4][0])
+                    self.data[:] = self.data[:-undo_storage[4][0]]
+                if undo_storage[4][1] > 0:
+                    quick_added_cols = undo_storage[4][1]
+                    self.del_col_positions(len(self.col_positions) - 1 - quick_added_cols, quick_added_cols)
+                    for rn in range(len(self.data)):
+                        self.data[rn][:] = self.data[rn][:-quick_added_cols]
+                    if not self.all_columns_displayed:
+                        self.displayed_columns[:] = self.displayed_columns[:-quick_added_cols]
+            if undo_storage[3]:
+                if isinstance(undo_storage[3][0], int):
+                    self.create_current(undo_storage[3][0], undo_storage[3][1], type_ = "cell", inside = True if self.cell_selected(undo_storage[3][0], undo_storage[3][1]) else False)
+                elif undo_storage[3][0] == "column":
+                    self.create_current(0, undo_storage[3][1], type_ = "column", inside = True)
+                elif undo_storage[3][0] == "row":
+                    self.create_current(undo_storage[3][1], 0, type_ = "row", inside = True)
+            elif start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
+                self.create_current(start_row, start_col, type_ = "cell", inside = True if self.cell_selected(start_row, start_col) else False)
+            if start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
+                self.see(r = start_row, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
+        
+        elif undo_storage[0] == "move_cols":
+            c = undo_storage[1]
+            to_move_min = undo_storage[2]
+            totalcols = len(undo_storage[4])
+            if to_move_min < c:
+                c += totalcols - 1
+            self.move_columns_adjust_options_dict(c, to_move_min, totalcols)
+        
+        elif undo_storage[0] == "move_rows":
+            rhs = [int(b - a) for a, b in zip(self.row_positions, islice(self.row_positions, 1, len(self.row_positions)))]
+            r = undo_storage[1]
+            to_move_min = undo_storage[2]
+            totalrows = len(undo_storage[4])
+            if to_move_min < r:
+                r += totalrows - 1
+            self.move_rows_adjust_options_dict(r, to_move_min, totalrows)
                     
-            elif undo_storage[0] == "insert_col":
-                self.displayed_columns = undo_storage[1]['displayed_columns']
-                qx = undo_storage[1]['data_col_num']
-                qnum = undo_storage[1]['numcols']
-                for rn in range(len(self.data)):
-                    self.data[rn][qx:qx + qnum] = []
+        elif undo_storage[0] == "insert_row":
+            self.data[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
+            try:
+                self._row_index[undo_storage[1]['data_row_num']:undo_storage[1]['data_row_num'] + undo_storage[1]['numrows']] = []
+            except:
+                pass
+            self.del_row_positions(undo_storage[1]['sheet_row_num'],
+                                    undo_storage[1]['numrows'],
+                                    deselect_all = False)
+            for r in range(undo_storage[1]['sheet_row_num'],
+                            undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']):
+                if r in self.row_options:
+                    del self.row_options[r]
+                if r in self.RI.cell_options:
+                    del self.RI.cell_options[r]
+            numrows = undo_storage[1]['numrows']
+            idx = undo_storage[1]['sheet_row_num'] + undo_storage[1]['numrows']
+            self.cell_options = {(rn if rn < idx else rn - numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()}
+            self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
+            self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
+            if len(self.row_positions) > 1:
+                start_row = undo_storage[1]['sheet_row_num'] if undo_storage[1]['sheet_row_num'] < len(self.row_positions) - 1 else undo_storage[1]['sheet_row_num'] - 1
+                self.RI.select_row(start_row)
+                self.see(r = start_row, c = 0, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
+                
+        elif undo_storage[0] == "insert_col":
+            self.displayed_columns = undo_storage[1]['displayed_columns']
+            qx = undo_storage[1]['data_col_num']
+            qnum = undo_storage[1]['numcols']
+            for rn in range(len(self.data)):
+                self.data[rn][qx:qx + qnum] = []
+            try:
+                self._headers[qx:qx + qnum] = []
+            except:
+                pass
+            self.del_col_positions(undo_storage[1]['sheet_col_num'],
+                                    undo_storage[1]['numcols'],
+                                    deselect_all = False)
+            for c in range(undo_storage[1]['sheet_col_num'],
+                            undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']):
+                if c in self.col_options:
+                    del self.col_options[c]
+                if c in self.CH.cell_options:
+                    del self.CH.cell_options[c]
+            numcols = undo_storage[1]['numcols']
+            idx = undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']
+            self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
+            self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items()}
+            self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items()}
+            if len(self.col_positions) > 1:
+                start_col = undo_storage[1]['sheet_col_num'] if undo_storage[1]['sheet_col_num'] < len(self.col_positions) - 1 else undo_storage[1]['sheet_col_num'] - 1
+                self.CH.select_col(start_col)
+                self.see(r = 0, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
+                
+        elif undo_storage[0] == "delete_rows":
+            for rn, r, h in reversed(undo_storage[1]['deleted_rows']):
+                self.data.insert(rn, r)
+                self.insert_row_position(idx = rn, height = h)
+            self.cell_options = undo_storage[1]['cell_options']
+            self.row_options = undo_storage[1]['row_options']
+            self.RI.cell_options = undo_storage[1]['RI_cell_options']
+            for rn, r in reversed(undo_storage[1]['deleted_index_values']):
                 try:
-                    self._headers[qx:qx + qnum] = []
+                    self._row_index.insert(rn, r)
                 except:
-                    pass
-                self.del_col_positions(undo_storage[1]['sheet_col_num'],
-                                       undo_storage[1]['numcols'],
-                                       deselect_all = False)
-                for c in range(undo_storage[1]['sheet_col_num'],
-                               undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']):
-                    if c in self.col_options:
-                        del self.col_options[c]
-                    if c in self.CH.cell_options:
-                        del self.CH.cell_options[c]
-                numcols = undo_storage[1]['numcols']
-                idx = undo_storage[1]['sheet_col_num'] + undo_storage[1]['numcols']
-                self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
-                self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items()}
-                self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items()}
-                if len(self.col_positions) > 1:
-                    start_col = undo_storage[1]['sheet_col_num'] if undo_storage[1]['sheet_col_num'] < len(self.col_positions) - 1 else undo_storage[1]['sheet_col_num'] - 1
-                    self.CH.select_col(start_col)
-                    self.see(r = 0, c = start_col, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
-                    
-            elif undo_storage[0] == "delete_rows":
-                for rn, r, h in reversed(undo_storage[1]['deleted_rows']):
-                    self.data.insert(rn, r)
-                    self.insert_row_position(idx = rn, height = h)
-                self.cell_options = undo_storage[1]['cell_options']
-                self.row_options = undo_storage[1]['row_options']
-                self.RI.cell_options = undo_storage[1]['RI_cell_options']
-                for rn, r in reversed(undo_storage[1]['deleted_index_values']):
-                    try:
-                        self._row_index.insert(rn, r)
-                    except:
-                        continue
-                self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
-                
-            elif undo_storage[0] == "delete_cols":
-                self.displayed_columns = undo_storage[1]['displayed_columns']
-                self.cell_options = undo_storage[1]['cell_options']
-                self.col_options = undo_storage[1]['col_options']
-                self.CH.cell_options = undo_storage[1]['CH_cell_options']
-                for cn, w in reversed(tuple(undo_storage[1]['colwidths'].items())):
-                    self.insert_col_position(idx = cn, width = w)
-                for cn, rowdict in reversed(tuple(undo_storage[1]['deleted_cols'].items())):
-                    for rn, v in rowdict.items():
-                        try:
-                            self.data[rn].insert(cn, v)
-                        except:
-                            continue
-                for cn, v in reversed(tuple(undo_storage[1]['deleted_hdr_values'].items())):
+                    continue
+            self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
+            
+        elif undo_storage[0] == "delete_cols":
+            self.displayed_columns = undo_storage[1]['displayed_columns']
+            self.cell_options = undo_storage[1]['cell_options']
+            self.col_options = undo_storage[1]['col_options']
+            self.CH.cell_options = undo_storage[1]['CH_cell_options']
+            for cn, w in reversed(tuple(undo_storage[1]['colwidths'].items())):
+                self.insert_col_position(idx = cn, width = w)
+            for cn, rowdict in reversed(tuple(undo_storage[1]['deleted_cols'].items())):
+                for rn, v in rowdict.items():
                     try:
-                        self._headers.insert(cn, v)
+                        self.data[rn].insert(cn, v)
                     except:
                         continue
-                self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
-            self.refresh()
-            if self.extra_end_ctrl_z_func is not None:
-                self.extra_end_ctrl_z_func(UndoEvent("end_ctrl_z", undo_storage[0], undo_storage))
-            
-    def bind_arrowkeys(self, event = None):
-        self.arrowkeys_enabled = True
+            for cn, v in reversed(tuple(undo_storage[1]['deleted_hdr_values'].items())):
+                try:
+                    self._headers.insert(cn, v)
+                except:
+                    continue
+            self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
+        self.refresh()
+        if self.extra_end_ctrl_z_func is not None:
+            self.extra_end_ctrl_z_func(UndoEvent("end_ctrl_z", undo_storage[0], undo_storage))
+
+    def bind_arrowkeys(self, keys: dict = {}):
         for canvas in (self, self.parentframe, self.CH, self.RI, self.TL):
-            canvas.bind("<Up>", self.arrowkey_UP)
-            canvas.bind("<Tab>", self.tab_key)
-            canvas.bind("<Right>", self.arrowkey_RIGHT)
-            canvas.bind("<Down>", self.arrowkey_DOWN)
-            canvas.bind("<Left>", self.arrowkey_LEFT)
-            canvas.bind("<Prior>", self.page_UP)
-            canvas.bind("<Next>", self.page_DOWN)
+            for k, func in keys.items():
+                canvas.bind(f"<{arrowkey_bindings_helper[k.lower()]}>", func)
 
-    def unbind_arrowkeys(self, event = None):
-        self.arrowkeys_enabled = False
+    def unbind_arrowkeys(self, keys: dict = {}):
         for canvas in (self, self.parentframe, self.CH, self.RI, self.TL):
-            canvas.unbind("<Up>")
-            canvas.unbind("<Right>")
-            canvas.unbind("<Tab>")
-            canvas.unbind("<Down>")
-            canvas.unbind("<Left>")
-            canvas.unbind("<Prior>")
-            canvas.unbind("<Next>")
+            for k, func in keys.items():
+                canvas.unbind(f"<{arrowkey_bindings_helper[k.lower()]}>")
 
     def see(self,
             r = None,
             c = None,
             keep_yscroll = False,
             keep_xscroll = False,
             bottom_right_corner = False,
@@ -1230,25 +1187,14 @@
             self.delete_selection_rects()
             self.create_current(r, c, type_ = "cell", inside = False)
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectCellEvent("select_cell", r, c))
 
-    def move_down(self):
-        currently_selected = self.currently_selected()
-        if currently_selected:
-            r, c = currently_selected.row, currently_selected.column
-            if (
-                r < len(self.row_positions) - 2 and
-                (self.single_selection_enabled or self.toggle_selection_enabled)
-                ):
-                self.select_cell(r + 1, c)
-                self.see(r + 1, c, keep_xscroll = True, bottom_right_corner = True, check_cell_visibility = True)
-
     def add_selection(self, r, c, redraw = False, run_binding_func = True, set_as_current = False):
         r = int(r)
         c = int(c)
         if set_as_current:
             items = self.find_withtag("Current_Outside")
             if items:
                 alltags = self.gettags(items[0])
@@ -1608,16 +1554,14 @@
             deselected = ("deselect_cell", deleted_boxes)
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.deselection_binding_func is not None:
             self.deselection_binding_func(DeselectionEvent(*deselected))
 
     def page_UP(self, event = None):
-        if not self.arrowkeys_enabled:
-            return
         height = self.winfo_height()
         top = self.canvasy(0)
         scrollto = top - height
         if scrollto < 0:
             scrollto = 0
         if self.page_up_down_select_row:
             r = bisect.bisect_left(self.row_positions, scrollto)
@@ -1636,16 +1580,14 @@
         else:
             args = ("moveto", scrollto / (self.row_positions[-1] + 100))
             self.yview(*args)
             self.RI.yview(*args)
             self.main_table_redraw_grid_and_text(redraw_row_index = True)
 
     def page_DOWN(self, event = None):
-        if not self.arrowkeys_enabled:
-            return
         height = self.winfo_height()
         top = self.canvasy(0)
         scrollto = top + height
         if self.page_up_down_select_row and self.RI.row_selection_enabled:
             r = bisect.bisect_left(self.row_positions, scrollto) - 1
             current = self.currently_selected()
             if current and current[0] == r:
@@ -1666,15 +1608,15 @@
             args = ("moveto", scrollto / (end + 100))
             self.yview(*args)
             self.RI.yview(*args)
             self.main_table_redraw_grid_and_text(redraw_row_index = True)
         
     def arrowkey_UP(self, event = None):
         currently_selected = self.currently_selected()
-        if not currently_selected or not self.arrowkeys_enabled:
+        if not currently_selected:
             return
         if currently_selected.type_ == "row":
             r = currently_selected.row
             if r != 0 and self.RI.row_selection_enabled:
                 if self.cell_completely_visible(r = r - 1, c = 0):
                     self.RI.select_row(r - 1, redraw = True)
                 else:
@@ -1691,15 +1633,15 @@
                     self.select_cell(r - 1, c, redraw = True)
                 else:
                     self.select_cell(r - 1, c)
                     self.see(r - 1, c, keep_xscroll = True, check_cell_visibility = False)
                 
     def arrowkey_RIGHT(self, event = None):
         currently_selected = self.currently_selected()
-        if not currently_selected or not self.arrowkeys_enabled:
+        if not currently_selected:
             return
         if currently_selected.type_ == "row":
             r = currently_selected.row
             if self.single_selection_enabled or self.toggle_selection_enabled:
                 if self.cell_completely_visible(r = r, c = 0):
                     self.select_cell(r, 0, redraw = True)
                 else:
@@ -1721,15 +1663,15 @@
                     self.select_cell(r, c + 1, redraw =True)
                 else:
                     self.select_cell(r, c + 1)
                     self.see(r, c + 1, keep_yscroll = True, bottom_right_corner = False if self.arrow_key_down_right_scroll_page else True, check_cell_visibility = False)
 
     def arrowkey_DOWN(self, event = None):
         currently_selected = self.currently_selected()
-        if not currently_selected or not self.arrowkeys_enabled:
+        if not currently_selected:
             return
         if currently_selected.type_ == "row":
             r = currently_selected.row
             if r < len(self.row_positions) - 2 and self.RI.row_selection_enabled:
                 if self.cell_completely_visible(r = min(r + 2, len(self.row_positions) - 2), c = 0):
                     self.RI.select_row(r + 1, redraw = True)
                 else:
@@ -1757,15 +1699,15 @@
                     if r + 2 < len(self.row_positions) - 2 and (self.row_positions[r + 3] - self.row_positions[r + 2]) + (self.row_positions[r + 2] - self.row_positions[r + 1]) + 5 < self.winfo_height():
                         self.see(r + 2, c, keep_xscroll = True, bottom_right_corner = True, check_cell_visibility = False)
                     elif not self.cell_completely_visible(r = r + 1, c = c):
                         self.see(r + 1, c, keep_xscroll = True, bottom_right_corner = False if self.arrow_key_down_right_scroll_page else True, check_cell_visibility = False)
                     
     def arrowkey_LEFT(self, event = None):
         currently_selected = self.currently_selected()
-        if not currently_selected or not self.arrowkeys_enabled:
+        if not currently_selected:
             return
         if currently_selected.type_ == "column":
             c = currently_selected.column
             if c != 0 and self.CH.col_selection_enabled:
                 if self.cell_completely_visible(r = 0, c = c - 1):
                     self.CH.select_col(c - 1, redraw = True)
                 else:
@@ -2198,15 +2140,15 @@
             self.CH.enable_bindings("drag_and_drop")
             self.CH.enable_bindings("double_click_column_resize")
             self.RI.enable_bindings("row_height_resize")
             self.RI.enable_bindings("double_click_row_resize")
             self.RI.enable_bindings("row_width_resize")
             self.RI.enable_bindings("row_select")
             self.RI.enable_bindings("drag_and_drop")
-            self.bind_arrowkeys()
+            self.bind_arrowkeys(self.arrowkey_binding_functions)
             self.edit_bindings(True)
             self.rc_delete_column_enabled = True
             self.rc_delete_row_enabled = True
             self.rc_insert_column_enabled = True
             self.rc_insert_row_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
@@ -2241,15 +2183,17 @@
             self.RI.enable_bindings("row_width_resize")
             self.TL.rw_state()
         elif binding == "row_select":
             self.RI.enable_bindings("row_select")
         elif binding == "row_drag_and_drop":
             self.RI.enable_bindings("drag_and_drop")
         elif binding == "arrowkeys":
-            self.bind_arrowkeys()
+            self.bind_arrowkeys(self.arrowkey_binding_functions)
+        elif binding in ("tab", "up", "right", "down", "left", "prior", "next"):
+            self.bind_arrowkeys(keys = {binding: self.arrowkey_binding_functions[binding]})
         elif binding == "edit_bindings":
             self.edit_bindings(True)
         elif binding == "rc_delete_column":
             self.rc_delete_column_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
         elif binding == "rc_delete_row":
@@ -2299,15 +2243,15 @@
             self.CH.disable_bindings("drag_and_drop")
             self.CH.disable_bindings("double_click_column_resize")
             self.RI.disable_bindings("row_height_resize")
             self.RI.disable_bindings("double_click_row_resize")
             self.RI.disable_bindings("row_width_resize")
             self.RI.disable_bindings("row_select")
             self.RI.disable_bindings("drag_and_drop")
-            self.unbind_arrowkeys()
+            self.unbind_arrowkeys(self.arrowkey_binding_functions)
             self.edit_bindings(False)
             self.rc_delete_column_enabled = False
             self.rc_delete_row_enabled = False
             self.rc_insert_column_enabled = False
             self.rc_insert_row_enabled = False
             self.rc_popup_menus_enabled = False
             self.rc_select_enabled = False
@@ -2340,15 +2284,17 @@
             self.RI.disable_bindings("row_width_resize")
             self.TL.rw_state("hidden")
         elif binding == "row_select":
             self.RI.disable_bindings("row_select")
         elif binding == "row_drag_and_drop":
             self.RI.disable_bindings("drag_and_drop")
         elif binding == "arrowkeys":
-            self.unbind_arrowkeys()
+            self.unbind_arrowkeys(self.arrowkey_binding_functions)
+        elif binding in ("tab", "up", "right", "down", "left", "prior", "next"):
+            self.unbind_arrowkeys(keys = {binding: self.arrowkey_binding_functions[binding]})
         elif binding == "rc_delete_column":
             self.rc_delete_column_enabled = False
         elif binding == "rc_delete_row":
             self.rc_delete_row_enabled = False
         elif binding == "rc_insert_column":
             self.rc_insert_column_enabled = False
         elif binding == "rc_insert_row":
@@ -2418,15 +2364,15 @@
                     pass
             if not mouse_over_resize:
                 self.reset_mouse_motion_creations()
         if self.extra_motion_func is not None:
             self.extra_motion_func(event)
 
     def rc(self, event = None):
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
         if self.single_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             r = self.identify_row(y = event.y)
             c = self.identify_col(x = event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 if self.col_selected(c):
@@ -2467,15 +2413,15 @@
                 popup_menu = self.empty_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def b1_press(self, event = None):
-        self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown()
+        self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         x1, y1, x2, y2 = self.get_canvas_visible_area()
         if self.identify_col(x = event.x, allow_end = False) is None or self.identify_row(y = event.y, allow_end = False) is None:
             self.deselect("all")
         r = self.identify_row(y = event.y)
         c = self.identify_col(x = event.x)
         if self.single_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
@@ -2518,15 +2464,15 @@
         self.disp_resize_lines = {}
         for t, sh in self.hidd_resize_lines.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_resize_lines[t] = False
 
     def shift_b1_press(self, event = None):
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if self.drag_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y = event.y))
             colsel = int(self.identify_col(x = event.x))
             if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
                 currently_selected = self.currently_selected()
@@ -2675,36 +2621,37 @@
             self.b1_pressed_loc = None
         self.RI.rsz_w = None
         self.CH.rsz_h = None
         if self.b1_pressed_loc is not None:
             r = self.identify_row(y = event.y, allow_end = False)
             c = self.identify_col(x = event.x, allow_end = False)
             if r is not None and c is not None and (r, c) == self.b1_pressed_loc:
-                dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-                if (r, dcol) in self.cell_options and ('dropdown' in self.cell_options[(r, dcol)] or 'checkbox' in self.cell_options[(r, dcol)]):
+                datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                if (r, datacn) in self.cell_options and ('dropdown' in self.cell_options[(r, datacn)] or 'checkbox' in self.cell_options[(r, datacn)]):
                     canvasx = self.canvasx(event.x)
-                    if (self.closed_dropdown != self.b1_pressed_loc and
-                        'dropdown' in self.cell_options[(r, dcol)] and
-                        canvasx > self.col_positions[c + 1] - self.txt_h - 5 and
-                        canvasx < self.col_positions[c + 1] - 1):
+                    if (
+                        (self.closed_dropdown != self.b1_pressed_loc and
+                         'dropdown' in self.cell_options[(r, datacn)] and
+                         canvasx > self.col_positions[c + 1] - self.txt_h - 5 and
+                         canvasx < self.col_positions[c + 1] - 1) 
+                        or
+                        ('checkbox' in self.cell_options[(r, datacn)] and 
+                         canvasx < self.col_positions[c] + self.txt_h + 5 and
+                         self.canvasy(event.y) < self.row_positions[r] + self.txt_h + 5)
+                        ):
                         self.open_cell(event)
-                    elif 'checkbox' in self.cell_options[(r, dcol)] and event.x < self.col_positions[c] + self.txt_h + 5 and event.y < self.row_positions[r] + self.txt_h + 5:
-                        self.open_cell(event)
-                        self.mouseclick_outside_editor_or_dropdown()
-                    else:
-                        self.mouseclick_outside_editor_or_dropdown()
             else:
-                self.mouseclick_outside_editor_or_dropdown()
+                self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.b1_pressed_loc = None
         self.closed_dropdown = None
         if self.extra_b1_release_func is not None:
             self.extra_b1_release_func(event)
 
     def double_b1(self, event = None):
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         x1, y1, x2, y2 = self.get_canvas_visible_area()
         if self.identify_col(x = event.x, allow_end = False) is None or self.identify_row(y = event.y, allow_end = False) is None:
             self.deselect("all")
         elif self.single_selection_enabled and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)):
             r = self.identify_row(y = event.y)
             c = self.identify_col(x = event.x)
@@ -2903,15 +2850,15 @@
             if reset_row_positions:
                 self.reset_row_positions()
         else:
             return self._font
 
     def set_fnt_help(self):
         self.txt_h = self.GetTextHeight("|ZXjy*'^")
-        self.txt_w = self.GetTextWidth("I")
+        self.txt_w = self.GetTextWidth("|")
         self.half_txt_h = ceil(self.txt_h / 2)
         if self.half_txt_h % 2 == 0:
             self.fl_ins = self.half_txt_h + 2
         else:
             self.fl_ins = self.half_txt_h + 3
         self.xtra_lines_increment = int(self.txt_h)
         self.min_rh = self.txt_h + 5
@@ -2942,15 +2889,15 @@
             self.hdr_fnt_wgt = newfont[2]
             self.set_hdr_fnt_help()
         else:
             return self._hdr_font
 
     def set_hdr_fnt_help(self):
         self.hdr_txt_h = self.GetHdrTextHeight("|ZXj*'^")
-        self.hdr_txt_w = self.GetHdrTextWidth("I")
+        self.hdr_txt_w = self.GetHdrTextWidth("|")
         self.hdr_half_txt_h = ceil(self.hdr_txt_h / 2)
         if self.hdr_half_txt_h % 2 == 0:
             self.hdr_fl_ins = self.hdr_half_txt_h + 2
         else:
             self.hdr_fl_ins = self.hdr_half_txt_h + 3
         self.hdr_xtra_lines_increment = self.hdr_txt_h
         self.hdr_min_rh = self.hdr_txt_h + 5
@@ -2959,17 +2906,27 @@
                                self.GetHdrLinesHeight(int(self.default_hh[0])) if self.default_hh[0] != "pixels" else self.default_hh[1])
         self.set_min_cw()
         self.CH.set_height(self.default_hh[1])
         
     def set_index_fnt_help(self):
         pass
 
-    def data_reference(self, newdataref = None, reset_col_positions = True, reset_row_positions = True, redraw = False, return_id = True):
+    def data_reference(self,
+                       newdataref = None, 
+                       reset_col_positions = True, 
+                       reset_row_positions = True,
+                       redraw = False, 
+                       return_id = True,
+                       keep_formatting = True):
         if isinstance(newdataref, (list, tuple)):
             self.data = newdataref
+            if keep_formatting:
+                self.reapply_formatting()
+            else:
+                self.delete_all_formatting(clear_values = False)
             self.undo_storage = deque(maxlen = self.max_undos)
             if reset_col_positions:
                 self.reset_col_positions()
             if reset_row_positions:
                 self.reset_row_positions()
             if redraw:
                 self.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
@@ -3118,17 +3075,17 @@
                     if txt:
                         itmcon(x2, text = txt)
                         b = itmbbx(x2)
                         w = b[2] - b[0] + self.hdr_txt_h + 7 if cn in self.CH.cell_options and 'dropdown' in self.CH.cell_options[cn] else b[2] - b[0] + 7
                     else:
                         w = self.min_cw + self.hdr_txt_h + 7 if cn in self.CH.cell_options and 'dropdown' in self.CH.cell_options[cn] else self.min_cw
                 except:
-                    if self.CH.default_hdr == "letters":
+                    if self.CH.default_header == "letters":
                         itmcon(x2, text = f"{num2alpha(cn)}")
-                    elif self.CH.default_hdr == "numbers":
+                    elif self.CH.default_header == "numbers":
                         itmcon(x2, text = f"{cn + 1}")
                     else:
                         itmcon(x2, text = f"{cn + 1} {num2alpha(cn)}")
                     b = itmbbx(x2)
                     w = b[2] - b[0] + 7
             for rn, r in enumerate(self.data):
                 if (rn, cn) in self.cell_options and 'checkbox' in self.cell_options[(rn, cn)]:
@@ -3444,21 +3401,21 @@
                                 del self._headers[self.displayed_columns[c]]
                             except:
                                 continue
             if self.undo_enabled:
                 self.undo_storage.append(("delete_cols", undo_storage))
             self.del_cell_options(list_of_coords)
             for c in reversed(seld_cols):
-                dcol = c if self.all_columns_displayed else self.displayed_columns[c]
+                datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                 self.del_col_position(c,
                                       deselect_all = False)
-                if dcol in self.col_options:
-                    del self.col_options[dcol]
-                if dcol in self.CH.cell_options:
-                    del self.CH.cell_options[dcol]
+                if datacn in self.col_options:
+                    del self.col_options[datacn]
+                if datacn in self.CH.cell_options:
+                    del self.CH.cell_options[datacn]
             numcols = len(seld_cols)
             idx = seld_cols[-1]
             self.cell_options = {(rn, cn if cn < idx else cn - numcols): t2 for (rn, cn), t2 in self.cell_options.items()}
             self.col_options = {cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items()}
             self.CH.cell_options = {cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items()}
             self.deselect("allcols", redraw = False)
             self.set_current_to_last()
@@ -3467,18 +3424,18 @@
                 for c in sorted(seldset):
                     self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
             self.refresh()
             if self.extra_end_del_cols_rc_func is not None:
                 self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
 
     def del_cell_options(self, list_of_coords):
-        for r, dcol in list_of_coords:
-            if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)]:
-                self.delete_dropdown(r, dcol)
-            del self.cell_options[(r, dcol)]
+        for r, datacn in list_of_coords:
+            if (r, datacn) in self.cell_options and 'dropdown' in self.cell_options[(r, datacn)]:
+                self.delete_dropdown(r, datacn)
+            del self.cell_options[(r, datacn)]
 
     def del_rows_rc(self, event = None):
         seld_rows = sorted(self.get_selected_rows())
         if seld_rows:
             if self.extra_begin_del_rows_rc_func is not None:
                 try:
                     self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
@@ -3712,31 +3669,32 @@
         else:
             if index is not None:
                 if isinstance(index, int):
                     return self._row_index[index]
             else:
                 return self._row_index
 
-    def total_data_cols(self, include_headers = True):
+    def total_data_cols(self, include_header = True):
         h_total = 0
         d_total = 0
-        if include_headers:
-            if isinstance(self._headers, list):
+        if include_header:
+            if isinstance(self._headers, (list, tuple)):
                 h_total = len(self._headers)
         try:
             d_total = len(max(self.data, key = len))
         except:
             pass
         return h_total if h_total > d_total else d_total
 
-    def total_data_rows(self):
+    def total_data_rows(self, include_index = True):
         i_total = 0
         d_total = 0
-        if isinstance(self._row_index, list):
-            i_total = len(self._row_index)
+        if include_index:
+            if isinstance(self._row_index, (list, tuple)):
+                i_total = len(self._row_index)
         d_total = len(self.data)
         return i_total if i_total > d_total else d_total
 
     def data_dimensions(self, total_rows = None, total_columns = None):
         if total_rows is None and total_columns is None:
             return self.total_data_rows(), self.total_data_cols()
         if total_rows is not None:
@@ -3771,133 +3729,133 @@
     def get_visible_columns(self, x1, x2):
         start_col = bisect.bisect_left(self.col_positions, x1)
         end_col = bisect.bisect_right(self.col_positions, x2)
         if not x2 >= self.col_positions[-1]:
             end_col += 1
         return start_col, end_col
 
-    def redraw_highlight_get_text_fg(self, r, c, fc, fr, sc, sr, c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, dcol, can_width):
+    def redraw_highlight_get_text_fg(self, r, c, fc, fr, sc, sr, c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, datarn, datacn, can_width):
         redrawn = False
         # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED CELLS ________________________
-        if (r, dcol) in self.cell_options and 'highlight' in self.cell_options[(r, dcol)] and (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg if self.cell_options[(r, dcol)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(r, dcol)]['highlight'][1]
-            if self.cell_options[(r, dcol)]['highlight'][0] is not None:
-                c_1 = self.cell_options[(r, dcol)]['highlight'][0] if self.cell_options[(r, dcol)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(r, dcol)]['highlight'][0]]
+        if (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and (r, c) in selected_cells:
+            tf = self.table_selected_cells_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
+            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
+                c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+                                                                                f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi")
             
-        elif r in self.row_options and 'highlight' in self.row_options[r] and (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg if self.row_options[r]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[r]['highlight'][1]
-            if self.row_options[r]['highlight'][0] is not None:
-                c_1 = self.row_options[r]['highlight'][0] if self.row_options[r]['highlight'][0].startswith("#") else Color_Map_[self.row_options[r]['highlight'][0]]
+        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and (r, c) in selected_cells:
+            tf = self.table_selected_cells_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
+            if self.row_options[datarn]['highlight'][0] is not None:
+                c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+                                                                                f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi",
-                                                can_width = can_width if self.row_options[r]['highlight'][2] else None)
+                                                can_width = can_width if self.row_options[datarn]['highlight'][2] else None)
             
-        elif dcol in self.col_options and 'highlight' in self.col_options[dcol] and (r, c) in selected_cells:
-            tf = self.table_selected_cells_fg if self.col_options[dcol]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[dcol]['highlight'][1]
-            if self.col_options[dcol]['highlight'][0] is not None:
-                c_1 = self.col_options[dcol]['highlight'][0] if self.col_options[dcol]['highlight'][0].startswith("#") else Color_Map_[self.col_options[dcol]['highlight'][0]]
+        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and (r, c) in selected_cells:
+            tf = self.table_selected_cells_fg if self.col_options[datacn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[datacn]['highlight'][1]
+            if self.col_options[datacn]['highlight'][0] is not None:
+                c_1 = self.col_options[datacn]['highlight'][0] if self.col_options[datacn]['highlight'][0].startswith("#") else Color_Map_[self.col_options[datacn]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_2_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+                                                                                f"{int((int(c_1[3:5], 16) + c_2_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_2_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi")
             
         # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED ROWS ________________________
-        elif (r, dcol) in self.cell_options and 'highlight' in self.cell_options[(r, dcol)] and r in actual_selected_rows:
-            tf = self.table_selected_rows_fg if self.cell_options[(r, dcol)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(r, dcol)]['highlight'][1]
-            if self.cell_options[(r, dcol)]['highlight'][0] is not None:
-                c_1 = self.cell_options[(r, dcol)]['highlight'][0] if self.cell_options[(r, dcol)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(r, dcol)]['highlight'][0]]
+        elif (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and r in actual_selected_rows:
+            tf = self.table_selected_rows_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
+            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
+                c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+                                                                                f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi")
             
-        elif r in self.row_options and 'highlight' in self.row_options[r] and r in actual_selected_rows:
-            tf = self.table_selected_rows_fg if self.row_options[r]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[r]['highlight'][1]
-            if self.row_options[r]['highlight'][0] is not None:
-                c_1 = self.row_options[r]['highlight'][0] if self.row_options[r]['highlight'][0].startswith("#") else Color_Map_[self.row_options[r]['highlight'][0]]
+        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and r in actual_selected_rows:
+            tf = self.table_selected_rows_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
+            if self.row_options[datarn]['highlight'][0] is not None:
+                c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+                                                                                f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi",
                                                 can_width = can_width if self.row_options[r]['highlight'][2] else None)
             
-        elif dcol in self.col_options and 'highlight' in self.col_options[dcol] and r in actual_selected_rows:
-            tf = self.table_selected_rows_fg if self.col_options[dcol]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[dcol]['highlight'][1]
-            if self.col_options[dcol]['highlight'][0] is not None:
-                c_1 = self.col_options[dcol]['highlight'][0] if self.col_options[dcol]['highlight'][0].startswith("#") else Color_Map_[self.col_options[dcol]['highlight'][0]]
+        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and r in actual_selected_rows:
+            tf = self.table_selected_rows_fg if self.col_options[datacn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[datacn]['highlight'][1]
+            if self.col_options[datacn]['highlight'][0] is not None:
+                c_1 = self.col_options[datacn]['highlight'][0] if self.col_options[datacn]['highlight'][0].startswith("#") else Color_Map_[self.col_options[datacn]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_4_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "",
+                                                                                f"{int((int(c_1[3:5], 16) + c_4_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_4_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
                                                 tag = "hi")
             
         # ________________________ CELL IS HIGHLIGHTED AND IN SELECTED COLUMNS ________________________
-        elif (r, dcol) in self.cell_options and 'highlight' in self.cell_options[(r, dcol)] and c in actual_selected_cols:
-            tf = self.table_selected_columns_fg if self.cell_options[(r, dcol)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(r, dcol)]['highlight'][1]
-            if self.cell_options[(r, dcol)]['highlight'][0] is not None:
-                c_1 = self.cell_options[(r, dcol)]['highlight'][0] if self.cell_options[(r, dcol)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(r, dcol)]['highlight'][0]]
+        elif (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and c in actual_selected_cols:
+            tf = self.table_selected_columns_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.cell_options[(datarn, datacn)]['highlight'][1]
+            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
+                c_1 = self.cell_options[(datarn, datacn)]['highlight'][0] if self.cell_options[(datarn, datacn)]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[(datarn, datacn)]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "",
+                                                                                f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
                                                 tag = "hi")
             
-        elif r in self.row_options and 'highlight' in self.row_options[r] and c in actual_selected_cols:
-            tf = self.table_selected_columns_fg if self.row_options[r]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[r]['highlight'][1]
-            if self.row_options[r]['highlight'][0] is not None:
-                c_1 = self.row_options[r]['highlight'][0] if self.row_options[r]['highlight'][0].startswith("#") else Color_Map_[self.row_options[r]['highlight'][0]]
+        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and c in actual_selected_cols:
+            tf = self.table_selected_columns_fg if self.row_options[datarn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.row_options[datarn]['highlight'][1]
+            if self.row_options[datarn]['highlight'][0] is not None:
+                c_1 = self.row_options[datarn]['highlight'][0] if self.row_options[datarn]['highlight'][0].startswith("#") else Color_Map_[self.row_options[datarn]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+                                                                                f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi",
-                                                can_width = can_width if self.row_options[r]['highlight'][2] else None)
+                                                can_width = can_width if self.row_options[datarn]['highlight'][2] else None)
             
-        elif dcol in self.col_options and 'highlight' in self.col_options[dcol] and c in actual_selected_cols:
-            tf = self.table_selected_columns_fg if self.col_options[dcol]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[dcol]['highlight'][1]
-            if self.col_options[dcol]['highlight'][0] is not None:
-                c_1 = self.col_options[dcol]['highlight'][0] if self.col_options[dcol]['highlight'][0].startswith("#") else Color_Map_[self.col_options[dcol]['highlight'][0]]
+        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and c in actual_selected_cols:
+            tf = self.table_selected_columns_fg if self.col_options[datacn]['highlight'][1] is None or self.display_selected_fg_over_highlights else self.col_options[datacn]['highlight'][1]
+            if self.col_options[datacn]['highlight'][0] is not None:
+                c_1 = self.col_options[datacn]['highlight'][0] if self.col_options[datacn]['highlight'][0].startswith("#") else Color_Map_[self.col_options[datacn]['highlight'][0]]
                 redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = (f"#{int((int(c_1[1:3], 16) + c_3_[0]) / 2):02X}" +
-                                                                      f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
-                                                                      f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "",
+                                                                                f"{int((int(c_1[3:5], 16) + c_3_[1]) / 2):02X}" +
+                                                                                f"{int((int(c_1[5:], 16) + c_3_[2]) / 2):02X}"),
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
                                                 tag = "hi")
 
         # ________________________ CELL IS HIGHLIGHTED AND NOT SELECTED ________________________
-        elif (r, dcol) in self.cell_options and 'highlight' in self.cell_options[(r, dcol)] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
-            tf = self.table_fg if self.cell_options[(r, dcol)]['highlight'][1] is None else self.cell_options[(r, dcol)]['highlight'][1]
-            if self.cell_options[(r, dcol)]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.cell_options[(r, dcol)]['highlight'][0],
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+        elif (datarn, datacn) in self.cell_options and 'highlight' in self.cell_options[(datarn, datacn)] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
+            tf = self.table_fg if self.cell_options[(datarn, datacn)]['highlight'][1] is None else self.cell_options[(datarn, datacn)]['highlight'][1]
+            if self.cell_options[(datarn, datacn)]['highlight'][0] is not None:
+                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.cell_options[(datarn, datacn)]['highlight'][0],
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi")
             
-        elif r in self.row_options and 'highlight' in self.row_options[r] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
-            tf = self.table_fg if self.row_options[r]['highlight'][1] is None else self.row_options[r]['highlight'][1]
-            if self.row_options[r]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.row_options[r]['highlight'][0],
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "", 
+        elif datarn in self.row_options and 'highlight' in self.row_options[datarn] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
+            tf = self.table_fg if self.row_options[datarn]['highlight'][1] is None else self.row_options[datarn]['highlight'][1]
+            if self.row_options[datarn]['highlight'][0] is not None:
+                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.row_options[datarn]['highlight'][0],
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "", 
                                                 tag = "hi",
-                                                can_width = can_width if self.row_options[r]['highlight'][2] else None)
+                                                can_width = can_width if self.row_options[datarn]['highlight'][2] else None)
             
-        elif dcol in self.col_options and 'highlight' in self.col_options[dcol] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
-            tf = self.table_fg if self.col_options[dcol]['highlight'][1] is None else self.col_options[dcol]['highlight'][1]
-            if self.col_options[dcol]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.col_options[dcol]['highlight'][0],
-                                                outline = self.table_fg if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)] and self.show_dropdown_borders else "",
+        elif datacn in self.col_options and 'highlight' in self.col_options[datacn] and (r, c) not in selected_cells and r not in actual_selected_rows and c not in actual_selected_cols:
+            tf = self.table_fg if self.col_options[datacn]['highlight'][1] is None else self.col_options[datacn]['highlight'][1]
+            if self.col_options[datacn]['highlight'][0] is not None:
+                redrawn = self.redraw_highlight(fc + 1, fr + 1, sc, sr, fill = self.col_options[datacn]['highlight'][0],
+                                                outline = self.table_fg if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)] and self.show_dropdown_borders else "",
                                                 tag = "hi")
         
         # ________________________ CELL IS JUST SELECTED ________________________
         elif (r, c) in selected_cells:
             tf = self.table_selected_cells_fg
         elif r in actual_selected_rows:
             tf = self.table_selected_rows_fg
@@ -4005,15 +3963,15 @@
                 x1, y2,
                 x1, y2-radius,
                 x1, y2-radius,
                 x1, y1+radius,
                 x1, y1+radius,
                 x1, y1]
 
-    def redraw_checkbox(self, r, dcol, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
+    def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
         points = self.get_checkbox_points(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill = outline, outline = fill)
             else:
@@ -4038,369 +3996,363 @@
                     self.itemconfig(t, fill = fill, outline = outline, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill = fill, outline = outline, tag = tag, smooth = True)
             self.disp_checkbox[t] = True
 
     def main_table_redraw_grid_and_text(self, redraw_header = False, redraw_row_index = False, redraw_table = True):
+        last_col_line_pos = self.col_positions[-1] + 1
+        last_row_line_pos = self.row_positions[-1] + 1
         try:
-            last_col_line_pos = self.col_positions[-1] + 1
-            last_row_line_pos = self.row_positions[-1] + 1
             can_width = self.winfo_width()
             can_height = self.winfo_height()
             self.configure(scrollregion = (0,
                                            0,
                                            last_col_line_pos + self.empty_horizontal,
                                            last_row_line_pos + self.empty_vertical))
-            if can_width >= last_col_line_pos + self.empty_horizontal and self.parentframe.xscroll_showing:
-                self.parentframe.xscroll.grid_forget()
-                self.parentframe.xscroll_showing = False
-            elif can_width < last_col_line_pos + self.empty_horizontal and not self.parentframe.xscroll_showing and not self.parentframe.xscroll_disabled and can_height > 45:
-                self.parentframe.xscroll.grid(row = 2, column = 0, columnspan = 2, sticky = "nswe")
-                self.parentframe.xscroll_showing = True
-            if can_height >= last_row_line_pos + self.empty_vertical and self.parentframe.yscroll_showing:
-                self.parentframe.yscroll.grid_forget()
-                self.parentframe.yscroll_showing = False
-            elif can_height < last_row_line_pos + self.empty_vertical and not self.parentframe.yscroll_showing and not self.parentframe.yscroll_disabled and can_width > 45:
-                self.parentframe.yscroll.grid(row = 0, column = 2, rowspan = 3, sticky = "nswe")
-                self.parentframe.yscroll_showing = True
-            scrollpos_bot = self.canvasy(can_height)
-            end_row = bisect.bisect_right(self.row_positions, scrollpos_bot)
-            if not scrollpos_bot >= self.row_positions[-1]:
-                end_row += 1
-            if redraw_row_index and self.show_index:
-                self.RI.auto_set_index_width(end_row - 1)
-            scrollpos_left = self.canvasx(0)
-            scrollpos_top = self.canvasy(0)
-            scrollpos_right = self.canvasx(can_width)
-            start_row = bisect.bisect_left(self.row_positions, scrollpos_top)
-            self.row_width_resize_bbox = (scrollpos_left, scrollpos_top, scrollpos_left + 2, scrollpos_bot)
-            self.header_height_resize_bbox = (scrollpos_left + 6, scrollpos_top, scrollpos_right, scrollpos_top + 2)
-            for k, v in self.disp_text.items():
-                if k in self.hidd_text:
-                    self.hidd_text[k] = self.hidd_text[k] | self.disp_text[k]
-                else:
-                    self.hidd_text[k] = v
-            self.disp_text = defaultdict(set)
-            for k, v in self.disp_high.items():
-                if k in self.hidd_high:
-                    self.hidd_high[k] = self.hidd_high[k] | self.disp_high[k]
-                else:
-                    self.hidd_high[k] = v
-            self.disp_high = defaultdict(set)
-            self.hidd_grid.update(self.disp_grid)
-            self.disp_grid = {}
-            self.hidd_dropdown.update(self.disp_dropdown)
-            self.disp_dropdown = {}
-            self.hidd_checkbox.update(self.disp_checkbox)
-            self.disp_checkbox = {}
-            start_col = bisect.bisect_left(self.col_positions, scrollpos_left)
-            end_col = bisect.bisect_right(self.col_positions, scrollpos_right)
-            if not scrollpos_right >= self.col_positions[-1]:
-                end_col += 1
-            if last_col_line_pos > scrollpos_right:
-                x_stop = scrollpos_right
-            else:
-                x_stop = last_col_line_pos
-            if last_row_line_pos > scrollpos_bot:
-                y_stop = scrollpos_bot
-            else:
-                y_stop = last_row_line_pos
-            scrollpos_bot_add2 = scrollpos_bot + 2
-            if self.show_horizontal_grid:
-                self.grid_cyc = cycle(self.grid_cyctup)
-                points = []
-                if self.horizontal_grid_to_end_of_window:
-                    x_grid_stop = scrollpos_right + can_width
-                else:
-                    if last_col_line_pos > scrollpos_right:
-                        x_grid_stop = x_stop + 1
-                    else:
-                        x_grid_stop = x_stop - 1
-                for r in range(start_row - 1, end_row):
-                    draw_y = self.row_positions[r]
-                    st_or_end = next(self.grid_cyc)
-                    if st_or_end == "st":
-                        points.extend([self.canvasx(0) - 1, draw_y, 
-                                       x_grid_stop, draw_y,
-                                       x_grid_stop, self.row_positions[r + 1] if len(self.row_positions) - 1 > r else draw_y])
-                    elif st_or_end == "end":
-                        points.extend([x_grid_stop, draw_y,
-                                       self.canvasx(0) - 1, draw_y,
-                                       self.canvasx(0) - 1, self.row_positions[r + 1] if len(self.row_positions) - 1 > r else draw_y])
-                if points:
-                    if self.hidd_grid:
-                        t, sh = self.hidd_grid.popitem()
-                        self.coords(t, points)
-                        if sh:
-                            self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1)
-                        else:
-                            self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, state = "normal")
-                        self.disp_grid[t] = True
+        except:
+            return
+        if can_width >= last_col_line_pos + self.empty_horizontal and self.parentframe.xscroll_showing:
+            self.parentframe.xscroll.grid_forget()
+            self.parentframe.xscroll_showing = False
+        elif can_width < last_col_line_pos + self.empty_horizontal and not self.parentframe.xscroll_showing and not self.parentframe.xscroll_disabled and can_height > 45:
+            self.parentframe.xscroll.grid(row = 2, column = 0, columnspan = 2, sticky = "nswe")
+            self.parentframe.xscroll_showing = True
+        if can_height >= last_row_line_pos + self.empty_vertical and self.parentframe.yscroll_showing:
+            self.parentframe.yscroll.grid_forget()
+            self.parentframe.yscroll_showing = False
+        elif can_height < last_row_line_pos + self.empty_vertical and not self.parentframe.yscroll_showing and not self.parentframe.yscroll_disabled and can_width > 45:
+            self.parentframe.yscroll.grid(row = 0, column = 2, rowspan = 3, sticky = "nswe")
+            self.parentframe.yscroll_showing = True
+        scrollpos_bot = self.canvasy(can_height)
+        end_row = bisect.bisect_right(self.row_positions, scrollpos_bot)
+        if not scrollpos_bot >= self.row_positions[-1]:
+            end_row += 1
+        if redraw_row_index and self.show_index:
+            self.RI.auto_set_index_width(end_row - 1)
+        scrollpos_left = self.canvasx(0)
+        scrollpos_top = self.canvasy(0)
+        scrollpos_right = self.canvasx(can_width)
+        start_row = bisect.bisect_left(self.row_positions, scrollpos_top)
+        self.row_width_resize_bbox = (scrollpos_left, scrollpos_top, scrollpos_left + 2, scrollpos_bot)
+        self.header_height_resize_bbox = (scrollpos_left + 6, scrollpos_top, scrollpos_right, scrollpos_top + 2)
+        for k, v in self.disp_text.items():
+            if k in self.hidd_text:
+                self.hidd_text[k] = self.hidd_text[k] | self.disp_text[k]
+            else:
+                self.hidd_text[k] = v
+        self.disp_text = defaultdict(set)
+        for k, v in self.disp_high.items():
+            if k in self.hidd_high:
+                self.hidd_high[k] = self.hidd_high[k] | self.disp_high[k]
+            else:
+                self.hidd_high[k] = v
+        self.disp_high = defaultdict(set)
+        self.hidd_grid.update(self.disp_grid)
+        self.disp_grid = {}
+        self.hidd_dropdown.update(self.disp_dropdown)
+        self.disp_dropdown = {}
+        self.hidd_checkbox.update(self.disp_checkbox)
+        self.disp_checkbox = {}
+        start_col = bisect.bisect_left(self.col_positions, scrollpos_left)
+        end_col = bisect.bisect_right(self.col_positions, scrollpos_right)
+        if not scrollpos_right >= self.col_positions[-1]:
+            end_col += 1
+        if last_col_line_pos > scrollpos_right:
+            x_stop = scrollpos_right
+        else:
+            x_stop = last_col_line_pos
+        if last_row_line_pos > scrollpos_bot:
+            y_stop = scrollpos_bot
+        else:
+            y_stop = last_row_line_pos
+        row_pos_exists = self.row_positions != [0] and self.row_positions
+        col_pos_exists = self.col_positions != [0] and self.col_positions
+        if self.show_horizontal_grid and row_pos_exists:
+            self.grid_cyc = cycle(self.grid_cyctup)
+            points = []
+            if self.horizontal_grid_to_end_of_window:
+                x_grid_stop = scrollpos_right + can_width
+            else:
+                if last_col_line_pos > scrollpos_right:
+                    x_grid_stop = x_stop + 1
+                else:
+                    x_grid_stop = x_stop - 1
+            for r in range(start_row - 1, end_row):
+                draw_y = self.row_positions[r]
+                st_or_end = next(self.grid_cyc)
+                if st_or_end == "st":
+                    points.extend([self.canvasx(0) - 1, draw_y, 
+                                    x_grid_stop, draw_y,
+                                    x_grid_stop, self.row_positions[r + 1] if len(self.row_positions) - 1 > r else draw_y])
+                elif st_or_end == "end":
+                    points.extend([x_grid_stop, draw_y,
+                                    self.canvasx(0) - 1, draw_y,
+                                    self.canvasx(0) - 1, self.row_positions[r + 1] if len(self.row_positions) - 1 > r else draw_y])
+            if points:
+                if self.hidd_grid:
+                    t, sh = self.hidd_grid.popitem()
+                    self.coords(t, points)
+                    if sh:
+                        self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1)
                     else:
-                        self.disp_grid[self.create_line(points, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, tag = "g")] = True
-            if self.show_vertical_grid:
-                self.grid_cyc = cycle(self.grid_cyctup)
-                points = []
-                if self.vertical_grid_to_end_of_window:
-                    y_grid_stop = scrollpos_bot + can_height
+                        self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, state = "normal")
+                    self.disp_grid[t] = True
                 else:
-                    if last_row_line_pos > scrollpos_bot:
-                        y_grid_stop = y_stop + 1
-                    else:
-                        y_grid_stop = y_stop - 1
-                for c in range(start_col - 1, end_col):
-                    draw_x = self.col_positions[c]
-                    st_or_end = next(self.grid_cyc)
-                    if st_or_end == "st":
-                        points.extend([draw_x, scrollpos_top - 1,
-                                       draw_x, y_grid_stop,
-                                       self.col_positions[c + 1] if len(self.col_positions) - 1 > c else draw_x, y_grid_stop])
-                    elif st_or_end == "end":
-                        points.extend([draw_x, y_grid_stop,
-                                       draw_x, scrollpos_top - 1,
-                                       self.col_positions[c + 1] if len(self.col_positions) - 1 > c else draw_x, scrollpos_top - 1])
-                if points:
-                    if self.hidd_grid:
-                        t, sh = self.hidd_grid.popitem()
-                        self.coords(t, points)
-                        if sh:
-                            self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1)
-                        else:
-                            self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, state = "normal")
-                        self.disp_grid[t] = True
+                    self.disp_grid[self.create_line(points, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, tag = "g")] = True
+        if self.show_vertical_grid and col_pos_exists:
+            self.grid_cyc = cycle(self.grid_cyctup)
+            points = []
+            if self.vertical_grid_to_end_of_window:
+                y_grid_stop = scrollpos_bot + can_height
+            else:
+                if last_row_line_pos > scrollpos_bot:
+                    y_grid_stop = y_stop + 1
+                else:
+                    y_grid_stop = y_stop - 1
+            for c in range(start_col - 1, end_col):
+                draw_x = self.col_positions[c]
+                st_or_end = next(self.grid_cyc)
+                if st_or_end == "st":
+                    points.extend([draw_x, scrollpos_top - 1,
+                                    draw_x, y_grid_stop,
+                                    self.col_positions[c + 1] if len(self.col_positions) - 1 > c else draw_x, y_grid_stop])
+                elif st_or_end == "end":
+                    points.extend([draw_x, y_grid_stop,
+                                    draw_x, scrollpos_top - 1,
+                                    self.col_positions[c + 1] if len(self.col_positions) - 1 > c else draw_x, scrollpos_top - 1])
+            if points:
+                if self.hidd_grid:
+                    t, sh = self.hidd_grid.popitem()
+                    self.coords(t, points)
+                    if sh:
+                        self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1)
                     else:
-                        self.disp_grid[self.create_line(points, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, tag = "g")] = True
-            if start_row > 0:
-                start_row -= 1
-            if start_col > 0:
-                start_col -= 1
-            end_row -= 1
-            c_2 = self.table_selected_cells_bg if self.table_selected_cells_bg.startswith("#") else Color_Map_[self.table_selected_cells_bg]
-            c_2_ = (int(c_2[1:3], 16), int(c_2[3:5], 16), int(c_2[5:], 16))
-            c_3 = self.table_selected_columns_bg if self.table_selected_columns_bg.startswith("#") else Color_Map_[self.table_selected_columns_bg]
-            c_3_ = (int(c_3[1:3], 16), int(c_3[3:5], 16), int(c_3[5:], 16))
-            c_4 = self.table_selected_rows_bg if self.table_selected_rows_bg.startswith("#") else Color_Map_[self.table_selected_rows_bg]
-            c_4_ = (int(c_4[1:3], 16), int(c_4[3:5], 16), int(c_4[5:], 16))
-            rows_ = tuple(range(start_row, end_row))
-            selected_cells, selected_rows, selected_cols, actual_selected_rows, actual_selected_cols = self.get_redraw_selections((start_row, start_col, end_row, end_col - 1))
-            font = self._font
-            if redraw_table:
-                for c in range(start_col, end_col - 1):
-                    for r in rows_:
-                        rtopgridln = self.row_positions[r]
-                        rbotgridln = self.row_positions[r + 1]
-                        if rbotgridln - rtopgridln < self.txt_h:
-                            continue
-                        if rbotgridln > scrollpos_bot_add2:
-                            rbotgridln = scrollpos_bot_add2
-                        cleftgridln = self.col_positions[c]
-                        crightgridln = self.col_positions[c + 1]
+                        self.itemconfig(t, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, state = "normal")
+                    self.disp_grid[t] = True
+                else:
+                    self.disp_grid[self.create_line(points, fill = self.table_grid_fg, capstyle = tk.BUTT, joinstyle = tk.ROUND, width = 1, tag = "g")] = True
+        if start_row > 0:
+            start_row -= 1
+        if start_col > 0:
+            start_col -= 1
+        end_row -= 1
+        c_2 = self.table_selected_cells_bg if self.table_selected_cells_bg.startswith("#") else Color_Map_[self.table_selected_cells_bg]
+        c_2_ = (int(c_2[1:3], 16), int(c_2[3:5], 16), int(c_2[5:], 16))
+        c_3 = self.table_selected_columns_bg if self.table_selected_columns_bg.startswith("#") else Color_Map_[self.table_selected_columns_bg]
+        c_3_ = (int(c_3[1:3], 16), int(c_3[3:5], 16), int(c_3[5:], 16))
+        c_4 = self.table_selected_rows_bg if self.table_selected_rows_bg.startswith("#") else Color_Map_[self.table_selected_rows_bg]
+        c_4_ = (int(c_4[1:3], 16), int(c_4[3:5], 16), int(c_4[5:], 16))
+        rows_ = tuple(range(start_row, end_row))
+        selected_cells, selected_rows, selected_cols, actual_selected_rows, actual_selected_cols = self.get_redraw_selections((start_row, start_col, end_row, end_col - 1))
+        font = self._font
+        if redraw_table:
+            for c in range(start_col, end_col - 1):
+                for r in rows_:
+                    rtopgridln = self.row_positions[r]
+                    rbotgridln = self.row_positions[r + 1]
+                    if rbotgridln - rtopgridln < self.txt_h:
+                        continue
+                    cleftgridln = self.col_positions[c]
+                    crightgridln = self.col_positions[c + 1]
+                    
+                    datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+                    
+                    fill, dd_drawn = self.redraw_highlight_get_text_fg(r, c, cleftgridln, rtopgridln, crightgridln, rbotgridln,
+                                                                        c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, 
+                                                                        datarn, datacn, can_width)
                         
-                        if self.all_columns_displayed:
-                            dcol = c
+                    if (datarn, datacn) in self.cell_options and 'align' in self.cell_options[(datarn, datacn)]:
+                        align = self.cell_options[(datarn, datacn)]['align']
+                    elif datarn in self.row_options and 'align' in self.row_options[datarn]:
+                        align = self.row_options[datarn]['align']
+                    elif datacn in self.col_options and 'align' in self.col_options[datacn]:
+                        align = self.col_options[datacn]['align']
+                    else:
+                        align = self.align
+                    
+                    if align == "w":
+                        draw_x = cleftgridln + 3
+                        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+                            mw = crightgridln - cleftgridln - self.txt_h - 2
+                            self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
+                                                fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
+                                                dd_is_open = self.cell_options[(datarn, datacn)]['dropdown']['window'] != "no dropdown open")
                         else:
-                            dcol = self.displayed_columns[c]
-                        
-                        fill, dd_drawn = self.redraw_highlight_get_text_fg(r, c, cleftgridln, rtopgridln, crightgridln, rbotgridln, c_2_, c_3_, c_4_, selected_cells, actual_selected_rows, actual_selected_cols, dcol, can_width)
-                            
-                        if (r, dcol) in self.cell_options and 'align' in self.cell_options[(r, dcol)]:
-                            align = self.cell_options[(r, dcol)]['align']
-                        elif r in self.row_options and 'align' in self.row_options[r]:
-                            align = self.row_options[r]['align']
-                        elif dcol in self.col_options and 'align' in self.col_options[dcol]:
-                            align = self.col_options[dcol]['align']
+                            mw = crightgridln - cleftgridln - 1
+
+                    elif align == "e":
+                        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+                            mw = crightgridln - cleftgridln - self.txt_h - 2
+                            draw_x = crightgridln - 5 - self.txt_h
+                            self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
+                                                fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
+                                                dd_is_open = self.cell_options[(datarn, datacn)]['dropdown']['window'] != "no dropdown open")
                         else:
-                            align = self.align
-                        
-                        if align == "w":
-                            draw_x = cleftgridln + 3
-                            if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)]:
-                                mw = crightgridln - cleftgridln - self.txt_h - 2
-                                self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
-                                                    fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                                    dd_is_open = self.cell_options[(r, dcol)]['dropdown']['window'] != "no dropdown open")
-                            else:
-                                mw = crightgridln - cleftgridln - 1
-                            
+                            mw = crightgridln - cleftgridln - 1
+                            draw_x = crightgridln - 3
 
-                        elif align == "e":
-                            if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)]:
-                                mw = crightgridln - cleftgridln - self.txt_h - 2
-                                draw_x = crightgridln - 5 - self.txt_h
-                                self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
-                                                    fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                                    dd_is_open = self.cell_options[(r, dcol)]['dropdown']['window'] != "no dropdown open")
-                            else:
-                                mw = crightgridln - cleftgridln - 1
-                                draw_x = crightgridln - 3
+                    elif align == "center":
+                        stop = cleftgridln + 5
+                        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+                            mw = crightgridln - cleftgridln - self.txt_h - 2
+                            draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.txt_h) / 2)
+                            self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
+                                                fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
+                                                dd_is_open = self.cell_options[(datarn, datacn)]['dropdown']['window'] != "no dropdown open")
+                        else:
+                            mw = crightgridln - cleftgridln - 1
+                            draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
 
-                        elif align == "center":
-                            stop = cleftgridln + 5
-                            if (r, dcol) in self.cell_options and 'dropdown' in self.cell_options[(r, dcol)]:
-                                mw = crightgridln - cleftgridln - self.txt_h - 2
-                                draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.txt_h) / 2)
-                                self.redraw_dropdown(cleftgridln, rtopgridln, crightgridln, self.row_positions[r + 1], 
-                                                    fill = fill, outline = fill, tag = f"dd_{r}_{c}", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                                    dd_is_open = self.cell_options[(r, dcol)]['dropdown']['window'] != "no dropdown open")
+                    if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+                        if mw > self.txt_h + 2:
+                            box_w = self.txt_h + 1
+                            mw -= box_w
+                            if align == "w":
+                                draw_x += box_w + 1
+                            elif align == "center":
+                                draw_x += ceil(box_w / 2) + 1
+                                mw -= 1
                             else:
-                                mw = crightgridln - cleftgridln - 1
-                                draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
-
-                        if (r, dcol) in self.cell_options and 'checkbox' in self.cell_options[(r, dcol)]:
-                            if mw > self.txt_h + 2:
-                                box_w = self.txt_h + 1
-                                mw -= box_w
-                                if align == "w":
-                                    draw_x += box_w + 1
-                                elif align == "center":
-                                    draw_x += ceil(box_w / 2) + 1
-                                    mw -= 1
-                                else:
-                                    mw -= 3
-                                try:
-                                    draw_check = self.data[r][dcol]
-                                except:
-                                    draw_check = False
-                                self.redraw_checkbox(r,
-                                                    dcol,
-                                                    cleftgridln + 2,
+                                mw -= 3
+                            try:
+                                draw_check = self.data[datarn][datacn]
+                            except:
+                                draw_check = False
+                            self.redraw_checkbox(cleftgridln + 2,
                                                     rtopgridln + 2,
                                                     cleftgridln + self.txt_h + 3,
                                                     rtopgridln + self.txt_h + 3,
-                                                    fill = fill if self.cell_options[(r, dcol)]['checkbox']['state'] == "normal" else self.table_grid_fg,
+                                                    fill = fill if self.cell_options[(datarn, datacn)]['checkbox']['state'] == "normal" else self.table_grid_fg,
                                                     outline = "", tag = "cb", draw_check = draw_check)
 
-                        if (r, dcol) in self.cell_options and 'checkbox' in self.cell_options[(r, dcol)]:
-                            lns = self.cell_options[(r, dcol)]['checkbox']['text'].split("\n") if isinstance(self.cell_options[(r, dcol)]['checkbox']['text'], str) else f"{self.cell_options[(r, dcol)]['checkbox']['text']}".split("\n")
-                        elif len(self.data) > r and len(self.data[r]) > dcol:
-                            lns = self.data[r][dcol].split("\n") if isinstance(self.data[r][dcol], str) else f"{self.data[r][dcol]}".split("\n")
-                        else:
-                            continue
-                        if lns != [''] and mw > self.txt_w and not ((align == "w" and draw_x > scrollpos_right) or
-                                                                    (align == "e" and cleftgridln + 5 > scrollpos_right) or
-                                                                    (align == "center" and stop > scrollpos_right)):
-                            draw_y = rtopgridln + self.fl_ins
-                            start_ln = int((scrollpos_top - rtopgridln) / self.xtra_lines_increment)
-                            if start_ln < 0:
-                                start_ln = 0
-                            draw_y += start_ln * self.xtra_lines_increment
-                            if draw_y + self.half_txt_h - 1 <= rbotgridln and len(lns) > start_ln:
-                                for txt in islice(lns, start_ln, None):
-                                    # for performance improvements in redrawing especially when just selecting cells
-                                    # option 0: text doesn't need moving or config
-                                    # option 1: text needs new x, y but has same config
-                                    # option 2: text needs new config but has same x, y
-                                    # option 3: text needs new x, y and new config
-                                    # option 4: text needs to be created
-                                    config = TextCfg(txt, fill, font, align)
-                                    k = None
-                                    if config in self.hidd_text:
-                                        k = config
-                                        iid, showing = self.hidd_text[k].pop()
-                                        cc1, cc2 = self.coords(iid)
-                                        if (int(cc1) == int(draw_x) and
-                                            int(cc2) == int(draw_y)):
-                                            option = 0 if showing else 2
-                                        else:
-                                            option = 1 if showing else 3
-                                    elif self.hidd_text:
-                                        k = next(iter(self.hidd_text))
-                                        iid, showing = self.hidd_text[k].pop()
-                                        cc1, cc2 = self.coords(iid)
-                                        if (int(cc1) == int(draw_x) and
-                                            int(cc2) == int(draw_y)):
-                                            option = 2 if showing else 3
-                                        else:
-                                            option = 3
+                    if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+                        lns = self.cell_options[(datarn, datacn)]['checkbox']['text'].split("\n") if isinstance(self.cell_options[(datarn, datacn)]['checkbox']['text'], str) else f"{self.cell_options[(datarn, datacn)]['checkbox']['text']}".split("\n")
+                    else:
+                        lns = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed = True).split("\n")
+                    if lns != [''] and mw > self.txt_w and not ((align == "w" and draw_x > scrollpos_right) or
+                                                                (align == "e" and cleftgridln + 5 > scrollpos_right) or
+                                                                (align == "center" and stop > scrollpos_right)):
+                        draw_y = rtopgridln + self.fl_ins
+                        start_ln = int((scrollpos_top - rtopgridln) / self.xtra_lines_increment)
+                        if start_ln < 0:
+                            start_ln = 0
+                        draw_y += start_ln * self.xtra_lines_increment
+                        if draw_y + self.half_txt_h - 1 <= rbotgridln and len(lns) > start_ln:
+                            for txt in islice(lns, start_ln, None):
+                                # for performance improvements in redrawing especially when just selecting cells
+                                # option 0: text doesn't need moving or config
+                                # option 1: text needs new x, y but has same config
+                                # option 2: text needs new config but has same x, y
+                                # option 3: text needs new x, y and new config
+                                # option 4: text needs to be created
+                                config = TextCfg(txt, fill, font, align)
+                                k = None
+                                if config in self.hidd_text:
+                                    k = config
+                                    iid, showing = self.hidd_text[k].pop()
+                                    cc1, cc2 = self.coords(iid)
+                                    if (int(cc1) == int(draw_x) and
+                                        int(cc2) == int(draw_y)):
+                                        option = 0 if showing else 2
                                     else:
-                                        iid, showing, option = self.create_text(draw_x, draw_y, text = txt, fill = fill, font = font, anchor = align, tag = "t"), 1, 4
-                                    if option in (1, 3):
-                                        self.coords(iid, draw_x, draw_y)
-                                    if option in (2, 3):
-                                        if showing:
-                                            self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align)
-                                        else:
-                                            self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align, state = "normal")
-                                    if k is not None and not self.hidd_text[k]:
-                                        del self.hidd_text[k]
-                                    wd = self.bbox(iid)
-                                    wd = wd[2] - wd[0]
-                                    if wd > mw:
-                                        if align == "w":
-                                            txt = txt[:int(len(txt) * (mw / wd))]
+                                        option = 1 if showing else 3
+                                elif self.hidd_text:
+                                    k = next(iter(self.hidd_text))
+                                    iid, showing = self.hidd_text[k].pop()
+                                    cc1, cc2 = self.coords(iid)
+                                    if (int(cc1) == int(draw_x) and
+                                        int(cc2) == int(draw_y)):
+                                        option = 2 if showing else 3
+                                    else:
+                                        option = 3
+                                else:
+                                    iid, showing, option = self.create_text(draw_x, draw_y, text = txt, fill = fill, font = font, anchor = align, tag = "t"), 1, 4
+                                if option in (1, 3):
+                                    self.coords(iid, draw_x, draw_y)
+                                if option in (2, 3):
+                                    if showing:
+                                        self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align)
+                                    else:
+                                        self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align, state = "normal")
+                                if k is not None and not self.hidd_text[k]:
+                                    del self.hidd_text[k]
+                                wd = self.bbox(iid)
+                                wd = wd[2] - wd[0]
+                                if wd > mw:
+                                    if align == "w":
+                                        txt = txt[:int(len(txt) * (mw / wd))]
+                                        self.itemconfig(iid, text = txt)
+                                        wd = self.bbox(iid)
+                                        while wd[2] - wd[0] > mw:
+                                            txt = txt[:-1]
                                             self.itemconfig(iid, text = txt)
                                             wd = self.bbox(iid)
-                                            while wd[2] - wd[0] > mw:
-                                                txt = txt[:-1]
-                                                self.itemconfig(iid, text = txt)
-                                                wd = self.bbox(iid)
-                                        elif align == "e":
-                                            txt = txt[len(txt) - int(len(txt) * (mw / wd)):]
+                                    elif align == "e":
+                                        txt = txt[len(txt) - int(len(txt) * (mw / wd)):]
+                                        self.itemconfig(iid, text = txt)
+                                        wd = self.bbox(iid)
+                                        while wd[2] - wd[0] > mw:
+                                            txt = txt[1:]
                                             self.itemconfig(iid, text = txt)
                                             wd = self.bbox(iid)
-                                            while wd[2] - wd[0] > mw:
-                                                txt = txt[1:]
-                                                self.itemconfig(iid, text = txt)
-                                                wd = self.bbox(iid)
-                                        elif align == "center":
-                                            self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
-                                            tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
-                                            txt = txt[tmod - 1:-tmod]
+                                    elif align == "center":
+                                        self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
+                                        tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
+                                        txt = txt[tmod - 1:-tmod]
+                                        self.itemconfig(iid, text = txt)
+                                        wd = self.bbox(iid)
+                                        while wd[2] - wd[0] > mw:
+                                            txt = txt[next(self.c_align_cyc)]
                                             self.itemconfig(iid, text = txt)
                                             wd = self.bbox(iid)
-                                            while wd[2] - wd[0] > mw:
-                                                txt = txt[next(self.c_align_cyc)]
-                                                self.itemconfig(iid, text = txt)
-                                                wd = self.bbox(iid)
-                                            self.coords(iid, draw_x, draw_y)
-                                        self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = 1))
-                                    else:
-                                        self.disp_text[config].add(DrawnItem(iid = iid, showing = 1))
-                                    draw_y += self.xtra_lines_increment
-                                    if draw_y + self.half_txt_h - 1 > rbotgridln:
-                                        break
-            if redraw_table:
-                self.tag_raise("t")
-                for cfg, set_ in self.hidd_text.items():
-                    for namedtup in tuple(set_):
-                        if namedtup.showing:
-                            self.itemconfig(namedtup.iid, state = "hidden")
-                            self.hidd_text[cfg].discard(namedtup)
-                            self.hidd_text[cfg].add(namedtup._replace(showing = 0))
-                for cfg, set_ in self.hidd_high.items():
-                    for namedtup in tuple(set_):
-                        if namedtup.showing:
-                            self.itemconfig(namedtup.iid, state = "hidden")
-                            self.hidd_high[cfg].discard(namedtup)
-                            self.hidd_high[cfg].add(namedtup._replace(showing = 0))
-                for t, sh in self.hidd_grid.items():
-                    if sh:
-                        self.itemconfig(t, state = "hidden")
-                        self.hidd_grid[t] = False
-                for t, sh in self.hidd_dropdown.items():
-                    if sh:
-                        self.itemconfig(t, state = "hidden")
-                        self.hidd_dropdown[t] = False
-                for t, sh in self.hidd_checkbox.items():
-                    if sh:
-                        self.itemconfig(t, state = "hidden")
-                        self.hidd_checkbox[t] = False
-                if self.show_selected_cells_border:
-                    self.tag_raise("CellSelectBorder")
-                    self.tag_raise("Current_Inside")
-                    self.tag_raise("Current_Outside")
-                    self.tag_raise("RowSelectBorder")
-                    self.tag_raise("ColSelectBorder")
-            if redraw_header and self.show_header:
-                self.CH.redraw_grid_and_text(last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, selected_cols, actual_selected_rows, actual_selected_cols)
-            if redraw_row_index and self.show_index:
-                self.RI.redraw_grid_and_text(last_row_line_pos, scrollpos_top, y_stop, start_row, end_row + 1, scrollpos_bot, selected_rows, actual_selected_cols, actual_selected_rows)
-        except:
-            return False
+                                        self.coords(iid, draw_x, draw_y)
+                                    self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
+                                else:
+                                    self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
+                                draw_y += self.xtra_lines_increment
+                                if draw_y + self.half_txt_h - 1 > rbotgridln:
+                                    break
+        if redraw_table:
+            self.tag_raise("t")
+            for cfg, set_ in self.hidd_text.items():
+                for namedtup in tuple(set_):
+                    if namedtup.showing:
+                        self.itemconfig(namedtup.iid, state = "hidden")
+                        self.hidd_text[cfg].discard(namedtup)
+                        self.hidd_text[cfg].add(namedtup._replace(showing = False))
+            for cfg, set_ in self.hidd_high.items():
+                for namedtup in tuple(set_):
+                    if namedtup.showing:
+                        self.itemconfig(namedtup.iid, state = "hidden")
+                        self.hidd_high[cfg].discard(namedtup)
+                        self.hidd_high[cfg].add(namedtup._replace(showing = False))
+            for t, sh in self.hidd_grid.items():
+                if sh:
+                    self.itemconfig(t, state = "hidden")
+                    self.hidd_grid[t] = False
+            for t, sh in self.hidd_dropdown.items():
+                if sh:
+                    self.itemconfig(t, state = "hidden")
+                    self.hidd_dropdown[t] = False
+            for t, sh in self.hidd_checkbox.items():
+                if sh:
+                    self.itemconfig(t, state = "hidden")
+                    self.hidd_checkbox[t] = False
+            if self.show_selected_cells_border:
+                self.tag_raise("CellSelectBorder")
+                self.tag_raise("Current_Inside")
+                self.tag_raise("Current_Outside")
+                self.tag_raise("RowSelectBorder")
+                self.tag_raise("ColSelectBorder")
+        if redraw_header and self.show_header:
+            self.CH.redraw_grid_and_text(last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, scrollpos_right, selected_cols, actual_selected_rows, actual_selected_cols, col_pos_exists)
+        if redraw_row_index and self.show_index:
+            self.RI.redraw_grid_and_text(last_row_line_pos, scrollpos_top, y_stop, start_row, end_row + 1, scrollpos_bot, selected_rows, actual_selected_cols, actual_selected_rows, row_pos_exists)
         return True
 
     def get_all_selection_items(self):
         return sorted(self.find_withtag("CellSelectFill") + self.find_withtag("RowSelectFill") + self.find_withtag("ColSelectFill") + self.find_withtag("Current_Inside") + self.find_withtag("Current_Outside"))
 
     def get_boxes(self):
         boxes = {}
@@ -5029,31 +4981,31 @@
 
     def open_cell(self, event = None, ignore_existing_editor = False):
         if not self.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.currently_selected()
         if not currently_selected:
             return
-        y1 = int(currently_selected[0])
-        x1 = int(currently_selected[1])
-        dcol = x1 if self.all_columns_displayed else self.displayed_columns[x1]
+        r, c = int(currently_selected[0]), int(currently_selected[1])
+        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if (
-            ((y1, dcol) in self.cell_options and 'readonly' in self.cell_options[(y1, dcol)]) or
-            (dcol in self.col_options and 'readonly' in self.col_options[dcol]) or
-            (y1 in self.row_options and 'readonly' in self.row_options[y1])
+            ((datarn, datacn) in self.cell_options and 'readonly' in self.cell_options[(datarn, datacn)]) or
+            (datacn in self.col_options and 'readonly' in self.col_options[datacn]) or
+            (datarn in self.row_options and 'readonly' in self.row_options[datarn])
             ):
             return
-        elif (y1, dcol) in self.cell_options and ('dropdown' in self.cell_options[(y1, dcol)] or 'checkbox' in self.cell_options[(y1, dcol)]):
+        elif (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 'checkbox' in self.cell_options[(datarn, datacn)]):
             if self.event_opens_dropdown_or_checkbox(event):
-                if 'dropdown' in self.cell_options[(y1, dcol)]:
-                    self.display_dropdown_window(y1, x1, event = event)
-                elif 'checkbox' in self.cell_options[(y1, dcol)]:
-                    self._click_checkbox(y1, x1, dcol)
+                if 'dropdown' in self.cell_options[(datarn, datacn)]:
+                    self.open_dropdown_window(r, c, event = event)
+                elif 'checkbox' in self.cell_options[(datarn, datacn)]:
+                    self._click_checkbox(r = r, c = c, datarn = datarn, datacn = datacn)
         else:
-            self.edit_cell_(event, r = y1, c = x1, dropdown = False)
+            self.edit_cell_(event, r = r, c = c, dropdown = False)
             
     def event_opens_dropdown_or_checkbox(self, event = None):
         if event is None:
             return False
         elif event == "rc":
             return True
         elif ((hasattr(event, 'keysym') and event.keysym == 'Return') or  # enter or f2
@@ -5070,18 +5022,21 @@
         extra_func_key = "??"
         if event is None or self.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, 'keysym') and event.keysym == 'Return':
                     extra_func_key = "Return"
                 elif hasattr(event, 'keysym') and event.keysym == 'F2':
                     extra_func_key = "F2"
-            text = f"{self.data[r][c]}" if self.all_columns_displayed else f"{self.data[r][self.displayed_columns[c]]}"
-        elif event is not None and (hasattr(event, 'keysym') and event.keysym == 'BackSpace'):
-            extra_func_key = "BackSpace"
-            text = ""
+            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+            if event is not None and (hasattr(event, 'keysym') and event.keysym == 'BackSpace'):
+                extra_func_key = "BackSpace"
+                text = ""
+            else:
+                text = f"{self.get_cell_data(datarn, datacn, none_to_empty_str = True)}"
         elif event is not None and ((hasattr(event, "char") and event.char.isalpha()) or
                                     (hasattr(event, "char") and event.char.isdigit()) or
                                     (hasattr(event, "char") and event.char in symbols_set)):
             extra_func_key = event.char
             text = event.char
         else:
             return False
@@ -5096,39 +5051,39 @@
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = True, run_binding = True)
         if not self.currently_selected():
             self.select_cell(r = r, c = c, keep_other_selections = True)
-        self.create_text_editor(r = r, c = c, text = text, set_data_ref_on_destroy = True, dropdown = dropdown)
+        self.create_text_editor(r = r, c = c, text = text, set_data_on_close = True, dropdown = dropdown)
         return True
     
     # displayed indexes
     def get_cell_align(self, r, c):
-        drow = r if self.all_rows_displayed else self.displayed_rows[r]
-        dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-        if (drow, dcol) in self.cell_options and 'align' in self.cell_options[(drow, dcol)]:
-            cell_alignment = self.cell_options[(drow, dcol)]['align']
-        elif drow in self.row_options and 'align' in self.row_options[drow]:
-            cell_alignment = self.row_options[drow]['align']
-        elif dcol in self.col_options and 'align' in self.col_options[dcol]:
-            cell_alignment = self.col_options[dcol]['align']
+        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        if (datarn, datacn) in self.cell_options and 'align' in self.cell_options[(datarn, datacn)]:
+            cell_alignment = self.cell_options[(datarn, datacn)]['align']
+        elif datarn in self.row_options and 'align' in self.row_options[datarn]:
+            cell_alignment = self.row_options[datarn]['align']
+        elif datacn in self.col_options and 'align' in self.col_options[datacn]:
+            cell_alignment = self.col_options[datacn]['align']
         else:
             cell_alignment = self.align
         return cell_alignment
 
     # displayed indexes
     def create_text_editor(self,
                            r = 0,
                            c = 0,
                            text = None,
                            state = "normal",
                            see = True,
-                           set_data_ref_on_destroy = False,
+                           set_data_on_close = False,
                            binding = None,
                            dropdown = False):
         if (r, c) == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
@@ -5137,19 +5092,19 @@
             if not has_redrawn:
                 self.refresh()
         self.text_editor_loc = (r, c)
         x = self.col_positions[c]
         y = self.row_positions[r]
         w = self.col_positions[c + 1] - x + 1
         h = self.row_positions[r + 1] - y + 1
-        dcol = c if self.all_columns_displayed else self.displayed_columns[c]
         if text is None:
-            text = self.data[r][dcol]
+            text = f"""{self.get_cell_data(r if self.all_rows_displayed else self.displayed_rows[r],
+                                           c if self.all_columns_displayed else self.displayed_columns[c],
+                                           none_to_empty_str=True)}"""
         self.hide_current()
-        #bg, fg = self.get_widget_bg_fg(r, dcol)
         bg, fg = self.table_bg, self.table_fg
         self.text_editor = TextEditor(self, 
                                       text = text, 
                                       font = self._font, 
                                       state = state, 
                                       width = w, 
                                       height = h, 
@@ -5178,48 +5133,48 @@
         for key, func in self.text_editor_user_bound_keys.items():
             self.text_editor.textedit.bind(key, func)
         if binding is not None:
             self.text_editor.textedit.bind("<Tab>", lambda x: binding((r, c, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: binding((r, c, "Return")))
             self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, c, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, c, "Escape")))
-        elif binding is None and set_data_ref_on_destroy:
+        elif binding is None and set_data_on_close:
             self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, c, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, c, "Return")))
             if not dropdown:
                 self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, c, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, c, "Escape")))
         else:
             self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
     
     # displayed indexes
     def text_editor_newline_binding(self, r = 0, c = 0, event = None, check_lines = True):
-        drow = r if self.all_rows_displayed else self.displayed_rows[r]
-        dcol = c if self.all_columns_displayed else self.displayed_columns[c]
+        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         curr_height = self.text_editor.winfo_height()
         if not check_lines or self.GetLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
             new_height = curr_height + self.xtra_lines_increment
             space_bot = self.get_space_bot(r)
             if new_height > space_bot:
                 new_height = space_bot
             if new_height != curr_height:
                 self.text_editor.config(height = new_height)
-                if ((r, dcol) in self.cell_options and
-                    'dropdown' in self.cell_options[(r, dcol)]):
+                if ((r, datacn) in self.cell_options and
+                    'dropdown' in self.cell_options[(r, datacn)]):
                     text_editor_h = self.text_editor.winfo_height()
-                    win_h, anchor = self.get_dropdown_height_anchor(drow, dcol, text_editor_h)
+                    win_h, anchor = self.get_dropdown_height_anchor(datarn, datacn, text_editor_h)
                     if anchor == "nw":
-                        self.coords(self.cell_options[(r, dcol)]['dropdown']['canvas_id'],
+                        self.coords(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
                                     self.col_positions[c], self.row_positions[r] + text_editor_h - 1)
-                        self.itemconfig(self.cell_options[(r, dcol)]['dropdown']['canvas_id'],
+                        self.itemconfig(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
                                         anchor = anchor, height = win_h)
                     elif anchor == "sw":
-                        self.coords(self.cell_options[(r, dcol)]['dropdown']['canvas_id'],
+                        self.coords(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
                                     self.col_positions[c], self.row_positions[r])
-                        self.itemconfig(self.cell_options[(r, dcol)]['dropdown']['canvas_id'],
+                        self.itemconfig(self.cell_options[(r, datacn)]['dropdown']['canvas_id'],
                                         anchor = anchor, height = win_h)
 
     def destroy_text_editor(self, event = None):
         if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
             self.extra_end_edit_cell_func(EditCellEvent(int(self.text_editor_loc[0]), int(self.text_editor_loc[1]), "Escape", None, "escape_edit_cell"))
         self.text_editor_loc = None
         try:
@@ -5239,38 +5194,40 @@
         except:
             pass
         self.show_current()
         if event is not None and len(event) >= 3 and "Escape" in event:
             self.focus_set()
 
     # c is displayed col
-    def close_text_editor(self, editor_info = None, r = None, c = None, set_data_ref_on_destroy = True, event = None, destroy = True, move_down = True, redraw = True, recreate = True):
+    def close_text_editor(self, editor_info = None, r = None, c = None, set_data_on_close = True, event = None, destroy = True, move_down = True, redraw = True, recreate = True):
         if self.focus_get() is None and editor_info:
             return "break"
         if editor_info is not None and len(editor_info) >= 3 and editor_info[2] == "Escape":
             self.destroy_text_editor("Escape")
-            self.hide_dropdown_window(r, c)
+            self.close_dropdown_window(r, c)
             return "break"
         if self.text_editor is not None:
             self.text_editor_value = self.text_editor.get()
         if destroy:
             self.destroy_text_editor()
-        if set_data_ref_on_destroy:
+        if set_data_on_close:
             if r is None and c is None and editor_info:
                 r, c = editor_info[0], editor_info[1]
-            if self.extra_end_edit_cell_func is None:
-                self._set_cell_data(r, c, value = self.text_editor_value, redraw = False)
-            elif self.extra_end_edit_cell_func is not None and not self.edit_cell_validation:
-                self._set_cell_data(r, c, value = self.text_editor_value, redraw = False)
+            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(datarn, datacn, self.text_editor_value):
+                self.set_cell_data_undo(r, c, datarn = datarn, datacn = datacn, value = self.text_editor_value, redraw = False, check_input_valid = False)
+            elif self.extra_end_edit_cell_func is not None and not self.edit_cell_validation and self.input_valid_for_cell(datarn, datacn, self.text_editor_value):
+                self.set_cell_data_undo(r, c, datarn = datarn, datacn = datacn, value = self.text_editor_value, redraw = False, check_input_valid = False)
                 self.extra_end_edit_cell_func(EditCellEvent(r, c, editor_info[2] if len(editor_info) >= 3 else "FocusOut", f"{self.text_editor_value}", "end_edit_cell"))
             elif self.extra_end_edit_cell_func is not None and self.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(EditCellEvent(r, c, editor_info[2] if len(editor_info) >= 3 else "FocusOut", f"{self.text_editor_value}", "end_edit_cell"))
-                if validation is not None:
-                    self.text_editor_value = validation
-                    self._set_cell_data(r, c, value = self.text_editor_value, redraw = False)
+                self.text_editor_value = validation
+                if validation is not None and self.input_valid_for_cell(datarn, datacn, self.text_editor_value):
+                    self.set_cell_data_undo(r, c, datarn = datarn, datacn = datacn, value = self.text_editor_value, redraw = False, check_input_valid = False)
         if move_down:
             if r is None and c is None and editor_info:
                 r, c = editor_info[0], editor_info[1]
             currently_selected = self.currently_selected()
             if (r is not None and
                 c is not None and
                 currently_selected and
@@ -5312,15 +5269,15 @@
                         if not moved:
                             if r + 1 == r2:
                                 new_r = r1
                             elif numrows > 1:
                                 new_r = r + 1
                     self.create_current(new_r, new_c, type_ = currently_selected.type_, inside = True)
                     self.see(new_r, new_c, keep_xscroll = False, bottom_right_corner = True, check_cell_visibility = True)
-        self.hide_dropdown_window(r, c)
+        self.close_dropdown_window(r, c)
         if recreate:
             self.recreate_all_selection_boxes()
         if redraw:
             self.refresh()
         if editor_info is not None and len(editor_info) >= 3 and editor_info[2] != "FocusOut":
             self.focus_set()
         return "break"
@@ -5352,98 +5309,345 @@
                 elif numrows > 1:
                     new_r = r + 1
         self.create_current(new_r, new_c, type_ = currently_selected.type_, inside = True)
         self.see(new_r, new_c, keep_xscroll = False, bottom_right_corner = True, check_cell_visibility = True)
         return "break"
 
     #internal event use
-    def _set_cell_data(self, r = 0, c = 0, drow = None, dcol = None, value = "", undo = True, cell_resize = True, redraw = True):
-        if dcol is None:
-            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-        if drow is None:
-            drow = r if self.all_rows_displayed else self.displayed_rows[r]
-        if r > len(self.data) - 1:
-            self.data.extend([list(repeat("", dcol + 1)) for i in range((r + 1) - len(self.data))])
-        elif dcol > len(self.data[r]) - 1:
-            self.data[r].extend(list(repeat("", (dcol + 1) - len(self.data[r]))))
-        if self.undo_enabled and undo:
-            if self.data[r][dcol] != value:
+    def set_cell_data_undo(self, r = 0, c = 0, datarn = None, datacn = None, value = "", undo = True, cell_resize = True, redraw = True, check_input_valid = True):
+        if datacn is None:
+            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        if datarn is None:
+            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        if not check_input_valid or self.input_valid_for_cell(datarn, datacn, value):
+            if self.undo_enabled and undo:
                 self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells",
-                                                                     {(r, dcol): self.data[r][dcol]},
-                                                                     (((r, c, r + 1, c + 1), "cells"), ),
-                                                                     self.currently_selected()))))
-        self.data[r][dcol] = value
+                                                                    {(datarn, datacn): self.get_cell_data(datarn, datacn)},
+                                                                    (((r, c, r + 1, c + 1), "cells"), ),
+                                                                    self.currently_selected()))))
+            self.set_cell_data(datarn, datacn, value)
         if cell_resize and self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = redraw, run_binding = True)
         return True
+    
+    def set_cell_data(self, datarn, datacn, value, kwargs = {}, expand_sheet = True):
+        if expand_sheet:
+            if datarn >= len(self.data):
+                self.data.extend([list(repeat("", datacn + 1)) for i in range((datarn + 1) - len(self.data))])
+            elif datacn >= len(self.data[datarn]):
+                self.data[datarn].extend(list(repeat("", (datacn + 1) - len(self.data[datarn]))))
+        if expand_sheet or (len(self.data) > datarn and len(self.data[datarn]) > datacn):
+            if not kwargs:
+                kwargs = self.get_format_kwargs(datarn, datacn)
+            if kwargs:
+                if kwargs['formatter'] is None:
+                    self.data[datarn][datacn] = format_data(value = value, **kwargs)
+                else:
+                    self.data[datarn][datacn] = kwargs['formatter'](value, **kwargs)
+            elif (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+                self.data[datarn][datacn] = to_bool(value)
+            else:
+                self.data[datarn][datacn] = value
 
     #internal event use
-    def _click_checkbox(self, r, c, dcol = None, undo = True, redraw = True):
-        if dcol is None:
-            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-        if self.cell_options[(r, dcol)]['checkbox']['state'] == "normal":
-            self._set_cell_data(r, c, dcol = dcol, value = not self.data[r][dcol] if type(self.data[r][dcol]) == bool else False, undo = undo, cell_resize = False)
-            if self.cell_options[(r, dcol)]['checkbox']['check_function'] is not None:
-                self.cell_options[(r, dcol)]['checkbox']['check_function']((r, c, "CheckboxClicked", f"{self.data[r][dcol]}"))
+    def _click_checkbox(self, r, c, datarn = None, datacn = None, undo = True, redraw = True):
+        if datarn is None:
+            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        if datacn is None:
+            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        if self.cell_options[(datarn, datacn)]['checkbox']['state'] == "normal":
+            self.set_cell_data_undo(r, c, 
+                                    value = not self.data[datarn][datacn] if type(self.data[datarn][datacn]) == bool else False, 
+                                    undo = undo, cell_resize = False, check_input_valid = False)
+            if self.cell_options[(datarn, datacn)]['checkbox']['check_function'] is not None:
+                self.cell_options[(datarn, datacn)]['checkbox']['check_function']((r, c, "CheckboxClicked", self.data[datarn][datacn]))
             if self.extra_end_edit_cell_func is not None:
-                self.extra_end_edit_cell_func(EditCellEvent(r, c, "Return", f"{self.data[r][dcol]}", "end_edit_cell"))
+                self.extra_end_edit_cell_func(EditCellEvent(r, c, "Return", self.data[datarn][datacn], "end_edit_cell"))
         if redraw:
             self.refresh()
 
-    def create_checkbox(self, r = 0, c = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
-        if (r, c) in self.cell_options and any(x in self.cell_options[(r, c)] for x in ('dropdown', 'checkbox')):
-            self.delete_dropdown_and_checkbox(r, c)
-        self._set_cell_data(r, dcol = c, value = checked, cell_resize = False, undo = False) #only works because cell_resize is false and undo is false, otherwise needs c arg
-        if (r, c) not in self.cell_options:
-            self.cell_options[(r, c)] = {}
-        self.cell_options[(r, c)]['checkbox'] = {'check_function': check_function,
-                                                 'state': state,
-                                                 'text': text}
+    def create_checkbox(self, datarn = 0, datacn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
+        self.delete_cell_format(datarn, datacn, clear_values = True)
+        if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
+                                                      'checkbox' in self.cell_options[(datarn, datacn)]):
+            self.delete_dropdown_and_checkbox(datarn, datacn)
+        self.set_cell_data(datarn, datacn, checked)
+        if (datarn, datacn) not in self.cell_options:
+            self.cell_options[(datarn, datacn)] = {}
+        self.cell_options[(datarn, datacn)]['checkbox'] = {'check_function': check_function,
+                                                           'state': state,
+                                                           'text': text}
         if redraw:
             self.refresh()
 
-    def create_dropdown(self, r = 0, c = 0, values = [], set_value = None, state = "readonly", redraw = True, selection_function = None, modified_function = None):
-        if (r, c) in self.cell_options and any(x in self.cell_options[(r, c)] for x in ('dropdown', 'checkbox')):
-            self.delete_dropdown_and_checkbox(r, c)
-        self._set_cell_data(r,
-                            dcol = c,
-                            value = set_value if set_value is not None else values[0] if values else "",
-                            cell_resize = False,
-                            undo = False) #only works because cell_resize is false and undo is false, otherwise needs c arg
-        if (r, c) not in self.cell_options:
-            self.cell_options[(r, c)] = {}
-        self.cell_options[(r, c)]['dropdown'] = {'values': values,
-                                                 'align': "w",
-                                                 'window': "no dropdown open",
-                                                 'canvas_id': "no dropdown open",
-                                                 'select_function': selection_function,
-                                                 'modified_function': modified_function,
-                                                 'state': state}
+    def create_dropdown(self, 
+                        datarn = 0, datacn = 0, 
+                        values = [], set_value = None,
+                        state = "normal", redraw = True, 
+                        selection_function = None, modified_function = None,
+                        search_function = dropdown_search_function, validate_input = True, text = None):
+        if (datarn, datacn) in self.cell_options and ('dropdown' in self.cell_options[(datarn, datacn)] or 
+                                                      'checkbox' in self.cell_options[(datarn, datacn)]):
+            self.delete_dropdown_and_checkbox(datarn, datacn)
+        self.set_cell_data(datarn, datacn, set_value if set_value is not None else values[0] if values else "")
+        if (datarn, datacn) not in self.cell_options:
+            self.cell_options[(datarn, datacn)] = {}
+        self.cell_options[(datarn, datacn)]['dropdown'] = {'values': values,
+                                                           'window': "no dropdown open",
+                                                           'canvas_id': "no dropdown open",
+                                                           'select_function': selection_function,
+                                                           'modified_function': modified_function,
+                                                           'search_function': search_function,
+                                                           'validate_input': validate_input,
+                                                           'text': text,
+                                                           'state': state}
         if redraw:
             self.refresh()
 
-    def get_widget_bg_fg(self, r, c):
-        bg = self.table_bg
-        fg = self.table_fg
-        if (r, c) in self.cell_options and 'highlight' in self.cell_options[(r, c)]:
-            if self.cell_options[(r, c)]['highlight'][0] is not None:
-                bg = self.cell_options[(r, c)]['highlight'][0]
-            if self.cell_options[(r, c)]['highlight'][1] is not None:
-                fg = self.cell_options[(r, c)]['highlight'][1]
-        elif r in self.row_options and 'highlight' in self.row_options[r]:
-            if self.row_options[r]['highlight'][0] is not None:
-                bg = self.row_options[r]['highlight'][0]
-            if self.row_options[r]['highlight'][1] is not None:
-                fg = self.row_options[r]['highlight'][1]
-        elif c in self.col_options and 'highlight' in self.col_options[c]:
-            if self.col_options[c]['highlight'][0] is not None:
-                bg = self.col_options[c]['highlight'][0]
-            if self.col_options[c]['highlight'][1] is not None:
-                fg = self.col_options[c]['highlight'][1]
-        return bg, fg
+    def format_cell(self,
+                    datarn, 
+                    datacn,
+                    **kwargs):
+        if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+            return
+        if 'value' in kwargs:
+            v = kwargs['value']
+        else:
+            v = self.get_cell_data(datarn, datacn)
+        kwargs = self.format_fix_kwargs(kwargs)
+        if (datarn, datacn) not in self.cell_options:
+            self.cell_options[(datarn, datacn)] = {}
+        self.cell_options[(datarn, datacn)]['format'] = kwargs
+        self.set_cell_data(datarn, datacn, value = v, kwargs = kwargs)
+        
+    def format_row(self, datarn, **kwargs):
+        kwargs = self.format_fix_kwargs(kwargs)
+        if datarn not in self.row_options:
+            self.row_options[datarn] = {}
+        self.row_options[datarn]['format'] = kwargs
+        for datacn in range(self.total_data_cols()):
+            self.set_cell_data(datarn, 
+                               datacn,
+                               value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
+                               kwargs = kwargs)
+            
+    def format_column(self, datacn, **kwargs):
+        kwargs = self.format_fix_kwargs(kwargs)
+        if datacn not in self.col_options:
+            self.col_options[datacn] = {}
+        self.col_options[datacn]['format'] = kwargs
+        for datarn in range(self.total_data_rows()):
+            self.set_cell_data(datarn, 
+                               datacn,
+                               value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
+                               kwargs = kwargs)
+            
+    def format_sheet(self, **kwargs):
+        kwargs = self.format_fix_kwargs(kwargs)
+        self.sheet_options['format'] = kwargs
+        for datarn in range(self.total_data_rows()):
+            for datacn in range(self.total_data_cols()):
+                self.set_cell_data(datarn, 
+                                   datacn,
+                                   value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
+                                   kwargs = kwargs)
+
+    def format_fix_kwargs(self, kwargs):
+        if kwargs['formatter'] is None:
+            if kwargs['nullable']:
+                if isinstance(kwargs['datatypes'], (list, tuple)):
+                    kwargs['datatypes'] = tuple(kwargs['datatypes']) + (type(None), )
+                else:
+                    kwargs['datatypes'] = (kwargs['datatypes'], type(None))
+            elif (isinstance(kwargs['datatypes'], (list, tuple)) and type(None) in kwargs['datatypes']) or kwargs['datatypes'] is type(None):
+                raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
+        if not isinstance(kwargs['invalid_value'], str):
+            kwargs['invalid_value'] = f"{kwargs['invalid_value']}"
+        return kwargs
+    
+    def reapply_formatting(self):
+        if 'format' in self.sheet_options:
+            for r in range(len(self.data)):
+                if r not in self.row_options:
+                    for c in range(len(self.data[r])):
+                        if not ((r, c) in self.cell_options and 'format' in self.cell_options[(r, c)] or
+                                c in self.col_options and 'format' in self.col_options[c]):
+                            self.set_cell_data(r, c, value = self.data[r][c])
+        for c in self.yield_formatted_columns():
+            for r in range(len(self.data)):
+                if not ((r, c) in self.cell_options and 'format' in self.cell_options[(r, c)] or
+                        r in self.row_options and 'format' in self.row_options[r]):
+                    self.set_cell_data(r, c, value = self.data[r][c])
+        for r in self.yield_formatted_rows():
+            for c in range(len(self.data[r])):
+                if not ((r, c) in self.cell_options and 'format' in self.cell_options[(r, c)]):
+                    self.set_cell_data(r, c, value = self.data[r][c])
+        for r, c in self.yield_formatted_cells():
+            if len(self.data) > r and len(self.data[r]) > c:
+                self.set_cell_data(r, c, value = self.data[r][c])
+    
+    def delete_all_formatting(self, clear_values = False):
+        self.delete_cell_format("all", clear_values = clear_values)
+        self.delete_row_format("all", clear_values = clear_values)
+        self.delete_column_format("all", clear_values = clear_values)
+        self.delete_sheet_format(clear_values = clear_values)
+
+    def delete_cell_format(self, datarn = "all", datacn = 0, clear_values = False):
+        if isinstance(datarn, str) and datarn.lower() == "all":
+            for datarn, datacn in self.yield_formatted_cells():
+                del self.cell_options[(datarn, datacn)]['format']
+                if clear_values:
+                    self.set_cell_data(datarn, datacn, "", expand_sheet = False)
+        else:
+            if (datarn, datacn) in self.cell_options and 'format' in self.cell_options[(datarn, datacn)]:
+                del self.cell_options[(datarn, datacn)]['format']
+                if clear_values:
+                    self.set_cell_data(datarn, datacn, "", expand_sheet = False)
+
+    def delete_row_format(self, datarn = "all", clear_values = False):
+        if isinstance(datarn, str) and datarn.lower() == "all":
+            for datarn in self.yield_formatted_rows():
+                del self.row_options[datarn]['format']
+                if clear_values:
+                    for datacn in range(len(self.data[datarn])):
+                        self.set_cell_data(datarn, datacn, "", expand_sheet = False)
+        else:
+            if datarn in self.row_options and 'format' in self.row_options[datarn]:
+                del self.row_options[datarn]['format']
+                if clear_values:
+                    for datacn in range(len(self.data[datarn])):
+                        self.set_cell_data(datarn, datacn, "", expand_sheet = False)
+            
+    def delete_column_format(self, datacn = "all", clear_values = False):
+        if isinstance(datacn, str) and datacn.lower() == "all":
+            for datacn in self.yield_formatted_columns():
+                del self.col_options[datacn]['format']
+                if clear_values:
+                    for datarn in range(len(self.data)):
+                        self.set_cell_data(datarn, datacn, "", expand_sheet = False)
+        else:
+            if datacn in self.col_options and 'format' in self.col_options[datacn]:
+                del self.col_options[datacn]['format']
+                if clear_values:
+                    for datarn in range(len(self.data)):
+                        self.set_cell_data(datarn, datacn, "", expand_sheet = False)
+    
+    def delete_sheet_format(self, clear_values = False):
+        if 'format' in self.sheet_options:
+            del self.sheet_options['format']
+            if clear_values:
+                total_cols = self.total_data_cols()
+                self.data = [list(repeat("", total_cols)) for i in range(len(self.data))]
+
+    # deals with possibility of formatter class being in self.data cell
+    # if cell is formatted - possibly returns invalid_value kwarg if cell value is not in datatypes kwarg
+    # if get displayed is true then Nones are replaced by ""
+    def get_valid_cell_data_as_str(self, datarn, datacn, get_displayed = False, **kwargs) -> str:
+        value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
+        kwargs = self.get_format_kwargs(datarn, datacn)
+        if kwargs:
+            if kwargs['formatter'] is None:
+                if get_displayed:
+                    return data_to_str(value, **kwargs)
+                else:
+                    return f"{get_data_with_valid_check(value, **kwargs)}"
+            else:
+                if get_displayed:
+                    return f"{value}" # assumed given formatter class has __str__() function
+                else:
+                    return f"{value.get_data_with_valid_check()}" # assumed given formatter class has get_data_with_valid_check() function
+        return f"{value}"
+
+    def get_cell_data(self, datarn, datacn, get_displayed = False, none_to_empty_str = False, **kwargs) -> Any:
+        value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
+        kwargs = self.get_format_kwargs(datarn, datacn)
+        if kwargs:
+            if kwargs['formatter'] is None:
+                if get_displayed:
+                    return data_to_str(value, **kwargs)
+            else:
+                if get_displayed:
+                    return f"{value}" # assumed given formatter class has __str__() function
+                else:
+                    value = value.value # assumed given formatter class has value attribute
+        return "" if (value is None and none_to_empty_str) else value
+    
+    def input_valid_for_cell(self, datarn, datacn, value):
+        if (datarn, datacn) in self.cell_options and 'readonly' in self.cell_options[(datarn, datacn)]:
+            return False
+        if datarn in self.row_options and 'readonly' in self.row_options[datarn]:
+            return False
+        if datacn in self.col_options and 'readonly' in self.col_options[datacn]:
+            return False
+        if self.cell_equal_to(datarn, datacn, value):
+            return False
+        if self.get_format_kwargs(datarn, datacn):
+            return True
+        if (datarn, datacn) in self.cell_options: 
+            if 'checkbox' in self.cell_options[(datarn, datacn)]:
+                return is_bool_like(value)
+            if ('dropdown' in self.cell_options[(datarn, datacn)] and 
+                self.cell_options[(datarn, datacn)]['dropdown']['validate_input'] and 
+                value not in self.cell_options[(datarn, datacn)]['dropdown']['values']):
+                return False
+        return True
+
+    def cell_equal_to(self, datarn, datacn, value, **kwargs):
+        v = self.get_cell_data(datarn, datacn)
+        kwargs = self.get_format_kwargs(datarn, datacn)
+        if kwargs and kwargs['formatter'] is None:
+            return v == format_data(value = value, **kwargs)
+        # assumed if there is a formatter class in cell then it has a __eq__() function anyway
+        # else if there is not a formatter class in cell and cell is not formatted
+        # then compare value as is
+        if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+            try:
+                return to_bool(v) == to_bool(value)
+            except:
+                return False
+        return v == value
+
+    def get_cell_clipboard(self, datarn, datacn) -> Union[str, int, float, bool]:
+        value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
+        kwargs = self.get_format_kwargs(datarn, datacn)
+        if kwargs:
+            if kwargs['formatter'] is None:
+                return get_clipboard_data(value, **kwargs)
+            else:
+                return value.get_clipboard_data() # assumed given formatter class has get_clipboard_data() function and it returns one of above type hints
+        return f"{value}"
+
+    def yield_formatted_cells(self, formatter = None):
+        if formatter is None:
+            yield from (cell for cell, options in self.cell_options.items() if 'format' in options and options['format']['formatter'] == formatter)
+        else:
+            yield from (cell for cell, options in self.cell_options.items() if 'format' in options)
+
+    def yield_formatted_rows(self, formatter = None):
+        if formatter is None:
+            yield from (r for r, options in self.row_options.items() if 'format' in options)
+        else:
+            yield from (r for r, options in self.row_options.items() if 'format' in options and options['format']['formatter'] == formatter)
+
+    def yield_formatted_columns(self, formatter = None):
+        if formatter is None:
+            yield from (c for c, options in self.col_options.items() if 'format' in options)
+        else:
+            yield from (c for c, options in self.col_options.items() if 'format' in options and options['format']['formatter'] == formatter)
+
+    def get_format_kwargs(self, datarn, datacn):
+        if (datarn, datacn) in self.cell_options and 'format' in self.cell_options[(datarn, datacn)]:
+            return self.cell_options[(datarn, datacn)]['format']
+        elif datarn in self.row_options and 'format' in self.row_options[datarn]:
+            return self.row_options[datarn]['format']
+        elif datacn in self.col_options and 'format' in self.col_options[datacn]:
+            return self.col_options[datacn]['format']
+        elif 'format' in self.sheet_options:
+            return self.sheet_options['format']
+        return {}
 
     def get_space_bot(self, r, text_editor_h = None):
         if len(self.row_positions) <= 1:
             if text_editor_h is None:
                 win_h = int(self.winfo_height())
                 sheet_h = int(1 + self.empty_vertical)
             else:
@@ -5458,28 +5662,28 @@
                 sheet_h = int(self.row_positions[-1] + 1 + self.empty_vertical - (self.row_positions[r] + text_editor_h))
         if win_h > 0:
             win_h -= 1
         if sheet_h > 0:
             sheet_h -= 1
         return win_h if win_h >= sheet_h else sheet_h
 
-    def get_dropdown_height_anchor(self, drow, dcol, text_editor_h = None):
+    def get_dropdown_height_anchor(self, datarn, datacn, text_editor_h = None):
         win_h = 5
-        for i, v in enumerate(self.cell_options[(drow, dcol)]['dropdown']['values']):
+        for i, v in enumerate(self.cell_options[(datarn, datacn)]['dropdown']['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
                 win_h += self.fl_ins + (v_numlines * self.xtra_lines_increment) + 5 # end of cell
             else:
                 win_h += self.min_rh
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
-        space_bot = self.get_space_bot(drow, text_editor_h)
-        space_top = int(self.row_positions[drow])
+        space_bot = self.get_space_bot(datarn, text_editor_h)
+        space_top = int(self.row_positions[datarn])
         anchor = "nw"
         win_h2 = int(win_h)
         if win_h > space_bot:
             if space_bot >= space_top:
                 anchor = "nw"
                 win_h = space_bot - 1
             elif space_top > space_bot:
@@ -5488,167 +5692,169 @@
         if win_h < self.txt_h + 5:
             win_h = self.txt_h + 5
         elif win_h > win_h2:
             win_h = win_h2
         return win_h, anchor
 
     # c is displayed col
-    def display_dropdown_window(self, r, c, event = None):
+    def open_dropdown_window(self, r, c, event = None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
-        drow = r if self.all_rows_displayed else self.displayed_rows[r]
-        dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-        if self.cell_options[(r, dcol)]['dropdown']['state'] == "normal":
+        datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+        if self.cell_options[(r, datacn)]['dropdown']['state'] == "normal":
             if not self.edit_cell_(r = r, c = c, dropdown = True, event = event):
                 return
-        win_h, anchor = self.get_dropdown_height_anchor(drow, dcol)
+        win_h, anchor = self.get_dropdown_height_anchor(datarn, datacn)
         window = self.parentframe.dropdown_class(self.winfo_toplevel(),
                                                  r,
                                                  c,
                                                  width = self.col_positions[c + 1] - self.col_positions[c] + 1,
                                                  height = win_h,
                                                  font = self._font,
                                                  colors = {'bg': self.popup_menu_bg, 
                                                            'fg': self.popup_menu_fg, 
                                                            'highlight_bg': self.popup_menu_highlight_bg,
                                                            'highlight_fg': self.popup_menu_highlight_fg},
                                                  outline_color = self.table_selected_cells_border_fg,
                                                  outline_thickness = 2,
-                                                 values = self.cell_options[(r, dcol)]['dropdown']['values'],
-                                                 hide_dropdown_window = self.hide_dropdown_window,
+                                                 values = self.cell_options[(datarn, datacn)]['dropdown']['values'],
+                                                 close_dropdown_window = self.close_dropdown_window,
+                                                 search_function = self.cell_options[(datarn, datacn)]['dropdown']['search_function'],
                                                  arrowkey_RIGHT = self.arrowkey_RIGHT,
                                                  arrowkey_LEFT = self.arrowkey_LEFT,
-                                                 align = self.cell_options[(r, dcol)]['dropdown']['align'])
-        if self.cell_options[(r, dcol)]['dropdown']['state'] == "normal":
+                                                 align = "w")#self.get_cell_align(r, c)
+        if self.cell_options[(datarn, datacn)]['dropdown']['state'] == "normal":
             if anchor == "nw":
                 ypos = self.row_positions[r] + self.text_editor.h_ - 1
             else:
                 ypos = self.row_positions[r]
-            self.cell_options[(r, dcol)]['dropdown']['canvas_id'] = self.create_window((self.col_positions[c], ypos),
-                                                                                        window = window,
-                                                                                        anchor = anchor)
-            if self.cell_options[(r, dcol)]['dropdown']['modified_function'] is not None:
-                self.text_editor.textedit.bind("<<TextModified>>", lambda x: self.cell_options[(r, dcol)]['dropdown']['modified_function'](DropDownModifiedEvent("ComboboxModified", r, dcol, self.text_editor.get())))
+            self.cell_options[(datarn, datacn)]['dropdown']['canvas_id'] = self.create_window((self.col_positions[c], ypos),
+                                                                                              window = window,
+                                                                                              anchor = anchor)
+            self.text_editor.textedit.bind("<<TextModified>>", 
+                                           lambda x: window.search_and_see(DropDownModifiedEvent("ComboboxModified", r, c, self.text_editor.get())))
+            if self.cell_options[(datarn, datacn)]['dropdown']['modified_function'] is not None:
+                window.modified_function = self.cell_options[(datarn, datacn)]['dropdown']['modified_function']
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
                 self.after(2, self.text_editor.scroll_to_bottom())
             except:
                 return
             redraw = False
         else:
-            
             if anchor == "nw":
                 ypos = self.row_positions[r + 1]
             else:
                 ypos = self.row_positions[r]
-            self.cell_options[(r, dcol)]['dropdown']['canvas_id'] = self.create_window((self.col_positions[c], ypos),
-                                                                                        window = window,
-                                                                                        anchor = anchor)
+            self.cell_options[(datarn, datacn)]['dropdown']['canvas_id'] = self.create_window((self.col_positions[c], ypos),
+                                                                                              window = window,
+                                                                                              anchor = anchor)
             self.update_idletasks()
-            window.bind("<FocusOut>", lambda x: self.hide_dropdown_window(r, c))
+            window.bind("<FocusOut>", lambda x: self.close_dropdown_window(r, c))
             window.focus()
             redraw = True
         self.existing_dropdown_window = window
-        self.cell_options[(r, dcol)]['dropdown']['window'] = window
-        self.existing_dropdown_canvas_id = self.cell_options[(r, dcol)]['dropdown']['canvas_id']
+        self.cell_options[(datarn, datacn)]['dropdown']['window'] = window
+        self.existing_dropdown_canvas_id = self.cell_options[(datarn, datacn)]['dropdown']['canvas_id']
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = False)
 
     # displayed indexes, not data
-    def hide_dropdown_window(self, r = None, c = None, selection = None, redraw = True):
+    def close_dropdown_window(self, r = None, c = None, selection = None, redraw = True):
         if r is not None and c is not None and selection is not None:
-            dcol = c if self.all_columns_displayed else self.displayed_columns[c]
-            drow = r if self.all_rows_displayed else self.displayed_rows[r]
-            if self.cell_options[(r, dcol)]['dropdown']['select_function'] is not None: # user has specified a selection function
-                self.cell_options[(r, dcol)]['dropdown']['select_function'](EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
+            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
+            datarn = r if self.all_rows_displayed else self.displayed_rows[r]
+            if self.cell_options[(datarn, datacn)]['dropdown']['select_function'] is not None: # user has specified a selection function
+                self.cell_options[(datarn, datacn)]['dropdown']['select_function'](EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
             if self.extra_end_edit_cell_func is None:
-                self._set_cell_data(r, c, dcol = dcol, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(r, c, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and self.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
                 if validation is not None:
                     selection = validation
-                self._set_cell_data(r, c, dcol = dcol, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(r, c, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and not self.edit_cell_validation:
-                self._set_cell_data(r, c, dcol = dcol, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(r, c, value = selection, redraw = not redraw)
                 self.extra_end_edit_cell_func(EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
             self.focus_set()
             self.recreate_all_selection_boxes()
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window(r, c)
         if redraw:
             self.refresh()
+            
+    def get_existing_dropdown_coords(self):
+        if self.existing_dropdown_window is not None:
+            return int(self.existing_dropdown_window.r), int(self.existing_dropdown_window.c)
+        return None
         
     def mouseclick_outside_editor_or_dropdown(self):
-        if self.existing_dropdown_window is not None:
-            closed_dd_coords = (int(self.existing_dropdown_window.r),
-                                int(self.existing_dropdown_window.c))
-        else:
-            closed_dd_coords = None
+        closed_dd_coords = self.get_existing_dropdown_coords()
         if self.text_editor_loc is not None and self.text_editor is not None:
             self.close_text_editor(editor_info = self.text_editor_loc + ("ButtonPress-1", ))
         else:
             self.destroy_text_editor("Escape")
-        if closed_dd_coords:
+        if closed_dd_coords is not None:
             self.destroy_opened_dropdown_window(closed_dd_coords[0], closed_dd_coords[1]) #displayed coords not data, necessary for b1 function
         return closed_dd_coords
+    
+    def mouseclick_outside_editor_or_dropdown_all_canvases(self):
+        self.CH.mouseclick_outside_editor_or_dropdown()
+        self.RI.mouseclick_outside_editor_or_dropdown()
+        return self.mouseclick_outside_editor_or_dropdown()
 
     # function can receive 4 None args
-    def destroy_opened_dropdown_window(self, r = None, c = None, drow = None, dcol = None):
-        if c is not None or dcol is not None:
-            if dcol is None:
-                dcol_ = c if self.all_columns_displayed else self.displayed_columns[c]
-            else:
-                dcol_ = dcol
-        else:
-            dcol_ = None
-        if r is not None or drow is not None:
-            if drow is None:
-                drow_ = r if self.all_rows_displayed else self.displayed_rows[r]
+    def destroy_opened_dropdown_window(self, r = None, c = None, datarn = None, datacn = None):
+        if r is None and datarn is None and c is None and datacn is None and self.existing_dropdown_window is not None:
+            r, c = self.get_existing_dropdown_coords()
+        if c is not None or datacn is not None:
+            if datacn is None:
+                datacn_ = c if self.all_columns_displayed else self.displayed_columns[c]
+            else:
+                datacn_ = datacn
+        else:
+            datacn_ = None
+        if r is not None or datarn is not None:
+            if datarn is None:
+                datarn_ = r if self.all_rows_displayed else self.displayed_rows[r]
             else:
-                drow_ = drow
+                datarn_ = datarn
         else:
-            drow_ = None
+            datarn_ = None
         try:
             self.delete(self.existing_dropdown_canvas_id)
         except:
             pass
         self.existing_dropdown_canvas_id = None
         try:
             self.existing_dropdown_window.destroy()
         except:
             pass
-        self.existing_dropdown_window = None
-        if (drow_, dcol_) in self.cell_options and 'dropdown' in self.cell_options[(drow_, dcol_)]:
-            self.cell_options[(drow_, dcol_)]['dropdown']['canvas_id'] = "no dropdown open"
-            self.cell_options[(drow_, dcol_)]['dropdown']['window'] = "no dropdown open"
+        if (datarn_, datacn_) in self.cell_options and 'dropdown' in self.cell_options[(datarn_, datacn_)]:
+            self.cell_options[(datarn_, datacn_)]['dropdown']['canvas_id'] = "no dropdown open"
+            self.cell_options[(datarn_, datacn_)]['dropdown']['window'] = "no dropdown open"
             try:
-                self.delete(self.cell_options[(drow_, dcol_)]['dropdown']['canvas_id'])
+                self.delete(self.cell_options[(datarn_, datacn_)]['dropdown']['canvas_id'])
             except:
                 pass
+        self.existing_dropdown_window = None
 
-    def get_displayed_col_from_dcol(self, dcol):
+    def get_displayed_col_from_datacn(self, datacn):
         try:
-            return self.displayed_columns.index(dcol)
+            return self.displayed_columns.index(datacn)
         except:
             return None
     
-    # c is dcol
-    def delete_dropdown(self, r, c):
-        self.destroy_opened_dropdown_window(r, dcol = c)
-        if (r, c) in self.cell_options and 'dropdown' in self.cell_options[(r, c)]:
-            del self.cell_options[(r, c)]['dropdown']
-
-    # c is dcol
-    def delete_checkbox(self, r, c):
-        if (r, c) in self.cell_options and 'checkbox' in self.cell_options[(r, c)]:
-            del self.cell_options[(r, c)]['checkbox']
-
-    # c is dcol
-    def delete_dropdown_and_checkbox(self, r, c):
-        self.delete_dropdown(r, c)
-        self.delete_checkbox(r, c)
-
-    # deprecated
-    def refresh_dropdowns(self, dropdowns = []):
-        pass
-
+    def delete_dropdown(self, datarn, datacn):
+        self.destroy_opened_dropdown_window(datarn = datarn, datacn = datacn)
+        if (datarn, datacn) in self.cell_options and 'dropdown' in self.cell_options[(datarn, datacn)]:
+            del self.cell_options[(datarn, datacn)]['dropdown']
+
+    def delete_checkbox(self, datarn, datacn):
+        if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
+            del self.cell_options[(datarn, datacn)]['checkbox']
+
+    def delete_dropdown_and_checkbox(self, datarn, datacn):
+        self.delete_dropdown(datarn, datacn)
+        self.delete_checkbox(datarn, datacn)
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet_other_classes.py` & `tksheet-6.0.0/tksheet/_tksheet_other_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -134,31 +134,31 @@
         return result
     
     def rc(self,event):
         self.focus_set()
         self.rc_popup_menu.tk_popup(event.x_root, event.y_root)
         
     def select_all(self, event = None):
-        self.event_generate("<Command-a>" if is_mac() else "<Control-a>")
+        self.event_generate("<Command-a>" if on_mac() else "<Control-a>")
         return "break"
     
     def cut(self, event = None):
-        self.event_generate("<Command-x>" if is_mac() else "<Control-x>")
+        self.event_generate("<Command-x>" if on_mac() else "<Control-x>")
         return "break"
     
     def copy(self, event = None):
-        self.event_generate("<Command-c>" if is_mac() else "<Control-c>")
+        self.event_generate("<Command-c>" if on_mac() else "<Control-c>")
         return "break"
     
     def paste(self, event = None):
-        self.event_generate("<Command-v>" if is_mac() else "<Control-v>")
+        self.event_generate("<Command-v>" if on_mac() else "<Control-v>")
         return "break"
 
     def undo(self, event = None):
-        self.event_generate("<Command-z>" if is_mac() else "<Control-z>")
+        self.event_generate("<Command-z>" if on_mac() else "<Control-z>")
         return "break"
 
 
 class TextEditor(tk.Frame):
     def __init__(self,
                  parent,
                  font = get_font(),
@@ -231,22 +231,61 @@
         
 class GeneratedMouseEvent:
     def __init__(self):
         self.keycode = "??"
         self.num = 1
 
 
+def dropdown_search_function(search_for, data):
+    search_len = len(search_for)
+    best_match = {'rn': float("inf"),
+                  'st': float("inf"),
+                  'len_diff': float("inf")}
+    for rn, row in enumerate(data):
+        dd_val = fr"{row[0]}".lower()
+        st = dd_val.find(search_for)
+        if st > -1:
+            # priority is start index
+            # if there's already a matching start
+            # then compare the len difference
+            len_diff = len(dd_val) - search_len
+            if (st < best_match['st'] or
+                (st == best_match['st'] and
+                 len_diff < best_match['len_diff'])
+                ):
+                best_match['rn'] = rn
+                best_match['st'] = st
+                best_match['len_diff'] = len_diff
+    if best_match['rn'] != float("inf"):
+        return best_match['rn']
+    return None
+
+def is_iterable(o):
+    try:
+        iter(o)
+        return True
+    except:
+        return False
+
 def num2alpha(n):
     s = ""
     n += 1
     while n > 0:
         n, r = divmod(n - 1, 26)
         s = chr(65 + r) + s
     return s
 
+def get_n2a(n = 0, _type = "numbers"):
+    if _type == "letters":
+        return num2alpha(n)
+    elif _type == "numbers":
+        return f"{n + 1}"
+    else:
+        return f"{num2alpha(n)} {n + 1}"
+
 def get_index_of_gap_in_sorted_integer_seq_forward(seq, start = 0):
     prevn = seq[start]
     for idx, n in enumerate(islice(seq, start + 1, None), start + 1):
         if n != prevn + 1:
             return idx
         prevn = n
     return None
@@ -255,15 +294,15 @@
     prevn = seq[start]
     for idx, n in zip(range(start, -1, -1), reversed(seq[:start])):
         if n != prevn - 1:
             return idx
         prevn = n
     return None
 
-def is_mac():
+def on_mac():
     if USER_OS == "darwin":
         return True
     else:
         return False
 
 def get_rc_binding():
     if USER_OS == "darwin":
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet_row_index.py` & `tksheet-6.0.0/tksheet/_tksheet_column_headers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,231 +1,247 @@
 from ._tksheet_vars import *
+from ._tksheet_formatters import *
 from ._tksheet_other_classes import *
 
 from itertools import islice, accumulate, chain, cycle, repeat
 from collections import defaultdict
 from math import floor, ceil
 import bisect
 import pickle
 import tkinter as tk
 import zlib
 
 
-class RowIndex(tk.Canvas):
+class ColumnHeaders(tk.Canvas):
     def __init__(self,
                  *args,
                  **kwargs):
         tk.Canvas.__init__(self,
                            kwargs['parentframe'],
-                           background = kwargs['index_bg'],
+                           background = kwargs['header_bg'],
                            highlightthickness = 0)
         self.parentframe = kwargs['parentframe']
+        self.current_height = None    # is set from within MainTable() __init__ or from Sheet parameters
         self.MT = None         # is set from within MainTable() __init__
-        self.CH = None      # is set from within MainTable() __init__
+        self.RI = None    # is set from within MainTable() __init__
         self.TL = None                # is set from within TopLeftRectangle() __init__
         self.extra_begin_edit_cell_func = None
         self.extra_end_edit_cell_func = None
         self.text_editor = None
         self.text_editor_id = None
         self.text_editor_loc = None
-        self.b1_pressed_loc = None
-        self.existing_dropdown_canvas_id = None
-        self.existing_dropdown_window = None
-        self.closed_dropdown = None
         self.centre_alignment_text_mod_indexes = (slice(1, None), slice(None, -1))
         self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
         self.grid_cyctup = ("st", "end")
         self.grid_cyc = cycle(self.grid_cyctup)
+        self.b1_pressed_loc = None
+        self.existing_dropdown_canvas_id = None
+        self.existing_dropdown_window = None
+        self.closed_dropdown = None
         self.being_drawn_rect = None
         self.extra_motion_func = None
         self.extra_b1_press_func = None
         self.extra_b1_motion_func = None
         self.extra_b1_release_func = None
+        self.extra_double_b1_func = None
+        self.ch_extra_begin_drag_drop_func = None
+        self.ch_extra_end_drag_drop_func = None
         self.extra_rc_func = None
         self.selection_binding_func = None
         self.shift_selection_binding_func = None
         self.drag_selection_binding_func = None
-        self.ri_extra_begin_drag_drop_func = None
-        self.ri_extra_end_drag_drop_func = None
-        self.extra_double_b1_func = None
-        self.row_height_resize_func = None
-        self.new_row_width = 0
-        self.cell_options = {}
-        self.drag_and_drop_enabled = False
-        self.dragged_row = None
+        self.column_width_resize_func = None
         self.width_resizing_enabled = False
         self.height_resizing_enabled = False
         self.double_click_resizing_enabled = False
-        self.row_selection_enabled = False
-        self.rc_insert_row_enabled = False
-        self.rc_delete_row_enabled = False
+        self.col_selection_enabled = False
+        self.drag_and_drop_enabled = False
+        self.rc_delete_col_enabled = False
+        self.rc_insert_col_enabled = False
+        self.hide_columns_enabled = False
         self.edit_cell_enabled = False
-        self.visible_row_dividers = {}
-        self.row_width_resize_bbox = tuple()
+        self.dragged_col = None
+        self.visible_col_dividers = {}
+        self.col_height_resize_bbox = tuple()
+        self.cell_options = {}
         self.rsz_w = None
         self.rsz_h = None
+        self.new_col_height = 0
+        self.lines_start_at = 0
         self.currently_resizing_width = False
         self.currently_resizing_height = False
-        self.ri_rc_popup_menu = None
+        self.ch_rc_popup_menu = None
         
         self.disp_text = defaultdict(set)
         self.disp_high = defaultdict(set)
         self.disp_grid = {}
         self.disp_fill_sels = {}
-        self.disp_bord_sels = {}
         self.disp_resize_lines = {}
         self.disp_dropdown = {}
         self.disp_checkbox = {}
         self.hidd_text = defaultdict(set)
         self.hidd_high = defaultdict(set)
         self.hidd_grid = {}
         self.hidd_fill_sels = {}
-        self.hidd_bord_sels = {}
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
         
-        self.row_drag_and_drop_perform = kwargs['row_drag_and_drop_perform']
-        if kwargs['row_index_width'] is None:
-            self.set_width(70)
-            self.default_width = 70
-        else:
-            self.set_width(kwargs['row_index_width'])
-            self.default_width = kwargs['row_index_width']
-        self.max_rh = float(kwargs['max_rh'])
-        self.max_row_width = float(kwargs['max_row_width'])
-        self.index_fg = kwargs['index_fg']
-        self.index_grid_fg = kwargs['index_grid_fg']
-        self.index_border_fg = kwargs['index_border_fg']
-        self.index_selected_cells_bg = kwargs['index_selected_cells_bg']
-        self.index_selected_cells_fg = kwargs['index_selected_cells_fg']
-        self.index_selected_rows_bg = kwargs['index_selected_rows_bg']
-        self.index_selected_rows_fg = kwargs['index_selected_rows_fg']
-        self.index_hidden_rows_expander_bg = kwargs['index_hidden_rows_expander_bg']
-        self.index_bg = kwargs['index_bg']
+        self.column_drag_and_drop_perform = kwargs['column_drag_and_drop_perform']
+        self.default_header = kwargs['default_header'].lower()
+        self.max_cw = float(kwargs['max_colwidth'])
+        self.max_header_height = float(kwargs['max_header_height'])
+        self.header_bg = kwargs['header_bg']
+        self.header_fg = kwargs['header_fg']
+        self.header_grid_fg = kwargs['header_grid_fg']
+        self.header_border_fg = kwargs['header_border_fg']
+        self.header_selected_cells_bg = kwargs['header_selected_cells_bg']
+        self.header_selected_cells_fg = kwargs['header_selected_cells_fg']
+        self.header_selected_columns_bg = kwargs['header_selected_columns_bg']
+        self.header_selected_columns_fg = kwargs['header_selected_columns_fg']
+        self.header_hidden_columns_expander_bg = kwargs['header_hidden_columns_expander_bg']
+        self.show_default_header_for_empty = kwargs['show_default_header_for_empty']
         self.drag_and_drop_bg = kwargs['drag_and_drop_bg']
         self.resizing_line_fg = kwargs['resizing_line_fg']
-        self.align = kwargs['row_index_align']
-        self.show_default_index_for_empty = kwargs['show_default_index_for_empty']
-        self.auto_resize_width = kwargs['auto_resize_width']
-        self.default_index = kwargs['default_row_index'].lower()
+        self.align = kwargs['header_align']
         self.basic_bindings()
-
+        
     def basic_bindings(self, enable = True):
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
             self.bind(get_rc_binding(), self.rc)
+            self.bind("<MouseWheel>", self.mousewheel)
         else:
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
             self.unbind(get_rc_binding())
+            self.unbind("<MouseWheel>")
+            
+    def mousewheel(self, event = None):
+        maxlines = 0
+        if isinstance(self.MT._headers, int):
+            if len(self.MT.data) > self.MT._headers:
+                maxlines = max(len(self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True).rstrip().split("\n")) for datacn in range(len(self.MT.data[self.MT._headers])))
+        elif isinstance(self.MT._headers, (list, tuple)):
+            maxlines = max(len(e.rstrip().split("\n")) if isinstance(e, str) else len(f"{e}".rstrip().split("\n")) for e in self.MT._headers)
+        if maxlines == 1:
+            maxlines = 0
+        if self.lines_start_at > maxlines:
+            self.lines_start_at = maxlines
+        if (event.delta < 0 or event.num == 5) and self.lines_start_at < maxlines:
+            self.lines_start_at += 1
+        elif (event.delta >= 0 or event.num == 4) and self.lines_start_at > 0:
+            self.lines_start_at -= 1
+        self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = False)
 
-    def set_width(self, new_width, set_TL = False):
-        self.current_width = new_width
+    def set_height(self, new_height, set_TL = False):
+        self.current_height = new_height
         try:
-            self.config(width = new_width)
+            self.config(height = new_height)
         except:
             return
         if set_TL:
-            self.TL.set_dimensions(new_w = new_width)
+            self.TL.set_dimensions(new_h = new_height)
 
     def enable_bindings(self, binding):
-        if binding == "row_width_resize":
+        if binding == "column_width_resize":
             self.width_resizing_enabled = True
-        elif binding == "row_height_resize":
+        if binding == "column_height_resize":
             self.height_resizing_enabled = True
-        elif binding == "double_click_row_resize":
+        if binding == "double_click_column_resize":
             self.double_click_resizing_enabled = True
-        elif binding == "row_select":
-            self.row_selection_enabled = True
-        elif binding == "drag_and_drop":
+        if binding == "column_select":
+            self.col_selection_enabled = True
+        if binding == "drag_and_drop":
             self.drag_and_drop_enabled = True
-        
+        if binding == "hide_columns":
+            self.hide_columns_enabled = True
+
     def disable_bindings(self, binding):
-        if binding == "row_width_resize":
+        if binding == "column_width_resize":
             self.width_resizing_enabled = False
-        elif binding == "row_height_resize":
+        if binding == "column_height_resize":
             self.height_resizing_enabled = False
-        elif binding == "double_click_row_resize":
+        if binding == "double_click_column_resize":
             self.double_click_resizing_enabled = False
-        elif binding == "row_select":
-            self.row_selection_enabled = False
-        elif binding == "drag_and_drop":
+        if binding == "column_select":
+            self.col_selection_enabled = False
+        if binding == "drag_and_drop":
             self.drag_and_drop_enabled = False
+        if binding == "hide_columns":
+            self.hide_columns_enabled = False
 
-    def check_mouse_position_height_resizers(self, x, y):
-        for r, (x1, y1, x2, y2) in self.visible_row_dividers.items():
+    def check_mouse_position_width_resizers(self, x, y):
+        for c, (x1, y1, x2, y2) in self.visible_col_dividers.items():
             if (x >= x1 and
                 y >= y1 and
                 x <= x2 and
                 y <= y2):
-                return r
+                return c
 
     def rc(self, event):
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
-        if self.MT.identify_row(y = event.y, allow_end = False) is None:
+        if self.MT.identify_col(x = event.x, allow_end = False) is None:
             self.MT.deselect("all")
             if self.MT.rc_popup_menus_enabled:
                 popup_menu = self.MT.empty_rc_popup_menu
-        elif self.row_selection_enabled and not self.currently_resizing_width and not self.currently_resizing_height:
-            r = self.MT.identify_row(y = event.y)
-            if r < len(self.MT.row_positions) - 1:
-                if self.MT.row_selected(r):
+        elif self.col_selection_enabled and not self.currently_resizing_width and not self.currently_resizing_height:
+            c = self.MT.identify_col(x = event.x)
+            if c < len(self.MT.col_positions) - 1:
+                if self.MT.col_selected(c):
                     if self.MT.rc_popup_menus_enabled:
-                        popup_menu = self.ri_rc_popup_menu
+                        popup_menu = self.ch_rc_popup_menu
                 else:
                     if self.MT.single_selection_enabled and self.MT.rc_select_enabled:
-                        self.select_row(r, redraw = True)
+                        self.select_col(c, redraw = True)
                     elif self.MT.toggle_selection_enabled and self.MT.rc_select_enabled:
-                        self.toggle_select_row(r, redraw = True)
+                        self.toggle_select_col(c, redraw = True)
                     if self.MT.rc_popup_menus_enabled:
-                        popup_menu = self.ri_rc_popup_menu
+                        popup_menu = self.ch_rc_popup_menu
         if self.extra_rc_func is not None:
             self.extra_rc_func(event)
         if popup_menu is not None:
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def shift_b1_press(self, event):
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.mouseclick_outside_editor_or_dropdown()
-        y = event.y
-        r = self.MT.identify_row(y = y)
-        if self.drag_and_drop_enabled or self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
-            if r < len(self.MT.row_positions) - 1:
-                r_selected = self.MT.row_selected(r)
-                if not r_selected and self.row_selection_enabled:
-                    r = int(r)
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
+        x = event.x
+        c = self.MT.identify_col(x = x)
+        if self.drag_and_drop_enabled or self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            if c < len(self.MT.col_positions) - 1:
+                c_selected = self.MT.col_selected(c)
+                if not c_selected and self.col_selection_enabled:
+                    c = int(c)
                     currently_selected = self.MT.currently_selected()
-                    if currently_selected and currently_selected.type_ == "row":
-                        min_r = int(currently_selected.row)
+                    if currently_selected and currently_selected.type_ == "column":
+                        min_c = int(currently_selected[1])
                         self.MT.delete_selection_rects(delete_current = False)
-                        if r > min_r:
-                            self.MT.create_selected(min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
-                            func_event = tuple(range(min_r, r + 1))
-                        elif r < min_r:
-                            self.MT.create_selected(r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows")
-                            func_event = tuple(range(r, min_r + 1))
+                        if c > min_c:
+                            self.MT.create_selected(0, min_c, len(self.MT.row_positions) - 1, c + 1, "columns")
+                            func_event = tuple(range(min_c, c + 1))
+                        elif c < min_c:
+                            self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, min_c + 1, "columns")
+                            func_event = tuple(range(c, min_c + 1))
                     else:
-                        self.select_row(r)
-                        func_event = (r, )
+                        self.select_col(c)
+                        func_event = (c, )
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.shift_selection_binding_func is not None:
-                        self.shift_selection_binding_func(SelectionBoxEvent("shift_select_rows", func_event))
-                elif r_selected:
-                    self.dragged_row = r
+                        self.shift_selection_binding_func(SelectionBoxEvent("shift_select_columns", func_event))
+                elif c_selected:
+                    self.dragged_col = c
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
                 self.itemconfig(t, width = width, fill = fill, tag = tag)
@@ -246,652 +262,577 @@
 
     def mouse_motion(self, event):
         if not self.currently_resizing_height and not self.currently_resizing_width:
             x = self.canvasx(event.x)
             y = self.canvasy(event.y)
             mouse_over_resize = False
             mouse_over_selected = False
-            if self.height_resizing_enabled and not mouse_over_resize:
-                r = self.check_mouse_position_height_resizers(x, y)
-                if r is not None:
-                    self.config(cursor = "sb_v_double_arrow")
-                    self.rsz_h = r
-                    mouse_over_resize = True
+            if self.width_resizing_enabled:
+                c = self.check_mouse_position_width_resizers(x, y)
+                if c is not None:
+                    self.rsz_w, mouse_over_resize = c, True
+                    self.config(cursor = "sb_h_double_arrow")
                 else:
-                    self.rsz_h = None
-            if self.width_resizing_enabled and not mouse_over_resize:
+                    self.rsz_w = None
+            if self.height_resizing_enabled and not mouse_over_resize:
                 try:
-                    x1, y1, x2, y2 = self.row_width_resize_bbox[0], self.row_width_resize_bbox[1], self.row_width_resize_bbox[2], self.row_width_resize_bbox[3]
+                    x1, y1, x2, y2 = self.col_height_resize_bbox[0], self.col_height_resize_bbox[1], self.col_height_resize_bbox[2], self.col_height_resize_bbox[3]
                     if x >= x1 and y >= y1 and x <= x2 and y <= y2:
-                        self.config(cursor = "sb_h_double_arrow")
-                        self.rsz_w = True
+                        self.config(cursor = "sb_v_double_arrow")
+                        self.rsz_h = True
                         mouse_over_resize = True
                     else:
-                        self.rsz_w = None
+                        self.rsz_h = None
                 except:
-                    self.rsz_w = None
+                    self.rsz_h = None
             if not mouse_over_resize:
-                if self.MT.row_selected(self.MT.identify_row(event, allow_end = False)):
+                if self.MT.col_selected(self.MT.identify_col(event, allow_end = False)):
                     self.config(cursor = "hand2")
                     mouse_over_selected = True
             if not mouse_over_resize and not mouse_over_selected:
                 self.MT.reset_mouse_motion_creations()
         if self.extra_motion_func is not None:
             self.extra_motion_func(event)
 
     def double_b1(self, event = None):
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.mouseclick_outside_editor_or_dropdown()
+        self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
-        if self.double_click_resizing_enabled and self.height_resizing_enabled and self.rsz_h is not None and not self.currently_resizing_height:
-            row = self.rsz_h - 1
-            old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
-            new_height = self.set_row_height(row)
+        if self.double_click_resizing_enabled and self.width_resizing_enabled and self.rsz_w is not None and not self.currently_resizing_width:
+            col = self.rsz_w - 1
+            old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
+            new_width = self.set_col_width(col)
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-            if self.row_height_resize_func is not None and old_height != new_height:
-                self.row_height_resize_func(ResizeEvent("row_height_resize", row, old_height, new_height))
-        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
-            self.set_width_of_index_to_text()
-        elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
-            r = self.MT.identify_row(y = event.y)
-            if r < len(self.MT.row_positions) - 1:
+            if self.column_width_resize_func is not None and old_width != new_width:
+                self.column_width_resize_func(ResizeEvent("column_width_resize", col, old_width, new_width))
+        elif self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+            c = self.MT.identify_col(x = event.x)
+            if c < len(self.MT.col_positions) - 1:
                 if self.MT.single_selection_enabled:
-                    self.select_row(r, redraw = True)
+                    self.select_col(c, redraw = True)
                 elif self.MT.toggle_selection_enabled:
-                    self.toggle_select_row(r, redraw = True)
-                drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-                if ((drow in self.cell_options and 'checkbox' in self.cell_options[drow]) or
-                    (drow in self.cell_options and 'dropdown' in self.cell_options[drow]) or
+                    self.toggle_select_col(c, redraw = True)
+                datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+                if ((datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]) or
+                    (datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]) or
                     self.edit_cell_enabled):
                     self.open_cell(event)
-        self.rsz_h = None
+        self.rsz_w = None
         self.mouse_motion(event)
         if self.extra_double_b1_func is not None:
             self.extra_double_b1_func(event)
         
     def b1_press(self, event = None):
         self.MT.unbind("<MouseWheel>")
         self.focus_set()
-        self.MT.mouseclick_outside_editor_or_dropdown()
-        self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown()
+        self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = self.canvasx(event.x)
         y = self.canvasy(event.y)
-        r = self.MT.identify_row(y = event.y)
-        self.b1_pressed_loc = r
-        if self.check_mouse_position_height_resizers(x, y) is None:
-            self.rsz_h = None
-        if not x >= self.row_width_resize_bbox[0] and y >= self.row_width_resize_bbox[1] and x <= self.row_width_resize_bbox[2] and y <= self.row_width_resize_bbox[3]:
+        c = self.MT.identify_col(x = event.x)
+        self.b1_pressed_loc = c
+        if self.check_mouse_position_width_resizers(x, y) is None:
             self.rsz_w = None
-        if self.height_resizing_enabled and self.rsz_h is not None:
-            self.currently_resizing_height = True
-            y = self.MT.row_positions[self.rsz_h]
-            line2y = self.MT.row_positions[self.rsz_h - 1]
+        if self.width_resizing_enabled and self.rsz_w is not None:
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-            self.create_resize_line(0, y, self.current_width, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
-            self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
-            self.create_resize_line(0, line2y, self.current_width, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
-            self.MT.create_resize_line(x1, line2y, x2, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
-        elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w == True:
             self.currently_resizing_width = True
+            x = self.MT.col_positions[self.rsz_w]
+            line2x = self.MT.col_positions[self.rsz_w - 1]
+            self.create_resize_line(x, 0, x, self.current_height, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+            self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+            self.create_resize_line(line2x, 0, line2x, self.current_height,width = 1, fill = self.resizing_line_fg, tag = "rwl2")
+            self.MT.create_resize_line(line2x, y1, line2x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl2")
+        elif self.height_resizing_enabled and self.rsz_w is None and self.rsz_h is not None:
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-            x = int(event.x)
-            if x < self.MT.min_cw:
-                x = int(self.MT.min_cw)
-            self.new_row_width = x
-            self.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
-        elif self.MT.identify_row(y = event.y, allow_end = False) is None:
+            self.currently_resizing_height = True
+            y = event.y
+            if y < self.MT.hdr_min_rh:
+                y = int(self.MT.hdr_min_rh)
+            self.new_col_height = y
+            self.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+        elif self.MT.identify_col(x = event.x, allow_end = False) is None:
             self.MT.deselect("all")
-        elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
-            r = self.MT.identify_row(y = event.y)
-            if r < len(self.MT.row_positions) - 1:
-                if self.MT.row_selected(r):
-                    drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-                    if ((drow in self.cell_options and 'dropdown' in self.cell_options[drow] and event.x < self.current_width and event.x > self.current_width - self.MT.txt_h - 4) or
-                        (drow in self.cell_options and 'checkbox' in self.cell_options[drow] and event.x < self.current_width + self.MT.txt_h + 5)) and y < self.MT.row_positions[r] + self.MT.txt_h + 5:
+        elif self.col_selection_enabled and self.rsz_w is None and self.rsz_h is None:
+            if c < len(self.MT.col_positions) - 1:
+                if self.MT.col_selected(c):
+                    datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+                    if ((datacn in self.cell_options and 'dropdown' in self.cell_options[datacn] and x < self.MT.col_positions[c + 1] and x > self.MT.col_positions[c + 1] - self.MT.hdr_txt_h - 4) or
+                        (datacn in self.cell_options and 'checkbox' in self.cell_options[datacn] and x < self.MT.col_positions[c] + self.MT.hdr_txt_h + 5)) and event.y < self.MT.hdr_txt_h + 5:
                         pass
                     else:
-                        self.dragged_row = r
+                        self.dragged_col = c
                 else:
-                    self.being_drawn_rect = (r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+                    self.being_drawn_rect = (0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
                     if self.MT.single_selection_enabled:
-                        self.select_row(r, redraw = True)
+                        self.select_col(c, redraw = True)
                     elif self.MT.toggle_selection_enabled:
-                        self.toggle_select_row(r, redraw = True)
+                        self.toggle_select_col(c, redraw = True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
     
     def b1_motion(self, event):
-        x1,y1,x2,y2 = self.MT.get_canvas_visible_area()
-        if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
-            y = self.canvasy(event.y)
-            size = y - self.MT.row_positions[self.rsz_h - 1]
-            if size >= self.MT.min_rh and size < self.max_rh:
+        x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+        if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
+            x = self.canvasx(event.x)
+            size = x - self.MT.col_positions[self.rsz_w - 1]
+            if size >= self.MT.min_cw and size < self.max_cw:
                 self.delete_resize_lines()
                 self.MT.delete_resize_lines()
-                line2y = self.MT.row_positions[self.rsz_h - 1]
-                self.create_resize_line(0, y, self.current_width, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
-                self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
-                self.create_resize_line(0, line2y, self.current_width, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
-                self.MT.create_resize_line(x1, line2y, x2, line2y, width = 1, fill = self.resizing_line_fg, tag = "rhl2")
-        elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
-            evx = event.x
+                line2x = self.MT.col_positions[self.rsz_w - 1]
+                self.create_resize_line(x, 0, x, self.current_height, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+                self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+                self.create_resize_line(line2x, 0, line2x, self.current_height,width = 1, fill = self.resizing_line_fg, tag = "rwl2")
+                self.MT.create_resize_line(line2x, y1, line2x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl2")
+        elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
+            evy = event.y
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            if evx > self.current_width:
-                x = self.MT.canvasx(evx - self.current_width)
-                if evx > self.max_row_width:
-                    evx = int(self.max_row_width)
-                    x = self.MT.canvasx(evx - self.current_width)
-                self.new_row_width = evx
-                self.MT.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
+            if evy > self.current_height:
+                y = self.MT.canvasy(evy - self.current_height)
+                if evy > self.max_header_height:
+                    evy = int(self.max_header_height)
+                    y = self.MT.canvasy(evy - self.current_height)
+                self.new_col_height = evy
+                self.MT.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
             else:
-                x = evx
-                if x < self.MT.min_cw:
-                    x = int(self.MT.min_cw)
-                self.new_row_width = x
-                self.create_resize_line(x, y1, x, y2, width = 1, fill = self.resizing_line_fg, tag = "rwl")
-        if self.drag_and_drop_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None and self.MT.anything_selected(exclude_cells = True, exclude_columns = True):
-            y = self.canvasy(event.y)
-            if y > 0 and y < self.MT.row_positions[-1]:
-                y = event.y
-                hend = self.winfo_height()
-                ycheck = self.yview()
-                if y >= hend - 0 and len(ycheck) > 1 and ycheck[1] < 1:
-                    if y >= hend + 15:
-                        self.MT.yview_scroll(2, "units")
-                        self.yview_scroll(2, "units")
+                y = evy
+                if y < self.MT.hdr_min_rh:
+                    y = int(self.MT.hdr_min_rh)
+                self.new_col_height = y
+                self.create_resize_line(x1, y, x2, y, width = 1, fill = self.resizing_line_fg, tag = "rhl")
+        elif self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
+            x = self.canvasx(event.x)
+            if x > 0 and x < self.MT.col_positions[-1]:
+                x = event.x
+                wend = self.winfo_width()
+                xcheck = self.xview()
+                if x >= wend - 0 and len(xcheck) > 1 and xcheck[1] < 1:
+                    if x >= wend + 15:
+                        self.MT.xview_scroll(2, "units")
+                        self.xview_scroll(2, "units")
                     else:
-                        self.MT.yview_scroll(1, "units")
-                        self.yview_scroll(1, "units")
-                    self.check_yview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
-                elif y <= 0 and len(ycheck) > 1 and ycheck[0] > 0:
-                    if y >= -15:
-                        self.MT.yview_scroll(-1, "units")
-                        self.yview_scroll(-1, "units")
+                        self.MT.xview_scroll(1, "units")
+                        self.xview_scroll(1, "units")
+                    self.check_xview()
+                    self.MT.main_table_redraw_grid_and_text(redraw_header = True)
+                elif x <= 0 and len(xcheck) > 1 and xcheck[0] > 0:
+                    if x >= -15:
+                        self.MT.xview_scroll(-1, "units")
+                        self.xview_scroll(-1, "units")
                     else:
-                        self.MT.yview_scroll(-2, "units")
-                        self.yview_scroll(-2, "units")
-                    self.check_yview()
-                    self.MT.main_table_redraw_grid_and_text(redraw_row_index = True)
-                row = self.MT.identify_row(y = event.y)
-                sels = self.MT.get_selected_rows()
+                        self.MT.xview_scroll(-2, "units")
+                        self.xview_scroll(-2, "units")
+                    self.check_xview()
+                    self.MT.main_table_redraw_grid_and_text(redraw_header = True)
+                col = self.MT.identify_col(x = event.x)
+                sels = self.MT.get_selected_cols()
                 selsmin = min(sels)
-                if row in sels:
-                    ypos = self.MT.row_positions[selsmin]
+                if col in sels:
+                    xpos = self.MT.col_positions[selsmin]
                 else:
-                    if row < selsmin:
-                        ypos = self.MT.row_positions[row]
+                    if col < selsmin:
+                        xpos = self.MT.col_positions[col]
                     else:
-                        ypos = self.MT.row_positions[row + 1]
+                        xpos = self.MT.col_positions[col + 1]
                 self.delete_resize_lines()
                 self.MT.delete_resize_lines()
-                self.create_resize_line(0, ypos, self.current_width, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
-                self.MT.create_resize_line(x1, ypos, x2, ypos, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
-        elif self.MT.drag_selection_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+                self.create_resize_line(xpos, 0, xpos, self.current_height, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+                self.MT.create_resize_line(xpos, y1, xpos, y2, width = 3, fill = self.drag_and_drop_bg, tag = "dd")
+        elif self.MT.drag_selection_enabled and self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             need_redraw = False
-            end_row = self.MT.identify_row(y = event.y)
+            end_col = self.MT.identify_col(x = event.x)
             currently_selected = self.MT.currently_selected()
-            if end_row < len(self.MT.row_positions) - 1 and currently_selected:
-                if currently_selected.type_ == "row":
-                    start_row = currently_selected.row
-                    if end_row >= start_row:
-                        rect = (start_row, 0, end_row + 1, len(self.MT.col_positions) - 1, "rows")
-                        func_event = tuple(range(start_row, end_row + 1))
-                    elif end_row < start_row:
-                        rect = (end_row, 0, start_row + 1, len(self.MT.col_positions) - 1, "rows")
-                        func_event = tuple(range(end_row, start_row + 1))
+            if end_col < len(self.MT.col_positions) - 1 and currently_selected:
+                if currently_selected.type_ == "column":
+                    start_col = currently_selected[1]
+                    if end_col >= start_col:
+                        rect = (0, start_col, len(self.MT.row_positions) - 1, end_col + 1, "columns")
+                        func_event = tuple(range(start_col, end_col + 1))
+                    elif end_col < start_col:
+                        rect = (0, end_col, len(self.MT.row_positions) - 1, start_col + 1, "columns")
+                        func_event = tuple(range(end_col, start_col + 1))
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         self.MT.delete_selection_rects(delete_current = False)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
-                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
-            ycheck = self.yview()
-            if event.y > self.winfo_height() and len(ycheck) > 1 and ycheck[1] < 1:
-                try:
-                    self.MT.yview_scroll(1, "units")
-                    self.yview_scroll(1, "units")
-                except:
-                    pass
-                self.check_yview()
-                need_redraw = True
-            elif event.y < 0 and self.canvasy(self.winfo_height()) > 0 and ycheck and ycheck[0] > 0:
-                try:
-                    self.yview_scroll(-1, "units")
-                    self.MT.yview_scroll(-1, "units")
-                except:
-                    pass
-                self.check_yview()
-                need_redraw = True
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
+                xcheck = self.xview()
+                if event.x > self.winfo_width() and len(xcheck) > 1 and xcheck[1] < 1:
+                    try:
+                        self.MT.xview_scroll(1, "units")
+                        self.xview_scroll(1, "units")
+                    except:
+                        pass
+                    self.check_xview()
+                    need_redraw = True
+                elif event.x < 0 and self.canvasx(self.winfo_width()) > 0 and xcheck and xcheck[0] > 0:
+                    try:
+                        self.xview_scroll(-1, "units")
+                        self.MT.xview_scroll(-1, "units")
+                    except:
+                        pass
+                    self.check_xview()
+                    need_redraw = True
             if need_redraw:
-                self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
+                self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False)
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
 
-    def check_yview(self):
-        ycheck = self.yview()
-        if ycheck and ycheck[0] < 0:
-            self.MT.set_yviews("moveto", 0)
-        if len(ycheck) > 1 and ycheck[1] > 1:
-            self.MT.set_yviews("moveto", 1)
+    def check_xview(self):
+        xcheck = self.xview()
+        if xcheck and xcheck[0] < 0:
+            self.MT.set_xviews("moveto", 0)
+        elif len(xcheck) > 1 and xcheck[1] > 1:
+            self.MT.set_xviews("moveto", 1)
             
     def b1_release(self, event = None):
         if self.being_drawn_rect is not None:
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.MT.create_selected(*to_sel)
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
-        if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
-            self.currently_resizing_height = False
-            new_row_pos = int(self.coords("rhl")[1])
+        if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
+            self.currently_resizing_width = False
+            new_col_pos = int(self.coords("rwl")[0])
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
-            size = new_row_pos - self.MT.row_positions[self.rsz_h - 1]
-            if size < self.MT.min_rh:
-                new_row_pos = ceil(self.MT.row_positions[self.rsz_h - 1] + self.MT.min_rh)
-            elif size > self.max_rh:
-                new_row_pos = floor(self.MT.row_positions[self.rsz_h - 1] + self.max_rh)
-            increment = new_row_pos - self.MT.row_positions[self.rsz_h]
-            self.MT.row_positions[self.rsz_h + 1:] = [e + increment for e in islice(self.MT.row_positions, self.rsz_h + 1, len(self.MT.row_positions))]
-            self.MT.row_positions[self.rsz_h] = new_row_pos
-            new_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
+            old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
+            size = new_col_pos - self.MT.col_positions[self.rsz_w - 1]
+            if size < self.MT.min_cw:
+                new_col_pos = ceil(self.MT.col_positions[self.rsz_w - 1] + self.MT.min_cw)
+            elif size > self.max_cw:
+                new_col_pos = floor(self.MT.col_positions[self.rsz_w - 1] + self.max_cw)
+            increment = new_col_pos - self.MT.col_positions[self.rsz_w]
+            self.MT.col_positions[self.rsz_w + 1:] = [e + increment for e in islice(self.MT.col_positions, self.rsz_w + 1, len(self.MT.col_positions))]
+            self.MT.col_positions[self.rsz_w] = new_col_pos
+            new_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             self.MT.recreate_all_selection_boxes()
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-            if self.row_height_resize_func is not None and old_height != new_height:
-                self.row_height_resize_func(ResizeEvent("row_height_resize", self.rsz_h - 1, old_height, new_height))
-        elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
-            self.currently_resizing_width = False
+            if self.column_width_resize_func is not None and old_width != new_width:
+                self.column_width_resize_func(ResizeEvent("column_width_resize", self.rsz_w - 1, old_width, new_width))
+        elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
+            self.currently_resizing_height = False
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            self.set_width(self.new_row_width, set_TL = True)
+            self.set_height(self.new_col_height,set_TL = True)
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-        if self.drag_and_drop_enabled and self.MT.anything_selected(exclude_cells = True, exclude_columns = True) and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None and self.dragged_row is not None:
+        elif self.drag_and_drop_enabled and self.col_selection_enabled and self.MT.anything_selected(exclude_cells = True, exclude_rows = True) and self.rsz_h is None and self.rsz_w is None and self.dragged_col is not None:
             self.delete_resize_lines()
             self.MT.delete_resize_lines()
-            y = event.y
-            r = self.MT.identify_row(y = y)
-            orig_selected = self.MT.get_selected_rows()
-            if r != self.dragged_row and r is not None and r not in orig_selected and len(orig_selected) != (len(self.MT.row_positions) - 1):
+            x = event.x
+            c = self.MT.identify_col(x = x)
+            orig_selected = self.MT.get_selected_cols()
+            if c != self.dragged_col and c is not None and c not in orig_selected and len(orig_selected) != len(self.MT.col_positions) - 1:
                 orig_selected = sorted(orig_selected)
                 if len(orig_selected) > 1:
-                    orig_min = orig_selected[0]
-                    orig_max = orig_selected[1]
-                    start_idx = bisect.bisect_left(orig_selected, self.dragged_row)
+                    start_idx = bisect.bisect_left(orig_selected, self.dragged_col)
                     forward_gap = get_index_of_gap_in_sorted_integer_seq_forward(orig_selected, start_idx)
                     reverse_gap = get_index_of_gap_in_sorted_integer_seq_reverse(orig_selected, start_idx)
                     if forward_gap is not None:
                         orig_selected[:] = orig_selected[:forward_gap]
                     if reverse_gap is not None:
                         orig_selected[:] = orig_selected[reverse_gap:]
                 rm1start = orig_selected[0]
-                totalrows = len(orig_selected)
+                totalcols = len(orig_selected)
                 extra_func_success = True
-                if r >= len(self.MT.row_positions) - 1:
-                    r -= 1
-                if self.ri_extra_begin_drag_drop_func is not None:
+                if c >= len(self.MT.col_positions) - 1:
+                    c -= 1
+                if self.ch_extra_begin_drag_drop_func is not None:
                     try:
-                        self.ri_extra_begin_drag_drop_func(BeginDragDropEvent("begin_row_index_drag_drop", tuple(orig_selected), int(r)))
+                        self.ch_extra_begin_drag_drop_func(BeginDragDropEvent("begin_column_header_drag_drop", tuple(orig_selected), int(c)))
                     except:
                         extra_func_success = False
                 if extra_func_success:
-                    new_selected, dispset = self.MT.move_rows_adjust_options_dict(r, 
-                                                                                  rm1start, totalrows, move_data = self.row_drag_and_drop_perform)
+                    new_selected, dispset = self.MT.move_columns_adjust_options_dict(c,
+                                                                                     rm1start, 
+                                                                                     totalcols,
+                                                                                     move_data = self.column_drag_and_drop_perform)
                     if self.MT.undo_enabled:
-                        self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_rows",
-                                                                                min(orig_selected),
-                                                                                new_selected[0],
-                                                                                new_selected[-1],
-                                                                                sorted(orig_selected)))))
+                        self.MT.undo_storage.append(zlib.compress(pickle.dumps(("move_cols",                 #0
+                                                                                int(orig_selected[0]),  #1
+                                                                                int(new_selected[0]),        #2
+                                                                                int(new_selected[-1]),       #3
+                                                                                sorted(orig_selected),  #4
+                                                                                dispset))))                  #5
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
-                    if self.ri_extra_end_drag_drop_func is not None:
-                        self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", tuple(orig_selected), new_selected, int(r)))
-                        
+                    if self.ch_extra_end_drag_drop_func is not None:
+                        self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", tuple(orig_selected), new_selected, int(c)))
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
-            r = self.MT.identify_row(y = event.y)
-            if r is not None and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
-                drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-                canvasy = self.canvasy(event.y)
-                if ((drow in self.cell_options and 'dropdown' in self.cell_options[drow] and event.x < self.current_width and event.x > self.current_width - self.MT.txt_h - 4) or
-                    (drow in self.cell_options and 'checkbox' in self.cell_options[drow] and event.x < self.MT.txt_h + 5)):
-                    if canvasy < self.MT.row_positions[r] + self.MT.txt_h:
-                        self.open_cell(event)
+            c = self.MT.identify_col(x = event.x)
+            if c is not None and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
+                datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+                canvasx = self.canvasx(event.x)
+                if (event.y < self.MT.hdr_txt_h + 5 and
+                    (
+                     (datacn in self.cell_options and 
+                      'dropdown' in self.cell_options[datacn] and 
+                      canvasx < self.MT.col_positions[c + 1] and 
+                      canvasx > self.MT.col_positions[c + 1] - self.MT.hdr_txt_h - 4)
+                     or
+                     (datacn in self.cell_options and 
+                      'checkbox' in self.cell_options[datacn] and
+                      canvasx < self.MT.col_positions[c] + self.MT.hdr_txt_h + 5)
+                    )
+                ):
+                    self.open_cell(event)
             else:
-                self.mouseclick_outside_editor_or_dropdown()
+                self.mouseclick_outside_editor_or_dropdown_all_canvases()
             self.b1_pressed_loc = None
-            self.closed_dropdown = None    
-        self.dragged_row = None
+            self.closed_dropdown = None
+        self.dragged_col = None
         self.currently_resizing_width = False
         self.currently_resizing_height = False
         self.rsz_w = None
         self.rsz_h = None
         self.mouse_motion(event)
         if self.extra_b1_release_func is not None:
             self.extra_b1_release_func(event)
             
-    def readonly_index(self, rows = [], readonly = True):
-        if isinstance(rows, int):
-            rows_ = [rows]
+    def readonly_header(self, columns = [], readonly = True):
+        if isinstance(columns, int):
+            columns_ = [columns]
         else:
-            rows_ = rows
+            columns_ = columns
         if not readonly:
-            for r in rows_:
-                if r in self.cell_options and 'readonly' in self.cell_options[r]:
-                    del self.cell_options[r]['readonly']
-        else:
-            for r in rows_:
-                if r not in self.cell_options:
-                    self.cell_options[r] = {}
-                self.cell_options[r]['readonly'] = True
+            for c in columns_:
+                if c in self.cell_options and 'readonly' in self.cell_options[c]:
+                    del self.cell_options[c]['readonly']
+        else:
+            for c in columns_:
+                if c not in self.cell_options:
+                    self.cell_options[c] = {}
+                self.cell_options[c]['readonly'] = True
 
-    def highlight_cells(self, r = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
+    def highlight_cells(self, c = 0, cells = tuple(), bg = None, fg = None, redraw = False, overwrite = True):
         if bg is None and fg is None:
             return
         if cells and not isinstance(cells, int):
             iterable = cells
         elif isinstance(cells, int):
             iterable = (cells, )
         else:
-            iterable = (r, )
-        for r_ in iterable:
-            if r_ not in self.cell_options:
-                self.cell_options[r_] = {}
-            if 'highlight' in self.cell_options[r_] and not overwrite:
-                self.cell_options[r_]['highlight'] = (self.cell_options[r_]['highlight'][0] if bg is None else bg,
-                                                        self.cell_options[r_]['highlight'][1] if fg is None else fg)
+            iterable = (c, )
+        for c_ in iterable:
+            if c_ not in self.cell_options:
+                self.cell_options[c_] = {}
+            if 'highlight' in self.cell_options[c_] and not overwrite:
+                self.cell_options[c_]['highlight'] = (self.cell_options[c_]['highlight'][0] if bg is None else bg,
+                                                      self.cell_options[c_]['highlight'][1] if fg is None else fg)
             else:
-                self.cell_options[r_]['highlight'] = (bg, fg)
+                self.cell_options[c_]['highlight'] = (bg, fg)
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(False, True)
+            self.MT.main_table_redraw_grid_and_text(True, False)
 
-    def select_row(self, r, redraw = False, keep_other_selections = False):
+    def select_col(self, c, redraw = False, keep_other_selections = False):
         ignore_keep = False
         if keep_other_selections:
-            if self.MT.row_selected(r):
-                self.MT.create_current(r, 0, type_ = "row", inside = True)
+            if self.MT.col_selected(c):
+                self.MT.create_current(0, c, type_ = "column", inside = True)
             else:
                 ignore_keep = True
         if ignore_keep or not keep_other_selections:
             self.MT.delete_selection_rects()
-            self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
-            self.MT.create_current(r, 0, type_ = "row", inside = True)
+            self.MT.create_current(0, c, type_ = "column", inside = True)
+            self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None:
-            self.selection_binding_func(SelectRowEvent("select_row", int(r)))
+            self.selection_binding_func(SelectColumnEvent("select_column", int(c)))
 
-    def toggle_select_row(self, row, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
+    def toggle_select_col(self, column, add_selection = True, redraw = True, run_binding_func = True, set_as_current = True):
         if add_selection:
-            if self.MT.row_selected(row):
-                self.MT.deselect(r = row, redraw = redraw)
+            if self.MT.col_selected(column):
+                self.MT.deselect(c = column, redraw = redraw)
             else:
-                self.add_selection(r = row, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
+                self.add_selection(c = column, redraw = redraw, run_binding_func = run_binding_func, set_as_current = set_as_current)
         else:
-            if self.MT.row_selected(row):
-                self.MT.deselect(r = row, redraw = redraw)
+            if self.MT.col_selected(column):
+                self.MT.deselect(c = column, redraw = redraw)
             else:
-                self.select_row(row, redraw = redraw)
+                self.select_col(column, redraw = redraw)
 
-    def add_selection(self, r, redraw = False, run_binding_func = True, set_as_current = True):
-        r = int(r)
+    def add_selection(self, c, redraw = False, run_binding_func = True, set_as_current = True):
+        c = int(c)
         if set_as_current:
             create_new_sel = False
             current = self.MT.get_tags_of_current()
             if current:
                 if current[0] == "Current_Outside":
                     create_new_sel = True
-            self.MT.create_current(r, 0, type_ = "row", inside = True)
+            self.MT.create_current(0, c, type_ = "column", inside = True)
             if create_new_sel:
                 r1, c1, r2, c2 = tuple(int(e) for e in current[1].split("_") if e)
                 self.MT.create_selected(r1, c1, r2, c2, current[2] + "s")
-        self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
+        self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True)
+            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
         if self.selection_binding_func is not None and run_binding_func:
-            self.selection_binding_func(("select_row", int(r)))
+            self.selection_binding_func(("select_column", int(c)))
 
-    def set_row_height(self, row, height = None, only_set_if_too_small = False, recreate = True, return_new_height = False, displayed_only = False):
-        r_norm = row + 1
-        r_extra = row + 2
-        min_rh = self.MT.min_rh
-        if height is None:
-            if self.MT.all_columns_displayed:
-                if displayed_only:
-                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                    start_col, end_col = self.MT.get_visible_columns(x1, x2)
-                else:
-                    start_col, end_col = 0, len(self.MT.data[row]) if self.MT.data else 0
-                iterable = range(start_col, end_col)
-            else:
-                if displayed_only:
-                    x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-                    start_col, end_col = self.MT.get_visible_columns(x1, x2)
-                else:
-                    start_col, end_col = 0, len(self.MT.displayed_columns)
-                iterable = self.MT.displayed_columns[start_col:end_col]
-            new_height = int(min_rh)
-            try:
-                if row in self.cell_options and 'checkbox' in self.cell_options[row]:
-                    txt = self.cell_options[row]['checkbox']['text']
-                else:
-                    if isinstance(self.MT._row_index[row], str):
-                        txt = self.MT._row_index[row]
-                    else:
-                        txt = f"{self.MT._row_index[row]}"
-            except:
-                txt = ""
-            if txt:
-                h = self.MT.GetTextHeight(txt) + 5
-            else:
-                h = min_rh
-            if h < min_rh:
-                h = int(min_rh)
-            elif h > self.max_rh:
-                h = int(self.max_rh)
-            if h > new_height:
-                new_height = h
-            if self.MT.data:
-                for cn in iterable:
-                    if (row, cn) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(row, cn)]:
-                        txt = self.MT.cell_options[(row, cn)]['checkbox']['text']
-                    else:
-                        try:
-                            if isinstance(self.MT.data[row][cn], str):
-                                txt = self.MT.data[row][cn]
-                            else:
-                                txt = f"{self.MT.data[row][cn]}"
-                        except:
-                            txt = ""
-                    if txt:
-                        h = self.MT.GetTextHeight(txt) + 5
-                    else:
-                        h = min_rh
-                    if h < min_rh:
-                        h = int(min_rh)
-                    elif h > self.max_rh:
-                        h = int(self.max_rh)
-                    if h > new_height:
-                        new_height = h
-        else:
-            new_height = int(height)
-        if new_height < min_rh:
-            new_height = int(min_rh)
-        elif new_height > self.max_rh:
-            new_height = int(self.max_rh)
-        if only_set_if_too_small and new_height <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
-            return self.MT.row_positions[row + 1] - self.MT.row_positions[row]
-        if not return_new_height:
-            new_row_pos = self.MT.row_positions[row] + new_height
-            increment = new_row_pos - self.MT.row_positions[r_norm]
-            self.MT.row_positions[r_extra:] = [e + increment for e in islice(self.MT.row_positions, r_extra, len(self.MT.row_positions))]
-            self.MT.row_positions[r_norm] = new_row_pos
-            if recreate:
-                self.MT.recreate_all_selection_boxes()
-        return new_height
-
-    def set_width_of_index_to_text(self, recreate = True):
-        if not self.MT._row_index and isinstance(self.MT._row_index, list):
+    def set_col_width(self, col, width = None, only_set_if_too_small = False, displayed_only = False, recreate = True, return_new_width = False):
+        if col < 0:
             return
         qconf = self.MT.txt_measure_canvas.itemconfig
         qbbox = self.MT.txt_measure_canvas.bbox
         qtxtm = self.MT.txt_measure_canvas_text
-        new_width = int(self.MT.min_cw)
-        if isinstance(self.MT._row_index, list):
-            for rn, row in enumerate(self.MT._row_index):
-                if rn in self.cell_options and 'checkbox' in self.cell_options[rn]:
-                    txt = self.cell_options[rn]['checkbox']['text']
-                else:
-                    try:
-                        if isinstance(row, str):
-                            txt = row
-                        else:
-                            txt = f"{row}"
-                    except:
-                        txt = ""
-                if txt:
-                    qconf(qtxtm, text = txt)
-                    b = qbbox(qtxtm)
-                    w = b[2] - b[0] + 10
-                else:
-                    w = self.default_width
-                if w < self.MT.min_cw:
-                    w = int(self.MT.min_cw)
-                elif w > self.max_row_width:
-                    w = int(self.max_row_width)
-                if rn in self.cell_options and 'checkbox' in self.cell_options[rn]:
-                    w += self.MT.txt_h + 6
-                elif rn in self.cell_options and 'dropdown' in self.cell_options[rn]:
-                    w += self.MT.txt_h + 4
-                if w > new_width:
-                    new_width = w
-        elif isinstance(self.MT._row_index, int):
-            c = self.MT._row_index
-            for rn, row in enumerate(self.MT.data):
-                if (rn, c) in self.MT.cell_options and 'checkbox' in self.MT.cell_options[(rn, c)]:
-                    txt = self.MT.cell_options[(rn, c)]['checkbox']['text']
-                else:
-                    try:
-                        if isinstance(row[c], str):
-                            txt = row[c]
+        qtxth = self.MT.txt_h
+        qclop = self.MT.cell_options
+        qfont = self.MT._font
+        if width is None:
+            w = self.MT.min_cw
+            hw = self.MT.min_cw
+            if displayed_only:
+                x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
+                start_row, end_row = self.MT.get_visible_rows(y1, y2)
+            else:
+                start_row, end_row = 0, None
+            datacn = col if self.MT.all_columns_displayed else self.MT.displayed_columns[col]
+            # header
+            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+                qconf(qtxtm, text = self.cell_options[datacn]['checkbox']['text'], font = self.MT._hdr_font)
+                b = qbbox(qtxtm)
+                hw = b[2] - b[0] + 7 + self.MT.hdr_txt_h
+            else:
+                txt = ""
+                if isinstance(self.MT._headers, int) or len(self.MT._headers) > datacn:
+                    txt = self.get_valid_cell_data_as_str(datacn, fix = False)
+                    if txt or (datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]):
+                        qconf(qtxtm, text = txt, font = self.MT._hdr_font)
+                        b = qbbox(qtxtm)
+                        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                            hw = b[2] - b[0] + 7 + self.MT.hdr_txt_h
                         else:
-                            txt = f"{row[c]}"
-                    except:
-                        txt = ""
-                if txt:
-                    qconf(qtxtm, text = txt)
+                            hw = b[2] - b[0] + 7
+                if not isinstance(self.MT._headers, int) and ((not txt and self.show_default_header_for_empty) or len(self.MT._headers) < datacn):
+                    if self.default_header == "letters":
+                        hw = self.MT.GetHdrTextWidth(num2alpha(datacn)) + 7
+                    elif self.default_header == "numbers":
+                        hw = self.MT.GetHdrTextWidth(f"{datacn + 1}") + 7
+                    else:
+                        hw = self.MT.GetHdrTextWidth(f"{datacn + 1} {num2alpha(datacn)}") + 7
+            # table
+            for rn, r in enumerate(islice(self.MT.data, start_row, end_row), start_row):
+                if (rn, datacn) in qclop and 'checkbox' in qclop[(rn, datacn)]:
+                    qconf(qtxtm, text = qclop[(rn, datacn)]['checkbox']['text'], font = qfont)
                     b = qbbox(qtxtm)
-                    w = b[2] - b[0] + 10
+                    tw = qtxth + 7 + b[2] - b[0]
+                    if tw > w:
+                        w = tw
                 else:
-                    w = self.default_width
-                if w < self.MT.min_cw:
-                    w = int(self.MT.min_cw)
-                elif w > self.max_row_width:
-                    w = int(self.max_row_width)
-                if w > new_width:
-                    new_width = w
-        if new_width == self.MT.min_cw:
-            new_width = self.MT.min_cw + 10
-        self.set_width(new_width, set_TL = True)
-        if recreate:
-            self.MT.recreate_all_selection_boxes()
-        self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
+                    txt = self.MT.get_valid_cell_data_as_str(rn, datacn, get_displayed = True)
+                    if txt:
+                        qconf(qtxtm, text = txt, font = qfont)
+                        b = qbbox(qtxtm)
+                        tw = b[2] - b[0] + qtxth + 7 if (rn, datacn) in qclop and 'dropdown' in qclop[(rn, datacn)] else b[2] - b[0] + 7
+                        if tw > w:
+                            w = tw
+            if w > hw:
+                new_width = w
+            else:
+                new_width = hw
+        else:
+            new_width = int(width)
+        if new_width <= self.MT.min_cw:
+            new_width = int(self.MT.min_cw)
+        elif new_width > self.max_cw:
+            new_width = int(self.max_cw)
+        if only_set_if_too_small:
+            if new_width <= self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
+                return self.MT.col_positions[col + 1] - self.MT.col_positions[col]
+        if not return_new_width:
+            new_col_pos = self.MT.col_positions[col] + new_width
+            increment = new_col_pos - self.MT.col_positions[col + 1]
+            self.MT.col_positions[col + 2:] = [e + increment for e in islice(self.MT.col_positions, col + 2, len(self.MT.col_positions))]
+            self.MT.col_positions[col + 1] = new_col_pos
+            if recreate:
+                self.MT.recreate_all_selection_boxes()
+        return new_width
 
-    def set_height_of_all_rows(self, height = None, only_set_if_too_small = False, recreate = True):
-        if height is None:
-            self.MT.row_positions = list(accumulate(chain([0], (self.set_row_height(rn, only_set_if_too_small = only_set_if_too_small, recreate = False, return_new_height = True) for rn in range(len(self.MT.data))))))
-        else:
-            self.MT.row_positions = list(accumulate(chain([0], (height for r in range(len(self.MT.data))))))
+    def set_width_of_all_cols(self, width = None, only_set_if_too_small = False, recreate = True):
+        if width is None:
+            if self.MT.all_columns_displayed:
+                iterable = range(self.MT.total_data_cols())
+            else:
+                iterable = range(len(self.MT.displayed_columns))
+            self.MT.col_positions = list(accumulate(chain([0], (self.set_col_width(cn, only_set_if_too_small = only_set_if_too_small, recreate = False, return_new_width = True) for cn in iterable))))
+        elif width is not None:
+            if self.MT.all_columns_displayed:
+                self.MT.col_positions = list(accumulate(chain([0], (width for cn in range(self.MT.total_data_cols())))))
+            else:
+                self.MT.col_positions = list(accumulate(chain([0], (width for cn in range(len(self.MT.displayed_columns))))))
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
-    def align_cells(self, rows = [], align = "global"):
-        if isinstance(rows, int):
-            rows = [rows]
+    def align_cells(self, columns = [], align = "global"):
+        if isinstance(columns, int):
+            cols = [columns]
         else:
-            rows = rows
+            cols = columns
         if align == "global":
-            for r in rows:
-                if r in self.cell_options and 'align' in self.cell_options[r]:
-                    del self.cell_options[r]['align']
-        else:
-            for r in rows:
-                if r not in self.cell_options:
-                    self.cell_options[r] = {}
-                self.cell_options[r]['align'] = align
-
-    def auto_set_index_width(self, end_row):
-        if not self.MT._row_index and not isinstance(self.MT._row_index, int) and self.auto_resize_width:
-            if self.default_index == "letters":
-                new_w = self.MT.GetTextWidth(f"{num2alpha(end_row)}") + 20
-                if self.current_width - new_w > 15 or new_w - self.current_width > 5:
-                    self.set_width(new_w, set_TL = True)
-                    return True
-            elif self.default_index == "numbers":
-                new_w = self.MT.GetTextWidth(f"{end_row}") + 20
-                if self.current_width - new_w > 15 or new_w - self.current_width > 5:
-                    self.set_width(new_w, set_TL = True)
-                    return True
-            elif self.default_index == "both":
-                new_w = self.MT.GetTextWidth(f"{end_row + 1} {num2alpha(end_row)}") + 20
-                if self.current_width - new_w > 15 or new_w - self.current_width > 5:
-                    self.set_width(new_w, set_TL = True)
-                    return True
-        return False
+            for c in cols:
+                if c in self.cell_options and 'align' in self.cell_options[c]:
+                    del self.cell_options[c]['align']
+        else:
+            for c in cols:
+                if c not in self.cell_options:
+                    self.cell_options[c] = {}
+                self.cell_options[c]['align'] = align
 
-    def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, hlrow):
+    def redraw_highlight_get_text_fg(self, fc, sc, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, hlcol):
         redrawn = False
-        if r in self.cell_options and 'highlight' in self.cell_options[r] and r in actual_selected_rows:
-            if self.cell_options[r]['highlight'][0] is not None:
-                c_1 = self.cell_options[r]['highlight'][0] if self.cell_options[r]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[r]['highlight'][0]]
-                redrawn = self.redraw_highlight(0,
-                                                fr + 1,
-                                                self.current_width - 1,
-                                                sr,
+        if hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol] and c in actual_selected_cols:
+            if self.cell_options[hlcol]['highlight'][0] is not None:
+                c_1 = self.cell_options[hlcol]['highlight'][0] if self.cell_options[hlcol]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[hlcol]['highlight'][0]]
+                redrawn = self.redraw_highlight(fc + 1,
+                                                0,
+                                                sc,
+                                                self.current_height - 1,
                                                 fill = (f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"),
-                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "",
-                                                tag = "s")
-            fill = self.index_selected_rows_fg if self.cell_options[r]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[r]['highlight'][1]
-        elif r in self.cell_options and 'highlight' in self.cell_options[r] and (r in selected_rows or selected_cols):
-            if self.cell_options[r]['highlight'][0] is not None:
-                c_1 = self.cell_options[r]['highlight'][0] if self.cell_options[r]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[r]['highlight'][0]]
-                redrawn = self.redraw_highlight(0,
-                                                fr + 1,
-                                                self.current_width - 1,
-                                                sr,
+                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "",
+                                                tag = "hi")
+            fill = self.header_selected_columns_fg if self.cell_options[hlcol]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[hlcol]['highlight'][1]
+        elif hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol] and (c in selected_cols or selected_rows):
+            if self.cell_options[hlcol]['highlight'][0] is not None:
+                c_1 = self.cell_options[hlcol]['highlight'][0] if self.cell_options[hlcol]['highlight'][0].startswith("#") else Color_Map_[self.cell_options[hlcol]['highlight'][0]]
+                redrawn = self.redraw_highlight(fc + 1,
+                                                0,
+                                                sc,
+                                                self.current_height - 1,
                                                 fill = (f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}" +
                                                         f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"),
-                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "",
-                                                tag = "s")
-            fill = self.index_selected_cells_fg if self.cell_options[r]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[r]['highlight'][1]
-        elif r in actual_selected_rows:
-            fill = self.index_selected_rows_fg
-        elif r in selected_rows or selected_cols:
-            fill = self.index_selected_cells_fg
-        elif r in self.cell_options and 'highlight' in self.cell_options[r]:
-            if self.cell_options[r]['highlight'][0] is not None:
-                redrawn = self.redraw_highlight(0, 
-                                                fr + 1, 
-                                                self.current_width - 1, 
-                                                sr,
-                                                fill = self.cell_options[r]['highlight'][0], 
-                                                outline = self.index_fg if hlrow in self.cell_options and 'dropdown' in self.cell_options[hlrow] and self.MT.show_dropdown_borders else "", 
-                                                tag = "s")
-            fill = self.index_fg if self.cell_options[r]['highlight'][1] is None else self.cell_options[r]['highlight'][1]
+                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "", 
+                                                tag = "hi")
+            fill = self.header_selected_cells_fg if self.cell_options[hlcol]['highlight'][1] is None or self.MT.display_selected_fg_over_highlights else self.cell_options[hlcol]['highlight'][1]
+        elif c in actual_selected_cols:
+            fill = self.header_selected_columns_fg
+        elif c in selected_cols or selected_rows:
+            fill = self.header_selected_cells_fg
+        elif hlcol in self.cell_options and 'highlight' in self.cell_options[hlcol]:
+            if self.cell_options[hlcol]['highlight'][0] is not None:
+                redrawn = self.redraw_highlight(fc + 1,
+                                                0, 
+                                                sc, 
+                                                self.current_height - 1, 
+                                                fill = self.cell_options[hlcol]['highlight'][0], 
+                                                outline = self.header_fg if hlcol in self.cell_options and 'dropdown' in self.cell_options[hlcol] and self.MT.show_dropdown_borders else "", 
+                                                tag = "hi")
+            fill = self.header_fg if self.cell_options[hlcol]['highlight'][1] is None else self.cell_options[hlcol]['highlight'][1]
         else:
-            fill = self.index_fg
+            fill = self.header_fg
         return fill, redrawn
-
+            
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
-        coords = (x1, y1, x2, y2)
+        coords = (x1 - 1 if outline else x1,
+                  y1 - 1 if outline else y1,
+                  x2, 
+                  y2)
         k = None
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
             if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
@@ -918,45 +859,45 @@
         
         if k is not None and not self.hidd_high[k]:
             del self.hidd_high[k]
 
         self.disp_high[config].add(DrawnItem(iid = iid, showing = 1))
         return True
 
-    def redraw_gridline(self, points, fill, width, tag):
+    def redraw_gridline(self,points, fill, width, tag):
         if self.hidd_grid:
             t, sh = self.hidd_grid.popitem()
             self.coords(t, points)
             if sh:
-                self.itemconfig(t, fill = fill, width = width, tag = tag)
+                self.itemconfig(t, fill = fill, width = width, tag = tag, capstyle = tk.BUTT, joinstyle = tk.ROUND)
             else:
-                self.itemconfig(t, fill = fill, width = width, tag = tag, state = "normal")
+                self.itemconfig(t, fill = fill, width = width, tag = tag, capstyle = tk.BUTT, joinstyle = tk.ROUND, state = "normal")
             self.disp_grid[t] = True
         else:
             self.disp_grid[self.create_line(points, fill = fill, width = width, tag = tag)] = True
             
     def redraw_dropdown(self, x1, y1, x2, y2, fill, outline, tag, draw_outline = True, draw_arrow = True, dd_is_open = False):
         if draw_outline and self.MT.show_dropdown_borders:
-            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.index_fg, tag = tag)
+            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill = "", outline = self.header_fg, tag = tag)
         if draw_arrow:
-            topysub = floor(self.MT.half_txt_h / 2)
-            mid_y = y1 + floor(self.MT.min_rh / 2)
-            if mid_y + topysub + 1 >= y1 + self.MT.txt_h - 1:
+            topysub = floor(self.MT.hdr_half_txt_h / 2)
+            mid_y = y1 + floor(self.MT.hdr_min_rh / 2)
+            if mid_y + topysub + 1 >= y1 + self.MT.hdr_txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
                 ty2 = mid_y - topysub + 3 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 3
             else:
                 ty1 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 2
                 ty2 = mid_y - topysub + 2 if dd_is_open else mid_y + topysub + 1
                 ty3 = mid_y + topysub + 1 if dd_is_open else mid_y - topysub + 2
-            tx1 = x2 - self.MT.txt_h + 1
-            tx2 = x2 - self.MT.half_txt_h - 1
+            tx1 = x2 - self.MT.hdr_txt_h + 1
+            tx2 = x2 - self.MT.hdr_half_txt_h - 1
             tx3 = x2 - 3
             if tx2 - tx1 > tx3 - tx2:
                 tx1 += (tx2 - tx1) - (tx3 - tx2)
             elif tx2 - tx1 < tx3 - tx2:
                 tx1 -= (tx3 - tx2) - (tx2 - tx1)
             points = (tx1, ty1, tx2, ty2, tx3, ty3)
             if self.hidd_dropdown:
@@ -967,15 +908,15 @@
                 else:
                     self.itemconfig(t, fill = fill, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_line(points, fill = fill, width = 2, capstyle = tk.ROUND, joinstyle = tk.ROUND, tag = tag)
             self.disp_dropdown[t] = True
             
-    def redraw_checkbox(self, r, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
+    def redraw_checkbox(self, datacn, x1, y1, x2, y2, fill, outline, tag, draw_check = False):
         points = self.MT.get_checkbox_points(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill = outline, outline = fill)
             else:
@@ -999,19 +940,22 @@
                 else:
                     self.itemconfig(t, fill = fill, outline = outline, tag = tag, state = "normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill = fill, outline = outline, tag = tag, smooth = True)
             self.disp_checkbox[t] = True
 
-    def redraw_grid_and_text(self, last_row_line_pos, scrollpos_top, y_stop, start_row, end_row, scrollpos_bot, selected_rows, selected_cols, actual_selected_rows):
-        self.configure(scrollregion = (0,
-                                       0,
-                                       self.current_width,
-                                       last_row_line_pos + self.MT.empty_vertical))
+    def redraw_grid_and_text(self, last_col_line_pos, scrollpos_left, x_stop, start_col, end_col, scrollpos_right, selected_cols, selected_rows, actual_selected_cols, col_pos_exists):
+        try:
+            self.configure(scrollregion = (0,
+                                           0,
+                                           last_col_line_pos + self.MT.empty_horizontal,
+                                           self.current_height))
+        except:
+            return
         for k, v in self.disp_text.items():
             if k in self.hidd_text:
                 self.hidd_text[k] = self.hidd_text[k] | self.disp_text[k]
             else:
                 self.hidd_text[k] = v
         self.disp_text = defaultdict(set)
         for k, v in self.disp_high.items():
@@ -1022,143 +966,128 @@
         self.disp_high = defaultdict(set)
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
         self.disp_dropdown = {}
         self.hidd_checkbox.update(self.disp_checkbox)
         self.disp_checkbox = {}
-        self.visible_row_dividers = {}
-        draw_y = self.MT.row_positions[start_row]
-        xend = self.current_width - 6
-        self.row_width_resize_bbox = (self.current_width - 2, scrollpos_top, self.current_width, scrollpos_bot)
-        if self.MT.show_horizontal_grid or self.height_resizing_enabled:
+        self.visible_col_dividers = {}
+        self.col_height_resize_bbox = (scrollpos_left, self.current_height - 2, x_stop, self.current_height)
+        draw_x = self.MT.col_positions[start_col]
+        yend = self.current_height - 5
+        if (self.MT.show_vertical_grid or self.width_resizing_enabled) and col_pos_exists:
             self.grid_cyc = cycle(self.grid_cyctup)
-            points = []
-            for r in range(start_row + 1, end_row):
-                draw_y = self.MT.row_positions[r]
-                if self.height_resizing_enabled:
-                    self.visible_row_dividers[r] = (1, draw_y - 2, xend, draw_y + 2)
+            points = [x_stop - 1, self.current_height - 1, 
+                      scrollpos_left - 1, self.current_height - 1,
+                      scrollpos_left - 1, -1]
+            for c in range(start_col + 1, end_col):
+                draw_x = self.MT.col_positions[c]
+                if self.width_resizing_enabled:
+                    self.visible_col_dividers[c] = (draw_x - 2, 1, draw_x + 2, yend)
                 st_or_end = next(self.grid_cyc)
                 if st_or_end == "st":
-                    points.extend([-1, draw_y,
-                                   self.current_width, draw_y,
-                                   self.current_width, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
+                    points.extend([draw_x, -1,
+                                   draw_x, self.current_height,
+                                   self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x, self.current_height])
                 elif st_or_end == "end":
-                    points.extend([self.current_width, draw_y,
-                                   -1, draw_y,
-                                   -1, self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y])
+                    points.extend([draw_x, self.current_height,
+                                   draw_x, -1,
+                                   self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x, -1])
                 if points:
-                    self.redraw_gridline(points = points, fill = self.index_grid_fg, width = 1, tag = "h")
-        self.redraw_gridline(points = (0, draw_y, self.current_width, draw_y), width = 1, fill = self.index_grid_fg, tag = "fh")
-        self.redraw_gridline(points = (self.current_width - 1, scrollpos_top, self.current_width - 1, y_stop), width = 1, fill = self.index_border_fg, tag = "v")
-        scrollpos_bot_add2 = scrollpos_bot + 2
-        c_2 = self.index_selected_cells_bg if self.index_selected_cells_bg.startswith("#") else Color_Map_[self.index_selected_cells_bg]
-        c_3 = self.index_selected_rows_bg if self.index_selected_rows_bg.startswith("#") else Color_Map_[self.index_selected_rows_bg]
-        font = self.MT._font
-        for r in range(start_row, end_row - 1):
-            rtopgridln = self.MT.row_positions[r]
-            rbotgridln = self.MT.row_positions[r + 1]
-            if rbotgridln - rtopgridln < self.MT.txt_h:
-                continue
-            if rbotgridln > scrollpos_bot_add2:
-                rbotgridln = scrollpos_bot_add2
-            if self.MT.all_rows_displayed:
-                drow = r
+                    self.redraw_gridline(points = points, fill = self.header_grid_fg, width = 1, tag = "v")
+        top = self.canvasy(0)
+        c_2 = self.header_selected_cells_bg if self.header_selected_cells_bg.startswith("#") else Color_Map_[self.header_selected_cells_bg]
+        c_3 = self.header_selected_columns_bg if self.header_selected_columns_bg.startswith("#") else Color_Map_[self.header_selected_columns_bg]
+        font = self.MT._hdr_font
+        for c in range(start_col, end_col - 1):
+            draw_y = self.MT.hdr_fl_ins
+            cleftgridln = self.MT.col_positions[c]
+            crightgridln = self.MT.col_positions[c + 1]
+            if self.MT.all_columns_displayed:
+                datacn = c
             else:
-                drow = self.MT.displayed_rows[r]
-            fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selected_rows, selected_cols, actual_selected_rows, drow)
-            
-            if r in self.cell_options and 'align' in self.cell_options[r]:
-                align = self.cell_options[r]['align']
+                datacn = self.MT.displayed_columns[c]
+            fill, dd_drawn = self.redraw_highlight_get_text_fg(cleftgridln, crightgridln, c, c_2, c_3, selected_cols, selected_rows, actual_selected_cols, datacn)
+
+            if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
+                align = self.cell_options[datacn]['align']
             else:
                 align = self.align
                 
             if align == "w":
-                draw_x = 3
-                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
-                    mw = self.current_width - self.MT.txt_h - 2
-                    self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
+                draw_x = cleftgridln + 3
+                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
+                    self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[datacn]['dropdown']['window'] != "no dropdown open")
                 else:
-                    mw = self.current_width - 2
+                    mw = crightgridln - cleftgridln - 1
 
             elif align == "e":
-                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
-                    mw = self.current_width - self.MT.txt_h - 2
-                    draw_x = self.current_width - 5 - self.MT.txt_h
-                    self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
+                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
+                    draw_x = crightgridln - 5 - self.MT.hdr_txt_h
+                    self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1,
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[datacn]['dropdown']['window'] != "no dropdown open")
                 else:
-                    mw = self.current_width - 2
-                    draw_x = self.current_width - 3
+                    mw = crightgridln - cleftgridln - 1
+                    draw_x = crightgridln - 3
 
             elif align == "center":
-                if r in self.cell_options and 'dropdown' in self.cell_options[r]:
-                    mw = self.current_width - self.MT.txt_h - 2
-                    draw_x = ceil((self.current_width - self.MT.txt_h) / 2)
-                    self.redraw_dropdown(0, rtopgridln, self.current_width - 1, rbotgridln - 1, 
+                #stop = cleftgridln + 5
+                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                    mw = crightgridln - cleftgridln - self.MT.hdr_txt_h - 2
+                    draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.MT.hdr_txt_h) / 2)
+                    self.redraw_dropdown(cleftgridln, 0, crightgridln, self.current_height - 1, 
                                          fill = fill, outline = fill, tag = "dd", draw_outline = not dd_drawn, draw_arrow = mw >= 5,
-                                         dd_is_open = self.cell_options[r]['dropdown']['window'] != "no dropdown open")
+                                         dd_is_open = self.cell_options[datacn]['dropdown']['window'] != "no dropdown open")
                 else:
-                    mw = self.current_width - 1
-                    draw_x = floor(self.current_width / 2)
+                    mw = crightgridln - cleftgridln - 1
+                    draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
 
-            if r in self.cell_options and 'checkbox' in self.cell_options[r]:
-                if mw > + 2:
-                    box_w = self.MT.txt_h + 1
+            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+                if mw > self.MT.hdr_txt_h + 2:
+                    box_w = self.MT.hdr_txt_h + 1
                     mw -= box_w
                     if align == "w":
                         draw_x += box_w + 1
                     elif align == "center":
                         draw_x += ceil(box_w / 2) + 1
                         mw -= 1
                     else:
                         mw -= 3
                     try:
-                        draw_check = self.MT._row_index[r] if isinstance(self.MT._row_index, (list, tuple)) else self.MT.data[r][self.MT._row_index]
+                        draw_check = self.MT._headers[datacn] if isinstance(self.MT._headers, (list, tuple)) else self.MT.data[self.MT._headers][datacn]
                     except:
                         draw_check = False
-                    self.redraw_checkbox(r,
+                    self.redraw_checkbox(datacn,
+                                         cleftgridln + 2,
                                          2,
-                                         rtopgridln + 2,
-                                         self.MT.txt_h + 3,
-                                         rtopgridln + self.MT.txt_h + 3,
-                                         fill = fill if self.cell_options[r]['checkbox']['state'] == "normal" else self.index_grid_fg,
+                                         cleftgridln + self.MT.hdr_txt_h + 3,
+                                         self.MT.hdr_txt_h + 3,
+                                         fill = fill if self.cell_options[datacn]['checkbox']['state'] == "normal" else self.header_grid_fg,
                                          outline = "",
-                                         tag = "cb",
+                                         tag = "cb", 
                                          draw_check = draw_check)
-
-            try:
-                if r in self.cell_options and 'checkbox' in self.cell_options[r]:
-                    lns = self.cell_options[r]['checkbox']['text'].split("\n") if isinstance(self.cell_options[r]['checkbox']['text'], str) else f"{self.cell_options[r]['checkbox']['text']}".split("\n")
-                elif isinstance(self.MT._row_index, int):
-                    lns = self.MT.data[r][self.MT._row_index].split("\n") if isinstance(self.MT.data[r][self.MT._row_index], str) else f"{self.MT.data[r][self.MT._row_index]}".split("\n")
-                else:
-                    lns = self.MT._row_index[r].split("\n") if isinstance(self.MT._row_index[r], str) else f"{self.MT._row_index[r]}".split("\n")
-                got_idx = True
-            except:
-                got_idx = False
-            if not got_idx or (lns == [""] and self.show_default_index_for_empty):
-                if self.default_index == "letters":
-                    lns = (num2alpha(r), )
-                elif self.default_index == "numbers":
-                    lns = (f"{r + 1}", )
+            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+                lns = self.cell_options[datacn]['checkbox']['text'].split("\n") if isinstance(self.cell_options[datacn]['checkbox']['text'], str) else f"{self.cell_options[datacn]['checkbox']['text']}".split("\n")
+            else:
+                lns = self.get_valid_cell_data_as_str(datacn, fix = False).split("\n")
+            if lns == [""]:
+                if self.show_default_header_for_empty:
+                    lns = (get_n2a(datacn, self.default_header), )
                 else:
-                    lns = (f"{r + 1} {num2alpha(r)}", )
-            draw_y = rtopgridln + self.MT.fl_ins
-            if mw > 5:
-                draw_y = rtopgridln + self.MT.fl_ins
-                start_ln = int((scrollpos_top - rtopgridln) / self.MT.xtra_lines_increment)
-                if start_ln < 0:
-                    start_ln = 0
-                draw_y += start_ln * self.MT.xtra_lines_increment
-                if draw_y + self.MT.half_txt_h - 1 <= rbotgridln and len(lns) > start_ln:
-                    for txt in islice(lns, start_ln, None):
+                    continue
+            if mw > self.MT.hdr_txt_w and not ((align == "w" and (draw_x > x_stop)) or
+                                               (align == "e" and (draw_x > x_stop)) or
+                                               (align == "center" and (cleftgridln + 5 > x_stop))):
+                for txt in islice(lns, self.lines_start_at if self.lines_start_at < len(lns) else len(lns) - 1, None):
+                    if draw_y > top:
                         config = TextCfg(txt, fill, font, align)
                         k = None
                         if config in self.hidd_text:
                             k = config
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
                             if (int(cc1) == int(draw_x) and
@@ -1185,271 +1114,264 @@
                             else:
                                 self.itemconfig(iid, text = txt, fill = fill, font = font, anchor = align, state = "normal")
                         if k is not None and not self.hidd_text[k]:
                             del self.hidd_text[k]
                         wd = self.bbox(iid)
                         wd = wd[2] - wd[0]
                         if wd > mw:
-                            if align == "w" and drow in self.cell_options and 'dropdown' in self.cell_options[drow]:
+                            if align == "w":
                                 txt = txt[:int(len(txt) * (mw / wd))]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[:-1]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
-                            elif align == "e" and drow in self.cell_options and 'checkbox' in self.cell_options[drow]:
+                            elif align == "e":
                                 txt = txt[len(txt) - int(len(txt) * (mw / wd)):]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[1:]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
-                            elif align == "center" and ((drow in self.cell_options and 'checkbox' in self.cell_options[drow]) or (drow in self.cell_options and 'dropdown' in self.cell_options[drow])):
+                            elif align == "center":
+                                self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
                                 tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
                                 txt = txt[tmod - 1:-tmod]
                                 self.itemconfig(iid, text = txt)
                                 wd = self.bbox(iid)
-                                self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[next(self.c_align_cyc)]
                                     self.itemconfig(iid, text = txt)
                                     wd = self.bbox(iid)
                                 self.coords(iid, draw_x, draw_y)
-                            self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = 1))
+                            self.disp_text[config._replace(txt = txt)].add(DrawnItem(iid = iid, showing = True))
                         else:
-                            self.disp_text[config].add(DrawnItem(iid = iid, showing = 1))
-                        draw_y += self.MT.xtra_lines_increment
-                        if draw_y + self.MT.half_txt_h - 1 > rbotgridln:
-                            break
+                            self.disp_text[config].add(DrawnItem(iid = iid, showing = True))
+                    draw_y += self.MT.hdr_xtra_lines_increment
+                    if draw_y - 1 > self.current_height:
+                        break
         self.tag_raise("t")
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
                     self.hidd_text[cfg].discard(namedtup)
-                    self.hidd_text[cfg].add(namedtup._replace(showing = 0))
+                    self.hidd_text[cfg].add(namedtup._replace(showing = False))
         for cfg, set_ in self.hidd_high.items():
             for namedtup in tuple(set_):
                 if namedtup.showing:
                     self.itemconfig(namedtup.iid, state = "hidden")
                     self.hidd_high[cfg].discard(namedtup)
-                    self.hidd_high[cfg].add(namedtup._replace(showing = 0))
+                    self.hidd_high[cfg].add(namedtup._replace(showing = False))
         for t, sh in self.hidd_grid.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_grid[t] = False
         for t, sh in self.hidd_dropdown.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_dropdown[t] = False
         for t, sh in self.hidd_checkbox.items():
             if sh:
                 self.itemconfig(t, state = "hidden")
                 self.hidd_checkbox[t] = False
                 
     def open_cell(self, event = None, ignore_existing_editor = False):
-        if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
+        if not self.MT.anything_selected()  or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
-        r = int(currently_selected[0])
-        drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if drow in self.cell_options and 'readonly' in self.cell_options[drow]:
+        x1 = int(currently_selected[1])
+        datacn = x1 if self.MT.all_columns_displayed else self.MT.displayed_columns[x1]
+        if datacn in self.cell_options and 'readonly' in self.cell_options[datacn]:
             return
-        elif drow in self.cell_options and ('dropdown' in self.cell_options[drow] or 'checkbox' in self.cell_options[drow]):
+        elif datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 'checkbox' in self.cell_options[datacn]):
             if self.MT.event_opens_dropdown_or_checkbox(event):
-                if 'dropdown' in self.cell_options[drow]:
-                    self.display_dropdown_window(r, event = event)
-                elif 'checkbox' in self.cell_options[drow]:
-                    self._click_checkbox(r, drow)
+                if 'dropdown' in self.cell_options[datacn]:
+                    self.open_dropdown_window(x1, event = event)
+                elif 'checkbox' in self.cell_options[datacn]:
+                    self._click_checkbox(x1, datacn)
         elif self.edit_cell_enabled:
-            self.edit_cell_(event, r = r, dropdown = False)
+            self.edit_cell_(event, c = x1, dropdown = False)
 
-    # r is displayed row
-    def edit_cell_(self, event = None, r = None, dropdown = False):
+    # c is displayed col
+    def edit_cell_(self, event = None, c = None, dropdown = False):
         text = None
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, 'keysym') and event.keysym == 'Return':
                     extra_func_key = "Return"
                 elif hasattr(event, 'keysym') and event.keysym == 'F2':
                     extra_func_key = "F2"
-            drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            if isinstance(self.MT._row_index, list):
-                if len(self.MT._row_index) <= drow:
-                    self.MT._row_index.extend(list(repeat("", drow - len(self.MT._row_index) + 1)))
-                text = f"{self.MT._row_index[drow]}"
-            elif isinstance(self.MT._row_index, int):
-                try:
-                    text = f"{self.MT.data[self.MT._row_index][drow]}"
-                except:
-                    text = ""
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+            text = self.get_cell_data(datacn, redirect_int = True)
         elif event is not None and ((hasattr(event, 'keysym') and event.keysym == 'BackSpace') or
-                                  event.keycode in (8, 855638143)
-                                  ):
+                                    event.keycode in (8, 855638143)):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and ((hasattr(event, "char") and event.char.isalpha()) or
                                     (hasattr(event, "char") and event.char.isdigit()) or
                                     (hasattr(event, "char") and event.char in symbols_set)):
             extra_func_key = event.char
             text = event.char
         else:
             return False
-        self.text_editor_loc = r
+        self.text_editor_loc = c
         if self.extra_begin_edit_cell_func is not None:
             try:
-                text = self.extra_begin_edit_cell_func(EditIndexEvent(r, extra_func_key, text, "begin_edit_index"))
+                text = self.extra_begin_edit_cell_func(EditHeaderEvent(c, extra_func_key, text, "begin_edit_header"))
             except:
                 return False
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
-            self.set_row_height_run_binding(r)
-        self.select_row(r = r, keep_other_selections = True, redraw = not dropdown)
-        self.create_text_editor(r = r, text = text, set_data_ref_on_destroy = True, dropdown = dropdown)
+            if self.height_resizing_enabled:
+                self.set_current_height_to_cell(datacn)
+            self.set_col_width_run_binding(c)
+        self.select_col(c = c, keep_other_selections = True)
+        self.create_text_editor(c = c, text = text, set_data_on_close = True, dropdown = dropdown)
         return True
     
     # displayed indexes
-    def get_cell_align(self, r):
-        drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if drow in self.cell_options and 'align' in self.cell_options[drow]:
-            align = self.cell_options[drow]['align']
+    def get_cell_align(self, c):
+        datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+        if datacn in self.cell_options and 'align' in self.cell_options[datacn]:
+            align = self.cell_options[datacn]['align']
         else:
             align = self.align
         return align
 
-    # r is displayed row
+    # c is displayed col
     def create_text_editor(self,
-                           r = 0,
+                           c = 0,
                            text = None,
                            state = "normal",
                            see = True,
-                           set_data_ref_on_destroy = False,
+                           set_data_on_close = False,
                            binding = None,
                            dropdown = False):
-        if r == self.text_editor_loc and self.text_editor is not None:
+        if c == self.text_editor_loc and self.text_editor is not None:
             self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
-            has_redrawn = self.MT.see(r = r, c = 0, keep_yscroll = True, check_cell_visibility = True)
+            has_redrawn = self.MT.see(r = 0, c = c, keep_yscroll = True, check_cell_visibility = True)
             if not has_redrawn:
                 self.MT.refresh()
-        self.text_editor_loc = r
-        x = 0
-        y = self.MT.row_positions[r] + 1
-        w = self.current_width + 1
-        h = self.MT.row_positions[r + 1] - y
-        drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+        self.text_editor_loc = c
+        x = self.MT.col_positions[c] + 1
+        y = 0
+        w = self.MT.col_positions[c + 1] - x
+        h = self.current_height + 1
+        datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         if text is None:
-            if isinstance(self.MT._row_index, list):
-                if len(self.MT._row_index) <= drow:
-                    self.MT._row_index.extend(list(repeat("", drow - len(self.MT._row_index) + 1)))
-                text = f"{self.MT._row_index[drow]}"
-            elif isinstance(self.MT._row_index, int):
-                try:
-                    text = f"{self.MT.data[self.MT._row_index][drow]}"
-                except:
-                    text = ""
-        #bg, fg = self.get_widget_bg_fg(drow)bg = 
-        bg, fg = self.index_bg, self.index_fg
+            text = self.get_valid_cell_data_as_str(datacn)
+        bg, fg = self.header_bg, self.header_fg
         self.text_editor = TextEditor(self,
                                       text = text,
-                                      font = self.MT._font,
+                                      font = self.MT._hdr_font,
                                       state = state,
                                       width = w,
                                       height = h,
                                       border_color = self.MT.table_selected_cells_border_fg,
                                       show_border = False,
                                       bg = bg,
                                       fg = fg,
                                       popup_menu_font = self.MT.popup_menu_font,
                                       popup_menu_fg = self.MT.popup_menu_fg,
                                       popup_menu_bg = self.MT.popup_menu_bg,
                                       popup_menu_highlight_bg = self.MT.popup_menu_highlight_bg,
                                       popup_menu_highlight_fg = self.MT.popup_menu_highlight_fg,
                                       binding = binding,
-                                      align = self.get_cell_align(r),
-                                      r = r,
-                                      newline_binding = self.text_editor_newline_binding)
+                                      align = self.get_cell_align(c),
+                                      c = c,
+                                      newline_binding = self.text_editor_has_wrapped)
         self.text_editor.update_idletasks()
         self.text_editor_id = self.create_window((x, y), window = self.text_editor, anchor = "nw")
         if not dropdown:
             self.text_editor.textedit.focus_set()
             self.text_editor.scroll_to_bottom()
-        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(r = r))
+        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(c = c))
         if USER_OS == 'darwin':
-            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(r = r))
+            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(c = c))
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.textedit.bind(key, func)
         if binding is not None:
-            self.text_editor.textedit.bind("<Tab>", lambda x: binding((r, "Tab")))
-            self.text_editor.textedit.bind("<Return>", lambda x: binding((r, "Return")))
-            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, "FocusOut")))
-            self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, "Escape")))
-        elif binding is None and set_data_ref_on_destroy:
-            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, "Tab")))
-            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, "Return")))
+            self.text_editor.textedit.bind("<Tab>", lambda x: binding((c, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: binding((c, "Return")))
+            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((c, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: binding((c, "Escape")))
+        elif binding is None and set_data_on_close:
+            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((c, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((c, "Return")))
             if not dropdown:
-                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, "FocusOut")))
-            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, "Escape")))
+                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((c, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((c, "Escape")))
         else:
             self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
-            
+    
+    # displayed indexes                             #just here to receive text editor arg
+    def text_editor_has_wrapped(self, r = 0, c = 0, check_lines = None):
+        if self.width_resizing_enabled:
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+            curr_width = self.text_editor.winfo_width()
+            new_width = curr_width + (self.MT.hdr_txt_h * 2)
+            if new_width != curr_width:
+                self.text_editor.config(width = new_width)
+                self.set_col_width_run_binding(c, width = new_width, only_set_if_too_small = False)
+                if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                    self.itemconfig(self.cell_options[datacn]['dropdown']['canvas_id'],
+                                    width = new_width)
+                    self.cell_options[datacn]['dropdown']['window'].update_idletasks()
+                    self.cell_options[datacn]['dropdown']['window']._reselect()
+                self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = True)
+    
+    # displayed indexes
     def text_editor_newline_binding(self, r = 0, c = 0, event = None, check_lines = True):
         if self.height_resizing_enabled:
-            drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             curr_height = self.text_editor.winfo_height()
-            if not check_lines or self.MT.GetLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
-                new_height = curr_height + self.MT.xtra_lines_increment
-                space_bot = self.MT.get_space_bot(r)
+            if not check_lines or self.MT.GetHdrLinesHeight(self.text_editor.get_num_lines() + 1) > curr_height:
+                new_height = curr_height + self.MT.hdr_xtra_lines_increment
+                space_bot = self.MT.get_space_bot(0)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
-                    self.set_row_height(drow, new_height)
-                    self.MT.refresh()
                     self.text_editor.config(height = new_height)
-                    if drow in self.cell_options and 'dropdown' in self.cell_options[drow]:
-                        text_editor_h = self.text_editor.winfo_height()
-                        win_h, anchor = self.get_dropdown_height_anchor(drow, text_editor_h)
-                        if anchor == "nw":
-                            self.coords(self.cell_options[drow]['dropdown']['canvas_id'],
-                                        self.MT.col_positions[c], self.MT.row_positions[r] + text_editor_h - 1)
-                            self.itemconfig(self.cell_options[drow]['dropdown']['canvas_id'],
-                                            anchor = anchor, height = win_h)
-                        elif anchor == "sw":
-                            self.coords(self.cell_options[drow]['dropdown']['canvas_id'],
-                                        self.MT.col_positions[c], self.MT.row_positions[r])
-                            self.itemconfig(self.cell_options[drow]['dropdown']['canvas_id'],
-                                            anchor = anchor, height = win_h)
+                    self.set_height(new_height, set_TL = True)
+                    if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+                        win_h, anchor = self.get_dropdown_height_anchor(datacn, new_height)
+                        self.coords(self.cell_options[datacn]['dropdown']['canvas_id'],
+                                    self.MT.col_positions[c], new_height - 1)
+                        self.itemconfig(self.cell_options[datacn]['dropdown']['canvas_id'],
+                                        anchor = anchor, height = win_h)
             
     def bind_cell_edit(self, enable = True):
         if enable:
             self.edit_cell_enabled = True
         else:
             self.edit_cell_enabled = False
 
-    def bind_text_editor_destroy(self, binding, r):
-        self.text_editor.textedit.bind("<Return>", lambda x: binding((r, "Return")))
-        self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, "FocusOut")))
-        self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, "Escape")))
+    def bind_text_editor_destroy(self, binding, c):
+        self.text_editor.textedit.bind("<Return>", lambda x: binding((c, "Return")))
+        self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((c, "FocusOut")))
+        self.text_editor.textedit.bind("<Escape>", lambda x: binding((c, "Escape")))
         self.text_editor.textedit.focus_set()
 
     def destroy_text_editor(self, event = None):
         if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
-            self.extra_end_edit_cell_func(EditHeaderEvent(int(self.text_editor_loc), "Escape", None, "escape_edit_index"))
+            self.extra_end_edit_cell_func(EditHeaderEvent(int(self.text_editor_loc), "Escape", None, "escape_edit_header"))
         self.text_editor_loc = None
         try:
             self.delete(self.text_editor_id)
         except:
             pass
         try:
             self.text_editor.destroy()
@@ -1462,280 +1384,388 @@
         try:
             self.text_editor_id = None
         except:
             pass
         if event is not None and len(event) >= 3 and "Escape" in event:
             self.focus_set()
 
-    # r is displayed row
-    def close_text_editor(self, editor_info = None, r = None, set_data_ref_on_destroy = True, event = None, destroy = True, move_down = True, redraw = True, recreate = True):
+    # c is displayed col
+    def close_text_editor(self, editor_info = None, c = None, set_data_on_close = True, event = None, destroy = True, move_down = True, redraw = True, recreate = True):
         if self.focus_get() is None and editor_info:
-            return "break"
+            return
         if editor_info is not None and len(editor_info) >= 2 and editor_info[1] == "Escape":
             self.destroy_text_editor("Escape")
-            self.hide_dropdown_window(r)
-            return "break"
+            self.close_dropdown_window(c)
+            return
         if self.text_editor is not None:
             self.text_editor_value = self.text_editor.get()
         if destroy:
             self.destroy_text_editor()
-        if set_data_ref_on_destroy:
-            if r is None and editor_info is not None and len(editor_info) >= 2:
-                r = editor_info[0]
-            if self.extra_end_edit_cell_func is None:
-                self._set_cell_data(r, drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r], value = self.text_editor_value)
-            elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation:
-                self._set_cell_data(r, drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r], value = self.text_editor_value)
-                self.extra_end_edit_cell_func(EditIndexEvent(r, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_index"))
+        if set_data_on_close:
+            if c is None and editor_info is not None and len(editor_info) >= 2:
+                c = editor_info[0]
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(datacn, self.text_editor_value):
+                self.set_cell_data_undo(c, datacn = datacn, value = self.text_editor_value, check_input_valid = False)
+            elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation and self.input_valid_for_cell(datacn, self.text_editor_value):
+                self.set_cell_data_undo(c, datacn = datacn, value = self.text_editor_value, check_input_valid = False)
+                self.extra_end_edit_cell_func(EditHeaderEvent(c, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_header"))
             elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
-                validation = self.extra_end_edit_cell_func(EditIndexEvent(r, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_index"))
+                validation = self.extra_end_edit_cell_func(EditHeaderEvent(c, editor_info[1] if len(editor_info) >= 2 else "FocusOut", f"{self.text_editor_value}", "end_edit_header"))
                 if validation is not None:
                     self.text_editor_value = validation
-                    self._set_cell_data(r, drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r], value = self.text_editor_value)
+                    if self.input_valid_for_cell(datacn, self.text_editor_value):
+                        self.set_cell_data_undo(c, datacn = datacn, value = self.text_editor_value, check_input_valid = False)
         if move_down:
             pass
-        self.hide_dropdown_window(r)
+        self.close_dropdown_window(c)
         if recreate:
             self.MT.recreate_all_selection_boxes()
         if redraw:
             self.MT.refresh()
         if editor_info is not None and len(editor_info) >= 2 and editor_info[1] != "FocusOut":
             self.focus_set()
         return "break"
-
+    
     #internal event use
-    def _set_cell_data(self, r = 0, drow = None, value = "", cell_resize = True, undo = True, redraw = True):
-        if drow is None:
-            drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if isinstance(self.MT._row_index, list):
-            if len(self.MT._row_index) <= drow:
-                self.MT._row_index.extend(list(repeat("", drow - len(self.MT._row_index) + 1)))
-            if self.MT.undo_enabled and undo:
-                if self.MT._row_index[drow] != value:
-                    self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_index",
-                                                                           {drow: self.MT._row_index[drow]},
-                                                                           (((r, 0, r + 1, len(self.MT.col_positions) - 1), "rows"), ),
-                                                                           self.MT.currently_selected()))))
-            self.MT._row_index[drow] = value
-        elif isinstance(self.MT._row_index, int):
-            self.MT._set_cell_data(r = r, c = self.MT._row_index, drow = drow, value = value, undo = True)
+    def set_cell_data_undo(self, c = 0, datacn = None, value = "", cell_resize = True, undo = True, redraw = True, check_input_valid = True):
+        if datacn is None:
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+        if isinstance(self.MT._headers, int):
+            self.MT.set_cell_data_undo(r = self.MT._headers, c = c, datacn = datacn, value = value, undo = True)
+        else:
+            self.fix_header(datacn)
+            if not check_input_valid or self.input_valid_for_cell(datacn, value):
+                if self.MT.undo_enabled and undo:
+                    self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_header",
+                                                                            {datacn: self.MT._headers[datacn]},
+                                                                            (((0, c, len(self.MT.row_positions) - 1, c + 1), "columns"), ),
+                                                                            self.MT.currently_selected()))))
+                self.set_cell_data(datacn = datacn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
-            self.set_row_height_run_binding(r, only_set_if_too_small = False)
+            if self.height_resizing_enabled:
+                self.set_current_height_to_cell(datacn)
+            self.set_col_width_run_binding(c)
         if redraw:
             self.MT.refresh()
+    
+    def set_cell_data(self, datacn = None, value = ""):
+        if isinstance(self.MT._headers, int):
+            self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = value)
+        else:
+            self.fix_header(datacn)
+            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+                self.MT._headers[datacn] = to_bool(value)
+            else:
+                self.MT._headers[datacn] = value
+    
+    def input_valid_for_cell(self, datacn, value):
+        if datacn in self.cell_options:
+            if 'readonly' in self.cell_options[datacn]:
+                return False
+            if 'checkbox' in self.cell_options[datacn]:
+                return is_bool_like(value)
+        if self.cell_equal_to(datacn, value):
+            return False
+        if (datacn in self.cell_options and 
+            'dropdown' in self.cell_options[datacn] and 
+            self.cell_options[datacn]['dropdown']['validate_input'] and 
+            value not in self.cell_options[datacn]['dropdown']['values']):
+            return False
         return True
+    
+    def cell_equal_to(self, datacn, value):
+        self.fix_header(datacn)
+        if isinstance(self.MT._headers, list):
+            if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+                try:
+                    return to_bool(self.MT._headers[datacn]) == to_bool(value)
+                except:
+                    return False
+            return self.MT._headers[datacn] == value
+        elif isinstance(self.MT._headers, int):
+            return self.MT.cell_equal_to(self.MT._headers, datacn, value)
             
-    def set_row_height_run_binding(self, r, only_set_if_too_small = True):
-        old_height = self.MT.row_positions[r + 1] - self.MT.row_positions[r]
-        new_height = self.set_row_height(r, only_set_if_too_small = only_set_if_too_small)
-        if self.row_height_resize_func is not None and old_height != new_height:
-            self.row_height_resize_func(ResizeEvent("row_height_resize", r, old_height, new_height))
+    def get_cell_data(self, datacn, get_displayed = False, redirect_int = False):
+        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None and get_displayed:
+            return self.cell_options[datacn]['dropdown']['text']
+        if redirect_int and isinstance(self.MT._headers, int):
+            return self.MT.get_cell_data(self.MT._headers, datacn, none_to_empty_str = True)
+        if isinstance(self.MT._headers, int) or not self.MT._headers or datacn >= len(self.MT._headers) or not self.MT._headers[datacn]:
+            if get_displayed and self.show_default_header_for_empty:
+                return get_n2a(datacn, self.default_header)
+            else:
+                return ""
+        return self.MT._headers[datacn]
+            
+    def get_valid_cell_data_as_str(self, datacn, fix = True) -> str:
+        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn] and self.cell_options[datacn]['dropdown']['text'] is not None:
+            return f"{self.cell_options[datacn]['dropdown']['text']}"
+        if isinstance(self.MT._headers, int):
+            return self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True)
+        if fix:
+            self.fix_header(datacn)
+        try:
+            return f"{self.MT._headers[datacn]}"
+        except:
+            return ""
+            
+    def fix_header(self, datacn = None):
+        if isinstance(self.MT._headers, int):
+            return
+        if isinstance(self.MT._headers, float):
+            self.MT._headers = int(self.MT._headers)
+            return
+        if not isinstance(self.MT._headers, list):
+            try:
+                self.MT._headers = list(self.MT._headers)
+            except:
+                self.MT._headers = []
+        if isinstance(datacn, int) and datacn >= len(self.MT._headers):
+            self.MT._headers.extend(list(repeat("", datacn - len(self.MT._headers) + 1)))
+    
+    # displayed indexes
+    def set_col_width_run_binding(self, c, width = None, only_set_if_too_small = True):
+        old_width = self.MT.col_positions[c + 1] - self.MT.col_positions[c]
+        new_width = self.set_col_width(c, width = width, only_set_if_too_small = only_set_if_too_small)
+        if self.column_width_resize_func is not None and old_width != new_width:
+            self.column_width_resize_func(ResizeEvent("column_width_resize", c, old_width, new_width))
 
     #internal event use
-    def _click_checkbox(self, r, drow = None, undo = True, redraw = True):
-        if drow is None:
-            drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if self.cell_options[drow]['checkbox']['state'] == "normal":
-            if isinstance(self.MT._row_index, list):
-                self._set_cell_data(r, drow = drow, value = not self.MT._row_index[drow] if type(self.MT._row_index[drow]) == bool else False, cell_resize = False)
-            elif isinstance(self.MT._row_index, int):
-                self._set_cell_data(r, drow = drow, value = not self.MT.data[self.MT._row_index][drow] if type(self.MT.data[self.MT._row_index][drow]) == bool else False, cell_resize = False)
-            if self.cell_options[drow]['checkbox']['check_function'] is not None:
-                self.cell_options[drow]['checkbox']['check_function']((r, 0, "IndexCheckboxClicked", f"{self.MT._row_index[drow] if isinstance(self.MT._row_index, list) else self.MT.data[self.MT._row_index][drow]}"))
+    def _click_checkbox(self, c, datacn = None, undo = True, redraw = True):
+        if datacn is None:
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+        if self.cell_options[datacn]['checkbox']['state'] == "normal":
+            if isinstance(self.MT._headers, list):
+                value = not self.MT._headers[datacn] if type(self.MT._headers[datacn]) == bool else False
+            elif isinstance(self.MT._headers, int):
+                value = not self.MT.data[self.MT._headers][datacn] if type(self.MT.data[self.MT._headers][datacn]) == bool else False
+            else:
+                value = False
+            self.set_cell_data_undo(c,
+                                    datacn = datacn, 
+                                    value = value, 
+                                    cell_resize = False)
+            if self.cell_options[datacn]['checkbox']['check_function'] is not None:
+                self.cell_options[datacn]['checkbox']['check_function']((0,
+                                                                         c, 
+                                                                         "HeaderCheckboxClicked", 
+                                                                         self.MT._headers[datacn] if isinstance(self.MT._headers, list) else self.MT.get_cell_data(self.MT._headers, datacn)))
             if self.extra_end_edit_cell_func is not None:
-                self.extra_end_edit_cell_func(EditIndexEvent(r, "Return", f"{self.MT._row_index[drow] if isinstance(self.MT._row_index, list) else self.MT.data[self.MT._row_index][drow]}", "end_edit_index"))
+                self.extra_end_edit_cell_func(EditHeaderEvent(c, 
+                                                              "Return",
+                                                              self.MT._headers[datacn] if isinstance(self.MT._headers, list) else self.MT.get_cell_data(self.MT._headers, datacn), 
+                                                              "end_edit_header"))
         if redraw:
             self.MT.refresh()
 
-    def create_checkbox(self, r = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
-        if r in self.cell_options and any(x in self.cell_options[r] for x in ('dropdown', 'checkbox')):
-            self.delete_dropdown_and_checkbox(r)
-        self._set_cell_data(drow = r, value = checked, cell_resize = False, undo = False) # only works because cell_resize and undo are false otherwise needs r arg
-        if r not in self.cell_options:
-            self.cell_options[r] = {}
-        self.cell_options[r]['checkbox'] = {'check_function': check_function,
-                                            'state': state,
-                                            'text': text}
+    def create_checkbox(self, datacn = 0, checked = False, state = "normal", redraw = False, check_function = None, text = ""):
+        if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 
+                                            'checkbox' in self.cell_options[datacn]):
+            self.delete_dropdown_and_checkbox(datacn)
+        self.set_cell_data(datacn = datacn,
+                            value = checked)
+        if datacn not in self.cell_options:
+            self.cell_options[datacn] = {}
+        self.cell_options[datacn]['checkbox'] = {'check_function': check_function,
+                                                 'state': state,
+                                                 'text': text}
         if redraw:
             self.MT.refresh()
 
-    def create_dropdown(self, r = 0, values = [], set_value = None, state = "readonly", redraw = True, selection_function = None, modified_function = None):
-        if r in self.cell_options and any(x in self.cell_options[r] for x in ('dropdown', 'checkbox')):
-            self.delete_dropdown_and_checkbox(r)
-        self._set_cell_data(drow = r, 
-                            value = set_value if set_value is not None else values[0] if values else "",
-                            cell_resize = False, 
-                            undo = False)
-        if r not in self.cell_options:
-            self.cell_options[r] = {}
-        self.cell_options[r]['dropdown'] = {'values': values,
-                                            'align': "w",
-                                            'window': "no dropdown open",
-                                            'canvas_id': "no dropdown open",
-                                            'select_function': selection_function,
-                                            'modified_function': modified_function,
-                                            'state': state}
+    def create_dropdown(self, 
+                        datacn = 0, 
+                        values = [], set_value = None, 
+                        state = "normal", redraw = True, 
+                        selection_function = None, modified_function = None,
+                        search_function = dropdown_search_function, validate_input = True, text = None):
+        if datacn in self.cell_options and ('dropdown' in self.cell_options[datacn] or 
+                                            'checkbox' in self.cell_options[datacn]):
+            self.delete_dropdown_and_checkbox(datacn)
+        self.set_cell_data(datacn = datacn, 
+                            value = set_value if set_value is not None else values[0] if values else "")
+        if datacn not in self.cell_options:
+            self.cell_options[datacn] = {}
+        self.cell_options[datacn]['dropdown'] = {'values': values,
+                                                 'window': "no dropdown open",
+                                                 'canvas_id': "no dropdown open",
+                                                 'select_function': selection_function,
+                                                 'modified_function': modified_function,
+                                                 'search_function': search_function,
+                                                 'validate_input': validate_input,
+                                                 'text': text,
+                                                 'state': state}
         if redraw:
             self.MT.refresh()
-            
-    def get_widget_bg_fg(self, r):
-        bg = self.index_bg
-        fg = self.index_fg
-        if r in self.cell_options and 'highlight' in self.cell_options[r]:
-            if self.cell_options[r]['highlight'][0] is not None:
-                bg = self.cell_options[r]['highlight'][0]
-            if self.cell_options[r]['highlight'][1] is not None:
-                fg = self.cell_options[r]['highlight'][1]
-        return bg, fg
-    
-    def get_dropdown_height_anchor(self, drow, text_editor_h = None):
+
+    def get_dropdown_height_anchor(self, datacn, text_editor_h = None):
         win_h = 5
-        for i, v in enumerate(self.cell_options[drow]['dropdown']['values']):
+        for i, v in enumerate(self.cell_options[datacn]['dropdown']['values']):
             v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
-                win_h += self.MT.fl_ins + (v_numlines * self.MT.xtra_lines_increment) + 5 # end of cell
+                win_h += self.MT.hdr_fl_ins + (v_numlines * self.MT.hdr_xtra_lines_increment) + 5 # end of cell
             else:
-                win_h += self.MT.min_rh
+                win_h += self.MT.hdr_min_rh
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.MT.get_space_bot(0, text_editor_h)
         win_h2 = int(win_h)
         if win_h > space_bot:
             win_h = space_bot - 1
-        if win_h < self.MT.txt_h + 5:
-            win_h = self.MT.txt_h + 5
+        if win_h < self.MT.hdr_txt_h + 5:
+            win_h = self.MT.hdr_txt_h + 5
         elif win_h > win_h2:
             win_h = win_h2
         return win_h, "nw"
-            
-    # r is displayed row
-    def display_dropdown_window(self, r, drow = None, event = None):
+
+    def set_current_height_to_cell(self, datacn):
+        x = self.MT.txt_measure_canvas.create_text(0,
+                                                   0,
+                                                   text = self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True) if isinstance(self.MT._headers, int) else self.MT._headers[datacn],
+                                                   font = self.MT._hdr_font)
+        b = self.MT.txt_measure_canvas.bbox(x)
+        self.MT.txt_measure_canvas.delete(x)
+        new_height = b[3] - b[1] + 5
+        space_bot = self.MT.get_space_bot(0)
+        if new_height > space_bot:
+            new_height = space_bot
+        self.set_height(new_height, set_TL = True)
+
+    def open_dropdown_window(self, c, datacn = None, event = None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
-        if drow is None:
-            drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-        if self.cell_options[drow]['dropdown']['state'] == "normal":
-            if not self.edit_cell_(r = r, dropdown = True, event = event):
+        if datacn is None:
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+        if self.cell_options[datacn]['dropdown']['state'] == "normal":
+            if not self.edit_cell_(c = c, dropdown = True, event = event):
                 return
-        win_h, anchor = self.get_dropdown_height_anchor(drow)
+        win_h, anchor = self.get_dropdown_height_anchor(datacn)
         window = self.MT.parentframe.dropdown_class(self.MT.winfo_toplevel(),
-                                                    r,
                                                     0,
-                                                    width = self.current_width,
+                                                    c,
+                                                    width = self.MT.col_positions[c + 1] - self.MT.col_positions[c] + 1,
                                                     height = win_h,
-                                                    font = self.MT._font,
+                                                    font = self.MT._hdr_font,
                                                     colors = {'bg': self.MT.popup_menu_bg, 
                                                               'fg': self.MT.popup_menu_fg, 
                                                               'highlight_bg': self.MT.popup_menu_highlight_bg,
                                                               'highlight_fg': self.MT.popup_menu_highlight_fg},
                                                     outline_color = self.MT.popup_menu_fg,
-                                                    values = self.cell_options[drow]['dropdown']['values'],
-                                                    hide_dropdown_window = self.hide_dropdown_window,
+                                                    values = self.cell_options[datacn]['dropdown']['values'],
+                                                    close_dropdown_window = self.close_dropdown_window,
+                                                    search_function = self.cell_options[datacn]['dropdown']['search_function'],
                                                     arrowkey_RIGHT = self.MT.arrowkey_RIGHT,
                                                     arrowkey_LEFT = self.MT.arrowkey_LEFT,
-                                                    align = self.cell_options[drow]['dropdown']['align'],
-                                                    single_index = "r")
-        ypos = self.MT.row_positions[r + 1]
-        self.cell_options[drow]['dropdown']['canvas_id'] = self.create_window((0, ypos),
-                                                                               window = window,
-                                                                               anchor = anchor)
-        if self.cell_options[drow]['dropdown']['state'] == "normal":
-            if self.cell_options[drow]['dropdown']['modified_function'] is not None:
-                self.text_editor.textedit.bind("<<TextModified>>", self.cell_options[drow]['dropdown']['modified_function'])
+                                                    align = "w",
+                                                    single_index = "c")
+        ypos = self.current_height - 1
+        self.cell_options[datacn]['dropdown']['canvas_id'] = self.create_window((self.MT.col_positions[c], ypos),
+                                                                                window = window,
+                                                                                anchor = anchor)
+        if self.cell_options[datacn]['dropdown']['state'] == "normal":
+            self.text_editor.textedit.bind("<<TextModified>>", 
+                                           lambda x: window.search_and_see(DropDownModifiedEvent("HeaderComboboxModified", 0, c, self.text_editor.get())))
+            if self.cell_options[datacn]['dropdown']['modified_function'] is not None:
+                window.modified_function = self.cell_options[datacn]['dropdown']['modified_function']
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
                 self.after(2, self.text_editor.scroll_to_bottom())
             except:
                 return
             redraw = False
         else:
-            window.bind("<FocusOut>", lambda x: self.hide_dropdown_window(r))
+            window.bind("<FocusOut>", lambda x: self.close_dropdown_window(c))
             self.update_idletasks()
             window.focus_set()
             redraw = True
         self.existing_dropdown_window = window
-        self.cell_options[drow]['dropdown']['window'] = window
-        self.existing_dropdown_canvas_id = self.cell_options[drow]['dropdown']['canvas_id']
+        self.cell_options[datacn]['dropdown']['window'] = window
+        self.existing_dropdown_canvas_id = self.cell_options[datacn]['dropdown']['canvas_id']
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(redraw_header = False, redraw_row_index = True, redraw_table = False)
-            
-    # r is displayed row
-    def hide_dropdown_window(self, r = None, selection = None, redraw = True):
-        if r is not None and selection is not None:
-            drow = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            if self.cell_options[drow]['dropdown']['select_function'] is not None: # user has specified a selection function
-                self.cell_options[drow]['dropdown']['select_function'](EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
+            self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = False, redraw_table = False)
+
+    def close_dropdown_window(self, c = None, selection = None, redraw = True):
+        if c is not None and selection is not None:
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+            if self.cell_options[datacn]['dropdown']['select_function'] is not None: # user has specified a selection function
+                self.cell_options[datacn]['dropdown']['select_function'](EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
             if self.extra_end_edit_cell_func is None:
-                self._set_cell_data(r, drow = drow, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(c, datacn = datacn, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
-                validation = self.extra_end_edit_cell_func(EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
+                validation = self.extra_end_edit_cell_func(EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
                 if validation is not None:
                     selection = validation
-                self._set_cell_data(r, drow = drow, value = selection, redraw = not redraw)
+                self.set_cell_data_undo(c, datacn = datacn, value = selection, redraw = not redraw)
             elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation:
-                self._set_cell_data(r, drow = drow, value = selection, redraw = not redraw)
-                self.extra_end_edit_cell_func(EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
+                self.set_cell_data_undo(c, datacn = datacn, value = selection, redraw = not redraw)
+                self.extra_end_edit_cell_func(EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"))
             self.focus_set()
             self.MT.recreate_all_selection_boxes()
         self.destroy_text_editor("Escape")
-        self.destroy_opened_dropdown_window(r)
+        self.destroy_opened_dropdown_window(c)
         if redraw:
             self.MT.refresh()
+            
+    def get_existing_dropdown_coords(self):
+        if self.existing_dropdown_window is not None:
+            return int(self.existing_dropdown_window.c)
+        return None
         
     def mouseclick_outside_editor_or_dropdown(self):
-        if self.existing_dropdown_window is not None:
-            closed_dd_coords = int(self.existing_dropdown_window.r)
-        else:
-            closed_dd_coords = None
+        closed_dd_coords = self.get_existing_dropdown_coords()
         if self.text_editor_loc is not None and self.text_editor is not None:
             self.close_text_editor(editor_info = (self.text_editor_loc, "ButtonPress-1"))
         else:
             self.destroy_text_editor("Escape")
-        if closed_dd_coords:
+        if closed_dd_coords is not None:
             self.destroy_opened_dropdown_window(closed_dd_coords) #displayed coords not data, necessary for b1 function
         return closed_dd_coords
+    
+    def mouseclick_outside_editor_or_dropdown_all_canvases(self):
+        self.RI.mouseclick_outside_editor_or_dropdown()
+        self.MT.mouseclick_outside_editor_or_dropdown()
+        return self.mouseclick_outside_editor_or_dropdown()
             
-    # r is displayed row, function can have two None args
-    def destroy_opened_dropdown_window(self, r = None, drow = None):
-        if r is not None or drow is not None:
-            if drow is None:
-                drow_ = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
+    # function can receive two None args
+    def destroy_opened_dropdown_window(self, c = None, datacn = None):
+        if c is None and datacn is None and self.existing_dropdown_window is not None:
+            c = self.get_existing_dropdown_coords()
+        if c is not None or datacn is not None:
+            if datacn is None:
+                datacn_ = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             else:
-                drow_ = r
+                datacn_ = datacn
         else:
-            drow_ = None
+            datacn_ = None
         try:
             self.delete(self.existing_dropdown_canvas_id)
         except:
             pass
         self.existing_dropdown_canvas_id = None
         try:
             self.existing_dropdown_window.destroy()
         except:
             pass
-        self.existing_dropdown_window = None
-        if drow_ in self.cell_options and 'dropdown' in self.cell_options[drow_]:
-            self.cell_options[drow_]['dropdown']['canvas_id'] = "no dropdown open"
-            self.cell_options[drow_]['dropdown']['window'] = "no dropdown open"
+        if datacn_ in self.cell_options and 'dropdown' in self.cell_options[datacn_]:
+            self.cell_options[datacn_]['dropdown']['canvas_id'] = "no dropdown open"
+            self.cell_options[datacn_]['dropdown']['window'] = "no dropdown open"
             try:
-                self.delete(self.cell_options[drow_]['dropdown']['canvas_id'])
+                self.delete(self.cell_options[datacn_]['dropdown']['canvas_id'])
             except:
                 pass
-            
-    # r is drow
-    def delete_dropdown(self, r):
-        self.destroy_opened_dropdown_window(drow = r)
-        if r in self.cell_options and 'dropdown' in self.cell_options[r]:
-            del self.cell_options[r]['dropdown']
-            
-    # r is drow
-    def delete_checkbox(self, r):
-        if r in self.cell_options and 'checkbox' in self.cell_options[r]:
-            del self.cell_options[r]['checkbox']
-
-    # r is drow
-    def delete_dropdown_and_checkbox(self, r):
-        self.delete_dropdown(r)
-        self.delete_checkbox(r)
+        self.existing_dropdown_window = None
+
+    def delete_dropdown(self, datacn):
+        self.destroy_opened_dropdown_window(datacn = datacn)
+        if datacn in self.cell_options and 'dropdown' in self.cell_options[datacn]:
+            del self.cell_options[datacn]['dropdown']
+
+    def delete_checkbox(self, datacn):
+        if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
+            del self.cell_options[datacn]['checkbox']
+
+    def delete_dropdown_and_checkbox(self, datacn):
+        self.delete_dropdown(datacn)
+        self.delete_checkbox(datacn)
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.0.0/tksheet/_tksheet_top_left_rectangle.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         self.extra_b1_motion_func = None
         self.extra_b1_release_func = None
         self.extra_double_b1_func = None
         self.extra_rc_func = None
         self.MT.TL = self
         self.RI.TL = self
         self.CH.TL = self
-        w = self.RI.current_width - 1
-        h = self.CH.current_height - 1
+        w = self.RI.current_width
+        h = self.CH.current_height
         self.create_rectangle(0, h - 5, w, h, fill = self.top_left_fg, outline = "", tag = "rw", state = "normal" if self.RI.width_resizing_enabled else "hidden")
         self.create_rectangle(w - 5, 0, w, h, fill = self.top_left_fg, outline = "", tag = "rh", state = "normal" if self.CH.height_resizing_enabled else "hidden")
         self.tag_bind("rw", "<Enter>", self.rw_enter)
         self.tag_bind("rh", "<Enter>", self.rh_enter)
         self.tag_bind("rw", "<Leave>", self.rw_leave)
         self.tag_bind("rh", "<Leave>", self.rh_leave)
         self.bind("<Motion>", self.mouse_motion)
@@ -82,20 +82,20 @@
             self.unbind("<Double-Button-1>")
             self.unbind(get_rc_binding())
 
     def set_dimensions(self, new_w = None, new_h = None):
         try:
             if new_w:
                 self.config(width = new_w)
-                w = new_w - 1
-                h = self.winfo_height() - 1
+                w = new_w
+                h = self.winfo_height()
             if new_h:
                 self.config(height = new_h)
-                w = self.winfo_width() - 1
-                h = new_h - 1
+                w = self.winfo_width()
+                h = new_h
         except:
             return
         self.coords("rw", 0, h - 5, w, h)
         self.coords("rh", w - 5, 0, w, h)
         self.MT.recreate_all_selection_boxes()
 
     def mouse_motion(self, event = None):
```

### Comparing `tksheet-5.6.8/tksheet/_tksheet_vars.py` & `tksheet-6.0.0/tksheet/_tksheet_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # for mac bindings
 from platform import system as get_os
-USER_OS = f"{get_os()}".lower()
 
+USER_OS = f"{get_os()}".lower()
 ctrl_key = "Command" if USER_OS == "darwin" else "Control"
 symbols_set = set("""!#\$%&'()*+,-./:;"@[]^_`{|}~>?= """)
+nonelike = {None, 'none', ''}
+truthy = {True, "true", "t", "yes", "y", "on", "1", 1, 1.0}
+falsy = {False, "false", "f", "no", "n", "off", "0", 0, 0.0}
+
+arrowkey_bindings_helper = {"tab": "Tab",
+                            "up": "Up",
+                            "right": "Right",
+                            "left": "Left",
+                            "down": "Down",
+                            "prior": "Prior",
+                            "next": "Next"}
 
 def get_font():
     return ("Calibri", 13 if USER_OS == "darwin" else 11, "normal")
 
 def get_index_font():
     return ('Calibri', 13 if USER_OS == "darwin" else 11, "normal")
 
 def get_heading_font():
     return ("Calibri", 13 if USER_OS == "darwin" else 11, "normal")
 
-def is_iterable(o):
-    try:
-        for e in o:
-            break
-        return True
-    except:
-        return False
-
 theme_light_blue = {
 'popup_menu_fg': "#000000",
 'popup_menu_bg': "#FFFFFF",
 'popup_menu_highlight_bg': "#DCDEE0",
 'popup_menu_highlight_fg': "#000000",
 'index_hidden_rows_expander_bg': "#747775",
 'header_hidden_columns_expander_bg': "#747775",
@@ -104,98 +107,98 @@
 'table_selected_rows_bg': "#E3E3E3",
 'table_selected_rows_fg': "black",
 'table_selected_columns_border_fg': "#217346",
 'table_selected_columns_bg': "#E3E3E3",
 'table_selected_columns_fg': "black"
 }
 
-theme_black = {
+theme_dark = {
 'popup_menu_fg': "white",
 'popup_menu_bg': "gray15",
-'popup_menu_highlight_bg': "gray35",
+'popup_menu_highlight_bg': "gray40",
 'popup_menu_highlight_fg': "white",
 'index_hidden_rows_expander_bg': "gray30",
 'header_hidden_columns_expander_bg': "gray30",
-'header_bg': "#000000",
+'header_bg': "#141414",
 'header_border_fg': "#505054",
 'header_grid_fg': "#8C8C8C",
-'header_fg': "#FBB86C",
+'header_fg': "gray70",
 'header_selected_cells_bg': "#545454",
-'header_selected_cells_fg': "#FBB86C",
-'index_bg': "#000000",
+'header_selected_cells_fg': "#6aa2fc",
+'index_bg': "#141414",
 'index_border_fg': "#505054",
 'index_grid_fg': "#8C8C8C",
-'index_fg': "#FBB86C",
+'index_fg': "gray70",
 'index_selected_cells_bg': "#545454",
-'index_selected_cells_fg': "#FBB86C",
-'top_left_bg': "#000000",
+'index_selected_cells_fg': "#6aa2fc",
+'top_left_bg': "#141414",
 'top_left_fg': "#505054",
-'top_left_fg_highlight': "#FBB86C",
+'top_left_fg_highlight': "white",
 'table_bg': "#000000",
-'table_grid_fg': "#505054",
-'table_fg': "#F2F2F2",
-'table_selected_cells_border_fg': "#FBB86C",
-'table_selected_cells_bg': "#333333",
-'table_selected_cells_fg': "#FFFFFF",
+'table_grid_fg': "#595959",
+'table_fg': "#E3E3E3",
+'table_selected_cells_border_fg': "#6aa2fc",
+'table_selected_cells_bg': "#404040",
+'table_selected_cells_fg': "#F7F7F7",
 'resizing_line_fg': "white",
 'drag_and_drop_bg': "#ecf0f2",
 'outline_color': "gray95",
-'header_selected_columns_bg': "#FBB86C",
-'header_selected_columns_fg': "#000000",
-'index_selected_rows_bg': "#FBB86C",
-'index_selected_rows_fg': "#000000",
-'table_selected_rows_border_fg': "#FBB86C",
-'table_selected_rows_bg': "#333333",
-'table_selected_rows_fg': "#FFFFFF",
-'table_selected_columns_border_fg': "#FBB86C",
-'table_selected_columns_bg': "#333333",
-'table_selected_columns_fg': "#FFFFFF"
+'header_selected_columns_bg': "#4489F7",
+'header_selected_columns_fg': "white",
+'index_selected_rows_bg': "#4489F7",
+'index_selected_rows_fg': "white",
+'table_selected_rows_border_fg': "#4489F7",
+'table_selected_rows_bg': "#404040",
+'table_selected_rows_fg': "#F7F7F7",
+'table_selected_columns_border_fg': "#4489F7",
+'table_selected_columns_bg': "#404040",
+'table_selected_columns_fg': "#F7F7F7"
 }
 
-theme_dark = {
+theme_black = {
 'popup_menu_fg': "white",
 'popup_menu_bg': "gray15",
-'popup_menu_highlight_bg': "gray35",
+'popup_menu_highlight_bg': "gray40",
 'popup_menu_highlight_fg': "white",
 'index_hidden_rows_expander_bg': "gray30",
 'header_hidden_columns_expander_bg': "gray30",
-'header_bg': "#141414",
+'header_bg': "#000000",
 'header_border_fg': "#505054",
 'header_grid_fg': "#8C8C8C",
-'header_fg': "gray70",
+'header_fg': "#FBB86C",
 'header_selected_cells_bg': "#545454",
-'header_selected_cells_fg': "#6aa2fc",
-'index_bg': "#141414",
+'header_selected_cells_fg': "#FBB86C",
+'index_bg': "#000000",
 'index_border_fg': "#505054",
 'index_grid_fg': "#8C8C8C",
-'index_fg': "gray70",
+'index_fg': "#FBB86C",
 'index_selected_cells_bg': "#545454",
-'index_selected_cells_fg': "#6aa2fc",
-'top_left_bg': "#323232",
+'index_selected_cells_fg': "#FBB86C",
+'top_left_bg': "#000000",
 'top_left_fg': "#505054",
-'top_left_fg_highlight': "white",
-'table_bg': "#323232",
-'table_grid_fg': "#505054",
-'table_fg': "#F2F2F2",
-'table_selected_cells_border_fg': "#6aa2fc",
-'table_selected_cells_bg': "#141414",
-'table_selected_cells_fg': "#fafafa",
+'top_left_fg_highlight': "#FBB86C",
+'table_bg': "#000000",
+'table_grid_fg': "#595959",
+'table_fg': "#E3E3E3",
+'table_selected_cells_border_fg': "#FBB86C",
+'table_selected_cells_bg': "#404040",
+'table_selected_cells_fg': "#F7F7F7",
 'resizing_line_fg': "white",
 'drag_and_drop_bg': "#ecf0f2",
 'outline_color': "gray95",
-'header_selected_columns_bg': "#4489F7",
-'header_selected_columns_fg': "white",
-'index_selected_rows_bg': "#4489F7",
-'index_selected_rows_fg': "white",
-'table_selected_rows_border_fg': "#4489F7",
-'table_selected_rows_bg': "#141414",
-'table_selected_rows_fg': "#fafafa",
-'table_selected_columns_border_fg': "#4489F7",
-'table_selected_columns_bg': "#141414",
-'table_selected_columns_fg': "#fafafa"
+'header_selected_columns_bg': "#FBB86C",
+'header_selected_columns_fg': "#000000",
+'index_selected_rows_bg': "#FBB86C",
+'index_selected_rows_fg': "#000000",
+'table_selected_rows_border_fg': "#FBB86C",
+'table_selected_rows_bg': "#404040",
+'table_selected_rows_fg': "#F7F7F7",
+'table_selected_columns_border_fg': "#FBB86C",
+'table_selected_columns_bg': "#404040",
+'table_selected_columns_fg': "#F7F7F7"
 }
 
 theme_dark_blue = theme_black.copy()
 theme_dark_blue['header_fg'] = "#6ACAD8"
 theme_dark_blue['header_selected_cells_fg'] = "#6ACAD8"
 theme_dark_blue['index_fg'] = "#6ACAD8"
 theme_dark_blue['index_selected_cells_fg'] = "#6ACAD8"
```

### Comparing `tksheet-5.6.8/tksheet.egg-info/PKG-INFO` & `tksheet-6.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 5.6.8
+Version: 6.0.0
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/5.6.8.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.0.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# tksheet [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
+# **tksheet** [![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.6+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt) [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
+## **Python tkinter table widget**
 
-Python tkinter table widget
+----
 
-```
+```python
+#To install using pip
 pip install tksheet
-```
-```
+
+#To update using pip
 pip install tksheet --upgrade
 ```
 
-### Help
- - [Documentation](https://github.com/ragardner/tksheet/wiki)
- - [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-
-### Features
- - Display and modify tabular data
- - Stores its display data as a Python list of lists, sublists being rows
- - Runs smoothly even with millions of rows/columns
- - Edit cells directly
- - Drag and drop columns and rows
- - Multiple line headers and rows
- - Expand row heights and column widths
- - Change fonts and font size
- - Change any colors in the sheet
- - Create an unlimited number of high performance dropdown and check boxes
- - Left `"w"`, Center `"center"` or Right `"e"` text alignment
- - Cell values can be any class with a `str` method
+## **Help**
+----
+- [Documentation](https://github.com/ragardner/tksheet/wiki)
+- [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
+- [Questions](https://github.com/ragardner/tksheet/wiki#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki#contributing).
+
+## **Features**
+----
+- Display and modify tabular data
+- Stores its display data as a Python list of lists, sublists being rows
+- Runs smoothly even with millions of rows/columns
+- Edit cells directly
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
+- Drag and drop columns and rows
+- Multiple line header and index cells
+- Expand row heights and column widths
+- Change fonts and font size (not for individual cells)
+- Change any colors in the sheet
+- Create an unlimited number of high performance dropdown and check boxes
+- Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
-### Light Blue Theme
+### **light blue theme**
+----
 
 ![alt text](https://i.imgur.com/ojU3IQi.jpeg)
 
-### Dark Theme
+### **black theme**
+----
 
 ![alt text](https://i.imgur.com/JeF9vJe.jpeg)
```

