# Comparing `tmp/tkutils-1.1.0.tar.gz` & `tmp/tkutils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkutils-1.1.0.tar", max compression
+gzip compressed data, was "tkutils-1.1.1.tar", max compression
```

## Comparing `tkutils-1.1.0.tar` & `tkutils-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     2817 2023-04-13 15:35:19.622223 tkutils-1.1.0/README.md
--rwxr-xr-x   0        0        0      752 2023-04-22 21:02:30.094308 tkutils-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     3571 2023-04-22 21:02:32.868476 tkutils-1.1.0/src/tkutils/__init__.py
--rwxr-xr-x   0        0        0      101 2022-12-22 16:54:42.632637 tkutils-1.1.0/src/tkutils/__main__.py
--rwxr-xr-x   0        0        0       22 2023-04-22 21:02:32.870438 tkutils-1.1.0/src/tkutils/__version__.py
--rwxr-xr-x   0        0        0     9327 2023-01-16 21:22:40.730857 tkutils-1.1.0/src/tkutils/grid_layout.py
--rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.645734 tkutils-1.1.0/src/tkutils/helpers/__init__.py
--rwxr-xr-x   0        0        0     4316 2023-01-16 18:36:26.640113 tkutils-1.1.0/src/tkutils/helpers/event_provider.py
--rwxr-xr-x   0        0        0     5290 2023-01-16 18:38:03.163623 tkutils-1.1.0/src/tkutils/helpers/keysym.py
--rwxr-xr-x   0        0        0    10198 2023-04-22 18:41:55.827669 tkutils-1.1.0/src/tkutils/images.py
--rwxr-xr-x   0        0        0       37 2022-12-22 16:54:42.728682 tkutils-1.1.0/src/tkutils/menu_builder/__init__.py
--rwxr-xr-x   0        0        0     2261 2023-01-15 23:06:06.313331 tkutils-1.1.0/src/tkutils/menu_builder/bases.py
--rwxr-xr-x   0        0        0     5047 2023-01-16 18:40:13.861655 tkutils-1.1.0/src/tkutils/menu_builder/menu_builder.py
--rwxr-xr-x   0        0        0     8300 2023-01-16 18:42:42.691137 tkutils-1.1.0/src/tkutils/menu_builder/menu_builder_options.py
--rwxr-xr-x   0        0        0      220 2022-12-22 16:54:42.802957 tkutils-1.1.0/src/tkutils/two_way_binding/__init__.py
--rwxr-xr-x   0        0        0    28483 2023-04-22 20:11:30.692562 tkutils-1.1.0/src/tkutils/two_way_binding/binder.py
--rwxr-xr-x   0        0        0    13926 2023-04-22 18:41:55.830751 tkutils-1.1.0/src/tkutils/two_way_binding/binding_descriptor.py
--rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.814650 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/__init__.py
--rwxr-xr-x   0        0        0     9282 2023-04-22 18:41:55.832202 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_binder_config.py
--rwxr-xr-x   0        0        0    10709 2023-01-16 18:23:18.891984 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configuration.py
--rwxr-xr-x   0        0        0     2856 2022-12-22 16:54:42.849190 tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py
--rwxr-xr-x   0        0        0      565 2022-12-22 16:54:42.850410 tkutils-1.1.0/src/tkutils/two_way_binding/errors.py
--rwxr-xr-x   0        0        0       55 2022-12-22 16:54:42.863360 tkutils-1.1.0/src/tkutils/utilities/__init__.py
--rwxr-xr-x   0        0        0    12657 2022-12-22 16:54:42.896203 tkutils-1.1.0/src/tkutils/utilities/singleton_namespace.py
--rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 tkutils-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2817 2023-04-22 21:02:45.313791 tkutils-1.1.1/README.md
+-rwxr-xr-x   0        0        0      752 2023-04-22 21:26:35.451151 tkutils-1.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     3571 2023-04-22 21:26:38.075873 tkutils-1.1.1/src/tkutils/__init__.py
+-rwxr-xr-x   0        0        0      101 2022-12-22 16:54:42.632637 tkutils-1.1.1/src/tkutils/__main__.py
+-rwxr-xr-x   0        0        0       22 2023-04-22 21:26:38.077458 tkutils-1.1.1/src/tkutils/__version__.py
+-rwxr-xr-x   0        0        0     9327 2023-04-22 21:02:45.584732 tkutils-1.1.1/src/tkutils/grid_layout.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.645734 tkutils-1.1.1/src/tkutils/helpers/__init__.py
+-rwxr-xr-x   0        0        0     4316 2023-04-22 21:02:45.586456 tkutils-1.1.1/src/tkutils/helpers/event_provider.py
+-rwxr-xr-x   0        0        0     5290 2023-04-22 21:02:45.603352 tkutils-1.1.1/src/tkutils/helpers/keysym.py
+-rwxr-xr-x   0        0        0    10200 2023-04-22 21:22:04.762277 tkutils-1.1.1/src/tkutils/images.py
+-rwxr-xr-x   0        0        0       37 2022-12-22 16:54:42.728682 tkutils-1.1.1/src/tkutils/menu_builder/__init__.py
+-rwxr-xr-x   0        0        0     2261 2023-04-22 21:02:45.611159 tkutils-1.1.1/src/tkutils/menu_builder/bases.py
+-rwxr-xr-x   0        0        0     5047 2023-04-22 21:02:45.638271 tkutils-1.1.1/src/tkutils/menu_builder/menu_builder.py
+-rwxr-xr-x   0        0        0     8300 2023-04-22 21:02:45.643707 tkutils-1.1.1/src/tkutils/menu_builder/menu_builder_options.py
+-rwxr-xr-x   0        0        0      220 2022-12-22 16:54:42.802957 tkutils-1.1.1/src/tkutils/two_way_binding/__init__.py
+-rwxr-xr-x   0        0        0    28483 2023-04-22 21:02:45.645441 tkutils-1.1.1/src/tkutils/two_way_binding/binder.py
+-rwxr-xr-x   0        0        0    13926 2023-04-22 21:02:45.646758 tkutils-1.1.1/src/tkutils/two_way_binding/binding_descriptor.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.814650 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/__init__.py
+-rwxr-xr-x   0        0        0     9282 2023-04-22 21:09:36.221905 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_binder_config.py
+-rwxr-xr-x   0        0        0    10709 2023-04-22 21:02:45.672479 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configuration.py
+-rwxr-xr-x   0        0        0     3174 2023-04-22 21:15:09.528146 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py
+-rwxr-xr-x   0        0        0      565 2022-12-22 16:54:42.850410 tkutils-1.1.1/src/tkutils/two_way_binding/errors.py
+-rwxr-xr-x   0        0        0       55 2022-12-22 16:54:42.863360 tkutils-1.1.1/src/tkutils/utilities/__init__.py
+-rwxr-xr-x   0        0        0    12657 2022-12-22 16:54:42.896203 tkutils-1.1.1/src/tkutils/utilities/singleton_namespace.py
+-rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 tkutils-1.1.1/PKG-INFO
```

### Comparing `tkutils-1.1.0/README.md` & `tkutils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/pyproject.toml` & `tkutils-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tkutils"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python tkinter utilities."
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 license = "FreeBSD"
 readme = "README.md"
 repository = "https://gitlab.com/frederic.zinelli/tkutils"
 homepage = "http://frederic.zinelli.gitlab.io/tkutils/"
