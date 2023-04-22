# Comparing `tmp/myodan-tools-0.0.2.tar.gz` & `tmp/myodan-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myodan-tools-0.0.2.tar", max compression
+gzip compressed data, was "myodan-tools-0.0.3.tar", max compression
```

## Comparing `myodan-tools-0.0.2.tar` & `myodan-tools-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       14 2023-04-22 09:57:29.778905 myodan-tools-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/__init__.py
--rw-r--r--   0        0        0       52 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/__main__.py
--rw-r--r--   0        0        0     2140 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc
--rw-r--r--   0        0        0     2450 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/downloader/mediafire.py
--rw-r--r--   0        0        0      836 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc
--rw-r--r--   0        0        0      722 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/extractor/mrcong.py
--rw-r--r--   0        0        0      745 2023-04-22 10:23:38.005444 myodan-tools-0.0.2/myodan_tools/main.py
--rw-r--r--   0        0        0      729 2023-04-22 10:31:46.940894 myodan-tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1026 2023-04-22 10:31:57.706540 myodan-tools-0.0.2/setup.py
--rw-r--r--   0        0        0      737 2023-04-22 10:31:57.707053 myodan-tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-04-22 09:57:29.778905 myodan-tools-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 10:23:38.005444 myodan-tools-0.0.3/myodan_tools/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-22 10:23:38.005444 myodan-tools-0.0.3/myodan_tools/__main__.py
+-rw-r--r--   0        0        0      154 2023-04-22 10:36:15.532631 myodan-tools-0.0.3/myodan_tools/downloader/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2199 2023-04-22 10:36:15.532631 myodan-tools-0.0.3/myodan_tools/downloader/__pycache__/mediafire.cpython-310.pyc
+-rw-r--r--   0        0        0     2450 2023-04-22 10:23:38.005444 myodan-tools-0.0.3/myodan_tools/downloader/mediafire.py
+-rw-r--r--   0        0        0      153 2023-04-22 10:36:15.756631 myodan-tools-0.0.3/myodan_tools/extractor/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      854 2023-04-22 10:36:15.760631 myodan-tools-0.0.3/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc
+-rw-r--r--   0        0        0      722 2023-04-22 10:23:38.005444 myodan-tools-0.0.3/myodan_tools/extractor/mrcong.py
+-rw-r--r--   0        0        0      747 2023-04-22 10:36:13.044634 myodan-tools-0.0.3/myodan_tools/main.py
+-rw-r--r--   0        0        0      729 2023-04-22 10:36:50.212598 myodan-tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-04-22 10:37:04.146681 myodan-tools-0.0.3/setup.py
+-rw-r--r--   0        0        0      737 2023-04-22 10:37:04.147096 myodan-tools-0.0.3/PKG-INFO
```

### Comparing `myodan-tools-0.0.2/myodan_tools/downloader/mediafire.py` & `myodan-tools-0.0.3/myodan_tools/downloader/mediafire.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.2/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc` & `myodan-tools-0.0.3/myodan_tools/extractor/__pycache__/mrcong.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 17 14:40:33 2023 UTC, .py size: 660 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 615a 3d64 9402 0000  o.......aZ=d....
+00000000: 6f0d 0d0a 0000 0000 aab5 4364 d202 0000  o.........Cd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6503 6602 6404 6405 8404 5a04  ..d.e.f.d.d...Z.
 00000050: 6403 6503 6602 6406 6407 8404 5a05 6401  d.e.f.d.d...Z.d.
 00000060: 5300 2908 e900 0000 004e 2901 da0d 4265  S.)......N)...Be
 00000070: 6175 7469 6675 6c53 6f75 70da 0775 726c  autifulSoup..url
