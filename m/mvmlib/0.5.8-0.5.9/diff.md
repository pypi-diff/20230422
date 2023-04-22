# Comparing `tmp/mvmlib-0.5.8.tar.gz` & `tmp/mvmlib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvmlib-0.5.8.tar", last modified: Tue Apr 18 23:42:22 2023, max compression
+gzip compressed data, was "mvmlib-0.5.9.tar", last modified: Sat Apr 22 06:08:10 2023, max compression
```

## Comparing `mvmlib-0.5.8.tar` & `mvmlib-0.5.9.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     3444 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      930 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.github/workflows/tests_dev.yml
--rw-r--r--   0        0        0     2183 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.github/workflows/tests_master.yml
--rw-r--r--   0        0        0     2072 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.gitignore
--rw-r--r--   0        0        0      633 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/Makefile
--rw-r--r--   0        0        0      162 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/_static/css/custom.css
--rw-r--r--   0        0        0     1834 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/api.rst
--rw-r--r--   0        0        0    16325 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/background.rst
--rw-r--r--   0        0        0     2488 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/conf.py
--rw-r--r--   0        0        0      317 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/examples.rst
--rw-r--r--   0        0        0     1675 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/getting_started.rst
--rw-r--r--   0        0        0      444 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/glossary.rst
--rw-r--r--   0        0        0    17166 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/history.rst
--rw-r--r--   0        0        0   403031 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/images/TRS_example/load_case.png
--rw-r--r--   0        0        0    31511 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/images/efm_example.png
--rw-r--r--   0        0        0   344431 2023-04-18 23:41:39.333292 mvmlib-0.5.8/docs/images/strut_example/MAN.png
--rw-r--r--   0        0        0   122730 2023-04-18 23:41:39.333292 mvmlib-0.5.8/docs/images/strut_example/simplified_strut_model.png
--rw-r--r--   0        0        0   806946 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/images/strut_example/strut_overview.png
--rw-r--r--   0        0        0     3117 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/index.rst
--rw-r--r--   0        0        0      799 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/make.bat
--rw-r--r--   0        0        0   132133 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/notebooks/PDF_examples.ipynb
--rw-r--r--   0        0        0   176595 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/notebooks/TRS_example.ipynb
--rw-r--r--   0        0        0   229076 2023-04-18 23:41:39.345293 mvmlib-0.5.8/docs/notebooks/strut_example.ipynb
--rw-r--r--   0        0        0      847 2023-04-18 23:41:39.345293 mvmlib-0.5.8/docs/refs.bib
--rw-r--r--   0        0        0      674 2023-04-18 23:41:39.345293 mvmlib-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      157 2023-04-18 23:41:39.345293 mvmlib-0.5.8/pytest.ini
--rw-r--r--   0        0        0     1786 2023-04-18 23:41:39.345293 mvmlib-0.5.8/readme.md
--rw-r--r--   0        0        0      102 2023-04-18 23:41:39.345293 mvmlib-0.5.8/requirements.txt
--rw-r--r--   0        0        0      407 2023-04-18 23:41:39.345293 mvmlib-0.5.8/requirements_dev.txt
--rw-r--r--   0        0        0     5131 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/DOELib.py
--rw-r--r--   0        0        0      964 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/__init__.py
--rw-r--r--   0        0        0   134203 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/designMarginsLib.py
--rw-r--r--   0        0        0    13107 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/fuzzyLib.py
--rw-r--r--   0        0        0    29002 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/uncertaintyLib.py
--rw-r--r--   0        0        0     3299 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/utilities.py
--rw-r--r--   0        0        0      129 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/__init__.py
--rw-r--r--   0        0        0      539 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_doe.py
--rw-r--r--   0        0        0    14496 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_fuzzy.py
--rw-r--r--   0        0        0    73185 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_marginNetwork.py
--rw-r--r--   0        0        0    14717 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_probFunction.py
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 mvmlib-0.5.8/setup.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 mvmlib-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     3828 2023-04-22 06:07:30.424950 mvmlib-0.5.9/.github/workflows/push.yml
+-rw-r--r--   0        0        0     4894 2023-04-22 06:07:30.424950 mvmlib-0.5.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2072 2023-04-22 06:07:30.424950 mvmlib-0.5.9/.gitignore
+-rw-r--r--   0        0        0      633 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/Makefile
+-rw-r--r--   0        0        0      162 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1834 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/api.rst
+-rw-r--r--   0        0        0    16325 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/background.rst
+-rw-r--r--   0        0        0     2488 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/conf.py
+-rw-r--r--   0        0        0      317 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/examples.rst
+-rw-r--r--   0        0        0     1675 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/getting_started.rst
+-rw-r--r--   0        0        0      444 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/glossary.rst
+-rw-r--r--   0        0        0    17311 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/history.rst
+-rw-r--r--   0        0        0   403031 2023-04-22 06:07:30.424950 mvmlib-0.5.9/docs/images/TRS_example/load_case.png
+-rw-r--r--   0        0        0    31511 2023-04-22 06:07:30.428951 mvmlib-0.5.9/docs/images/efm_example.png
+-rw-r--r--   0        0        0   344431 2023-04-22 06:07:30.428951 mvmlib-0.5.9/docs/images/strut_example/MAN.png
+-rw-r--r--   0        0        0   122730 2023-04-22 06:07:30.428951 mvmlib-0.5.9/docs/images/strut_example/simplified_strut_model.png
+-rw-r--r--   0        0        0   806946 2023-04-22 06:07:30.436951 mvmlib-0.5.9/docs/images/strut_example/strut_overview.png
+-rw-r--r--   0        0        0     3117 2023-04-22 06:07:30.436951 mvmlib-0.5.9/docs/index.rst
+-rw-r--r--   0        0        0      799 2023-04-22 06:07:30.436951 mvmlib-0.5.9/docs/make.bat
+-rw-r--r--   0        0        0   132133 2023-04-22 06:07:30.436951 mvmlib-0.5.9/docs/notebooks/PDF_examples.ipynb
+-rw-r--r--   0        0        0   176595 2023-04-22 06:07:30.436951 mvmlib-0.5.9/docs/notebooks/TRS_example.ipynb
+-rw-r--r--   0        0        0   229076 2023-04-22 06:07:30.440951 mvmlib-0.5.9/docs/notebooks/strut_example.ipynb
+-rw-r--r--   0        0        0      847 2023-04-22 06:07:30.440951 mvmlib-0.5.9/docs/refs.bib
+-rw-r--r--   0        0        0      674 2023-04-22 06:07:30.440951 mvmlib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-22 06:07:30.440951 mvmlib-0.5.9/pytest.ini
+-rw-r--r--   0        0        0     1786 2023-04-22 06:07:30.440951 mvmlib-0.5.9/readme.md
+-rw-r--r--   0        0        0      102 2023-04-22 06:07:30.440951 mvmlib-0.5.9/requirements.txt
+-rw-r--r--   0        0        0      405 2023-04-22 06:07:30.440951 mvmlib-0.5.9/requirements_dev.txt
+-rw-r--r--   0        0        0     5131 2023-04-22 06:07:30.440951 mvmlib-0.5.9/src/mvm/DOELib.py
+-rw-r--r--   0        0        0      964 2023-04-22 06:07:30.440951 mvmlib-0.5.9/src/mvm/__init__.py
+-rw-r--r--   0        0        0   135272 2023-04-22 06:07:30.440951 mvmlib-0.5.9/src/mvm/designMarginsLib.py
+-rw-r--r--   0        0        0    13107 2023-04-22 06:07:30.440951 mvmlib-0.5.9/src/mvm/fuzzyLib.py
+-rw-r--r--   0        0        0    29002 2023-04-22 06:07:30.440951 mvmlib-0.5.9/src/mvm/uncertaintyLib.py
+-rw-r--r--   0        0        0     3299 2023-04-22 06:07:30.440951 mvmlib-0.5.9/src/mvm/utilities.py
+-rw-r--r--   0        0        0      129 2023-04-22 06:07:30.440951 mvmlib-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0      539 2023-04-22 06:07:30.440951 mvmlib-0.5.9/tests/test_doe.py
+-rw-r--r--   0        0        0    14544 2023-04-22 06:07:30.440951 mvmlib-0.5.9/tests/test_fuzzy.py
+-rw-r--r--   0        0        0    73969 2023-04-22 06:07:30.440951 mvmlib-0.5.9/tests/test_marginNetwork.py
+-rw-r--r--   0        0        0    14765 2023-04-22 06:07:30.444951 mvmlib-0.5.9/tests/test_probFunction.py
+-rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 mvmlib-0.5.9/setup.py
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 mvmlib-0.5.9/PKG-INFO
```

### Comparing `mvmlib-0.5.8/.github/workflows/release.yml` & `mvmlib-0.5.9/.github/workflows/release.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,182 @@
 name: release
 on:
   # the 1st condition
   release:
     branches: [master]
     types: [published]
