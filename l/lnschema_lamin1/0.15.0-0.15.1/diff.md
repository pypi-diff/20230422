# Comparing `tmp/lnschema_lamin1-0.15.0.tar.gz` & `tmp/lnschema_lamin1-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.15.0.tar", last modified: Sat Apr 22 05:34:49 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.15.1.tar", last modified: Sat Apr 22 11:07:31 2023, max compression
```

## Comparing `lnschema_lamin1-0.15.0.tar` & `lnschema_lamin1-0.15.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.15.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.15.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.15.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.15.0/.gitignore
--rw-r--r--   0        0        0     1753 2023-04-22 03:48:11.222542 lnschema_lamin1-0.15.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      145 2023-04-22 05:28:10.791672 lnschema_lamin1-0.15.0/README.md
--rw-r--r--   0        0        0      276 2023-04-22 05:34:28.878680 lnschema_lamin1-0.15.0/docs/changelog.md
--rw-r--r--   0        0        0     5036 2023-04-22 04:45:45.601083 lnschema_lamin1-0.15.0/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-04-22 04:45:45.613158 lnschema_lamin1-0.15.0/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5395 2023-04-22 04:45:45.614909 lnschema_lamin1-0.15.0/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.15.0/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.15.0/docs/index.md
--rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.15.0/docs/reference.md
--rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.15.0/lamin-project.yaml
--rw-r--r--   0        0        0      607 2023-04-22 05:33:51.699540 lnschema_lamin1-0.15.0/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     2738 2023-04-22 05:28:10.791910 lnschema_lamin1-0.15.0/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     1460 2023-04-22 05:28:10.792065 lnschema_lamin1-0.15.0/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      253 2023-04-22 05:28:10.792283 lnschema_lamin1-0.15.0/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.15.0/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.15.0/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.15.0/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      250 2023-04-22 05:28:10.792423 lnschema_lamin1-0.15.0/lnschema_lamin1/link.py
--rw-r--r--   0        0        0      979 2023-03-24 23:23:34.184309 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-14-3ed88d3699fd-v0_6_0.py
--rw-r--r--   0        0        0     1188 2023-03-24 23:23:34.184393 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-01360b6492cc-v0_7_0.py
--rw-r--r--   0        0        0      630 2023-03-24 23:23:34.184479 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-05efb2ed6192-v0_6_0.post1.py
--rw-r--r--   0        0        0      940 2023-03-24 23:23:34.184551 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-a171e861e473-v0_7_1.py
--rw-r--r--   0        0        0      620 2023-03-24 23:23:34.184623 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-e2507b7564f0-v0_7_0.post1.py
--rw-r--r--   0        0        0     2173 2023-03-24 23:23:34.184690 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-20-a5d6b07f1401-v0_7_2.py
--rw-r--r--   0        0        0     2174 2023-03-24 23:23:34.184767 lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-11-03-bfda12fc80a8-v0_8_0.py
--rw-r--r--   0        0        0      777 2023-04-22 05:28:10.792624 lnschema_lamin1-0.15.0/noxfile.py
--rw-r--r--   0        0        0      779 2023-04-22 03:51:54.773135 lnschema_lamin1-0.15.0/pyproject.toml
--rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.15.0/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.15.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 lnschema_lamin1-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.15.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.15.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.15.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.15.1/.gitignore
+-rw-r--r--   0        0        0     1753 2023-04-22 03:48:11.222542 lnschema_lamin1-0.15.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      145 2023-04-22 05:28:10.791672 lnschema_lamin1-0.15.1/README.md
+-rw-r--r--   0        0        0      276 2023-04-22 11:06:42.620232 lnschema_lamin1-0.15.1/docs/changelog.md
+-rw-r--r--   0        0        0     5036 2023-04-22 04:45:45.601083 lnschema_lamin1-0.15.1/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-04-22 04:45:45.613158 lnschema_lamin1-0.15.1/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     5395 2023-04-22 04:45:45.614909 lnschema_lamin1-0.15.1/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.15.1/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.15.1/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.15.1/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.15.1/lamin-project.yaml
+-rw-r--r--   0        0        0      607 2023-04-22 11:06:31.753223 lnschema_lamin1-0.15.1/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     2738 2023-04-22 05:28:10.791910 lnschema_lamin1-0.15.1/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     1460 2023-04-22 05:28:10.792065 lnschema_lamin1-0.15.1/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      253 2023-04-22 05:28:10.792283 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/_id.py
+-rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.15.1/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      250 2023-04-22 05:28:10.792423 lnschema_lamin1-0.15.1/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0      979 2023-03-24 23:23:34.184309 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-14-3ed88d3699fd-v0_6_0.py
+-rw-r--r--   0        0        0     1188 2023-03-24 23:23:34.184393 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-01360b6492cc-v0_7_0.py
+-rw-r--r--   0        0        0      630 2023-03-24 23:23:34.184479 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-05efb2ed6192-v0_6_0.post1.py
+-rw-r--r--   0        0        0      940 2023-03-24 23:23:34.184551 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-a171e861e473-v0_7_1.py
+-rw-r--r--   0        0        0      620 2023-03-24 23:23:34.184623 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-e2507b7564f0-v0_7_0.post1.py
+-rw-r--r--   0        0        0     2173 2023-03-24 23:23:34.184690 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-20-a5d6b07f1401-v0_7_2.py
+-rw-r--r--   0        0        0     2174 2023-03-24 23:23:34.184767 lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-11-03-bfda12fc80a8-v0_8_0.py
+-rw-r--r--   0        0        0      777 2023-04-22 05:28:10.792624 lnschema_lamin1-0.15.1/noxfile.py
+-rw-r--r--   0        0        0      742 2023-04-22 11:07:17.974070 lnschema_lamin1-0.15.1/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.15.1/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.15.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 lnschema_lamin1-0.15.1/PKG-INFO
```

### Comparing `lnschema_lamin1-0.15.0/.github/workflows/build.yml` & `lnschema_lamin1-0.15.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.15.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/.gitignore` & `lnschema_lamin1-0.15.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/.pre-commit-config.yaml` & `lnschema_lamin1-0.15.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.15.1/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.15.1/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/docs/guide/10-migrate.ipynb` & `lnschema_lamin1-0.15.1/docs/guide/10-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
 _migration = None
