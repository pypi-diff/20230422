# Comparing `tmp/ifunnygifmaker-0.2.1.tar.gz` & `tmp/ifunnygifmaker-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifunnygifmaker-0.2.1.tar", last modified: Sat Apr 22 19:06:49 2023, max compression
+gzip compressed data, was "ifunnygifmaker-0.2.2.tar", last modified: Sat Apr 22 19:16:45 2023, max compression
```

## Comparing `ifunnygifmaker-0.2.1.tar` & `ifunnygifmaker-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.2.1/README.md
--rw-r--r--   0        0        0     6148 2023-04-21 04:24:08.705576 ifunnygifmaker-0.2.1/ifunnygifmaker/.DS_Store
--rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.2.1/ifunnygifmaker/__init__.py
--rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.2.1/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
--rw-r--r--   0        0        0     4952 2023-04-22 19:05:06.047762 ifunnygifmaker-0.2.1/ifunnygifmaker/mememaker.py
--rw-r--r--   0        0        0      459 2023-04-22 19:06:25.214391 ifunnygifmaker-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-04-17 15:21:16.673815 ifunnygifmaker-0.2.2/README.md
+-rw-r--r--   0        0        0     6148 2023-04-21 04:24:08.705576 ifunnygifmaker-0.2.2/ifunnygifmaker/.DS_Store
+-rw-r--r--   0        0        0       39 2023-04-20 03:35:46.032714 ifunnygifmaker-0.2.2/ifunnygifmaker/__init__.py
+-rw-r--r--   0        0        0    25492 2020-05-28 04:55:50.000000 ifunnygifmaker-0.2.2/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf
+-rw-r--r--   0        0        0     4935 2023-04-22 19:16:27.890457 ifunnygifmaker-0.2.2/ifunnygifmaker/mememaker.py
+-rw-r--r--   0        0        0      459 2023-04-22 19:16:38.456853 ifunnygifmaker-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 ifunnygifmaker-0.2.2/PKG-INFO
```

### Comparing `ifunnygifmaker-0.2.1/ifunnygifmaker/.DS_Store` & `ifunnygifmaker-0.2.2/ifunnygifmaker/.DS_Store`

 * *Files identical despite different names*

### Comparing `ifunnygifmaker-0.2.1/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf` & `ifunnygifmaker-0.2.2/ifunnygifmaker/fonts/Futura Condensed Extra Bold.otf`

 * *Files identical despite different names*

### Comparing `ifunnygifmaker-0.2.1/ifunnygifmaker/mememaker.py` & `ifunnygifmaker-0.2.2/ifunnygifmaker/mememaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 font = ImageFont.truetype(font_path, 15)
 
                 # Get the size of the text
                 text_size = draw.textsize(text, font=font)
 
                 # Calculate the position for the text
                 text_y = ((padding_size - 50) - text_size[1]) // 2
-                wrap = new_im.width * 0.05
+                wrap = 40
                 size = self.__calculate_fontsize(
                     text=text,
                     rect_len=padding_size,
                     rect_width=new_im.width,
                     wrap=wrap,
                     font_name=font_path,
                 )
```

