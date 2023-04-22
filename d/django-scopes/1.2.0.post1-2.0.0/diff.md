# Comparing `tmp/django-scopes-1.2.0.post1.tar.gz` & `tmp/django-scopes-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-scopes-1.2.0.post1.tar", last modified: Thu Apr  7 09:19:14 2022, max compression
+gzip compressed data, was "django-scopes-2.0.0.tar", last modified: Sat Apr 22 17:05:58 2023, max compression
```

## Comparing `django-scopes-1.2.0.post1.tar` & `django-scopes-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      304 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/AUTHORS
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11358 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11895 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11026 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/README.md
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/django_scopes/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      269 2022-04-07 09:18:16.000000 django-scopes-1.2.0.post1/django_scopes/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/django_scopes/exceptions.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      456 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/django_scopes/forms.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3022 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/django_scopes/manager.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      596 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/django_scopes/state.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/django_scopes.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)    11895 2022-04-07 09:19:14.000000 django-scopes-1.2.0.post1/django_scopes.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)      658 2022-04-07 09:19:14.000000 django-scopes-1.2.0.post1/django_scopes.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2022-04-07 09:19:14.000000 django-scopes-1.2.0.post1/django_scopes.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2022-04-07 09:19:14.000000 django-scopes-1.2.0.post1/django_scopes.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       20 2022-04-07 09:19:14.000000 django-scopes-1.2.0.post1/django_scopes.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      329 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1293 2022-04-07 09:10:45.000000 django-scopes-1.2.0.post1/setup.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/tests/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/tests/testapp/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/tests/testapp/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)       95 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/tests/testapp/apps.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      555 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/tests/testapp/forms.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2022-04-07 09:19:14.773310 django-scopes-1.2.0.post1/tests/testapp/migrations/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1283 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      638 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/tests/testapp/migrations/0002_bookmark.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      951 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/tests/testapp/migrations/0003_commentgroup.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/tests/testapp/migrations/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1122 2022-04-07 09:09:52.000000 django-scopes-1.2.0.post1/tests/testapp/models.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/tests/testapp/urls.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      394 2022-02-19 18:46:36.000000 django-scopes-1.2.0.post1/tests/testapp/wsgi.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:05:58.818596 django-scopes-2.0.0/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      304 2019-05-10 11:53:52.000000 django-scopes-2.0.0/AUTHORS
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    11358 2019-05-10 11:53:56.000000 django-scopes-2.0.0/LICENSE
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    12542 2023-04-22 17:05:58.818596 django-scopes-2.0.0/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    11699 2023-04-08 19:55:17.000000 django-scopes-2.0.0/README.md
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:05:58.818596 django-scopes-2.0.0/django_scopes/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      263 2023-04-08 19:56:40.000000 django-scopes-2.0.0/django_scopes/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2022-04-19 08:12:54.000000 django-scopes-2.0.0/django_scopes/exceptions.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      456 2019-05-12 14:43:55.000000 django-scopes-2.0.0/django_scopes/forms.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3022 2022-04-19 08:12:54.000000 django-scopes-2.0.0/django_scopes/manager.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      679 2023-04-08 19:55:17.000000 django-scopes-2.0.0/django_scopes/state.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:05:58.818596 django-scopes-2.0.0/django_scopes.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    12542 2023-04-22 17:05:58.000000 django-scopes-2.0.0/django_scopes.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      678 2023-04-22 17:05:58.000000 django-scopes-2.0.0/django_scopes.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-22 17:05:58.000000 django-scopes-2.0.0/django_scopes.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       12 2023-04-22 17:05:58.000000 django-scopes-2.0.0/django_scopes.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       20 2023-04-22 17:05:58.000000 django-scopes-2.0.0/django_scopes.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      329 2023-04-22 17:05:58.818596 django-scopes-2.0.0/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1293 2023-04-22 17:05:57.000000 django-scopes-2.0.0/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:05:58.818596 django-scopes-2.0.0/tests/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     6787 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/test_query.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:05:58.818596 django-scopes-2.0.0/tests/testapp/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2019-05-10 11:54:17.000000 django-scopes-2.0.0/tests/testapp/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       95 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/testapp/apps.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      555 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/testapp/forms.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-22 17:05:58.818596 django-scopes-2.0.0/tests/testapp/migrations/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1283 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      638 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/testapp/migrations/0002_bookmark.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      951 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/testapp/migrations/0003_commentgroup.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2019-05-10 11:54:17.000000 django-scopes-2.0.0/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1122 2022-04-19 08:12:54.000000 django-scopes-2.0.0/tests/testapp/models.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       18 2019-05-10 11:54:17.000000 django-scopes-2.0.0/tests/testapp/urls.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      394 2019-05-10 12:52:08.000000 django-scopes-2.0.0/tests/testapp/wsgi.py
```

### Comparing `django-scopes-1.2.0.post1/LICENSE` & `django-scopes-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-scopes-1.2.0.post1/PKG-INFO` & `django-scopes-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: django-scopes
-Version: 1.2.0.post1
-Summary: Scope querys in multi-tenant django applications
-Home-page: https://github.com/raphaelm/django-scopes
-Author: Raphael Michel
-Author-email: mail@raphaelmichel.de
-License: Apache License 2.0
-Keywords: json database models
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 django-scopes
 =============
 
 ![Build status](https://github.com/raphaelm/django-scopes/actions/workflows/tests.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/django-scopes.svg)
 [![Python versions](https://img.shields.io/pypi/pyversions/django-scopes.svg)](https://pypi.org/project/django-scopes/)
 ![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-scopes)
@@ -219,14 +195,32 @@
 with scope(user=request.user.pk):
 	# do something :)
 ```
 
 Caveats
 -------
 
+### Locking
+
+With django-scopes, a seemingly innocent query like
+
+```python
+Comment.objects.select_for_update().get(pk=3)
+```
+
+could cause unexpected locking across your database, since django-scopes will auto-add one or more ``JOIN`` statements to the query, and joined tables will **also be locked**.
+One possible fix is of course using ``scopes_disabled()``, around this query.
+On most modern databases, there's also a way to specify explicitly which tables you want locked:
+
+```python
+Comment.objects.select_for_update(of=("self",)).get(pk=3)
+```
+
+You can check if your database supports this feature at runtime using ``connection.features.has_select_for_update_of``.
+
 ### Admin
 
 **django-scopes** is not compatible with the django admin out of the box, integration requires a
 custom middleware. (If you write one, please open a PR to include it in this package!)
 
 ### Testing
 
@@ -338,9 +332,7 @@
 ## Further reading
 
 If you'd like to read more about the practical use of django-scopes, there is a [blog
 post](https://behind.pretix.eu/2019/06/17/scopes/) about its introduction in the [pretix](https://pretix.eu) project.
 
 [Here](https://rixx.de/blog/using-the-django-shell-with-django-scopes/) is a guide on how to write a ``shell_scoped``
 django-admin command to provide a scoped Django shell.
-
-
```

### Comparing `django-scopes-1.2.0.post1/README.md` & `django-scopes-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: django-scopes
+Version: 2.0.0
+Summary: Scope querys in multi-tenant django applications
+Home-page: https://github.com/raphaelm/django-scopes
+Author: Raphael Michel
+Author-email: mail@raphaelmichel.de
+License: Apache License 2.0
+Keywords: json database models
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
 django-scopes
 =============
 
 ![Build status](https://github.com/raphaelm/django-scopes/actions/workflows/tests.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/django-scopes.svg)
 [![Python versions](https://img.shields.io/pypi/pyversions/django-scopes.svg)](https://pypi.org/project/django-scopes/)
 ![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-scopes)
@@ -195,14 +218,32 @@
 with scope(user=request.user.pk):
 	# do something :)
 ```
 
 Caveats
 -------
 
+### Locking
+
+With django-scopes, a seemingly innocent query like
+
+```python
+Comment.objects.select_for_update().get(pk=3)
+```
+
+could cause unexpected locking across your database, since django-scopes will auto-add one or more ``JOIN`` statements to the query, and joined tables will **also be locked**.
+One possible fix is of course using ``scopes_disabled()``, around this query.
+On most modern databases, there's also a way to specify explicitly which tables you want locked:
+
+```python
+Comment.objects.select_for_update(of=("self",)).get(pk=3)
+```
+
+You can check if your database supports this feature at runtime using ``connection.features.has_select_for_update_of``.
+
 ### Admin
 
 **django-scopes** is not compatible with the django admin out of the box, integration requires a
 custom middleware. (If you write one, please open a PR to include it in this package!)
 
 ### Testing
```

### Comparing `django-scopes-1.2.0.post1/django_scopes/manager.py` & `django-scopes-2.0.0/django_scopes/manager.py`

 * *Files identical despite different names*

### Comparing `django-scopes-1.2.0.post1/django_scopes/state.py` & `django-scopes-2.0.0/django_scopes/state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from contextlib import contextmanager
-from threading import local
+from contextvars import ContextVar
+from typing import Optional
 
-state = local()
+state: ContextVar[Optional[dict]] = ContextVar('state', default=None)
 
 
 @contextmanager
 def scopes_disabled():
     with scope(_enabled=False):
         yield
 
 
 @contextmanager
 def scope(**scope_kwargs):
-    if not hasattr(state, 'scope'):
-        state.scope = {}
+    previous_scope = state.get()
+    if previous_scope is None:
+        previous_scope = {}
+        state.set(previous_scope)
 
-    previous_scope = getattr(state, 'scope', {})
     new_scope = dict(previous_scope)
     new_scope['_enabled'] = True
     new_scope.update(scope_kwargs)
-    state.scope = new_scope
+    state.set(new_scope)
     try:
         yield
     finally:
-        state.scope = previous_scope
+        state.set(previous_scope)
 
 
 def get_scope():
-    return dict(getattr(state, 'scope', {}))
+    return state.get() or {}
```

### Comparing `django-scopes-1.2.0.post1/django_scopes.egg-info/PKG-INFO` & `django-scopes-2.0.0/django_scopes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: django-scopes
-Version: 1.2.0.post1
+Version: 2.0.0
 Summary: Scope querys in multi-tenant django applications
 Home-page: https://github.com/raphaelm/django-scopes
 Author: Raphael Michel
 Author-email: mail@raphaelmichel.de
 License: Apache License 2.0
 Keywords: json database models
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -219,14 +218,32 @@
 with scope(user=request.user.pk):
 	# do something :)
 ```
 
 Caveats
 -------
 
+### Locking
+
+With django-scopes, a seemingly innocent query like
+
+```python
+Comment.objects.select_for_update().get(pk=3)
+```
+
+could cause unexpected locking across your database, since django-scopes will auto-add one or more ``JOIN`` statements to the query, and joined tables will **also be locked**.
+One possible fix is of course using ``scopes_disabled()``, around this query.
+On most modern databases, there's also a way to specify explicitly which tables you want locked:
+
+```python
+Comment.objects.select_for_update(of=("self",)).get(pk=3)
+```
+
+You can check if your database supports this feature at runtime using ``connection.features.has_select_for_update_of``.
+
 ### Admin
 
 **django-scopes** is not compatible with the django admin out of the box, integration requires a
 custom middleware. (If you write one, please open a PR to include it in this package!)
 
 ### Testing
 
@@ -338,9 +355,7 @@
 ## Further reading
 
 If you'd like to read more about the practical use of django-scopes, there is a [blog
 post](https://behind.pretix.eu/2019/06/17/scopes/) about its introduction in the [pretix](https://pretix.eu) project.
 
 [Here](https://rixx.de/blog/using-the-django-shell-with-django-scopes/) is a guide on how to write a ``shell_scoped``
 django-admin command to provide a scoped Django shell.
-
-
```

### Comparing `django-scopes-1.2.0.post1/django_scopes.egg-info/SOURCES.txt` & `django-scopes-2.0.0/django_scopes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 django_scopes/manager.py
 django_scopes/state.py
 django_scopes.egg-info/PKG-INFO
 django_scopes.egg-info/SOURCES.txt
 django_scopes.egg-info/dependency_links.txt
 django_scopes.egg-info/requires.txt
 django_scopes.egg-info/top_level.txt
+tests/test_query.py
 tests/testapp/__init__.py
 tests/testapp/apps.py
 tests/testapp/forms.py
 tests/testapp/models.py
 tests/testapp/urls.py
 tests/testapp/wsgi.py
 tests/testapp/migrations/0001_initial.py
```

### Comparing `django-scopes-1.2.0.post1/setup.py` & `django-scopes-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     author_email='mail@raphaelmichel.de',
     license='Apache License 2.0',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         'Intended Audience :: Developers',
         'Intended Audience :: Other Audience',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         "Framework :: Django",
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
     ],
     keywords='json database models',
```

### Comparing `django-scopes-1.2.0.post1/tests/testapp/forms.py` & `django-scopes-2.0.0/tests/testapp/forms.py`

 * *Files identical despite different names*

### Comparing `django-scopes-1.2.0.post1/tests/testapp/migrations/0001_initial.py` & `django-scopes-2.0.0/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-scopes-1.2.0.post1/tests/testapp/migrations/0002_bookmark.py` & `django-scopes-2.0.0/tests/testapp/migrations/0002_bookmark.py`

 * *Files identical despite different names*

### Comparing `django-scopes-1.2.0.post1/tests/testapp/migrations/0003_commentgroup.py` & `django-scopes-2.0.0/tests/testapp/migrations/0003_commentgroup.py`

 * *Files identical despite different names*

### Comparing `django-scopes-1.2.0.post1/tests/testapp/models.py` & `django-scopes-2.0.0/tests/testapp/models.py`

 * *Files identical despite different names*

