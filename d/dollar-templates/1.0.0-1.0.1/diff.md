# Comparing `tmp/dollar_templates-1.0.0.tar.gz` & `tmp/dollar_templates-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dollar_templates-1.0.0.tar", last modified: Sat Apr 22 19:25:14 2023, max compression
+gzip compressed data, was "dollar_templates-1.0.1.tar", last modified: Sat Apr 22 20:30:51 2023, max compression
```

## Comparing `dollar_templates-1.0.0.tar` & `dollar_templates-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-04-22 19:25:14.674970 dollar_templates-1.0.0/
--rw-r--r--   0 frank     (1000) frank     (1000)     3222 2023-04-22 19:25:14.674970 dollar_templates-1.0.0/PKG-INFO
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-04-22 19:25:14.666971 dollar_templates-1.0.0/dollar_templates/
--rw-r--r--   0 frank     (1000) frank     (1000)      583 2023-04-22 05:20:20.000000 dollar_templates-1.0.0/dollar_templates/__init__.py
--rw-r--r--   0 frank     (1000) frank     (1000)     2142 2023-04-22 05:25:53.000000 dollar_templates-1.0.0/dollar_templates/parser.py
--rw-r--r--   0 frank     (1000) frank     (1000)     2825 2023-04-22 19:00:07.000000 dollar_templates-1.0.0/dollar_templates/syntax.py
--rw-r--r--   0 frank     (1000) frank     (1000)     1763 2023-04-22 16:29:32.000000 dollar_templates-1.0.0/dollar_templates/tokenizer.py
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-04-22 19:25:14.670971 dollar_templates-1.0.0/dollar_templates.egg-info/
--rw-r--r--   0 frank     (1000) frank     (1000)     3222 2023-04-22 19:25:14.000000 dollar_templates-1.0.0/dollar_templates.egg-info/PKG-INFO
--rw-r--r--   0 frank     (1000) frank     (1000)      281 2023-04-22 19:25:14.000000 dollar_templates-1.0.0/dollar_templates.egg-info/SOURCES.txt
--rw-r--r--   0 frank     (1000) frank     (1000)        1 2023-04-22 19:25:14.000000 dollar_templates-1.0.0/dollar_templates.egg-info/dependency_links.txt
--rw-r--r--   0 frank     (1000) frank     (1000)       17 2023-04-22 19:25:14.000000 dollar_templates-1.0.0/dollar_templates.egg-info/top_level.txt
--rw-r--r--   0 frank     (1000) frank     (1000)       38 2023-04-22 19:25:14.674970 dollar_templates-1.0.0/setup.cfg
--rw-r--r--   0 frank     (1000) frank     (1000)      778 2023-04-22 19:24:25.000000 dollar_templates-1.0.0/setup.py
+drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-04-22 20:30:51.108695 dollar_templates-1.0.1/
+-rw-r--r--   0 frank     (1000) frank     (1000)     3222 2023-04-22 20:30:51.108695 dollar_templates-1.0.1/PKG-INFO
+drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-04-22 20:30:51.096694 dollar_templates-1.0.1/dollar_templates/
+-rw-r--r--   0 frank     (1000) frank     (1000)      583 2023-04-22 05:20:20.000000 dollar_templates-1.0.1/dollar_templates/__init__.py
+-rw-r--r--   0 frank     (1000) frank     (1000)     2130 2023-04-22 20:25:25.000000 dollar_templates-1.0.1/dollar_templates/parser.py
+-rw-r--r--   0 frank     (1000) frank     (1000)     2825 2023-04-22 19:00:07.000000 dollar_templates-1.0.1/dollar_templates/syntax.py
+-rw-r--r--   0 frank     (1000) frank     (1000)     1763 2023-04-22 16:29:32.000000 dollar_templates-1.0.1/dollar_templates/tokenizer.py
+drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-04-22 20:30:51.104695 dollar_templates-1.0.1/dollar_templates.egg-info/
+-rw-r--r--   0 frank     (1000) frank     (1000)     3222 2023-04-22 20:30:51.000000 dollar_templates-1.0.1/dollar_templates.egg-info/PKG-INFO
+-rw-r--r--   0 frank     (1000) frank     (1000)      281 2023-04-22 20:30:51.000000 dollar_templates-1.0.1/dollar_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 frank     (1000) frank     (1000)        1 2023-04-22 20:30:51.000000 dollar_templates-1.0.1/dollar_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 frank     (1000) frank     (1000)       17 2023-04-22 20:30:51.000000 dollar_templates-1.0.1/dollar_templates.egg-info/top_level.txt
+-rw-r--r--   0 frank     (1000) frank     (1000)       38 2023-04-22 20:30:51.108695 dollar_templates-1.0.1/setup.cfg
+-rw-r--r--   0 frank     (1000) frank     (1000)      778 2023-04-22 20:29:49.000000 dollar_templates-1.0.1/setup.py
```

### Comparing `dollar_templates-1.0.0/PKG-INFO` & `dollar_templates-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dollar_templates
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pandoc style dollar templates for python
 Home-page: https://github.com/seifferth/dollar_templates
 Author: Frank Seifferth
 Author-email: frankseifferth@posteo.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `dollar_templates-1.0.0/dollar_templates/__init__.py` & `dollar_templates-1.0.1/dollar_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `dollar_templates-1.0.0/dollar_templates/parser.py` & `dollar_templates-1.0.1/dollar_templates/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     if end == 'else':
         elsetree, end = __parse(l, endtokens=['endif'])
     elif end.startswith('elseif('):
         assert end[:4] == 'else'
         l.insert(0, MetaToken(end[4:]))
         elsetree, _ = __parse(l, endtokens=['endif'])
     else:
-        elsetree = Str(PlainToken(''))
+        elsetree = Str('')
     return If(condition, thentree, elsetree)
 def __parse_for(tokens: list[Token]) -> For:
     l = tokens
     assert l[0].content[:4] == "for(" and l[0].content[-1:] == ")"
     it = l.pop(0).content[4:-1]
     main, end = __parse(l, endtokens=['sep', 'endfor'])
     sep = __parse(l, endtokens=['endfor'])[0] if end == 'sep' else None
```

### Comparing `dollar_templates-1.0.0/dollar_templates/syntax.py` & `dollar_templates-1.0.1/dollar_templates/syntax.py`

 * *Files identical despite different names*

### Comparing `dollar_templates-1.0.0/dollar_templates/tokenizer.py` & `dollar_templates-1.0.1/dollar_templates/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dollar_templates-1.0.0/dollar_templates.egg-info/PKG-INFO` & `dollar_templates-1.0.1/dollar_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dollar-templates
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pandoc style dollar templates for python
 Home-page: https://github.com/seifferth/dollar_templates
 Author: Frank Seifferth
 Author-email: frankseifferth@posteo.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `dollar_templates-1.0.0/setup.py` & `dollar_templates-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dollar_templates',
-    version='1.0.0',
+    version='1.0.1',
     packages=['dollar_templates'],
     python_requires='>=3.9',
     author='Frank Seifferth',
     author_email='frankseifferth@posteo.net',
     description='Pandoc style dollar templates for python',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

