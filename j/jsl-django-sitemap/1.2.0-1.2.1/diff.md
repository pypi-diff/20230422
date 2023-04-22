# Comparing `tmp/jsl_django_sitemap-1.2.0.tar.gz` & `tmp/jsl_django_sitemap-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsl_django_sitemap-1.2.0.tar", last modified: Sun Jan 16 04:33:51 2022, max compression
+gzip compressed data, was "dist/jsl_django_sitemap-1.2.1.tar", last modified: Sat Apr 22 12:16:35 2023, max compression
```

## Comparing `jsl_django_sitemap-1.2.0.tar` & `jsl_django_sitemap-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2022-01-16 04:33:51.016309 jsl_django_sitemap-1.2.0/
--rw-r--r--   0 dhananjay   (501) staff       (20)     1070 2021-05-18 08:59:11.000000 jsl_django_sitemap-1.2.0/LICENSE
--rw-r--r--   0 dhananjay   (501) staff       (20)      169 2021-05-18 06:49:38.000000 jsl_django_sitemap-1.2.0/MANIFEST.in
--rw-r--r--   0 dhananjay   (501) staff       (20)     4200 2022-01-16 04:33:51.016443 jsl_django_sitemap-1.2.0/PKG-INFO
--rw-r--r--   0 dhananjay   (501) staff       (20)     2979 2022-01-16 04:32:55.000000 jsl_django_sitemap-1.2.0/README.md
-drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2022-01-16 04:33:51.010813 jsl_django_sitemap-1.2.0/jsl_django_sitemap/
--rw-r--r--   0 dhananjay   (501) staff       (20)        0 2021-05-18 08:34:27.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/__init__.py
--rw-r--r--   0 dhananjay   (501) staff       (20)      109 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/apps.py
--rw-r--r--   0 dhananjay   (501) staff       (20)     1029 2021-05-23 09:46:25.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/default_settings.py
--rw-r--r--   0 dhananjay   (501) staff       (20)     2009 2021-05-27 11:39:35.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/jsl_sitemap_utils.py
-drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2022-01-16 04:33:51.015810 jsl_django_sitemap-1.2.0/jsl_django_sitemap/migrations/
--rw-r--r--   0 dhananjay   (501) staff       (20)        0 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/migrations/__init__.py
--rw-r--r--   0 dhananjay   (501) staff       (20)       57 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/models.py
--rw-r--r--   0 dhananjay   (501) staff       (20)       60 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/tests.py
--rw-r--r--   0 dhananjay   (501) staff       (20)      628 2021-05-18 07:22:54.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap/views.py
-drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2022-01-16 04:33:51.015054 jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/
--rw-r--r--   0 dhananjay   (501) staff       (20)     4200 2022-01-16 04:33:50.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (501) staff       (20)      521 2022-01-16 04:33:51.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (501) staff       (20)        1 2022-01-16 04:33:50.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (501) staff       (20)       12 2022-01-16 04:33:50.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (501) staff       (20)       19 2022-01-16 04:33:50.000000 jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/top_level.txt
--rw-r--r--   0 dhananjay   (501) staff       (20)      105 2022-01-16 04:33:51.017117 jsl_django_sitemap-1.2.0/setup.cfg
--rw-r--r--   0 dhananjay   (501) staff       (20)     2190 2022-01-16 04:32:55.000000 jsl_django_sitemap-1.2.0/setup.py
+drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2023-04-22 12:16:35.355470 jsl_django_sitemap-1.2.1/
+-rw-r--r--   0 dhananjay   (501) staff       (20)     1070 2021-05-18 08:59:11.000000 jsl_django_sitemap-1.2.1/LICENSE
+-rw-r--r--   0 dhananjay   (501) staff       (20)      169 2021-05-18 06:49:38.000000 jsl_django_sitemap-1.2.1/MANIFEST.in
+-rw-r--r--   0 dhananjay   (501) staff       (20)     4200 2023-04-22 12:16:35.355601 jsl_django_sitemap-1.2.1/PKG-INFO
+-rw-r--r--   0 dhananjay   (501) staff       (20)     2979 2022-03-02 11:05:57.000000 jsl_django_sitemap-1.2.1/README.md
+drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2023-04-22 12:16:35.351052 jsl_django_sitemap-1.2.1/jsl_django_sitemap/
+-rw-r--r--   0 dhananjay   (501) staff       (20)        0 2021-05-18 08:34:27.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/__init__.py
+-rw-r--r--   0 dhananjay   (501) staff       (20)      109 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/apps.py
+-rw-r--r--   0 dhananjay   (501) staff       (20)     1054 2023-04-22 12:08:51.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/default_settings.py
+-rw-r--r--   0 dhananjay   (501) staff       (20)     2008 2023-04-22 11:52:13.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/jsl_sitemap_utils.py
+drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2023-04-22 12:16:35.355261 jsl_django_sitemap-1.2.1/jsl_django_sitemap/migrations/
+-rw-r--r--   0 dhananjay   (501) staff       (20)        0 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/migrations/__init__.py
+-rw-r--r--   0 dhananjay   (501) staff       (20)       57 2021-05-18 06:48:08.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/models.py
+-rw-r--r--   0 dhananjay   (501) staff       (20)       33 2023-04-22 12:09:15.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/tests.py
+-rw-r--r--   0 dhananjay   (501) staff       (20)      919 2023-04-22 12:07:43.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap/views.py
+drwxr-xr-x   0 dhananjay   (501) staff       (20)        0 2023-04-22 12:16:35.354345 jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/
+-rw-r--r--   0 dhananjay   (501) staff       (20)     4200 2023-04-22 12:16:35.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (501) staff       (20)      521 2023-04-22 12:16:35.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (501) staff       (20)        1 2023-04-22 12:16:35.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (501) staff       (20)       12 2023-04-22 12:16:35.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (501) staff       (20)       19 2023-04-22 12:16:35.000000 jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/top_level.txt
+-rw-r--r--   0 dhananjay   (501) staff       (20)      105 2023-04-22 12:16:35.356342 jsl_django_sitemap-1.2.1/setup.cfg
+-rw-r--r--   0 dhananjay   (501) staff       (20)     2190 2022-03-02 11:06:22.000000 jsl_django_sitemap-1.2.1/setup.py
```

### Comparing `jsl_django_sitemap-1.2.0/LICENSE` & `jsl_django_sitemap-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsl_django_sitemap-1.2.0/PKG-INFO` & `jsl_django_sitemap-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: jsl_django_sitemap
-Version: 1.2.0
+Version: 1.2.1
 Summary: JSL Django Sitemap is a Django utility which iterates over all the url patterns in your main Django project and creates a ready to use sitemap. The sitemap.xml is useful in crawlers such as Google, Bing, Yahoo. We hope you like our app! Leave a star on our GitHub repository. Thanks!
 Home-page: https://github.com/JSoftwareLabs/jsl_django_sitemap
 Author: JSoftwareLabs.com
 Author-email: info@jsoftwarelabs.com
 License: MIT