-__version__ = "0.15.0"
+__version__ = "0.15.1"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
```

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/_core.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/_core.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/_link.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/_link.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-14-3ed88d3699fd-v0_6_0.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-14-3ed88d3699fd-v0_6_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-01360b6492cc-v0_7_0.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-01360b6492cc-v0_7_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-05efb2ed6192-v0_6_0.post1.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-05efb2ed6192-v0_6_0.post1.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-a171e861e473-v0_7_1.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-a171e861e473-v0_7_1.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-19-e2507b7564f0-v0_7_0.post1.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-19-e2507b7564f0-v0_7_0.post1.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-10-20-a5d6b07f1401-v0_7_2.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-10-20-a5d6b07f1401-v0_7_2.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/lnschema_lamin1/migrations/versions/2022-11-03-bfda12fc80a8-v0_8_0.py` & `lnschema_lamin1-0.15.1/lnschema_lamin1/migrations/versions/2022-11-03-bfda12fc80a8-v0_8_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/noxfile.py` & `lnschema_lamin1-0.15.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/pyproject.toml` & `lnschema_lamin1-0.15.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 [project]
 name = "lnschema_lamin1"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    # do not pin a lamindb version
-    # just set a lower bound
-    "lamindb[bionty,wetlab]==0.38.0",
+    "lnschema_core",
+    "lnbase_biolab",
     "openpyxl",
     "psycopg2-binary",
     "gcsfs",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnschema-lamin1"
@@ -24,14 +23,15 @@
     "pre-commit",
     "nox",
 ]
 test = [
     "pytest>=6.0",
     "pytest-cov",
     "nbproject_test>=0.4.1",
+    "lamindb[bionty]",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
 testpaths = [
```

### Comparing `lnschema_lamin1-0.15.0/tests/test_migrations.py` & `lnschema_lamin1-0.15.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.15.0/PKG-INFO` & `lnschema_lamin1-0.15.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.15.0
+Version: 0.15.1
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lamindb[bionty,wetlab]==0.38.0
+Requires-Dist: lnschema_core
+Requires-Dist: lnbase_biolab
 Requires-Dist: openpyxl
 Requires-Dist: psycopg2-binary
 Requires-Dist: gcsfs
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject_test>=0.4.1 ; extra == "test"
+Requires-Dist: lamindb[bionty] ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-lamin1
 Provides-Extra: dev
 Provides-Extra: test
 
 # lnschema-lamin1: Customized schema of Lamin
 
 Latest developer docs: [netlify](https://lnschema-lamin1-tvhn.netlify.app/docs/lnschema-lamin1/).
```

