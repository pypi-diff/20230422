# Comparing `tmp/wagtail-markdown-0.8.0.tar.gz` & `tmp/wagtail-markdown-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-markdown-0.8.0.tar", last modified: Fri Feb 25 18:23:08 2022, max compression
+gzip compressed data, was "wagtail-markdown-0.9.0.tar", last modified: Fri Jul  1 17:18:54 2022, max compression
```

## Comparing `wagtail-markdown-0.8.0.tar` & `wagtail-markdown-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-02-25 18:23:08.880529 wagtail-markdown-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7541 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-02-25 18:23:08.880529 wagtail-markdown-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.872529 wagtail-markdown-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-02-25 18:23:08.000000 wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-02-25 18:23:08.000000 wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 18:23:08.000000 wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-02-25 18:23:08.000000 wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-25 18:23:08.000000 wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/edit_handlers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1243 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linker/
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linkers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linkers/document.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linkers/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linkers/page.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/tables/
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.872529 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.872529 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/css/
--rw-r--r--   0 runner    (1001) docker     (121)    12518 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/css/easymde.min.css
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/css/easymde.tweaks.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1400 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.attach.js
--rw-r--r--   0 runner    (1001) docker     (121)   323416 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/markdown-textarea-adapter.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:08.876529 wagtail-markdown-0.8.0/src/wagtailmarkdown/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/templatetags/wagtailmarkdown.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5191 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-02-25 18:23:05.000000 wagtail-markdown-0.8.0/src/wagtailmarkdown/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.790602 wagtail-markdown-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-01 17:18:54.790602 wagtail-markdown-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8361 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-07-01 17:18:54.790602 wagtail-markdown-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.782601 wagtail-markdown-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-07-01 17:18:54.000000 wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-07-01 17:18:54.000000 wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-01 17:18:54.000000 wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-01 17:18:54.000000 wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-07-01 17:18:54.000000 wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtailmarkdown/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/edit_handlers.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      272 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linker/
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linkers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linkers/document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linkers/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linkers/page.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/tables/
+-rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.782601 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.782601 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.786602 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/css/
+-rw-r--r--   0 runner    (1001) docker     (121)    12518 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/css/easymde.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/css/easymde.tweaks.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.790602 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1480 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.attach.js
+-rw-r--r--   0 runner    (1001) docker     (121)   323416 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/markdown-textarea-adapter.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:54.790602 wagtail-markdown-0.9.0/src/wagtailmarkdown/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/templatetags/wagtailmarkdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4777 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-07-01 17:18:51.000000 wagtail-markdown-0.9.0/src/wagtailmarkdown/widgets.py
```

### Comparing `wagtail-markdown-0.8.0/CHANGELOG.md` & `wagtail-markdown-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
 ## Unreleased
 
