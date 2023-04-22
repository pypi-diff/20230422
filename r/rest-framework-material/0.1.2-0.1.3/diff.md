# Comparing `tmp/rest_framework_material-0.1.2.tar.gz` & `tmp/rest_framework_material-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_material-0.1.2.tar", max compression
+gzip compressed data, was "rest_framework_material-0.1.3.tar", max compression
```

## Comparing `rest_framework_material-0.1.2.tar` & `rest_framework_material-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.2/LICENSE
--rw-r--r--   0        0        0      589 2023-04-22 06:05:51.348094 rest_framework_material-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.2/rest_framework_material/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.2/rest_framework_material/admin.py
--rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.2/rest_framework_material/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.2/rest_framework_material/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.2/rest_framework_material/models.py
--rw-r--r--   0        0        0    23726 2023-04-22 06:18:34.089471 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1181 2023-04-21 17:25:31.881402 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      643 2023-04-22 06:24:14.550903 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4252 2023-04-21 17:33:58.678317 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.2/rest_framework_material/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.2/rest_framework_material/views.py
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 rest_framework_material-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-21 17:36:10.988103 rest_framework_material-0.1.3/LICENSE
+-rw-r--r--   0        0        0      589 2023-04-22 06:33:55.596017 rest_framework_material-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-04-21 17:40:45.269789 rest_framework_material-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_material-0.1.3/rest_framework_material/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_material-0.1.3/rest_framework_material/admin.py
+-rw-r--r--   0        0        0      248 2023-04-21 17:38:09.789518 rest_framework_material-0.1.3/rest_framework_material/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_material-0.1.3/rest_framework_material/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_material-0.1.3/rest_framework_material/models.py
+-rw-r--r--   0        0        0    23726 2023-04-22 06:18:34.089471 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1181 2023-04-21 17:25:31.881402 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      682 2023-04-22 06:32:18.842409 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4252 2023-04-21 17:33:58.678317 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_material-0.1.3/rest_framework_material/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_material-0.1.3/rest_framework_material/views.py
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 rest_framework_material-0.1.3/PKG-INFO
```

### Comparing `rest_framework_material-0.1.2/LICENSE` & `rest_framework_material-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/pyproject.toml` & `rest_framework_material-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-material"
-version = "0.1.2"
+version = "0.1.3"
 description = "Redesign of the browsable api of Django REST Framework using MD Bootstrap"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_material"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_material-0.1.2/README.md` & `rest_framework_material-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/api.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/filters/base.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/filters/ordering.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/filters/search.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/filters/search.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 {% load i18n %}
 
 <h5>{% translate "Search" %}</h5>
 <form class="form-inline">
-  <div class="from-floating mb-4">
+  <div class="form-floating mb-4">
     <input
-      type="search"
       id="search"
+      type="search"
       class="form-control"
       name="{{ param }}"
       value="{{ term }}"
       placeholder="{% translate 'Type here to search...' %}"
     />
     <label for="search" class="form-label">
-      {% translate 'Search' %}
+      {% translate 'Type here to search...' %}
     </label>
   </div>
   <button class="btn btn-lg btn-primary w-100" type="submit">
-    <strong class="d-flex align-items-center gap-3">
+    <strong class="d-flex align-items-center justify-content-center gap-3">
       <i class="bi bi-search"></i>
       {% translate "Search" %}
     </strong>
   </button>
 </form>
```

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/input.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/radio.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/select.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/horizontal/textarea.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/login.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/pagination/numbers.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_material-0.1.3/rest_framework_material/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_material-0.1.2/PKG-INFO` & `rest_framework_material-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-material
-Version: 0.1.2
+Version: 0.1.3
 Summary: Redesign of the browsable api of Django REST Framework using MD Bootstrap
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