+
+env:
+  documentation-source-directory: ./docs
+  documentation-build-directory: ./docs/build
+  deploy-python-version: '3.11'
+
 jobs:
   docs:
     name: documentation
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
+
     steps:
 
     - name: Checkout
       uses: actions/checkout@master
       with:
         fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
 
     - name: setup python
       uses: actions/setup-python@v2
       with:
-        python-version: '3.7'
+        python-version: ${{ matrix.python-version }}
         cache: 'pip'
 
     - name: setup pandoc environment
       uses: r-lib/actions/setup-pandoc@v1
       with:
-        pandoc-version: '2.0.1' # The pandoc version to download (if necessary) and use.
+        pandoc-version: '2.3' # The pandoc version to download (if necessary) and use.
 
     - name: install dependencies
       run: |
+        python -m pip install --upgrade pip
         pip install -r requirements_dev.txt
         echo "# Test" | pandoc -t html
 
     - name: Build flit package and install dependencies
       run: |
         # install package using flit locally to run documentation notebooks
         flit build
         flit install --deps=develop --symlink
 
-    - name: Build documentation and commit
-      uses: sphinx-notes/pages@v2
-      with:
-        documentation_path: ./docs
-        requirements_path: ./requirements.txt
-        target_branch: gh-pages
-    
-    - name: Push changes
-      uses: ad-m/github-push-action@master
+    - name: Build documentation
+      run: |
+        sphinx-build ${{env.documentation-source-directory}} ${{env.documentation-build-directory}}
+
+    - name: Cache built documentation
+      uses: actions/cache@v2
+      env:
+        cache-name: cache-docs
       with:
