# Comparing `tmp/pysparkplus-0.0.1.tar.gz` & `tmp/pysparkplus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkplus-0.0.1.tar", max compression
+gzip compressed data, was "pysparkplus-0.0.2.tar", max compression
```

## Comparing `pysparkplus-0.0.1.tar` & `pysparkplus-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-22 10:34:16.168105 pysparkplus-0.0.1/LICENSE
--rw-r--r--   0        0        0     2685 2023-04-22 11:07:37.937923 pysparkplus-0.0.1/README.md
--rw-r--r--   0        0        0     1025 2023-04-22 10:55:59.157979 pysparkplus-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-22 10:34:16.188105 pysparkplus-0.0.1/pysparkplus/__init__.py
--rw-r--r--   0        0        0     3066 2023-04-22 10:34:16.188105 pysparkplus-0.0.1/pysparkplus/dataframe.py
--rw-r--r--   0        0        0       28 2023-04-22 10:34:16.188105 pysparkplus-0.0.1/pysparkplus/main.py
--rw-r--r--   0        0        0     3405 1970-01-01 00:00:00.000000 pysparkplus-0.0.1/setup.py
--rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 pysparkplus-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-22 10:34:16.168105 pysparkplus-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2485 2023-04-22 13:12:53.607243 pysparkplus-0.0.2/README.md
+-rw-r--r--   0        0        0     1044 2023-04-22 13:13:32.717240 pysparkplus-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-22 10:34:16.188105 pysparkplus-0.0.2/pysparkplus/__init__.py
+-rw-r--r--   0        0        0     3554 2023-04-22 13:08:34.067266 pysparkplus-0.0.2/pysparkplus/functions.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pysparkplus-0.0.2/setup.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 pysparkplus-0.0.2/PKG-INFO
```

### Comparing `pysparkplus-0.0.1/LICENSE` & `pysparkplus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysparkplus-0.0.1/README.md` & `pysparkplus-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,14 @@
 <br>
 
 
 <br>
 
 ### Development on go!
 