```

### Comparing `tkutils-1.1.0/src/tkutils/__init__.py` & `tkutils-1.1.1/src/tkutils/__init__.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/grid_layout.py` & `tkutils-1.1.1/src/tkutils/grid_layout.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/helpers/event_provider.py` & `tkutils-1.1.1/src/tkutils/helpers/event_provider.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/helpers/keysym.py` & `tkutils-1.1.1/src/tkutils/helpers/keysym.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/images.py` & `tkutils-1.1.1/src/tkutils/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 
 def images_factory(
     project_name:str,
     *path_to_images:str,
     any_file_in_project:str=None,
-    image_only:bool=True
+    image_only:bool=False,
 ):
     """ Build an image factory, digging through the project hierarchy to access the image files
         directly inside their location when using the returned factory function.
 
         Given the full path of `any_file_in_project` and the `project_name` of the root directory
         holding the project as well as the relative path segments to the location of the images,
         this function:
```

### Comparing `tkutils-1.1.0/src/tkutils/menu_builder/bases.py` & `tkutils-1.1.1/src/tkutils/menu_builder/bases.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/menu_builder/menu_builder.py` & `tkutils-1.1.1/src/tkutils/menu_builder/menu_builder.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/menu_builder/menu_builder_options.py` & `tkutils-1.1.1/src/tkutils/menu_builder/menu_builder_options.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/two_way_binding/binder.py` & `tkutils-1.1.1/src/tkutils/two_way_binding/binder.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/two_way_binding/binding_descriptor.py` & `tkutils-1.1.1/src/tkutils/two_way_binding/binding_descriptor.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_binder_config.py` & `tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_binder_config.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configuration.py` & `tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py` & `tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,38 +21,43 @@
     images_user_location: str = 'Not defined'
     build_image_from: Callable[ [str, IntOrNone, IntOrNone, IntOrNone],
                                 Tuple[PhotoImage, IntOrNone, IntOrNone] ] = None
 
     def configure_image_factory(
         project_name:str,
         *path_to_images:str,
-        any_file_in_project:str=None
+        any_file_in_project:str=None,
+        image_only=False,
     ):
         """ Configure the path to the directory holding images, to use `Binder.with_image`.
             The interface is the same as the one of `tk_image_from`:
 
             Parameters:
                 project_name:        Name of the root directory of the project
                 *path_to_images:     Path of subdirectories to the one containing the images.
                 any_file_in_project: To provide only if the `project_name` directory isn't in
                                      the path of the file of the caller.
