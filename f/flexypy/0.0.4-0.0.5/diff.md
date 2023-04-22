# Comparing `tmp/flexypy-0.0.4.tar.gz` & `tmp/flexypy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.0.4.tar", last modified: Mon Apr 17 11:07:00 2023, max compression
+gzip compressed data, was "flexypy-0.0.5.tar", last modified: Sat Apr 22 16:53:47 2023, max compression
```

## Comparing `flexypy-0.0.4.tar` & `flexypy-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.347640 flexypy-0.0.4/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 11:07:00.347640 flexypy-0.0.4/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.339640 flexypy-0.0.4/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.4/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.4/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.4/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.4/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.4/flexypy/exceptions/extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.4/flexypy/exceptions/render.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.4/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.4/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.4/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.4/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.4/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.4/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.4/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.4/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.4/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.4/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.4/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      254 2023-04-17 08:31:23.000000 flexypy-0.0.4/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.4/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1168 2023-04-14 14:37:12.000000 flexypy-0.0.4/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2635 2023-04-17 09:53:46.000000 flexypy-0.0.4/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     8877 2023-04-17 11:05:48.000000 flexypy-0.0.4/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.4/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.343640 flexypy-0.0.4/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.4/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.4/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.4/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.4/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.347640 flexypy-0.0.4/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.4/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.4/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 11:07:00.339640 flexypy-0.0.4/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 11:07:00.000000 flexypy-0.0.4/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1200 2023-04-17 11:07:00.000000 flexypy-0.0.4/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-17 11:07:00.000000 flexypy-0.0.4/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-17 11:07:00.000000 flexypy-0.0.4/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-17 11:07:00.000000 flexypy-0.0.4/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-17 11:05:56.000000 flexypy-0.0.4/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-17 11:07:00.347640 flexypy-0.0.4/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.376408 flexypy-0.0.5/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-22 16:53:47.376408 flexypy-0.0.5/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.076403 flexypy-0.0.5/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.5/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.5/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.176405 flexypy-0.0.5/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.5/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.5/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.5/flexypy/exceptions/extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.5/flexypy/exceptions/render.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.5/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.5/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.236406 flexypy-0.0.5/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.5/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.5/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.5/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.248406 flexypy-0.0.5/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.5/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.5/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.264406 flexypy-0.0.5/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.5/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.280406 flexypy-0.0.5/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.5/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.5/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.5/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      197 2023-04-19 17:14:31.000000 flexypy-0.0.5/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.324407 flexypy-0.0.5/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.5/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2031 2023-04-22 16:10:45.000000 flexypy-0.0.5/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2635 2023-04-17 09:53:46.000000 flexypy-0.0.5/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     9967 2023-04-22 16:47:47.000000 flexypy-0.0.5/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.324407 flexypy-0.0.5/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.5/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.344407 flexypy-0.0.5/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.5/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.5/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.5/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.5/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.364408 flexypy-0.0.5/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.5/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.5/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-22 16:53:47.092404 flexypy-0.0.5/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-22 16:53:46.000000 flexypy-0.0.5/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1200 2023-04-22 16:53:46.000000 flexypy-0.0.5/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-22 16:53:46.000000 flexypy-0.0.5/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-22 16:53:46.000000 flexypy-0.0.5/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-22 16:53:46.000000 flexypy-0.0.5/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-22 16:53:29.000000 flexypy-0.0.5/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-22 16:53:47.376408 flexypy-0.0.5/setup.cfg
```

### Comparing `flexypy-0.0.4/flexypy/exceptions/web/server.py` & `flexypy-0.0.5/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.4/flexypy/generate_templates/generator.py` & `flexypy-0.0.5/flexypy/generate_templates/generator.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.4/flexypy/http/routing.py` & `flexypy-0.0.5/flexypy/http/routing.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.4/flexypy/http/server.py` & `flexypy-0.0.5/flexypy/http/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,22 @@
         self.server_address = util.application_uri(self.environ).replace(self.root_url, '')
         self.render: RenderTemplate = RenderTemplate()
         self.routes: list[Type[UserRoute]] = []
         self.router = None
         self.request = Request
         self._get_fxp_apps()
         self.router = Router(self.environ, self.routes, self.full_url)
+        self._set_server_cookie()
+
+    def _set_server_cookie(self):
+        try:
+            if 'HTTP_COOKIE' in self.environ:
+                self.request.set_server_cookie(self.environ['HTTP_COOKIE'])
+        except Exception as e:
+            pass
 
     def _route(self) -> HtmlResponse:
         path_found = False
         match self.environ['REQUEST_METHOD']:
             case 'GET':
                 if self.router.check_url():
                     path_found = True
@@ -61,14 +69,15 @@
 
                     mddl_app, mddl_redirect = self._run_middlewares(app)
                     if mddl_redirect:
                         if mddl_redirect.from_path and mddl_redirect.to_path:
                             if self.full_url == mddl_redirect.from_path:
                                 return self.render.render_redirect(mddl_redirect.to_path)
                     return self._method_get(mddl_app)
+
                 if self.router.check_static_file():
                     return self._method_get_static_files(self.router.check_static_file())
 
                 # If path not found
                 if not path_found:
                     t = PathNotFound(self.full_url, [self.server_address + i().get_path() for i in self.routes])
                     return self.render.render_traceback(t.code, t.html)
@@ -144,20 +153,40 @@
             for mddl in mddl_list:
                 m: Middleware = mddl(self.request, app)
                 m.start()
                 mddl_app = m.app
                 redirect = MddlRedirect(m.redirect_from, m.redirect_to)
         return [mddl_app, redirect]
 
+    def _set_cookie(self, header):
+        """
+        Set the cookies that the user writes to the request.
+        After the data is written to the header the field in the request is cleared.
+        """
+        if self.request.get_user_set_cookie():
+            header.extend(("set-cookie", morsel.OutputString())
+                          for morsel in self.request.get_user_set_cookie().values())
+            # clear request cookies
+            self.request.clear_request_cookie()
+
     def start(self):
         resp = self._route()
+
+        if 'HTTP_COOKIE' in self.environ:
+            self.request.set_server_cookie(self.environ['HTTP_COOKIE'])
         if resp:
+            # set header cookies
+            self._set_cookie(resp.header)
+
             self.start_response(resp.code, resp.header)
             return [resp.html]
         else:
+            mime_type = self.environ['SCRIPT_NAME']
+            header = [('Content-type', mime_type)]
+            self.start_response('404 Not found', header)
             return [b'']
 
     def _get_fxp_apps(self):
         for p in PATH_TO_FXP_APPS:
             import_path = p.replace('/', '.').strip('.') + '.fxp'
             importlib.import_module(import_path)
         self.routes = UserRoute.__subclasses__()
```

### Comparing `flexypy-0.0.4/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.0.5/flexypy/http/template/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.4/flexypy/http/template/extensions/template_ext.py` & `flexypy-0.0.5/flexypy/http/template/extensions/template_ext.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.4/flexypy/http/template/render.py` & `flexypy-0.0.5/flexypy/http/template/render.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.4/flexypy.egg-info/SOURCES.txt` & `flexypy-0.0.5/flexypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