-Download-URL: https://github.com/JSoftwareLabs/jsl_django_sitemap/archive/refs/tags/1.2.0.tar.gz
+Download-URL: https://github.com/JSoftwareLabs/jsl_django_sitemap/archive/refs/tags/1.2.1.tar.gz
 Keywords: Django sitemap,JSoftwareLabs,sitemap.xml,Django automated sitemaps
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
@@ -101,11 +101,11 @@
 
 Start the development server and visit http://127.0.0.1:8000/sitemap.xml
 
 -----
 
 ## Current Releases
 
-[1.2.0](https://github.com/JSoftwareLabs/jsl_django_sitemap/releases/tag/1.2.0)
+[1.2.1](https://github.com/JSoftwareLabs/jsl_django_sitemap/releases/tag/1.2.1)
```

### Comparing `jsl_django_sitemap-1.2.0/README.md` & `jsl_django_sitemap-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,9 +78,9 @@
 
 Start the development server and visit http://127.0.0.1:8000/sitemap.xml
 
 -----
 
 ## Current Releases
 
-[1.2.0](https://github.com/JSoftwareLabs/jsl_django_sitemap/releases/tag/1.2.0)
+[1.2.1](https://github.com/JSoftwareLabs/jsl_django_sitemap/releases/tag/1.2.1)
```

### Comparing `jsl_django_sitemap-1.2.0/jsl_django_sitemap/default_settings.py` & `jsl_django_sitemap-1.2.1/jsl_django_sitemap/default_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.conf import settings
 
 logger = logging.getLogger(__name__)
 FETCH_URL_FROM = "FETCH_URL_FROM"
 DEFAULT_FETCH_URL_FROM = "pattern"
 ENABLE = "ENABLE"
 INCLUDE_APPS = "INCLUDE_APPS"
+IGNORE_URL_PATTERNS = ()
 
 FETCH_URL_FROM_ALLOWED_PARAMS = ["name", "pattern"]
 
 
 def fetch_default_settings():
 	if getattr(settings, 'JSL_DJANGO_SITEMAP_SETTINGS', None) is None:
 		JSL_DJANGO_SITEMAP_SETTINGS = {
```

### Comparing `jsl_django_sitemap-1.2.0/jsl_django_sitemap/jsl_sitemap_utils.py` & `jsl_django_sitemap-1.2.1/jsl_django_sitemap/jsl_sitemap_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,12 +60,11 @@
 def get_django_urls(urlpatterns, default_settings=None):
 	if default_settings is None:
 		logger.error("Please set JSL_DJANGO_SITEMAP_SETTINGS in your Django settings")
 		return []
 	enable = default_settings.get('ENABLE')
 	include_apps = default_settings.get('INCLUDE_APPS')
 	if enable and include_apps is not None:
-
 		all_urls = filter_include_apps_in_url(urlpatterns, include_apps)
 		return list(iterate_over_django_urls(all_urls, default_settings))
 	else:
 		return []
```

### Comparing `jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/PKG-INFO` & `jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: jsl-django-sitemap
-Version: 1.2.0
+Version: 1.2.1
 Summary: JSL Django Sitemap is a Django utility which iterates over all the url patterns in your main Django project and creates a ready to use sitemap. The sitemap.xml is useful in crawlers such as Google, Bing, Yahoo. We hope you like our app! Leave a star on our GitHub repository. Thanks!
 Home-page: https://github.com/JSoftwareLabs/jsl_django_sitemap
 Author: JSoftwareLabs.com
 Author-email: info@jsoftwarelabs.com
 License: MIT
-Download-URL: https://github.com/JSoftwareLabs/jsl_django_sitemap/archive/refs/tags/1.2.0.tar.gz
+Download-URL: https://github.com/JSoftwareLabs/jsl_django_sitemap/archive/refs/tags/1.2.1.tar.gz
 Keywords: Django sitemap,JSoftwareLabs,sitemap.xml,Django automated sitemaps
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
@@ -101,11 +101,11 @@
 
 Start the development server and visit http://127.0.0.1:8000/sitemap.xml
 
 -----
 
 ## Current Releases
 
-[1.2.0](https://github.com/JSoftwareLabs/jsl_django_sitemap/releases/tag/1.2.0)
+[1.2.1](https://github.com/JSoftwareLabs/jsl_django_sitemap/releases/tag/1.2.1)
```

### Comparing `jsl_django_sitemap-1.2.0/jsl_django_sitemap.egg-info/SOURCES.txt` & `jsl_django_sitemap-1.2.1/jsl_django_sitemap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsl_django_sitemap-1.2.0/setup.py` & `jsl_django_sitemap-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 	long_description = f.read()
 
 setup(
 	name='jsl_django_sitemap',  # How you named your package folder (MyLib)
 	packages=setuptools.find_packages(),  # Chose the same as "name"
-	version='1.2.0',  # Start with a small number and increase it with every change you make
+	version='1.2.1',  # Start with a small number and increase it with every change you make
 	license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
 	description='JSL Django Sitemap is a Django utility which iterates over all the url patterns in your main Django project and creates a ready to use sitemap. The sitemap.xml is useful in crawlers such as Google, Bing, Yahoo. We hope you like our app! Leave a star on our GitHub repository. Thanks!',
 	# Give a short description about your library
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='JSoftwareLabs.com',  # Type in your name
 	author_email='info@jsoftwarelabs.com',  # Type in your E-Mail
 	url='https://github.com/JSoftwareLabs/jsl_django_sitemap',
 	# Provide either the link to your github or to your website
-	download_url='https://github.com/JSoftwareLabs/jsl_django_sitemap/archive/refs/tags/1.2.0.tar.gz',
+	download_url='https://github.com/JSoftwareLabs/jsl_django_sitemap/archive/refs/tags/1.2.1.tar.gz',
 	# I explain this later on
 	keywords=['Django sitemap', 'JSoftwareLabs', 'sitemap.xml', 'Django automated sitemaps'],
 	# Keywords that define your package best
 	install_requires=[  # I get to this in a second
 		'Django>=2.2',
 	],
 	include_package_data=True,
```