-        github_token: ${{ secrets.GITHUB_TOKEN }}
-        branch: gh-pages
+        path: ${{env.documentation-build-directory}} # documentation path
+        key: ${{ runner.os }}-docs-${{ env.cache-name }}-python-${{ matrix.python-version }}
 
   tests:
     name: pre-release tests
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
+
     steps:
 
     - name: Checkout
       uses: actions/checkout@master
       with:
         fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
 
     - name: setup python
       uses: actions/setup-python@v2
       with:
-        python-version: '3.7'
+        python-version: ${{ matrix.python-version }}
         cache: 'pip'
 
     - name: install dependencies
       run: |
+        python -m pip install --upgrade pip
         pip install -r requirements_dev.txt
         pip install -r requirements.txt
         pip install -e .
 
     - name: Build flit package and install dependencies
       run: |
         # install package using flit locally to run documentation notebooks
         flit build
         flit install --deps=develop --symlink
 
     - name: Run unit tests
       run: python -m pytest --import-mode=append tests/
 
+  deploy_docs:
+    name: publish_docs
+    needs: [docs,tests]
+    runs-on: ubuntu-latest
+
+    steps:
+
+    - name: Checkout
+      uses: actions/checkout@master
+      with:
+        fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
+
+    - name: Cache built documentation
+      uses: actions/cache@v2
+      env:
+        cache-name: cache-docs
+      with:
+        path: ${{env.documentation-build-directory}} # built documentation path
+        key: ${{ runner.os }}-docs-${{ env.cache-name }}-python-${{env.deploy-python-version}}
+    
+    - name: Deploy documentation to gh pages
+      uses: peaceiris/actions-gh-pages@v3
+      with:
+        publish_branch: gh-pages
+        github_token: ${{ secrets.GITHUB_TOKEN }}
+        publish_dir: ${{env.documentation-build-directory}}
+        force_orphan: true
+
   deploy_test:
     name: publish test PyPI
     needs: [docs,tests]
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout source
       uses: actions/checkout@v2
 
 
     - name: setup python
       uses: actions/setup-python@v2
       with:
-        python-version: '3.7'
+        python-version: ${{env.deploy-python-version}}
         cache: 'pip'
 
     - name: install dependencies
       run: |
+        python -m pip install --upgrade pip
         pip install -r requirements_dev.txt
         pip install -r requirements.txt
 
     - name: Build and publish to TestPyPI
       run: |
         flit publish
       env:
         FLIT_INDEX_URL: https://test.pypi.org/legacy/
         FLIT_USERNAME: __token__
         FLIT_PASSWORD: ${{ secrets.TEST_PYPI_API_TOKEN }}
 
   deploy:
     name: publish PyPI
-    needs: [docs,tests,deploy_test]
+    needs: [deploy_test]
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout source
       uses: actions/checkout@v2
 
 
     - name: setup python
       uses: actions/setup-python@v2
       with:
-        python-version: '3.7'
+        python-version: ${{env.deploy-python-version}}
         cache: 'pip'
 
     - name: install dependencies
       run: |
+        python -m pip install --upgrade pip
         pip install -r requirements_dev.txt
         pip install -r requirements.txt
 
     - name: Build and publish to TestPyPI
       run: |
         flit publish
       env:
```

### Comparing `mvmlib-0.5.8/.gitignore` & `mvmlib-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/Makefile` & `mvmlib-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/api.rst` & `mvmlib-0.5.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/background.rst` & `mvmlib-0.5.9/docs/background.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/conf.py` & `mvmlib-0.5.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'mvmlib'
 copyright = '2021, Khalil Al Handawi'
 author = 'Khalil Al Handawi'
 
 # The full version, including alpha/beta/rc tags
-release = '0.5.8'
+release = '0.5.9'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `mvmlib-0.5.8/docs/getting_started.rst` & `mvmlib-0.5.9/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/history.rst` & `mvmlib-0.5.9/docs/history.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 .. toctree::
    :titlesonly:
 
 *********
 Changelog
 *********
 
+.. _release-0.5.9:
+
+0.5.9
+=====
+
+:Date: April 22, 2023
+
+Fixes
+-----
+* Fix compatibility with python versions `3.11`, `3.11`, `3.11`, and `3.11`
+
 .. _release-0.5.8:
 
 0.5.8
 =====
 
 :Date: April 18, 2023
```

