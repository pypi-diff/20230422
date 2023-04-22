# Comparing `tmp/django-utilitas-1.2.9.tar.gz` & `tmp/django-utilitas-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-utilitas-1.2.9.tar", last modified: Thu Apr 20 15:25:07 2023, max compression
+gzip compressed data, was "django-utilitas-1.3.0.tar", last modified: Sat Apr 22 06:45:48 2023, max compression
```

## Comparing `django-utilitas-1.2.9.tar` & `django-utilitas-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-20 15:25:07.132364 django-utilitas-1.2.9/
--rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.2.9/LICENSE
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4040 2023-04-20 15:25:07.132619 django-utilitas-1.2.9/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)     3795 2023-04-20 15:24:38.000000 django-utilitas-1.2.9/README.md
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-20 15:25:07.122295 django-utilitas-1.2.9/django_utilitas.egg-info/
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4040 2023-04-20 15:25:07.000000 django-utilitas-1.2.9/django_utilitas.egg-info/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-04-20 15:25:07.000000 django-utilitas-1.2.9/django_utilitas.egg-info/SOURCES.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-04-20 15:25:07.000000 django-utilitas-1.2.9/django_utilitas.egg-info/dependency_links.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-04-20 15:25:07.000000 django-utilitas-1.2.9/django_utilitas.egg-info/requires.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-04-20 15:25:07.000000 django-utilitas-1.2.9/django_utilitas.egg-info/top_level.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-04-20 15:25:07.133237 django-utilitas-1.2.9/setup.cfg
--rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.2.9/setup.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-20 15:25:07.131180 django-utilitas-1.2.9/utilitas/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.2.9/utilitas/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.2.9/utilitas/admin.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.2.9/utilitas/apps.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.2.9/utilitas/exception_handler.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.2.9/utilitas/exceptions.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.2.9/utilitas/managers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.2.9/utilitas/metadata.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.2.9/utilitas/middlewares.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-20 15:25:07.132058 django-utilitas-1.2.9/utilitas/migrations/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.2.9/utilitas/migrations/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1454 2022-12-05 07:25:03.000000 django-utilitas-1.2.9/utilitas/models.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.2.9/utilitas/pagination.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.2.9/utilitas/renderer.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.2.9/utilitas/serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.2.9/utilitas/swagger_query_params.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.2.9/utilitas/swagger_serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.2.9/utilitas/tests.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.2.9/utilitas/urls.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)    13342 2023-03-06 17:39:30.000000 django-utilitas-1.2.9/utilitas/views.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.511867 django-utilitas-1.3.0/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.0/LICENSE
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4209 2023-04-22 06:45:48.512078 django-utilitas-1.3.0/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     3964 2023-04-22 06:44:50.000000 django-utilitas-1.3.0/README.md
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.497208 django-utilitas-1.3.0/django_utilitas.egg-info/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4209 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/requires.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/top_level.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-04-22 06:45:48.513785 django-utilitas-1.3.0/setup.cfg
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.0/setup.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.510914 django-utilitas-1.3.0/utilitas/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/admin.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.0/utilitas/apps.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.0/utilitas/exception_handler.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.0/utilitas/exceptions.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.0/utilitas/managers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.0/utilitas/metadata.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.0/utilitas/middlewares.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.511430 django-utilitas-1.3.0/utilitas/migrations/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/migrations/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1454 2022-12-05 07:25:03.000000 django-utilitas-1.3.0/utilitas/models.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.0/utilitas/pagination.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.0/utilitas/renderer.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.0/utilitas/serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.0/utilitas/swagger_query_params.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.0/utilitas/swagger_serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/tests.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.0/utilitas/urls.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    13433 2023-04-22 06:43:45.000000 django-utilitas-1.3.0/utilitas/views.py
```

### Comparing `django-utilitas-1.2.9/LICENSE` & `django-utilitas-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/PKG-INFO` & `django-utilitas-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.2.9
+Version: 1.3.0
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -103,14 +103,16 @@
         model = Book
         fields = "__all__"
         list_serializer_class = BaseListSerializer
 ```
 
 ## Changelog
 
+- 1.3.0
+    - removed the need for `related_fields` parameter. Prefetching related fields is now done automatically using the `expand` parameter provided by the client.
 - 1.2.9
     - renamed file from `migrations.py` to `middlewares.py` (my stupid mistake in the first place)
 - 1.2.8
     - bug fixes
 - 1.2.7
     - bug fixes
 - 1.2.6
```

### Comparing `django-utilitas-1.2.9/README.md` & `django-utilitas-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -94,14 +94,16 @@
         model = Book
         fields = "__all__"
         list_serializer_class = BaseListSerializer
 ```
 
 ## Changelog
 
+- 1.3.0
+    - removed the need for `related_fields` parameter. Prefetching related fields is now done automatically using the `expand` parameter provided by the client.
 - 1.2.9
     - renamed file from `migrations.py` to `middlewares.py` (my stupid mistake in the first place)
 - 1.2.8
     - bug fixes
 - 1.2.7
     - bug fixes
 - 1.2.6
```

### Comparing `django-utilitas-1.2.9/django_utilitas.egg-info/PKG-INFO` & `django-utilitas-1.3.0/django_utilitas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.2.9
+Version: 1.3.0
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -103,14 +103,16 @@
         model = Book
         fields = "__all__"
         list_serializer_class = BaseListSerializer
 ```
 
 ## Changelog
 
+- 1.3.0
+    - removed the need for `related_fields` parameter. Prefetching related fields is now done automatically using the `expand` parameter provided by the client.
 - 1.2.9
     - renamed file from `migrations.py` to `middlewares.py` (my stupid mistake in the first place)
 - 1.2.8
     - bug fixes
 - 1.2.7
     - bug fixes
 - 1.2.6
```

### Comparing `django-utilitas-1.2.9/django_utilitas.egg-info/SOURCES.txt` & `django-utilitas-1.3.0/django_utilitas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/metadata.py` & `django-utilitas-1.3.0/utilitas/metadata.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/middlewares.py` & `django-utilitas-1.3.0/utilitas/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/models.py` & `django-utilitas-1.3.0/utilitas/models.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/pagination.py` & `django-utilitas-1.3.0/utilitas/pagination.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/serializers.py` & `django-utilitas-1.3.0/utilitas/serializers.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/swagger_query_params.py` & `django-utilitas-1.3.0/utilitas/swagger_query_params.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.2.9/utilitas/views.py` & `django-utilitas-1.3.0/utilitas/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     # query_params' names
     fields_param = "fields"
     sorts_param = "sorts"
     expand_param = "expand"
     # customizing the response format
     renderer_classes = [CustomRenderer, BrowsableAPIRenderer]
 
-    related_fields = []
 
     @classmethod
     def _validate_attributes(cls, **kwargs):
         for i in [{"var": "model", "parent_class": BaseModel},
                   {"var": "serializer", "parent_class": (BaseSerializer, BaseModelSerializer)}]:
 
             # making sure certain class variables are implemented.
@@ -87,17 +86,22 @@
 
         if fields is None:
             fields = []
 
         if expand is None:
             expand = []
         # query from the database
+
+        translated_expand = []
+        for i in expand:
+            translated_expand.append(i.replace(".", "__"))
+
         queryset = (
             self.model.objects.filter(**filter_params).exclude(**exclude_params)
-            .prefetch_related(*self.related_fields)
+            .prefetch_related(*translated_expand)
             .all()
             .order_by(*sorts)
         )
 
         # paginate the queryset
         paginated_data = self.paginate_queryset(queryset, request)
```