+## [0.9.0] - 2022-07-01
+
+### Changed
+
+- `wagtailmarkdown.edit_handlers.MarkdownPanel` is deprecated and will be removed in the next minor version.
+  Use the Wagtail core `FieldPanel` instead.
+- Updated the easymde/codemirror setup logic.
+
+### Removed
+
+- Dropped support for Wagtail < 2.15
+- Removed long deprecated `wagtailmarkdown.fields.MarkdownBlock` import
+
 ## [0.8.0] - 2022-02-25
 
 ### Added
 - Add Wagtail 2.16 and Django 4.0 compatibility ([#94](https://github.com/torchbox/wagtail-markdown/pull/94))
 - Update to EasyMDE 2.16.1 ([#95](https://github.com/torchbox/wagtail-markdown/pull/95))
 
 ### Fixed
@@ -57,11 +70,12 @@
 ### 0.5a1 - 2017-12-7
 
 - Fix problem with app loading
 - Make it compatible with newer versions of Wagtail that require `context` parameters in blocks' `render_basic` method.
 - Restructure app, refactor code. Add depreciation warnings.
 
 
+[0.9.0]: https://github.com/torchbox/wagtail-markdown/releases/tag/v0.8.0
 [0.8.0]: https://github.com/torchbox/wagtail-markdown/releases/tag/v0.8.0
 [0.7.0]: https://github.com/torchbox/wagtail-markdown/releases/tag/0.7.0
 [0.6]: https://github.com/torchbox/wagtail-markdown/releases/tag/0.6
 [0.5]: https://github.com/torchbox/wagtail-markdown/releases/tag/0.5
```

### Comparing `wagtail-markdown-0.8.0/LICENSE` & `wagtail-markdown-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-markdown-0.8.0/PKG-INFO` & `wagtail-markdown-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 1.2
 Name: wagtail-markdown
-Version: 0.8.0
+Version: 0.9.0
 Summary: Markdown support for Wagtail
 Home-page: https://github.com/torchbox/wagtail-markdown
 Author: Felicity Tarnell
 Author-email: hello@torchbox.com
 Maintainer: Dan Braghis
 Maintainer-email: dan.braghis@torchbox.com
 License: zlib
 Project-URL: Changelog, https://github.com/torchbox/wagtail-markdown/blob/main/CHANGELOG.md
-Description: Provides Markdown page field and streamfield block for Wagtail. More info: https://github.com/torchbox/wagtail-markdown/blob/10b286a16ad9a37e4554f06bc3c08c7afb374855/README.md
+Description: Provides Markdown page field and streamfield block for Wagtail. More info: https://github.com/torchbox/wagtail-markdown/blob/4237fe933b4e7ad067bab2ec9270688e322eeee7/README.md
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
```

### Comparing `wagtail-markdown-0.8.0/README.md` & `wagtail-markdown-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -103,14 +103,40 @@
     )
     return format_html(elem)
 ```
 
 Note that due to the way EasyMDE defines the toolbar icons it is not compatible with
 [Wagtail FontAwesome](https://gitlab.com/alexgleason/wagtailfontawesome)
 
+##### Using with django-compressor
+
+You may have your own SCSS sources that you want to precompile on the fly.
+We can invoke django-compressor to fetch our Font Awesome SCSS sources like this:
+
+```python
+# Content of app_name/wagtail_hooks.py
+from compressor.css import CssCompressor
+from wagtail.core import hooks
+from django.conf import settings
+from django.utils.html import format_html
+
+
+@hooks.register("insert_global_admin_css")
+def import_fontawesome_stylesheet():
+    elem = '<link rel="stylesheet" type="text/x-scss" href="{}scss/fontawesome.scss">'.format(
+        settings.STATIC_URL
+    )
+    compressor = CssCompressor("css", content=elem)
+    output = ""
+    for s in compressor.hunks():
+        output += s
+    return format_html(output)
+```
+
+
 #### Markdown extensions - `extensions`/`extension_configs`
 
 You can configure wagtail-markdown to use additional Markdown extensions using the `extensions` setting.
 
 For example, to enable the [Table of Contents](https://python-markdown.github.io/extensions/toc/) and
 [Sane Lists](https://python-markdown.github.io/extensions/sane_lists/) extensions:
 
@@ -181,26 +207,26 @@
 ```
 
 <img src="https://i.imgur.com/4NFcfHd.png" width="728px" alt="">
 
 Or use as a page field:
 
 ```python
+from wagtail.admin.edit_handlers import FieldPanel
 from wagtail.core.models import Page
 
-from wagtailmarkdown.edit_handlers import MarkdownPanel
 from wagtailmarkdown.fields import MarkdownField
 
 
 class MyPage(Page):
     body = MarkdownField()
 
     content_panels = [
         FieldPanel("title", classname="full title"),
-        MarkdownPanel("body"),
+        FieldPanel("body"),
     ]
 ```
 
 And render the content in a template:
 
 ```html+django
 {% load wagtailmarkdown %}
@@ -208,14 +234,18 @@
 {{ self.body|markdown }}
 </article>
 ```
 
 <img src="https://i.imgur.com/Sj1f4Jh.png" width="728px" alt="">
 
 
+## Compatibility
+
+wagtail-markdown supports Wagtail 2.15 and above.
+
 ## Contributing
 
 All contributions are welcome!
 
 Note that this project uses [pre-commit](https://github.com/pre-commit/pre-commit). To set up locally:
 
 ```shell
```

### Comparing `wagtail-markdown-0.8.0/setup.py` & `wagtail-markdown-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-#! /usr/bin/env/python
-# vim:sw=4 ts=4 et:
-#
-# Copyright (c) 2015 Torchbox Ltd.
-# felicity@torchbox.com 2015-09-14
-#
-# Permission is granted to anyone to use this software for any purpose,
-# including commercial applications, and to alter it and redistribute it
-# freely. This software is provided 'as-is', without any express or implied
-# warranty.
-#
-
 import subprocess
 
 from setuptools import find_packages, setup
 
 
 def get_git_revision_hash():
     try:
@@ -27,40 +15,40 @@
 README = "https://github.com/torchbox/wagtail-markdown/blob/{hash}/README.md"
 README = README.format(hash=get_git_revision_hash())
 
 
 INSTALL_REQUIRES = [
     "Markdown>=3,<4",
     "bleach>=3.3.0,<4",
-    "Wagtail>=2.0",
+    "Wagtail>=2.15",
 ]
 
 
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: zlib/libpng License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Wagtail",
     "Framework :: Wagtail :: 2",
+    "Framework :: Wagtail :: 3",
 ]
 
 
 setup(
     name="wagtail-markdown",
-    version="0.8.0",
+    version="0.9.0",
     description="Markdown support for Wagtail",
     long_description="Provides Markdown page field and streamfield block for "
     "Wagtail. More info: {}".format(README),
     author="Felicity Tarnell",
     author_email="hello@torchbox.com",
     maintainer="Dan Braghis",
     maintainer_email="dan.braghis@torchbox.com",
```

### Comparing `wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/PKG-INFO` & `wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 1.2
 Name: wagtail-markdown
-Version: 0.8.0
+Version: 0.9.0
 Summary: Markdown support for Wagtail
 Home-page: https://github.com/torchbox/wagtail-markdown
 Author: Felicity Tarnell
 Author-email: hello@torchbox.com
 Maintainer: Dan Braghis
 Maintainer-email: dan.braghis@torchbox.com
 License: zlib
 Project-URL: Changelog, https://github.com/torchbox/wagtail-markdown/blob/main/CHANGELOG.md
-Description: Provides Markdown page field and streamfield block for Wagtail. More info: https://github.com/torchbox/wagtail-markdown/blob/10b286a16ad9a37e4554f06bc3c08c7afb374855/README.md
+Description: Provides Markdown page field and streamfield block for Wagtail. More info: https://github.com/torchbox/wagtail-markdown/blob/4237fe933b4e7ad067bab2ec9270688e322eeee7/README.md
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: zlib/libpng License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
```

### Comparing `wagtail-markdown-0.8.0/src/wagtail_markdown.egg-info/SOURCES.txt` & `wagtail-markdown-0.9.0/src/wagtail_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linker/__init__.py` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linker/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,41 @@
-# vim:sw=4 ts=4 et:
-# Copyright (c) 2015 Torchbox Ltd.
-# felicity@torchbox.com 2015-09-14
-#
-# Permission is granted to anyone to use this software for any purpose,
-# including commercial applications, and to alter it and redistribute it
-# freely. This software is provided 'as-is', without any express or implied
-# warranty.
-#
 from importlib import import_module
 
-import markdown
+from markdown import Extension
+from markdown.inlinepatterns import Pattern
 
 
 LINKER_RE = r"<:([a-z]+:)?([^>|\n]+)((\|[^>|\n]+){0,})>"
 
 
-class LinkerPattern(markdown.inlinepatterns.Pattern):
+class LinkerPattern(Pattern):
     def __init__(self, re, md, linktypes):
-        markdown.inlinepatterns.Pattern.__init__(self, re, md)
+        super().__init__(re, md)
         self.linktypes = linktypes
 
     def handleMatch(self, m):
         linktypes = self.linktypes
         opts = []
         if m.group(3) is not None and len(m.group(4)):
             opts = m.group(4).split("|")[1:]
 
-        type = m.group(2)
-        if type is None:
-            type = "__default__"
-        mod = import_module(linktypes[type])
+        link_type = m.group(2)
+        if link_type is None:
+            link_type = "__default__"
+        mod = import_module(linktypes[link_type])
         c = mod.Linker()
 
         return c.run(m.group(3), opts)
         return "[invalid link]"
 
 
-class LinkerExtension(markdown.Extension):
+class LinkerExtension(Extension):
     def __init__(self, linktypes):
-        markdown.Extension.__init__(self)
+        super().__init__()
         self.linktypes = linktypes
 
-    def extendMarkdown(self, md, md_globals):
+    def extendMarkdown(self, md):
         md.inlinePatterns["linker"] = LinkerPattern(LINKER_RE, md, self.linktypes)
 
 
 def makeExtension(configs=None):
     return LinkerExtension(configs=configs)
```

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/linkers/image.py` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/linkers/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-# vim:sw=4 ts=4 et:
-# Copyright (c) 2015 Torchbox Ltd.
-# felicity@torchbox.com 2015-09-14
-#
-# Permission is granted to anyone to use this software for any purpose,
-# including commercial applications, and to alter it and redistribute it
-# freely. This software is provided 'as-is', without any express or implied
-# warranty.
-#
 from django.core.exceptions import MultipleObjectsReturned, ObjectDoesNotExist
 
-from markdown.util import etree
-
+from wagtail.images import get_image_model
 
-try:  # wagtail < 2.0
-    from wagtail.wagtailimages import get_image_model
-except ImportError:  # wagtail >= 2.0
-    from wagtail.images import get_image_model
+from markdown.util import etree
 
 
 # TODO: Default spec and class should be configurable, because they're
 # dependent on how the project is set up.  Hard-coding of 'left',
 # 'right' and 'full-width' should be removed.
```

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/mdx/tables/__init__.py` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/mdx/tables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,14 @@
                 row = row[:-1]
         return row.split("|")
 
 
 class TableExtension(Extension):
     """Add tables to Markdown."""
 
-    def extendMarkdown(self, md, md_globals):
+    def extendMarkdown(self, md):
         """Add an instance of TableProcessor to BlockParser."""
         md.parser.blockprocessors.add("table", TableProcessor(md.parser), "<hashheader")
 
 
 def makeExtension(configs=None):
     return TableExtension(configs=configs)
```

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/css/easymde.min.css` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/css/easymde.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.attach.js` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.attach.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 /*
  * vim:sw=4 ts=4 et:
- * Copyright (c) 2015 Torchbox Ltd.
- * felicity@torchbox.com 2015-09-14
+ * Copyright (c) 2015-present Torchbox Ltd.
+ * hello@torchbox.com
  *
  * Permission is granted to anyone to use this software for any purpose,
  * including commercial applications, and to alter it and redistribute it
  * freely. This software is provided 'as-is', without any express or implied
  * warranty.
  */
 
@@ -20,32 +20,36 @@
     });
     mde.render();
 
     // Save the codemirror instance on the original html element for later use.
     mde.element.codemirror = mde.codemirror;
 
     mde.codemirror.on("change", function() {
-        $('#' + id).val(mde.value());
+        document.getElementById(id).value = mde.value();
     });
 }
 
+
 /*
- * Used to initialize Simple MDE when MarkdownFields are used on a page.
+ * Used to initialize content when MarkdownFields are used in admin panels.
  */
-$(document).ready(function() {
-    $(".object.markdown textarea").each(function(index, elem) {
-        easymdeAttach(elem.id);
+function refreshCodeMirror(e) {
+    setTimeout(
+        function() {
+            e.CodeMirror.refresh();
+        }, 100
+    );
+}
+
+// Wagtail < 3.0
+document.addEventListener('shown.bs.tab', function() {
+    document.querySelectorAll('.CodeMirror').forEach(function(e) {
+        refreshCodeMirror(e)
     });
 });
 
-/*
- * Used to initialize content when MarkdownFields are used in admin panels.
- */
-$(document).on('shown.bs.tab', function(e) {
-    $('.CodeMirror').each(function(i, el) {
-        setTimeout(
-            function() {
-                el.CodeMirror.refresh();
-            }, 100
-        );
+// Wagtail >= 3.0
+document.addEventListener('wagtail:tab-changed', function() {
+    document.querySelectorAll('.CodeMirror').forEach(function(e) {
+        refreshCodeMirror(e)
     });
 });
```

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.min.js` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/easymde.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-markdown-0.8.0/src/wagtailmarkdown/static/wagtailmarkdown/js/markdown-textarea-adapter.js` & `wagtail-markdown-0.9.0/src/wagtailmarkdown/static/wagtailmarkdown/js/markdown-textarea-adapter.js`

 * *Files identical despite different names*