@@ -16,38 +16,39 @@
 000000f0: 6408 8302 7d04 7c02 7c04 a006 6409 a101  d...}.|.|...d...
 00000100: 3700 7d02 7105 290a 4e72 0100 0000 54e9  7.}.q.).Nr....T.
 00000110: 0100 0000 7a06 2f70 6167 652f 6994 0100  ....z./page/i...
 00000120: 00e9 c800 0000 da03 6572 72da 046c 786d  ........err..lxm
 00000130: 6c7a 252e 706f 7374 2d62 6f78 2d74 6974  lz%.post-box-tit
 00000140: 6c65 2061 5b68 7265 662a 3d22 6d72 636f  le a[href*="mrco
 00000150: 6e67 2e63 6f6d 225d 2907 da08 7265 7175  ng.com"])...requ
-00000160: 6573 7473 da03 6765 745a 0b73 7461 7475  ests..getZ.statu
+00000160: 6573 7473 da03 6765 74da 0b73 7461 7475  ests..get..statu
 00000170: 735f 636f 6465 da05 7072 696e 7472 0200  s_code..printr..
 00000180: 0000 da04 7465 7874 da06 7365 6c65 6374  ....text..select
 00000190: 2905 7203 0000 005a 0c63 7572 7265 6e74  ).r....Z.current
 000001a0: 5f70 6167 65da 056c 696e 6b73 da04 7061  _page..links..pa
-000001b0: 6765 da02 6273 a900 7210 0000 00fa 2d2f  ge..bs..r.....-/
+000001b0: 6765 da02 6273 a900 7211 0000 00fa 3a2f  ge..bs..r.....:/
 000001c0: 686f 6d65 2f72 756e 6e65 722f 6d79 6f64  home/runner/myod
-000001d0: 616e 2d74 6f6f 6c73 2f65 7874 7261 6374  an-tools/extract
-000001e0: 6f72 2f6d 7263 6f6e 672e 7079 da0d 6578  or/mrcong.py..ex
-000001f0: 7472 6163 745f 706f 7374 7305 0000 0073  tract_posts....s
-00000200: 1a00 0000 0401 0401 0202 0801 1401 0a02  ................
-00000210: 0201 0408 0afa 0801 0c02 0e01 02f5 7212  ..............r.
-00000220: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000230: 0400 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
-00000240: 0074 00a0 017c 00a1 017d 0174 027c 016a  .t...|...}.t.|.j
-00000250: 0364 0183 027d 027c 02a0 0464 02a1 017d  .d...}.|...d...}
-00000260: 037c 0353 0029 034e 7207 0000 007a 1861  .|.S.).Nr....z.a
-00000270: 5b68 7265 662a 3d22 6d65 6469 6166 6972  [href*="mediafir
-00000280: 652e 636f 6d22 5d29 0572 0800 0000 7209  e.com"]).r....r.
-00000290: 0000 0072 0200 0000 720b 0000 0072 0c00  ...r....r....r..
-000002a0: 0000 2904 7203 0000 0072 0e00 0000 720f  ..).r....r....r.
-000002b0: 0000 0072 0d00 0000 7210 0000 0072 1000  ...r....r....r..
-000002c0: 0000 7211 0000 00da 1665 7874 7261 6374  ..r......extract
-000002d0: 5f64 6f77 6e6c 6f61 645f 6c69 6e6b 7319  _download_links.
-000002e0: 0000 0073 0800 0000 0a01 0c01 0a01 0402  ...s............
-000002f0: 7213 0000 0029 0672 0800 0000 5a03 6273  r....).r....Z.bs
-00000300: 3472 0200 0000 da03 7374 7272 1200 0000  4r......strr....
-00000310: 7213 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000320: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-00000330: 6c65 3e01 0000 0073 0800 0000 0800 0c01  le>....s........
-00000340: 0e03 1214                                ....
+000001d0: 616e 2d74 6f6f 6c73 2f6d 796f 6461 6e5f  an-tools/myodan_
+000001e0: 746f 6f6c 732f 6578 7472 6163 746f 722f  tools/extractor/
+000001f0: 6d72 636f 6e67 2e70 79da 1265 7874 7261  mrcong.py..extra
+00000200: 6374 5f70 6f73 745f 6c69 6e6b 7307 0000  ct_post_links...
+00000210: 0073 1a00 0000 0401 0401 0202 0801 1401  .s..............
+00000220: 0a02 0201 0408 0afa 0801 0c02 0e01 02f5  ................
+00000230: 7213 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000240: 0000 0400 0000 0300 0000 4300 0000 7324  ..........C...s$
+00000250: 0000 0074 00a0 017c 00a1 017d 0174 027c  ...t...|...}.t.|
+00000260: 016a 0364 0183 027d 027c 02a0 0464 02a1  .j.d...}.|...d..
+00000270: 017d 037c 0353 0029 034e 7207 0000 007a  .}.|.S.).Nr....z
+00000280: 1861 5b68 7265 662a 3d22 6d65 6469 6166  .a[href*="mediaf
+00000290: 6972 652e 636f 6d22 5d29 0572 0800 0000  ire.com"]).r....
+000002a0: 7209 0000 0072 0200 0000 720c 0000 0072  r....r....r....r
+000002b0: 0d00 0000 2904 7203 0000 0072 0f00 0000  ....).r....r....
+000002c0: 7210 0000 0072 0e00 0000 7211 0000 0072  r....r....r....r
+000002d0: 1100 0000 7212 0000 00da 1665 7874 7261  ....r......extra
+000002e0: 6374 5f64 6f77 6e6c 6f61 645f 6c69 6e6b  ct_download_link
+000002f0: 731b 0000 0073 0800 0000 0a01 0c01 0a01  s....s..........
+00000300: 0402 7214 0000 0029 0672 0800 0000 5a03  ..r....).r....Z.
+00000310: 6273 3472 0200 0000 da03 7374 7272 1300  bs4r......strr..
+00000320: 0000 7214 0000 0072 1100 0000 7211 0000  ..r....r....r...
+00000330: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
+00000340: 6475 6c65 3e01 0000 0073 0800 0000 0800  dule>....s......
+00000350: 0c01 0e05 1214                           ......
```

### Comparing `myodan-tools-0.0.2/myodan_tools/extractor/mrcong.py` & `myodan-tools-0.0.3/myodan_tools/extractor/mrcong.py`

 * *Files identical despite different names*

### Comparing `myodan-tools-0.0.2/myodan_tools/main.py` & `myodan-tools-0.0.3/myodan_tools/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from urllib.parse import urlparse
 import typer
 