### Comparing `mvmlib-0.5.8/docs/images/TRS_example/load_case.png` & `mvmlib-0.5.9/docs/images/TRS_example/load_case.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/images/efm_example.png` & `mvmlib-0.5.9/docs/images/efm_example.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/images/strut_example/MAN.png` & `mvmlib-0.5.9/docs/images/strut_example/MAN.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/images/strut_example/simplified_strut_model.png` & `mvmlib-0.5.9/docs/images/strut_example/simplified_strut_model.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/images/strut_example/strut_overview.png` & `mvmlib-0.5.9/docs/images/strut_example/strut_overview.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/index.rst` & `mvmlib-0.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/make.bat` & `mvmlib-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/notebooks/PDF_examples.ipynb` & `mvmlib-0.5.9/docs/notebooks/PDF_examples.ipynb`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/notebooks/TRS_example.ipynb` & `mvmlib-0.5.9/docs/notebooks/TRS_example.ipynb`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/notebooks/strut_example.ipynb` & `mvmlib-0.5.9/docs/notebooks/strut_example.ipynb`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/docs/refs.bib` & `mvmlib-0.5.9/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/pyproject.toml` & `mvmlib-0.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mvmlib"
 authors = [{name = "Khalil Al Handawi", email = "khalil.alhandawi@mail.mcgill.ca"}]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ['version', 'description']
 
 dependencies = [
-"matplotlib==3.4.3",
+"matplotlib==3.7.0",
 "pyDOE==0.3.8",
 "scikit-fuzzy==0.4.2",
 "smt==1.1.0",
 "multiprocess==0.70.12.2"
 ]
 
 [tool.flit.module]
```

### Comparing `mvmlib-0.5.8/readme.md` & `mvmlib-0.5.9/readme.md`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/src/mvm/DOELib.py` & `mvmlib-0.5.9/src/mvm/DOELib.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/src/mvm/__init__.py` & `mvmlib-0.5.9/src/mvm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 A library based on the margin value method for computing design 
 margins using fuzzy logic and probabilistic methods for 
 uncertainty modelling
 
 """
 
-__version__ = '0.5.8'
+__version__ = '0.5.9'
 __all__ = ['TriangularFunc', 'FuzzySet', 'FuzzyRule', 'FuzzySystem', 'GaussianFunc', 'UniformFunc', 'Distribution',
            'VisualizeDist', 'compute_cdf', 'Design', 'MarginNode', 'InputSpec', 'FixedParam', 'DesignParam',
            'Behaviour', 'MatrixParam', 'ScalarParam', 'VectorParam', 'Performance', 'MarginNetwork', 'Decision', 'nearest']
 
 from .fuzzyLib import TriangularFunc, FuzzySet, FuzzyRule, FuzzySystem
 from .uncertaintyLib import GaussianFunc, UniformFunc, Distribution, VisualizeDist, compute_cdf
 from .DOELib import Design
```

### Comparing `mvmlib-0.5.8/src/mvm/designMarginsLib.py` & `mvmlib-0.5.9/src/mvm/designMarginsLib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1113,15 +1113,16 @@
         if isinstance(i,(int,float,np.floating)):
             self._inverted = np.array([i,])
         else:
             assert len(i) == 1, 'expected %i parameters, got %i parameters' %(1,len(i))
             self._inverted = np.array(i)
 
     def train_surrogate(self,variable_dict: Dict[str, Dict[str,Union[Tuple[int,int], Tuple[float,float], List[str], str]] ],
-                        n_samples: int, bandwidth: List[float] = [0.01], num_threads: int = 1, sm_type: float = 'KRG', *args, **kwargs):
+                        n_samples: int, bandwidth: List[float] = [0.01], num_threads: int = 1, sm_type: float = 'KRG', 
+                        random_state: Union[int,np.random.RandomState] = None, *args, **kwargs):
         """
         trains a Kriging surrogate model of the behaviour model to make computations less expensive
         surrogate model returns an array of shape 
         [n_samples , (n_intermediate + n_performance + n_decided_value + n_target_threshold) ]
         the inputs are 
         [n_samples , other arguments ]
 
@@ -1134,14 +1135,17 @@
             number of samples drawn from the behaviour model for training
         bandwidth : List[float], optional
             bandwidth of the correlation function used by Kriging, by default [0.01]
         sm_type : str, optional
             type of surrogate model to train, possible values ['KRG','LS'], by default 'KRG'
         num_threads : int, optional
             number of threads to parallelize sampling the training data by, by default 1
+        random_state : Union[int,np.random.RandomState], optional
+            Random seed or random generator instance used to generate training samples, 
+            If None is provided a random seed is used, by default None
         """
         for key,value in variable_dict.items():
             assert value['type'] in ['FLOAT','INT','ENUM','fixed'], 'Unexpected type (%s) for variable (%s) provided \
                 , expecting "FLOAT", "INT", or "ENUM"' %(value['type'], key)
 
             if value['type'] in ['INT', 'FLOAT']:
                 assert type(value['limits']) in [list,tuple], 'Unexpected limits (%s) for variable (%s) provided \
@@ -1184,15 +1188,16 @@
                 args += (value['limits'],)
 
         assert len(xlimits) > 0, 'at least one variable should not be fixed'
 
         self.xtypes = xtypes
         self.xlimits = xlimits
         sampling = MixedIntegerSamplingMethod(xtypes=self.xtypes, xlimits=self.xlimits,
-                                                sampling_method_class=LHS, criterion="ese")
+                                                sampling_method_class=LHS, criterion="ese",
+                                                random_state=random_state)
 
         input_samples = sampling(n_samples)
 
         # Parallel computation if num_threads > 1
         behaviour_objs = []
         for pid in range(num_threads):
             behaviour_objs += [deepcopy(self)]
