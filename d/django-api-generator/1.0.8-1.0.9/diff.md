# Comparing `tmp/django-api-generator-1.0.8.tar.gz` & `tmp/django-api-generator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-generator-1.0.8.tar", last modified: Tue Nov  1 03:21:23 2022, max compression
+gzip compressed data, was "django-api-generator-1.0.9.tar", last modified: Tue Feb 14 08:22:42 2023, max compression
```

## Comparing `django-api-generator-1.0.8.tar` & `django-api-generator-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.648058 django-api-generator-1.0.8/
--rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-api-generator-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      101 2022-10-21 06:48:01.000000 django-api-generator-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4707 2022-11-01 03:21:23.647036 django-api-generator-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3615 2022-11-01 03:19:24.000000 django-api-generator-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.576153 django-api-generator-1.0.8/django_api_gen/
--rw-rw-rw-   0        0        0      233 2022-10-20 16:53:05.000000 django-api-generator-1.0.8/django_api_gen/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.590154 django-api-generator-1.0.8/django_api_gen/api/
--rw-rw-rw-   0        0        0       78 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/api/__init__.py
--rw-rw-rw-   0        0        0      120 2022-10-21 04:40:05.000000 django-api-generator-1.0.8/django_api_gen/api/serializers.py
--rw-rw-rw-   0        0        0      167 2022-10-21 04:40:11.000000 django-api-generator-1.0.8/django_api_gen/api/urls.py
--rw-rw-rw-   0        0        0      351 2022-10-21 04:40:24.000000 django-api-generator-1.0.8/django_api_gen/api/views.py
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.601191 django-api-generator-1.0.8/django_api_gen/management/
--rw-rw-rw-   0        0        0       78 2022-10-20 15:04:06.000000 django-api-generator-1.0.8/django_api_gen/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.604155 django-api-generator-1.0.8/django_api_gen/management/commands/
--rw-rw-rw-   0        0        0       78 2022-10-21 16:31:14.000000 django-api-generator-1.0.8/django_api_gen/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4394 2022-10-22 08:22:11.000000 django-api-generator-1.0.8/django_api_gen/management/commands/generate-api.py
--rw-rw-rw-   0        0        0     4511 2022-10-21 16:30:41.000000 django-api-generator-1.0.8/django_api_gen/manager.py
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.617036 django-api-generator-1.0.8/django_api_gen/serializers/
--rw-rw-rw-   0        0        0       78 2022-10-20 15:04:06.000000 django-api-generator-1.0.8/django_api_gen/serializers/__init__.py
--rw-rw-rw-   0        0        0       43 2022-10-20 17:45:18.000000 django-api-generator-1.0.8/django_api_gen/serializers/base_imports
--rw-rw-rw-   0        0        0      135 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/serializers/base_serializer
--rw-rw-rw-   0        0        0       40 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/serializers/library_imports
--rw-rw-rw-   0        0        0       57 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/serializers/serializers_structure
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.625038 django-api-generator-1.0.8/django_api_gen/urls/
--rw-rw-rw-   0        0        0       78 2022-10-20 15:04:06.000000 django-api-generator-1.0.8/django_api_gen/urls/__init__.py
--rw-rw-rw-   0        0        0       27 2022-10-20 17:34:16.000000 django-api-generator-1.0.8/django_api_gen/urls/base_imports
--rw-rw-rw-   0        0        0       74 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/urls/base_urls_path
--rw-rw-rw-   0        0        0       87 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/urls/library_imports
--rw-rw-rw-   0        0        0       75 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/urls/urls_structure
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.633062 django-api-generator-1.0.8/django_api_gen/views/
--rw-rw-rw-   0        0        0       78 2022-10-20 15:04:06.000000 django-api-generator-1.0.8/django_api_gen/views/__init__.py
--rw-rw-rw-   0        0        0       31 2022-10-21 04:02:22.000000 django-api-generator-1.0.8/django_api_gen/views/base_imports
--rw-rw-rw-   0        0        0     2479 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/views/base_views
--rw-rw-rw-   0        0        0      271 2022-10-07 05:06:33.000000 django-api-generator-1.0.8/django_api_gen/views/library_imports
--rw-rw-rw-   0        0        0       69 2022-10-21 09:54:40.000000 django-api-generator-1.0.8/django_api_gen/views/views_structure
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.643040 django-api-generator-1.0.8/django_api_generator.egg-info/
--rw-rw-rw-   0        0        0     4707 2022-11-01 03:21:23.000000 django-api-generator-1.0.8/django_api_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1185 2022-11-01 03:21:23.000000 django-api-generator-1.0.8/django_api_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-01 03:21:23.000000 django-api-generator-1.0.8/django_api_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-21 17:30:45.000000 django-api-generator-1.0.8/django_api_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2022-11-01 03:21:23.000000 django-api-generator-1.0.8/django_api_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-11-01 03:21:23.000000 django-api-generator-1.0.8/django_api_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-01 03:21:23.645036 django-api-generator-1.0.8/docs/
--rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-api-generator-1.0.8/docs/blank.txt
--rw-rw-rw-   0        0        0       42 2022-11-01 03:21:23.648058 django-api-generator-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1394 2022-11-01 03:19:42.000000 django-api-generator-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.062404 django-api-generator-1.0.9/
+-rw-rw-rw-   0        0        0     1113 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      101 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4789 2023-02-14 08:22:42.062404 django-api-generator-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3697 2023-02-14 08:13:45.000000 django-api-generator-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.001372 django-api-generator-1.0.9/django_api_gen/
+-rw-rw-rw-   0        0        0      233 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.009369 django-api-generator-1.0.9/django_api_gen/api/
+-rw-rw-rw-   0        0        0       78 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/api/__init__.py
+-rw-rw-rw-   0        0        0      120 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/api/serializers.py
+-rw-rw-rw-   0        0        0      167 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/api/urls.py
+-rw-rw-rw-   0        0        0      351 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/api/views.py
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.011371 django-api-generator-1.0.9/django_api_gen/management/
+-rw-rw-rw-   0        0        0       78 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.014383 django-api-generator-1.0.9/django_api_gen/management/commands/
+-rw-rw-rw-   0        0        0       78 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4726 2023-02-14 08:11:00.000000 django-api-generator-1.0.9/django_api_gen/management/commands/generate-api.py
+-rw-rw-rw-   0        0        0     4511 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/manager.py
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.030389 django-api-generator-1.0.9/django_api_gen/serializers/
+-rw-rw-rw-   0        0        0       78 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/serializers/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/serializers/base_imports
+-rw-rw-rw-   0        0        0      135 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/serializers/base_serializer
+-rw-rw-rw-   0        0        0       40 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/serializers/library_imports
+-rw-rw-rw-   0        0        0       57 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/serializers/serializers_structure
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.039372 django-api-generator-1.0.9/django_api_gen/urls/
+-rw-rw-rw-   0        0        0       78 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/urls/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/urls/base_imports
+-rw-rw-rw-   0        0        0       74 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/urls/base_urls_path
+-rw-rw-rw-   0        0        0       87 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/urls/library_imports
+-rw-rw-rw-   0        0        0       75 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/urls/urls_structure
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.048370 django-api-generator-1.0.9/django_api_gen/views/
+-rw-rw-rw-   0        0        0       78 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/views/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/views/base_imports
+-rw-rw-rw-   0        0        0     2479 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/views/base_views
+-rw-rw-rw-   0        0        0      271 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/views/library_imports
+-rw-rw-rw-   0        0        0       69 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/django_api_gen/views/views_structure
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.059370 django-api-generator-1.0.9/django_api_generator.egg-info/
+-rw-rw-rw-   0        0        0     4789 2023-02-14 08:22:41.000000 django-api-generator-1.0.9/django_api_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1185 2023-02-14 08:22:41.000000 django-api-generator-1.0.9/django_api_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-14 08:22:41.000000 django-api-generator-1.0.9/django_api_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-14 08:22:41.000000 django-api-generator-1.0.9/django_api_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-02-14 08:22:41.000000 django-api-generator-1.0.9/django_api_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-02-14 08:22:41.000000 django-api-generator-1.0.9/django_api_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-14 08:22:42.060370 django-api-generator-1.0.9/docs/
+-rw-rw-rw-   0        0        0       13 2023-01-19 12:32:12.000000 django-api-generator-1.0.9/docs/blank.txt
+-rw-rw-rw-   0        0        0       42 2023-02-14 08:22:42.063369 django-api-generator-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-02-14 08:12:06.000000 django-api-generator-1.0.9/setup.py
```

### Comparing `django-api-generator-1.0.8/LICENSE.md` & `django-api-generator-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-api-generator-1.0.8/PKG-INFO` & `django-api-generator-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-generator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Django API generator over DRF
 Home-page: https://github.com/app-generator/django-api-generator
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -103,14 +103,16 @@
 
 <br />
 
 > **Step #5** - `Generate API` 
 
 ```bash
 $ python manage.py generate-api
+// OR 
+$ python manage.py generate-api -f # supress confirmation (forcing mode)
 ```
 
 The code is generated under the `api` folder in the ROOT of the project. At each iteration the **API code is overwritten**.
 
 <br />
 
 > **Step #6** - `Update routing`, include APIs