-<a href="https://github.com/wiseupdata/wiseupdata">
-<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pysparkplus/main/assets/imgs/under_construction.gif" width="200" />
 
 <br>
 
 # References 🌍 🗄️
 
 1. [Pyspark+](https://wiseupdata.github.io/pysparkplus/index.html)
 1. [Wise Up Data](https://github.com/wiseupdata)
```

#### html2text {}

```diff
@@ -22,14 +22,14 @@
 
 
 
 * [Documentation and examples! ](https://wiseupdata.github.io/pysparkplus/
 index.html)!
 
 
-### Development on go! [img]_
-#_References_ð_ðï¸_1._[Pyspark+](https://wiseupdata.github.io/
-pysparkplus/index.html)_1._[Wise_Up_Data](https://github.com/wiseupdata)_1._
-[Emojis](https://github.com/wiseupdata/emojis)_
+### Development on go!
+# References ð ðï¸ 1. [Pyspark+](https://wiseupdata.github.io/
+pysparkplus/index.html) 1. [Wise Up Data](https://github.com/wiseupdata) 1.
+[Emojis](https://github.com/wiseupdata/emojis)
 
----_####_Maintainer_ð¤_ð¨âð»_Sivio_Liborio_ð§
-silvio.liborio@wiseupdata.com_silvio-de-melo-liborio_[LinkedIN]_
+--- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
+silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
```

### Comparing `pysparkplus-0.0.1/pyproject.toml` & `pysparkplus-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkplus"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["wiseupdata <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 packages = [{include = "pysparkplus"}]
 
 description = "Pyspark extra functions!"
 
 classifiers = [
@@ -17,14 +17,15 @@
 "Homepage" = "https://github.com/wiseupdata/pysparkplus"
 "Bug Tracker" = "https://github.com/wiseupdata/pysparkplus/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyspark = "^3.4.0"
+strplus = "^1.0.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 mkdocs = "^1.4.2"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mkdocs-gen-files = "^0.4.0"
```

### Comparing `pysparkplus-0.0.1/setup.py` & `pysparkplus-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['pysparkplus']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyspark>=3.4.0,<4.0.0']
+['pyspark>=3.4.0,<4.0.0', 'strplus>=1.0.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysparkplus',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Pyspark extra functions!',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/pysparkplus)\n[![pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://pypi.python.org/pypi/pysparkplus)\n[![downloads](https://pepy.tech/badge/pysparkplus/month)](https://pepy.tech/project/pysparkplus)\n[![versions](https://img.shields.io/pypi/pyversions/pysparkplus.svg)](https://github.com/wiseupdata/pysparkplus)\n\n---\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pysparkplus/main/assets/imgs/pyspark.png" width="300" />\n</a>\n\n<h1>\nPyspark extra functions ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/pysparkplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n</a>\n\n<br>\n<br>\n<br>\n\n* [Documentation and examples! ](https://wiseupdata.github.io/pysparkplus/index.html)! \n<br>\n<br>\n\n\n<br>\n\n### Development on go!\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pysparkplus/main/assets/imgs/under_construction.gif" width="200" />\n\n<br>\n\n# References 🌍 🗄️\n\n1. [Pyspark+](https://wiseupdata.github.io/pysparkplus/index.html)\n1. [Wise Up Data](https://github.com/wiseupdata)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n\n<br><br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/pysparkplus)\n[![pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://pypi.python.org/pypi/pysparkplus)\n[![downloads](https://pepy.tech/badge/pysparkplus/month)](https://pepy.tech/project/pysparkplus)\n[![versions](https://img.shields.io/pypi/pyversions/pysparkplus.svg)](https://github.com/wiseupdata/pysparkplus)\n\n---\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pysparkplus/main/assets/imgs/pyspark.png" width="300" />\n</a>\n\n<h1>\nPyspark extra functions ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/pysparkplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n</a>\n\n<br>\n<br>\n<br>\n\n* [Documentation and examples! ](https://wiseupdata.github.io/pysparkplus/index.html)! \n<br>\n<br>\n\n\n<br>\n\n### Development on go!\n\n\n<br>\n\n# References 🌍 🗄️\n\n1. [Pyspark+](https://wiseupdata.github.io/pysparkplus/index.html)\n1. [Wise Up Data](https://github.com/wiseupdata)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n\n<br><br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n',
     'author': 'wiseupdata',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['pysparkplus'] package_data = \ {'': ['*']} install_requires = \
-['pyspark>=3.4.0,<4.0.0'] setup_kwargs = { 'name': 'pysparkplus', 'version':
-'0.0.1', 'description': 'Pyspark extra functions!', 'long_description': '\n_
-[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s_Discord]\n\n\n_[wise_Up
-Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n![visitors](https://
-visitor-badge.glitch.me/
+['pyspark>=3.4.0,<4.0.0', 'strplus>=1.0.6,<2.0.0'] setup_kwargs = { 'name':
+'pysparkplus', 'version': '0.0.2', 'description': 'Pyspark extra functions!',
+'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
+Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
+[visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/pysparkplus)\n[!
 [pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://
 pypi.python.org/pypi/pysparkplus)\n[![downloads](https://pepy.tech/badge/
 pysparkplus/month)](https://pepy.tech/project/pysparkplus)\n[![versions](https:
 //img.shields.io/pypi/pyversions/pysparkplus.svg)](https://github.com/
 wiseupdata/pysparkplus)\n\n---\n\n\n[img]\n\n\n
@@ -29,18 +29,18 @@
 \n\n
 \n
 \n
 \n\n* [Documentation and examples! ](https://wiseupdata.github.io/pysparkplus/
 index.html)! \n
 \n
 \n\n\n
-\n\n### Development on go!\n\n\n[img]\n\n
-\n\n#_References_ð_ðï¸\n\n1._[Pyspark+](https://wiseupdata.github.io/
-pysparkplus/index.html)\n1._[Wise_Up_Data](https://github.com/wiseupdata)\n1._
+\n\n### Development on go!\n\n\n
+\n\n# References ð ðï¸\n\n1. [Pyspark+](https://wiseupdata.github.io/
+pysparkplus/index.html)\n1. [Wise Up Data](https://github.com/wiseupdata)\n1.
 [Emojis](https://github.com/wiseupdata/emojis)\n\n
 
-\n---\n\n####_Maintainer_ð¤_ð¨\u200dð»\n\nSivio_Liborio\n\nð§
+\n---\n\n#### Maintainer ð¤ ð¨\u200dð»\n\nSivio Liborio\n\nð§
 silvio.liborio@wiseupdata.com\n\nsilvio-de-melo-liborio_[LinkedIN]\n\n',
-'author':_'wiseupdata',_'author_email':_'silvio.liborio@wiseupdata.com',
-'maintainer':_'None',_'maintainer_email':_'None',_'url':_'None',_'packages':
-packages,_'package_data':_package_data,_'install_requires':_install_requires,
-'python_requires':_'>=3.9,<4.0',_}_setup(**setup_kwargs)_
+'author': 'wiseupdata', 'author_email': 'silvio.liborio@wiseupdata.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
+packages, 'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `pysparkplus-0.0.1/PKG-INFO` & `pysparkplus-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pysparkplus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pyspark extra functions!
 Author: wiseupdata
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pyspark (>=3.4.0,<4.0.0)
+Requires-Dist: strplus (>=1.0.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/wiseupdata/wiseupdata">
   <img align="left" alt="Wise Up Data's Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   
 </a> 
 <a href="https://github.com/wiseupdata/wiseupdata">
   <img align="left" alt="wise Up Data's Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />
@@ -75,16 +76,14 @@
 <br>
 
 
 <br>
 
 ### Development on go!
 
-<a href="https://github.com/wiseupdata/wiseupdata">
-<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pysparkplus/main/assets/imgs/under_construction.gif" width="200" />
 
 <br>
 
 # References 🌍 🗄️
 
 1. [Pyspark+](https://wiseupdata.github.io/pysparkplus/index.html)
 1. [Wise Up Data](https://github.com/wiseupdata)
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: pysparkplus Version: 0.0.1 Summary: Pyspark extra
+Metadata-Version: 2.1 Name: pysparkplus Version: 0.0.2 Summary: Pyspark extra
 functions! Author: wiseupdata Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 Requires-Dist:
-pyspark (>=3.4.0,<4.0.0) Description-Content-Type: text/markdown [Wise_Up
-Data's_Instagram] [wise_Up_Data's_Discord] [wise_Up_Data_|_Twitter] [wise_Up
-Data's_LinkedIN] ![visitors](https://visitor-badge.glitch.me/
+pyspark (>=3.4.0,<4.0.0) Requires-Dist: strplus (>=1.0.6,<2.0.0) Description-
+Content-Type: text/markdown [Wise_Up_Data's_Instagram] [wise_Up_Data's_Discord]
+[wise_Up_Data_|_Twitter] [wise_Up_Data's_LinkedIN] ![visitors](https://visitor-
+badge.glitch.me/
 badge?page_id=wiseupdata.pysparkplus&left_color=green&right_color=black) !
 [license](https://img.shields.io/github/license/wiseupdata/pysparkplus) [!
 [pypi](https://img.shields.io/pypi/v/pysparkplus?color=green)](https://
 pypi.python.org/pypi/pysparkplus) [![downloads](https://pepy.tech/badge/
 pysparkplus/month)](https://pepy.tech/project/pysparkplus) [![versions](https:/
 /img.shields.io/pypi/pyversions/pysparkplus.svg)](https://github.com/
 wiseupdata/pysparkplus) --- [img]
@@ -30,14 +31,14 @@
 
 
 
 * [Documentation and examples! ](https://wiseupdata.github.io/pysparkplus/
 index.html)!
 
 
-### Development on go! [img]_
-#_References_ð_ðï¸_1._[Pyspark+](https://wiseupdata.github.io/
-pysparkplus/index.html)_1._[Wise_Up_Data](https://github.com/wiseupdata)_1._
-[Emojis](https://github.com/wiseupdata/emojis)_
+### Development on go!
+# References ð ðï¸ 1. [Pyspark+](https://wiseupdata.github.io/
+pysparkplus/index.html) 1. [Wise Up Data](https://github.com/wiseupdata) 1.
+[Emojis](https://github.com/wiseupdata/emojis)
 
----_####_Maintainer_ð¤_ð¨âð»_Sivio_Liborio_ð§
-silvio.liborio@wiseupdata.com_silvio-de-melo-liborio_[LinkedIN]_
+--- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
+silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
```