+                image_only:          Define what the output of the factory function will be. If
+                                     True, only the image is returned, otherwise, it is a
+                                     `Tuple[image,width,height]`
 
             !!! tip
                 The location of the project is discovered through inspection of the call stack,
                 getting the filename of the caller of the function.
         """
         nonlocal build_image_from, images_user_location
 
         caller = any_file_in_project or inspect.stack()[1].filename
 
         images_user_location = os.path.join(project_name, *path_to_images)
         build_image_from     = images_factory(
             project_name,
             *path_to_images,
-            any_file_in_project=caller
+            any_file_in_project=caller,
+            image_only=image_only,
         )
 
 
     def reset_image_factory():
         """ Reset the factory image "data" (testing purpose only: not provided to the user) """
         nonlocal images_user_location, build_image_from
         images_user_location = 'Not defined'
@@ -78,14 +83,17 @@
     return (
         get_image_factory,
         get_image_factory_config_location,
         configure_image_factory,
         reset_image_factory
     )
 
+
+
+
 (
     get_image_factory,
     get_image_factory_config_location,
     configure_image_factory,
     reset_image_factory,
 
-)= __scoped_image_factory_definitions()
+) = __scoped_image_factory_definitions()
```

### Comparing `tkutils-1.1.0/src/tkutils/two_way_binding/errors.py` & `tkutils-1.1.1/src/tkutils/two_way_binding/errors.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/src/tkutils/utilities/singleton_namespace.py` & `tkutils-1.1.1/src/tkutils/utilities/singleton_namespace.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.0/PKG-INFO` & `tkutils-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkutils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python tkinter utilities.
 Home-page: http://frederic.zinelli.gitlab.io/tkutils/
 License: FreeBSD
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