```

### Comparing `django-api-generator-1.0.8/README.md` & `django-api-generator-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 
 <br />
 
 > **Step #5** - `Generate API` 
 
 ```bash
 $ python manage.py generate-api
+// OR 
+$ python manage.py generate-api -f # supress confirmation (forcing mode)
 ```
 
 The code is generated under the `api` folder in the ROOT of the project. At each iteration the **API code is overwritten**.
 
 <br />
 
 > **Step #6** - `Update routing`, include APIs
```

### Comparing `django-api-generator-1.0.8/django_api_gen/management/commands/generate-api.py` & `django-api-generator-1.0.9/django_api_gen/management/commands/generate-api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
 
 class Command(BaseCommand):
     help = 'API Code generator'
 
+    def add_arguments(self, parser):
+        parser.add_argument(
+            '-f',
+            action='store_true',
+            help='Forcing Generate API for all models (no checks).',
+        )
+
     def handle(self, *args, **options):
 
         #################################################    
         # Validate settings
 
         # BASE_DIR -> ROOT or the project
         if not hasattr(settings, 'BASE_DIR'):
@@ -68,19 +75,24 @@
 
         #################################################    
         # User Confirmation
 
         self.stdout.write(f" > Configuration looks good.")
         self.stdout.write(f"   !!! The API folder will be overwritten !!! ")
 
