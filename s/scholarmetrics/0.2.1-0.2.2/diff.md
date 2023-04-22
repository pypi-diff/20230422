# Comparing `tmp/scholarmetrics-0.2.1.tar.gz` & `tmp/scholarmetrics-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scholarmetrics-0.2.1.tar", last modified: Wed Aug  2 17:26:41 2017, max compression
+gzip compressed data, was "scholarmetrics-0.2.2.tar", last modified: Sat Apr 22 17:10:11 2023, max compression
```

## Comparing `scholarmetrics-0.2.1.tar` & `scholarmetrics-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,37 @@
-drwxrwxrwx   0 merose    (1000) merose    (1000)        0 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/
--rwxrwxrwx   0 merose    (1000) merose    (1000)      222 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/.codeclimate.yml
--rwxrwxrwx   0 merose    (1000) merose    (1000)      284 2017-04-03 19:07:36.000000 scholarmetrics-0.2.1/.travis.yml
--rwxrwxrwx   0 merose    (1000) merose    (1000)       93 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/AUTHORS
--rwxrwxrwx   0 merose    (1000) merose    (1000)      692 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/ChangeLog
--rwxrwxrwx   0 merose    (1000) merose    (1000)     2888 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/CONTRIBUTING.rst
-drwxrwxrwx   0 merose    (1000) merose    (1000)        0 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/docs/
--rwxrwxrwx   0 merose    (1000) merose    (1000)     8932 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/docs/conf.py
--rwxrwxrwx   0 merose    (1000) merose    (1000)       33 2017-04-03 19:00:45.000000 scholarmetrics-0.2.1/docs/contributing.rst
-drwxrwxrwx   0 merose    (1000) merose    (1000)        0 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/docs/generated/
--rwxrwxrwx   0 merose    (1000) merose    (1000)      113 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/docs/generated/scholarmetrics.euclidean.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)      104 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/docs/generated/scholarmetrics.gindex.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)      104 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/docs/generated/scholarmetrics.hindex.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)       28 2017-04-03 19:00:45.000000 scholarmetrics-0.2.1/docs/history.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)      724 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/docs/index.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)     1195 2017-04-03 19:00:45.000000 scholarmetrics-0.2.1/docs/installation.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)     6475 2017-04-03 19:00:45.000000 scholarmetrics-0.2.1/docs/make.bat
--rwxrwxrwx   0 merose    (1000) merose    (1000)     6794 2017-04-03 19:00:45.000000 scholarmetrics-0.2.1/docs/Makefile
--rwxrwxrwx   0 merose    (1000) merose    (1000)      119 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/docs/reference.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)      248 2017-04-08 12:36:13.000000 scholarmetrics-0.2.1/HISTORY.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)     1072 2017-04-03 19:00:45.000000 scholarmetrics-0.2.1/LICENSE
--rwxrwxrwx   0 merose    (1000) merose    (1000)     2877 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/PKG-INFO
--rwxrwxrwx   0 merose    (1000) merose    (1000)     1589 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/README.rst
--rwxrwxrwx   0 merose    (1000) merose    (1000)       15 2017-08-02 17:16:05.000000 scholarmetrics-0.2.1/requirements.txt
-drwxrwxrwx   0 merose    (1000) merose    (1000)        0 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics/
--rwxrwxrwx   0 merose    (1000) merose    (1000)     3907 2017-04-08 14:24:17.000000 scholarmetrics-0.2.1/scholarmetrics/metrics.py
-drwxrwxrwx   0 merose    (1000) merose    (1000)        0 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics/tests/
--rwxrwxrwx   0 merose    (1000) merose    (1000)     1635 2017-04-08 12:36:14.000000 scholarmetrics-0.2.1/scholarmetrics/tests/test_metrics.py
--rwxrwxrwx   0 merose    (1000) merose    (1000)       73 2017-04-08 12:36:13.000000 scholarmetrics-0.2.1/scholarmetrics/tests/__init__.py
--rwxrwxrwx   0 merose    (1000) merose    (1000)      331 2017-08-02 17:24:50.000000 scholarmetrics-0.2.1/scholarmetrics/__init__.py
-drwxrwxrwx   0 merose    (1000) merose    (1000)        0 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/
--rwxrwxrwx   0 merose    (1000) merose    (1000)        1 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/dependency_links.txt
--rwxrwxrwx   0 merose    (1000) merose    (1000)        1 2017-03-14 09:36:06.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/not-zip-safe
--rwxrwxrwx   0 merose    (1000) merose    (1000)       47 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/pbr.json
--rwxrwxrwx   0 merose    (1000) merose    (1000)     2877 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/PKG-INFO
--rwxrwxrwx   0 merose    (1000) merose    (1000)       15 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/requires.txt
--rwxrwxrwx   0 merose    (1000) merose    (1000)      774 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/SOURCES.txt
--rwxrwxrwx   0 merose    (1000) merose    (1000)       15 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/scholarmetrics.egg-info/top_level.txt
--rwxrwxrwx   0 merose    (1000) merose    (1000)      886 2017-08-02 17:26:41.000000 scholarmetrics-0.2.1/setup.cfg
--rwxrwxrwx   0 merose    (1000) merose    (1000)       93 2017-08-02 17:16:36.000000 scholarmetrics-0.2.1/setup.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 17:10:11.446325 scholarmetrics-0.2.2/
+-rw-rw-r--   0 panther   (1000) panther   (1000)      182 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/.codeclimate.yml
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1045 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/.gitignore
+-rw-rw-r--   0 panther   (1000) panther   (1000)      284 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/.travis.yml
+-rw-rw-r--   0 panther   (1000) panther   (1000)      147 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/AUTHORS.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2951 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)      675 2023-04-22 17:08:09.000000 scholarmetrics-0.2.2/HISTORY.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1072 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/LICENSE
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3060 2023-04-22 17:10:11.446325 scholarmetrics-0.2.2/PKG-INFO
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1651 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/README.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 17:10:11.442324 scholarmetrics-0.2.2/docs/
+-rw-rw-r--   0 panther   (1000) panther   (1000)     6794 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/Makefile
+-rw-rw-r--   0 panther   (1000) panther   (1000)       28 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/authors.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     9050 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/conf.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)       33 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/contributing.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 17:10:11.442324 scholarmetrics-0.2.2/docs/generated/
+-rw-rw-r--   0 panther   (1000) panther   (1000)      113 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/generated/scholarmetrics.euclidean.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)      104 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/generated/scholarmetrics.gindex.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)      104 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/generated/scholarmetrics.hindex.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)       28 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/history.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)      746 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/index.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1195 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/installation.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     6475 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/make.bat
+-rw-rw-r--   0 panther   (1000) panther   (1000)      119 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/docs/reference.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1658 2023-04-22 17:06:02.000000 scholarmetrics-0.2.2/pyproject.toml
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 17:10:11.442324 scholarmetrics-0.2.2/scholarmetrics/
+-rw-rw-r--   0 panther   (1000) panther   (1000)      331 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/scholarmetrics/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3907 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/scholarmetrics/metrics.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 17:10:11.446325 scholarmetrics-0.2.2/scholarmetrics/tests/
+-rw-rw-r--   0 panther   (1000) panther   (1000)       73 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/scholarmetrics/tests/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1635 2023-04-22 15:42:24.000000 scholarmetrics-0.2.2/scholarmetrics/tests/test_metrics.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 17:10:11.442324 scholarmetrics-0.2.2/scholarmetrics.egg-info/
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3060 2023-04-22 17:10:11.000000 scholarmetrics-0.2.2/scholarmetrics.egg-info/PKG-INFO
+-rw-rw-r--   0 panther   (1000) panther   (1000)      668 2023-04-22 17:10:11.000000 scholarmetrics-0.2.2/scholarmetrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)        1 2023-04-22 17:10:11.000000 scholarmetrics-0.2.2/scholarmetrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)       15 2023-04-22 17:10:11.000000 scholarmetrics-0.2.2/scholarmetrics.egg-info/top_level.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)       38 2023-04-22 17:10:11.446325 scholarmetrics-0.2.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scholarmetrics-0.2.1/CONTRIBUTING.rst` & `scholarmetrics-0.2.2/CONTRIBUTING.rst`

 * *Files 9% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     $ python setup.py develop
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
+   Feel free to add your name to `AUTHORS.rst <AUTHORS.rst>`_.
 
 5. Commit your changes and push your branch to GitHub::
 
     $ git add .
     $ git commit -m "Your detailed description of your changes."
     $ git push origin name-of-your-bugfix-or-feature
```

