# Comparing `tmp/django_object_safety-0.1.3.tar.gz` & `tmp/django_object_safety-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-0.1.3.tar", max compression
+gzip compressed data, was "django_object_safety-0.1.4.tar", max compression
```

## Comparing `django_object_safety-0.1.3.tar` & `django_object_safety-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/LICENSE
--rw-r--r--   0        0        0      135 2023-04-22 18:07:55.917732 django_object_safety-0.1.3/README.md
--rw-r--r--   0        0        0      698 2023-04-22 18:08:26.409693 django_object_safety-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.1.3/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.1.3/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.1.3/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.1.3/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/models.py
--rw-r--r--   0        0        0    12352 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/shortcuts.py
--rw-r--r--   0        0        0     6111 2023-04-22 17:57:27.834494 django_object_safety-0.1.3/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.1.3/safety/views.py
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 django_object_safety-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-22 18:09:42.813595 django_object_safety-0.1.4/README.md
+-rw-r--r--   0        0        0      688 2023-04-22 18:10:00.117572 django_object_safety-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-0.1.4/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/models.py
+-rw-r--r--   0        0        0    12352 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/shortcuts.py
+-rw-r--r--   0        0        0     6111 2023-04-22 17:57:27.834494 django_object_safety-0.1.4/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-0.1.4/safety/views.py
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 django_object_safety-0.1.4/PKG-INFO
```

### Comparing `django_object_safety-0.1.3/LICENSE` & `django_object_safety-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/pyproject.toml` & `django_object_safety-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "0.1.3"
+version = "0.1.4"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
-homepage = "https://django-object-safety-docs.readthedocs.io/en/latest/"
+homepage = "https://django-object-safety-docs.readthedocs.io/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
 packages = [{ include = "safety" }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
```

### Comparing `django_object_safety-0.1.3/safety/migrations/0001_initial.py` & `django_object_safety-0.1.4/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-0.1.4/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-0.1.4/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-0.1.4/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-0.1.4/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/models.py` & `django_object_safety-0.1.4/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/shortcuts.py` & `django_object_safety-0.1.4/safety/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/safety/tests.py` & `django_object_safety-0.1.4/safety/tests.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-0.1.3/PKG-INFO` & `django_object_safety-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 0.1.3
+Version: 0.1.4
 Summary: Adds object permissions to Django.
-Home-page: https://django-object-safety-docs.readthedocs.io/en/latest/
+Home-page: https://django-object-safety-docs.readthedocs.io/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.2,<5.0)
 Project-URL: Repository, https://github.com/williammferreira/django-object-safety/
 Description-Content-Type: text/markdown
 
 ## Implements object permissions and groups in django
 
-View the documentation at http://django-object-safety.readthedocs.org/en/latest/
+View the documentation at http://django-object-safety-docs.readthedocs.io/
```