@@ -2514,15 +2519,16 @@
             strategy = [strategy,] * len(self.margin_nodes)
 
         self.forward(allocate_margin=True, strategy=strategy)  # do not randomize the man for deterioration
         self.initial_decision = self.decision_vector
         self.reset(n=1)
 
     def train_performance_surrogate(self, n_samples: int = 100, sampling_freq: int = 1, bandwidth: List[float] = [1e-2], 
-                                    sm_type: str = 'KRG', num_threads: int = 1, ext_samples: Tuple[np.ndarray, np.ndarray] = None):
+                                    sm_type: str = 'KRG', num_threads: int = 1, ext_samples: Tuple[np.ndarray, np.ndarray] = None,
+                                    random_state: Union[int,np.random.RandomState] = None):
         """
         Constructs a surrogate model y(x), where x are the excess values and 
         y are the performance parameters that can be used to calculate threshold 
         performances
 
         Parameters
         ----------
@@ -2538,20 +2544,23 @@
         num_threads : int, optional
             number of threads to parallelize sampling process, by default 1
         ext_samples : tuple[np.ndarray,np.ndarray], optional
             if sample data provided externally then use directly to fit the response surface, 
             Tuple must have length 2, ext_samples[0] must have shape (N_samples,len(margin_nodes)),
             ext_samples[1] must have shape (N_samples,len(performances)),
             by default None
+        random_state : Union[int,np.random.RandomState], optional
+            Random seed or random generator instance used to generate training samples, 
+            If None is provided a random seed is used, by default None
         """
         if ext_samples is None:
             # generate training data for response surface using an LHS grid of design parameter and input
             # specification space
 
-            input_samples = self._sample_inputs(n_samples)
+            input_samples = self._sample_inputs(n_samples,random_state)
 
             # Parallel computation if num_threads > 1
             man_objs = []
             for pid in range(num_threads):
                 man_objs += [deepcopy(self)]
 
             kwargs = {
@@ -3260,43 +3269,47 @@
             for p in range(len(self.performances)):
                 self.performances[p] = pickle.load(f)
 
         if not results_only:
             for behaviour in self.behaviours:
                 behaviour.load(filename=path)
 
-    def _sample_inputs(self,n_samples: int) -> np.ndarray:
+    def _sample_inputs(self,n_samples: int, random_state: Union[int,np.random.RandomState] = None) -> np.ndarray:
         """
         samples the design space of the MAN
 
         Parameters
         ----------
         n_samples : int
             number of samples
 
         Returns
         -------
         np.ndarray
             An array of samples with shape (n_samples,n_variables), 
             where n_variables is the total number of design variables
+        random_state : Union[int,np.random.RandomState], optional
+            Random seed or random generator instance used to generate training samples, 
+            If None is provided a random seed is used, by default None
         """
         xtypes = []
         xlimits = []
         for xtype, limits in zip(self.variable_type, self.universe):
             if xtype == 'FLOAT':
                 xtypes += [FLOAT, ]
             elif xtype == 'INT':
                 xtypes += [ORD, ]
             elif xtype == 'ENUM':
                 xtypes += [(ENUM, len(limits)), ]
 
             xlimits += [limits]
 
         sampling = MixedIntegerSamplingMethod(xtypes=xtypes, xlimits=xlimits,
-                                                sampling_method_class=LHS, criterion="ese")
+                                                sampling_method_class=LHS, criterion="ese",
+                                                random_state=random_state)
 
         input_samples = sampling(n_samples)
 
         return input_samples
 
     def _bounded_perf(self,inputs: np.ndarray) -> np.ndarray:
         """
@@ -3481,15 +3494,15 @@
         pid = mp.current_process()._identity[0] - process_ids[0]
         man = mans[pid]
 
     tt_samples, spec, perf_samples = _sample_man(input_i,man,sampling_freq)
 
     return tt_samples, spec, perf_samples
 
-def _sample_behaviour(*args, variable_dict=None, **kwargs) -> List[Union[int,float]]:
+def _sample_behaviour(*args, variable_dict = None, **kwargs) -> List[Union[int,float]]:
     """
     samples the decision universe
     *args are expected to vary
     **kwargs are fixed
 
     Parameters
     ----------