### Comparing `scholarmetrics-0.2.1/docs/conf.py` & `scholarmetrics-0.2.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,18 +125,25 @@
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     'github_user': 'Michael-E-Rose',
     'github_repo': 'scholarmetrics',
-    'github_button': True,
-    'travis_button': "true",
-    'codecov_button': True,
-    'sidebar_width': "200px"
+    'github_banner': 'true',
+    'github_button': 'false',
+    'travis_button': 'true',
+    'sidebar_width': '240px',
+}
+html_sidebars = {
+    '**': [
+        'about.html',
+        'navigation.html',
+        'searchbox.html',
+    ]
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 #html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
```

### Comparing `scholarmetrics-0.2.1/docs/index.rst` & `scholarmetrics-0.2.2/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 .. toctree::
    :maxdepth: 1
 
    installation
    reference
    contributing
+   authors
+   history
 
 
 ==================
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `scholarmetrics-0.2.1/docs/installation.rst` & `scholarmetrics-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scholarmetrics-0.2.1/docs/make.bat` & `scholarmetrics-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scholarmetrics-0.2.1/docs/Makefile` & `scholarmetrics-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scholarmetrics-0.2.1/LICENSE` & `scholarmetrics-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scholarmetrics-0.2.1/PKG-INFO` & `scholarmetrics-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,90 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: scholarmetrics
-Version: 0.2.1
+Version: 0.2.2
 Summary: Compute scholarly metrics in Python with Pandas and NumPy Edit
-Home-page: https://scholarmetrics.readthedocs.io/en/latest/
-Author: Michael E. Rose
-Author-email: Michael.Ernst.Rose@gmail.com
+Author-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
+Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 License: MIT
-Description: ===============================
-        scholarmetrics
-        ===============================
-        
-        Compute scholarly metrics in Python with Pandas and NumPy.
-        
-        
-        **Documentation**: https://scholarmetrics.readthedocs.io.
-        
-        .. image:: https://img.shields.io/pypi/v/scholarmetrics.svg
-                :target: https://pypi.python.org/pypi/scholarmetrics
-        
-        .. image:: https://readthedocs.org/projects/scholarmetrics/badge/?version=latest
-                :target: https://scholarmetrics.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics/badges/gpa.svg
-                :target: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics
-                :alt: Code Climate
-        
-        .. image:: https://travis-ci.org/Michael-E-Rose/scholarmetrics.svg?branch=master
-                :target: https://travis-ci.org/Michael-E-Rose/scholarmetrics
-                :alt: Build Status
-        
-        
-        Examples
-        --------
-        
-        * J.E. Hirsch's h-index or Hirsch-index:
-        
-        .. code:: python
-        
-            >>> from scholarmetrics import hindex
-            >>> citations = [6, 10, 5, 46, 0, 2]
-            >>> hindex(citations)
-            4
-        
-        * Euclidean index:
-        
-        .. code:: python
-        
-            >>> from scholarmetrics import euclidean
-            >>> citations = [6, 10, 5, 46, 0, 2]
-            >>> euclidean(citations)
-            47.75981574503821
-        
-        
-        Contributing
-        ------------
-        
-        .. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
-             :target: https://github.com/Michael-E-Rose/scholarmetrics/issues
-             :alt: Contributions welcome
-        
-        Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
-        
-        License
-        -------
-        MIT License, see `LICENSE <LICENSE>`_.
-        
-        
-Keywords: scholarmetrics
-metrics
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/Michael-E-Rose/scholarmetrics
+Project-URL: Bug Tracker, https://github.com/Michael-E-Rose/scholarmetrics/issues
+Project-URL: Documentation (stable), https://scholarmetrics.readthedocs.io/en/stable/
+Project-URL: Documentation (latest), https://scholarmetrics.readthedocs.io/en/latest/
+Keywords: metrics,researchers,scientists,academics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===============================
+scholarmetrics
+===============================
+
+Compute scholarly metrics in Python with Pandas and NumPy.
+
+
+**Documentation**: https://scholarmetrics.readthedocs.io.
+
+.. image:: https://img.shields.io/pypi/v/scholarmetrics.svg
+        :target: https://pypi.python.org/pypi/scholarmetrics
+
+.. image:: https://readthedocs.org/projects/scholarmetrics/badge/?version=latest
+        :target: https://scholarmetrics.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics/badges/gpa.svg
+        :target: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics
+        :alt: Code Climate
+
+.. image:: https://travis-ci.org/Michael-E-Rose/scholarmetrics.svg?branch=master
+        :target: https://travis-ci.org/Michael-E-Rose/scholarmetrics
+        :alt: Build Status
+
+
+Examples
+--------
+
+* J.E. Hirsch's h-index or Hirsch-index:
+
+.. code:: python
+
+    >>> from scholarmetrics import hindex
+    >>> citations = [6, 10, 5, 46, 0, 2]
+    >>> hindex(citations)
+    4
+
+* Euclidean index:
+
+.. code:: python
+
+    >>> from scholarmetrics import euclidean
+    >>> citations = [6, 10, 5, 46, 0, 2]
+    >>> euclidean(citations)
+    47.75981574503821
+
+
+Contributing
+------------
+
+.. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+     :target: https://github.com/Michael-E-Rose/scholarmetrics/issues
+     :alt: Contributions welcome
+
+Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+
+For a list of contributors see `AUTHORS.rst <AUTHORS.rst>`_.
+
+License
+-------
+MIT License, see `LICENSE <LICENSE>`_.
```

### Comparing `scholarmetrics-0.2.1/README.rst` & `scholarmetrics-0.2.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -50,10 +50,12 @@
 
 .. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
      :target: https://github.com/Michael-E-Rose/scholarmetrics/issues
      :alt: Contributions welcome
 
 Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
 
+For a list of contributors see `AUTHORS.rst <AUTHORS.rst>`_.
+
 License
 -------
 MIT License, see `LICENSE <LICENSE>`_.
```

### Comparing `scholarmetrics-0.2.1/scholarmetrics/metrics.py` & `scholarmetrics-0.2.2/scholarmetrics/metrics.py`

 * *Files identical despite different names*

### Comparing `scholarmetrics-0.2.1/scholarmetrics/tests/test_metrics.py` & `scholarmetrics-0.2.2/scholarmetrics/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scholarmetrics-0.2.1/scholarmetrics.egg-info/PKG-INFO` & `scholarmetrics-0.2.2/scholarmetrics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,90 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: scholarmetrics
-Version: 0.2.1
+Version: 0.2.2
 Summary: Compute scholarly metrics in Python with Pandas and NumPy Edit
-Home-page: https://scholarmetrics.readthedocs.io/en/latest/
-Author: Michael E. Rose
-Author-email: Michael.Ernst.Rose@gmail.com
+Author-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
+Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 License: MIT
-Description: ===============================
-        scholarmetrics
-        ===============================
-        
-        Compute scholarly metrics in Python with Pandas and NumPy.
-        
-        
-        **Documentation**: https://scholarmetrics.readthedocs.io.
-        
-        .. image:: https://img.shields.io/pypi/v/scholarmetrics.svg
-                :target: https://pypi.python.org/pypi/scholarmetrics
-        
-        .. image:: https://readthedocs.org/projects/scholarmetrics/badge/?version=latest
-                :target: https://scholarmetrics.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics/badges/gpa.svg
-                :target: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics
-                :alt: Code Climate
-        
-        .. image:: https://travis-ci.org/Michael-E-Rose/scholarmetrics.svg?branch=master
-                :target: https://travis-ci.org/Michael-E-Rose/scholarmetrics
-                :alt: Build Status
-        
-        
-        Examples
-        --------
-        
-        * J.E. Hirsch's h-index or Hirsch-index:
-        
-        .. code:: python
-        
-            >>> from scholarmetrics import hindex
-            >>> citations = [6, 10, 5, 46, 0, 2]
-            >>> hindex(citations)
-            4
-        
-        * Euclidean index:
-        
-        .. code:: python
-        
-            >>> from scholarmetrics import euclidean
-            >>> citations = [6, 10, 5, 46, 0, 2]
-            >>> euclidean(citations)
-            47.75981574503821
-        
-        
-        Contributing
-        ------------
-        
-        .. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
-             :target: https://github.com/Michael-E-Rose/scholarmetrics/issues
-             :alt: Contributions welcome
-        
-        Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
-        
-        License
-        -------
-        MIT License, see `LICENSE <LICENSE>`_.
-        
-        
-Keywords: scholarmetrics
-metrics
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/Michael-E-Rose/scholarmetrics
+Project-URL: Bug Tracker, https://github.com/Michael-E-Rose/scholarmetrics/issues
+Project-URL: Documentation (stable), https://scholarmetrics.readthedocs.io/en/stable/
+Project-URL: Documentation (latest), https://scholarmetrics.readthedocs.io/en/latest/
+Keywords: metrics,researchers,scientists,academics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===============================
+scholarmetrics
+===============================
+
+Compute scholarly metrics in Python with Pandas and NumPy.
+
+
+**Documentation**: https://scholarmetrics.readthedocs.io.
+
+.. image:: https://img.shields.io/pypi/v/scholarmetrics.svg
+        :target: https://pypi.python.org/pypi/scholarmetrics
+
+.. image:: https://readthedocs.org/projects/scholarmetrics/badge/?version=latest
+        :target: https://scholarmetrics.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics/badges/gpa.svg
+        :target: https://codeclimate.com/github/Michael-E-Rose/scholarmetrics
+        :alt: Code Climate
+
+.. image:: https://travis-ci.org/Michael-E-Rose/scholarmetrics.svg?branch=master
+        :target: https://travis-ci.org/Michael-E-Rose/scholarmetrics
+        :alt: Build Status
+
+
+Examples
+--------
+
+* J.E. Hirsch's h-index or Hirsch-index:
+
+.. code:: python
+
+    >>> from scholarmetrics import hindex
+    >>> citations = [6, 10, 5, 46, 0, 2]
+    >>> hindex(citations)
+    4
+
+* Euclidean index:
+
+.. code:: python
+
+    >>> from scholarmetrics import euclidean
+    >>> citations = [6, 10, 5, 46, 0, 2]
+    >>> euclidean(citations)
+    47.75981574503821
+
+
+Contributing
+------------
+
+.. image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+     :target: https://github.com/Michael-E-Rose/scholarmetrics/issues
+     :alt: Contributions welcome
+
+Please see `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+
+For a list of contributors see `AUTHORS.rst <AUTHORS.rst>`_.
+
+License
+-------
+MIT License, see `LICENSE <LICENSE>`_.
```

### Comparing `scholarmetrics-0.2.1/scholarmetrics.egg-info/SOURCES.txt` & `scholarmetrics-0.2.2/scholarmetrics.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 .codeclimate.yml
+.gitignore
 .travis.yml
-AUTHORS
+AUTHORS.rst
 CONTRIBUTING.rst
-ChangeLog
 HISTORY.rst
 LICENSE
 README.rst
-requirements.txt
-setup.cfg
-setup.py
+pyproject.toml
 docs/Makefile
+docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/reference.rst
@@ -21,13 +20,10 @@
 docs/generated/scholarmetrics.gindex.rst
 docs/generated/scholarmetrics.hindex.rst
 scholarmetrics/__init__.py
 scholarmetrics/metrics.py
 scholarmetrics.egg-info/PKG-INFO
 scholarmetrics.egg-info/SOURCES.txt
 scholarmetrics.egg-info/dependency_links.txt
-scholarmetrics.egg-info/not-zip-safe
-scholarmetrics.egg-info/pbr.json
-scholarmetrics.egg-info/requires.txt
 scholarmetrics.egg-info/top_level.txt
 scholarmetrics/tests/__init__.py
 scholarmetrics/tests/test_metrics.py
```