-        answer = input("Continue? [Y/n]")
+        if options['f']:
 
-        if answer.upper() not in ["Y", "YES"]:
-            self.stdout.write(f"API generation cancelled.")
-            return 
+            self.stdout.write(f" > Generate API (forcing mode).")
+
+        else:
+            answer = input("Continue? [Y/n]")
+
+            if answer.upper() not in ["Y", "YES"]:
+                self.stdout.write(f"API generation cancelled.")
+                return 
 
         #################################################    
         # API folder - deleted at each cycle
         
         API_DIR        = os.path.join( settings.BASE_DIR, 'api' )
         API_FILE_INIT  = os.path.join( API_DIR, '__init__.py' )
         API_FILE_VIEWS = os.path.join( API_DIR, 'views.py' )
```

### Comparing `django-api-generator-1.0.8/django_api_gen/manager.py` & `django-api-generator-1.0.9/django_api_gen/manager.py`

 * *Files identical despite different names*

### Comparing `django-api-generator-1.0.8/django_api_gen/views/base_views` & `django-api-generator-1.0.9/django_api_gen/views/base_views`

 * *Files identical despite different names*

### Comparing `django-api-generator-1.0.8/django_api_generator.egg-info/PKG-INFO` & `django-api-generator-1.0.9/django_api_generator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-generator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Django API generator over DRF
 Home-page: https://github.com/app-generator/django-api-generator
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -103,14 +103,16 @@
 
 <br />
 
 > **Step #5** - `Generate API` 
 
 ```bash
 $ python manage.py generate-api
+// OR 
+$ python manage.py generate-api -f # supress confirmation (forcing mode)
 ```
 
 The code is generated under the `api` folder in the ROOT of the project. At each iteration the **API code is overwritten**.
 
 <br />
 
 > **Step #6** - `Update routing`, include APIs
```

### Comparing `django-api-generator-1.0.8/django_api_generator.egg-info/SOURCES.txt` & `django-api-generator-1.0.9/django_api_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-api-generator-1.0.8/setup.py` & `django-api-generator-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-api-generator',
-version='1.0.8',
+version='1.0.9',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Django API generator over DRF',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://github.com/app-generator/django-api-generator',
```