```

### Comparing `mvmlib-0.5.8/src/mvm/fuzzyLib.py` & `mvmlib-0.5.9/src/mvm/fuzzyLib.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/src/mvm/uncertaintyLib.py` & `mvmlib-0.5.9/src/mvm/uncertaintyLib.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/src/mvm/utilities.py` & `mvmlib-0.5.9/src/mvm/utilities.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/tests/test_doe.py` & `mvmlib-0.5.9/tests/test_doe.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.8/tests/test_fuzzy.py` & `mvmlib-0.5.9/tests/test_fuzzy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import pytest
 import numpy as np
 import matplotlib.pyplot as plt
+import random
+
+random.seed(0)
+np.random.seed(0)
 
 from mvm import TriangularFunc, FuzzySet, FuzzyRule, FuzzySystem
 
 def create_set(lb,ub):
     """" Create a fuzzy set from a given range """
 
     universe = np.linspace(lb, ub, 11) # grid for all variables
```

### Comparing `mvmlib-0.5.8/tests/test_marginNetwork.py` & `mvmlib-0.5.9/tests/test_marginNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import pytest
 import numpy as np
 import os
 from scipy.stats import norm
 import matplotlib
 from typing import List, Tuple
 from scipy.optimize import fsolve, minimize
+import random
 
+random.seed(0)
+np.random.seed(0)
 matplotlib.use('Agg')
 
 from mvm import Design, GaussianFunc, UniformFunc, MarginNode, Performance, MarginNetwork, \
     InputSpec, DesignParam, Behaviour, Decision, compute_cdf, nearest
 from mvm.designMarginsLib import _secant_method
 from mvm.utilities import check_folder
 
+# numpy random number generator instance (for reproducing SMT related tests)
+@pytest.fixture
+def random_generator() -> np.random.RandomState:
+    return np.random.RandomState(0)
+
 # root finding functions
 @pytest.fixture
 def f():
     def _f(x):
         return x ** 2 - 2
 
     return _f
@@ -556,14 +564,15 @@
     man = MAN(design_parameters,input_specs,[],behaviours,decisions,margin_nodes,performances,'MAN_test')
 
     return man
 
 def decision_man_inverse(design_parameters: List[DesignParam],
                          man_components: Tuple[List[Behaviour],List[Performance],List[MarginNode]],
                          deterministic_specs: Tuple[np.ndarray,List[InputSpec]],
+                         random_generator: np.random.RandomState,
                          tt_factor: List[float]=3*[1.0,], use_surrogates: bool=False) -> MarginNetwork:
     ######################################################
     # Construct MAN
     behaviours, decisions, performances, margin_nodes = man_components
     centers,input_specs = deterministic_specs
 
     s1,s2 = input_specs
@@ -572,21 +581,21 @@
 
     if use_surrogates:
         variable_dict = {
             'w' : {'type' : 'FLOAT', 'limits' : [decision_5.universe[0],decision_5.universe[-1],]},
             's1' : {'type' : 'FLOAT', 'limits' : s1.universe},
             's2' : {'type' : 'FLOAT', 'limits' : s2.universe},
         }
-        behaviours[8].train_surrogate(variable_dict,n_samples=100,sm_type='KRG')
+        behaviours[8].train_surrogate(variable_dict,n_samples=100,sm_type='KRG',random_state=random_generator)
         behaviours[8].train_inverse('w')
 
         variable_dict = {
             'value' : {'type' : 'ENUM', 'limits' : decision_2.universe},
         }
-        behaviours[9].train_surrogate(variable_dict,n_samples=100,sm_type='KRG')
+        behaviours[9].train_surrogate(variable_dict,n_samples=100,sm_type='KRG',random_state=random_generator)
         behaviours[9].train_inverse(sm_type='LS')
 
     class MAN(MarginNetwork):
         def randomize(self):
             pass
 
         def forward(self,recalculate_decisions=False,allocate_margin=False,strategy=['min_excess',]*len(margin_nodes),outputs=['dv',]*len(margin_nodes),**kwargs):
@@ -819,15 +828,15 @@
     'deviation',
     [
         pytest.param(0.0, marks=pytest.mark.dependency(name='impact_d1')),
         pytest.param(0.5, marks=pytest.mark.dependency(name='impact_d2')),
     ]
 )
 def test_deterministic_ImpactMatrix(man_components:Tuple[List[Behaviour],List[Performance],List[MarginNode]],
-    Impact_test_inputs:Tuple[np.ndarray,np.ndarray],deviation:float):
+    Impact_test_inputs:Tuple[np.ndarray,np.ndarray],deviation:float,random_generator: np.random.RandomState):
     """
     Tests the ImpactMatrix calculation method for deterministic threshold and decided values
     """
 
     ######################################################
     # Construct MAN
 