-from extractor import mrcong
-from downloader import mediafire
+from .downloader import mediafire
+from .extractor import mrcong
 
 app = typer.Typer()
 
 
 @app.callback()
 def callback(url_str: str):
     url = urlparse(url_str)
```

### Comparing `myodan-tools-0.0.2/pyproject.toml` & `myodan-tools-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "myodan-tools"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Jongho Hong <myodan@pm.me>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
-myodan-tools = "myodan_tools.main:app"
+myodan-tools = "myodan-tools.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.11"
 numpy = "^1.22.2"
 replit = "^3.2.4"
 Flask = "^2.2.0"
 urllib3 = "^1.26.12"
```

### Comparing `myodan-tools-0.0.2/setup.py` & `myodan-tools-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,19 +17,19 @@
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.2,<3.0.0',
  'six>=1.16.0,<2.0.0',
  'typer[all]>=0.7.0,<0.8.0',
  'urllib3>=1.26.12,<2.0.0']
 
 entry_points = \
-{'console_scripts': ['myodan-tools = myodan_tools.main:app']}
+{'console_scripts': ['myodan-tools = myodan-tools.main:app']}
 
 setup_kwargs = {
     'name': 'myodan-tools',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': '# myodan-tools',
     'author': 'Jongho Hong',
     'author_email': 'myodan@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `myodan-tools-0.0.2/PKG-INFO` & `myodan-tools-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myodan-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Jongho Hong
 Author-email: myodan@pm.me
 Requires-Python: >=3.10.0,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Flask (>=2.2.0,<3.0.0)
```

