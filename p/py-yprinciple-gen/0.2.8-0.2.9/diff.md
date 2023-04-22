# Comparing `tmp/py_yprinciple_gen-0.2.8.tar.gz` & `tmp/py_yprinciple_gen-0.2.9.tar.gz`

## Comparing `py_yprinciple_gen-0.2.8.tar` & `py_yprinciple_gen-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.pydevproject
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/scripts/install
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/basemwtest.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/basesmwtest.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/basetest.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_editor.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_python.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_smw.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/tests/test_smw_generate.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/__init__.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/editor.py
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/genapi.py
--rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/gengrid.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/profiler.py
--rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/smw_targets.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/target.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/version.py
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/ypcell.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/ypgen.py
--rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/ypgenapp.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/yprinciple/resources/static/css/md_style_indigo.css
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/LICENSE
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/README.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/.pydevproject
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/scripts/install
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/basemwtest.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/basesmwtest.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/basetest.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/test_editor.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/test_python.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/test_smw.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/tests/test_smw_generate.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/__init__.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/editor.py
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/genapi.py
+-rw-r--r--   0        0        0    13170 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/gengrid.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/profiler.py
+-rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/smw_targets.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/target.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/version.py
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/ypcell.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/ypgen.py
+-rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/ypgenapp.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/yprinciple/resources/static/css/md_style_indigo.css
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/README.md
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 py_yprinciple_gen-0.2.9/PKG-INFO
```

### Comparing `py_yprinciple_gen-0.2.8/.github/workflows/build.yml` & `py_yprinciple_gen-0.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/.github/workflows/upload-to-pypi.yml` & `py_yprinciple_gen-0.2.9/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/scripts/test` & `py_yprinciple_gen-0.2.9/scripts/test`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/tests/basemwtest.py` & `py_yprinciple_gen-0.2.9/tests/basemwtest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/tests/basesmwtest.py` & `py_yprinciple_gen-0.2.9/tests/basesmwtest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/tests/basetest.py` & `py_yprinciple_gen-0.2.9/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/tests/test_editor.py` & `py_yprinciple_gen-0.2.9/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/tests/test_smw.py` & `py_yprinciple_gen-0.2.9/tests/test_smw.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/tests/test_smw_generate.py` & `py_yprinciple_gen-0.2.9/tests/test_smw_generate.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/editor.py` & `py_yprinciple_gen-0.2.9/yprinciple/editor.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/genapi.py` & `py_yprinciple_gen-0.2.9/yprinciple/genapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,8 +236,11 @@
                     (None,f"{{{{#ask: [[Topic name::{topic_name}]]|?Topic context=context}}}}","context")     
                 ]:   
                 if not page_titles:
                     page_titles=wikiPush.query(page_query, wiki=self.smwSourceAccess.wikiClient, queryField=query_field)
                 all_page_titles.extend(page_title for page_title in page_titles if page_title not in all_page_titles)    
         failed=wikiPush.push(pageTitles=all_page_titles,force=force,ignore=ignore,withImages=True)
         if len(failed)>0:
-            print(f"Warning {len(failed)} push attempts failed")
+            print(f"️Error {len(failed)} push attempts failed ❌️")
+            for i,fail_name in enumerate(failed[:20]):
+                print(f"    {i+1:2}: {fail_name} ❌") 
+
```

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/gengrid.py` & `py_yprinciple_gen-0.2.9/yprinciple/gengrid.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/profiler.py` & `py_yprinciple_gen-0.2.9/yprinciple/profiler.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/smw_targets.py` & `py_yprinciple_gen-0.2.9/yprinciple/smw_targets.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/target.py` & `py_yprinciple_gen-0.2.9/yprinciple/target.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/version.py` & `py_yprinciple_gen-0.2.9/yprinciple/version.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/ypcell.py` & `py_yprinciple_gen-0.2.9/yprinciple/ypcell.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/ypgen.py` & `py_yprinciple_gen-0.2.9/yprinciple/ypgen.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/ypgenapp.py` & `py_yprinciple_gen-0.2.9/yprinciple/ypgenapp.py`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/yprinciple/resources/static/css/md_style_indigo.css` & `py_yprinciple_gen-0.2.9/yprinciple/resources/static/css/md_style_indigo.css`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/.gitignore` & `py_yprinciple_gen-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/LICENSE` & `py_yprinciple_gen-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/README.md` & `py_yprinciple_gen-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/pyproject.toml` & `py_yprinciple_gen-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_yprinciple_gen-0.2.8/PKG-INFO` & `py_yprinciple_gen-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-yprinciple-gen
-Version: 0.2.8
+Version: 0.2.9
 Project-URL: Home, https://github.com/WolfgangFahl/py-yprinciple-gen
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/Py-yprinciple-gen
 Project-URL: Source, https://github.com/WolfgangFahl/py-yprinciple-gen
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