@@ -873,15 +882,15 @@
     n_samples = 1000
     doe_node = Design(-np.ones(len(margin_nodes)),np.ones(len(margin_nodes)),n_samples,'LHS').unscale()
 
     p_space = np.empty((n_samples,len(performances)))
     p_space[:,0] = np.apply_along_axis(man.behaviours[1].p1_model,axis=1,arr=doe_node+dv_vector) # mat + vec is automatically broadcasted
     p_space[:,1] = np.apply_along_axis(man.behaviours[1].p2_model,axis=1,arr=doe_node+dv_vector) # mat + vec is automatically broadcasted
 
-    man.train_performance_surrogate(n_samples=100,sm_type='KRG',ext_samples=(doe_node+dv_vector,p_space))
+    man.train_performance_surrogate(n_samples=100,sm_type='KRG',ext_samples=(doe_node+dv_vector,p_space),random_state=random_generator)
     man.forward()
     man.view_perf(e_indices=[0,1],p_index=0)
     man.compute_impact(use_estimate=True)
 
     # Compute test impact
     input = np.tile(dv_vector+deviation,(len(margin_nodes),1))
 
@@ -903,15 +912,16 @@
     #     [-0.61538462, -0.22222222]
     #     ])
 
     assert np.allclose(man.impact_matrix.value, test_impact, rtol=1e-1)
 
 @pytest.mark.dependency()
 def test_stochastic_ImpactMatrix(man_components:Tuple[List[Behaviour],List[Performance],List[MarginNode]],
-                                 Impact_test_inputs:Tuple[np.ndarray,np.ndarray], noise:GaussianFunc):
+                                 Impact_test_inputs:Tuple[np.ndarray,np.ndarray], noise:GaussianFunc, 
+                                 random_generator: np.random.RandomState):
     """
     Tests the ImpactMatrix calculation method for stochastic threshold and decided values
     """
 
     ######################################################
     # Construct MAN
 
@@ -957,15 +967,15 @@
     n_samples = 100
     doe_node = Design(-np.ones(len(margin_nodes)),np.ones(len(margin_nodes)),n_samples,'LHS').unscale()
 
     p_space = np.empty((n_samples,len(performances)))
     p_space[:,0] = np.apply_along_axis(man.behaviours[1].p1_model,axis=1,arr=doe_node+dv_vector) # mat + vec is automatically broadcasted
     p_space[:,1] = np.apply_along_axis(man.behaviours[1].p2_model,axis=1,arr=doe_node+dv_vector) # mat + vec is automatically broadcasted
 
-    man.train_performance_surrogate(n_samples=100,ext_samples=(doe_node+dv_vector,p_space))
+    man.train_performance_surrogate(n_samples=100,ext_samples=(doe_node+dv_vector,p_space),random_state=random_generator)
 
     n_runs = 1000
     for n in range(n_runs):
         man.forward()
         man.compute_impact(use_estimate=True)
 
     mean_impact = np.mean(man.impact_matrix.values,axis=2)
@@ -1476,15 +1486,16 @@
 
     assert np.allclose(mean_absorption, test_absorption, rtol=1e-1)
     assert np.allclose(mean_utilization, test_utilization, rtol=1e-1)
 
 @pytest.mark.dependency()
 def test_mixed_variables(man_components: Tuple[List[Behaviour],List[Performance],List[MarginNode]],
                          deterministic_specs: Tuple[np.ndarray,List[InputSpec]],
-                         design_parameters: List[DesignParam]):
+                         design_parameters: List[DesignParam],
+                         random_generator: np.random.RandomState):
 
     """
     Tests the train performance surrogate functionality when decision nodes are present
     """
     n_threads = 1
     ######################################################
     # Construct MAN
@@ -1507,15 +1518,15 @@
             'tt_factor' : [1.0,1.0,1.0],
             'tt_vector' : [4.84,3.2,2.2],
         }
 
     man = decision_man(design_parameters,man_components,deterministic_specs,test_dict['tt_factor'])
 
     # Create surrogate model for estimating threshold performance
-    man.train_performance_surrogate(n_samples=100, sm_type='KRG', sampling_freq=1, num_threads=n_threads, bandwidth=[1e-3, ])
+    man.train_performance_surrogate(n_samples=100, sm_type='KRG', sampling_freq=1, num_threads=n_threads, bandwidth=[1e-3, ], random_state=random_generator)
     man.init_decisions(num_threads=n_threads)
     man.allocate_margins()
     man.forward()
     man.compute_impact(use_estimate=True)
 
     ######################################################
     # Calculate the test values
@@ -1604,15 +1615,16 @@
     [
         pytest.param(False, marks=pytest.mark.dependency(name='impact_i1')),
         pytest.param(True, marks=pytest.mark.dependency(name='impact_i2')),
     ]
 )
 def test_mixed_variables_inverse(man_components: Tuple[List[Behaviour],List[Performance],List[MarginNode]],
                                  deterministic_specs: Tuple[np.ndarray,List[InputSpec]],
-                                 design_parameters: List[DesignParam], surrogate: bool):
+                                 design_parameters: List[DesignParam], surrogate: bool,
+                                 random_generator: np.random.RandomState):
 
     """
     Tests the impact on performance functionality when decision nodes are present
     """
     n_threads = 1
     ######################################################
     # Construct MAN
@@ -1631,15 +1643,15 @@
 
     test_dict = {
             'true_decisions' : [1.6,'1','1'],
             'tt_factor' : [1.0,1.0,1.0],
             'tt_vector' : [4.84,3.2,2.2],
         }
 
-    man = decision_man_inverse(design_parameters,man_components,deterministic_specs,test_dict['tt_factor'],use_surrogates=surrogate)
+    man = decision_man_inverse(design_parameters,man_components,deterministic_specs,random_generator,test_dict['tt_factor'],use_surrogates=surrogate)
 
     # Create surrogate model for estimating threshold performance
     man.init_decisions(num_threads=n_threads)
     man.allocate_margins()
     man.forward()
     man.compute_impact(use_estimate=False)
 
@@ -1889,15 +1901,15 @@
     #test_utilization = [len(margin_nodes), len(input_specs)]
 
     assert np.allclose(mean_absorption, test_absorption, rtol=1e-1)
     assert np.allclose(mean_utilization, test_utilization, rtol=1e-1)
 
 
 @pytest.mark.parametrize('n_threads', [1,])
-def test_behaviour(n_threads):
+def test_behaviour(n_threads,random_generator: np.random.RandomState):
 
     def fun(x,value):
         if value == '1':
             p = -0.1 * x
         elif value == '2':
             p = 0.5 * x
         elif value == '3':
@@ -1912,15 +1924,15 @@
     b = B1(n_i=0,n_p=0,n_dv=0,n_tt=1)
 
     # Train surrogate
     variable_dict = {
         'x' : {'type' : 'FLOAT', 'limits' : [-100,100]},
         'value' : {'type' : 'ENUM', 'limits' : ['1','2','3']},
     }
-    b.train_surrogate(variable_dict,n_outputs=1,n_samples=100,num_threads=n_threads)
+    b.train_surrogate(variable_dict,n_outputs=1,n_samples=100,num_threads=n_threads,random_rate=random_generator)
 
     # test outputs
     test_values = [[1.0, '1',],[1.0, '2',],[1.0, '3',]]
     for test_values in test_values:
         b(test_values[0],test_values[1])
         assert fun(test_values[0],test_values[1]) == b.threshold
```

### Comparing `mvmlib-0.5.8/tests/test_probFunction.py` & `mvmlib-0.5.9/tests/test_probFunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import pytest
 import numpy as np
 import matplotlib.pyplot as plt
+import random
+
+random.seed(0)
+np.random.seed(0)
 
 from mvm import Design, GaussianFunc, UniformFunc, Distribution
 
 # Input set 1
 @pytest.fixture
 def example_mean_std():
```

### Comparing `mvmlib-0.5.8/setup.py` & `mvmlib-0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 package_data = \
 {'': ['*']}
 
 package_dir = \
 {'': 'src'}
 
 install_requires = \
-['matplotlib==3.4.3',
+['matplotlib==3.7.0',
  'pyDOE==0.3.8',
  'scikit-fuzzy==0.4.2',
  'smt==1.1.0',
  'multiprocess==0.70.12.2']
 
 extras_require = \
 {'doc': ['sphinx', 'sphinx-autobuild', 'nbsphinx'],
  'test': ['pytest>=6.2.5',
           'pytest-cov==3.0.0',
           'pytest-dependency==0.5.1',
           'pandoc']}
 
 setup(name='mvmlib',
-      version='0.5.8',
+      version='0.5.9',
       description='Margin Value Method Library',
       author=None,
       author_email='Khalil Al Handawi <khalil.alhandawi@mail.mcgill.ca>',
       url=None,
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
       install_requires=install_requires,
       extras_require=extras_require,
-      python_requires='>=3.7',
+      python_requires='>=3.8',
      )
```

### Comparing `mvmlib-0.5.8/PKG-INFO` & `mvmlib-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mvmlib
-Version: 0.5.8
+Version: 0.5.9
 Summary: Margin Value Method Library
 Author-email: Khalil Al Handawi <khalil.alhandawi@mail.mcgill.ca>
-Requires-Python: >=3.7
-Requires-Dist: matplotlib==3.4.3
+Requires-Python: >=3.8
+Requires-Dist: matplotlib==3.7.0
 Requires-Dist: pyDOE==0.3.8
 Requires-Dist: scikit-fuzzy==0.4.2
 Requires-Dist: smt==1.1.0
 Requires-Dist: multiprocess==0.70.12.2
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-autobuild ; extra == "doc"
 Requires-Dist: nbsphinx ; extra == "doc"
```

