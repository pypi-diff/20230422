# Comparing `tmp/fastapi_mvc_framework-1.2.3.tar.gz` & `tmp/fastapi_mvc_framework-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.2.3.tar", last modified: Fri Apr 21 08:11:39 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.2.4.tar", last modified: Sat Apr 22 11:28:03 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.2.3.tar` & `fastapi_mvc_framework-1.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:11:39.296298 fastapi_mvc_framework-1.2.3/
--rw-rw-rw-   0        0        0     6592 2023-04-21 08:11:39.294304 fastapi_mvc_framework-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5785 2023-04-21 08:11:39.000000 fastapi_mvc_framework-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 08:11:39.284330 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      267 2023-04-10 12:07:43.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0     1751 2023-04-13 05:28:34.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0    10362 2023-04-18 05:30:28.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0    10336 2023-04-19 06:43:16.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     4355 2023-04-18 14:40:31.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     4182 2023-04-18 06:15:50.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    13008 2023-04-18 15:41:45.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    12417 2023-04-21 06:50:57.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/database.py
--rw-rw-rw-   0        0        0     7615 2023-04-21 07:20:04.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:11:39.293305 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     6592 2023-04-21 08:11:39.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-04-21 08:11:39.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:11:39.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      753 2023-04-21 08:11:39.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-21 08:11:39.000000 fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 08:11:39.296298 fastapi_mvc_framework-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2612 2023-04-21 08:10:58.000000 fastapi_mvc_framework-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 11:28:03.611656 fastapi_mvc_framework-1.2.4/
+-rw-rw-rw-   0        0        0     6797 2023-04-22 11:28:03.610659 fastapi_mvc_framework-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5990 2023-04-22 11:28:03.000000 fastapi_mvc_framework-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 11:28:03.603678 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      274 2023-04-21 10:08:22.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0     1751 2023-04-13 05:28:34.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0    10559 2023-04-22 10:44:30.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0    10336 2023-04-19 06:43:16.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     4355 2023-04-18 14:40:31.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     4182 2023-04-18 06:15:50.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    12565 2023-04-22 10:37:38.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    12485 2023-04-22 10:57:52.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     6280 2023-04-19 08:32:59.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/database.py
+-rw-rw-rw-   0        0        0     7615 2023-04-21 07:20:04.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-22 11:28:03.609662 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     6797 2023-04-22 11:28:03.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-04-22 11:28:03.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 11:28:03.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      753 2023-04-22 11:28:03.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-22 11:28:03.000000 fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 11:28:03.611656 fastapi_mvc_framework-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2612 2023-04-22 11:26:49.000000 fastapi_mvc_framework-1.2.4/setup.py
```

### Comparing `fastapi_mvc_framework-1.2.3/PKG-INFO` & `fastapi_mvc_framework-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_mvc_framework
-Version: 1.2.3
+Version: 1.2.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -91,32 +91,32 @@
         text = "Hello World! I'm in FastapiMvcFramework"
         routers_map = application.routers_map
         routers = application.routes 
         return self.view()
     
     @api.get("/xml",auth='user')
     def get_legacy_data(self):
-        """:title XML(Protected)"""
+        """:title XML(only bruce)"""
 
         data = """<?xml version="1.0"?>
         <shampoo>
         <Header>
             Apply shampoo here.
         </Header>
         <Body>
             You'll have to use soap here.
         </Body>
         </shampoo>
         """
         return self.view(content=data,media_type="application/xml")
           
-    @api.get("/chatgpt")
+    @api.get("/chatgpt",auth="user")
     def chatgpt(self):
         """
-        :title Chat
+        :title Chat(only alice)
         """
         return self.view()
 
 
  
  
 websockets:Dict[str,WebSocket] = {}
@@ -160,24 +160,28 @@
     <meta charset="utf-8">
     <title>FastApi MVC Framework</title>
     <link rel="stylesheet" href="home.css" />
 
 </head>
 
 <body>
-    <header>
-        <h1>Hello Python</h1>
+    <header style="text-align:left;display: flex;">
+        <h1>Python</h1>
+        <h4>on FastApi</h4>
+
     </header>
     <nav>
-        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endfor %}
+        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
+        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b> Logout</a> {% endif %}
+        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+                Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
         <p>here is the `text` variable in class method:{{text}}</p>
         <p style="color:red"><b>{{flash}}</b></p>
     </section>
```

### Comparing `fastapi_mvc_framework-1.2.3/README.md` & `fastapi_mvc_framework-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,32 +71,32 @@
         text = "Hello World! I'm in FastapiMvcFramework"
         routers_map = application.routers_map
         routers = application.routes 
         return self.view()
     
     @api.get("/xml",auth='user')
     def get_legacy_data(self):
-        """:title XML(Protected)"""
+        """:title XML(only bruce)"""
 
         data = """<?xml version="1.0"?>
         <shampoo>
         <Header>
             Apply shampoo here.
         </Header>
         <Body>
             You'll have to use soap here.
         </Body>
         </shampoo>
         """
         return self.view(content=data,media_type="application/xml")
           
-    @api.get("/chatgpt")
+    @api.get("/chatgpt",auth="user")
     def chatgpt(self):
         """
-        :title Chat
+        :title Chat(only alice)
         """
         return self.view()
 
 
  
  
 websockets:Dict[str,WebSocket] = {}
@@ -140,24 +140,28 @@
     <meta charset="utf-8">
     <title>FastApi MVC Framework</title>
     <link rel="stylesheet" href="home.css" />
 
 </head>
 
 <body>
-    <header>
-        <h1>Hello Python</h1>
+    <header style="text-align:left;display: flex;">
+        <h1>Python</h1>
+        <h4>on FastApi</h4>
+
     </header>
     <nav>
-        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endfor %}
+        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
+        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b> Logout</a> {% endif %}
+        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+                Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
         <p>here is the `text` variable in class method:{{text}}</p>
         <p style="color:red"><b>{{flash}}</b></p>
     </section>
```

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from starlette.authentication import AuthenticationBackend, AuthenticationError, SimpleUser, AuthCredentials,BaseUser
 from starlette.middleware.authentication import AuthenticationMiddleware
 from starlette.authentication import BaseUser,SimpleUser,UnauthenticatedUser
 from casbin.persist.adapters import FileAdapter
 from casbin.persist.adapter import Adapter
 # from .midware_casbin import CasbinMiddleware
  
-from .config import config
+from .config import config,_log
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
+AUTH_EXPIRED='[EXPIRED]!'
+
 _session_name:str = ""
 class AuthenticationBackend_(AuthenticationBackend):
     def create_access_token(self,**kwargs):
         raise NotImplementedError()
     def clear_userinfo(self,request:Request):
         raise NotImplementedError()
     pass
@@ -60,28 +62,29 @@
                 scheme, credentials = auth.split() 
                 token = self.__get_token_from_header(authorization=auth, prefix=prefix)
                 
                 del kwargs['username_field']
                 try:
                     payload = jwt.decode(token,**kwargs)
                 except jwt.InvalidTokenError as e:
+                    _log.debug('token:'+token + ' has been expired.')
                     request.session[self.__session_name] = None
                     return "","",None
                 if is_datetime_format(payload['exp']):
                     payload['exp'] = datetime.fromisoformat(payload['exp'])
 
 
                 return  payload[username_field],token,payload
             elif userobj:
                 if 'token' in userobj:
                     try:
                         payload = jwt.decode(userobj['token'],**kwargs)
                     except jwt.InvalidTokenError as e:#Signature has expired
                         request.session[self.__session_name] = None
-                        return "","",None
+                        return AUTH_EXPIRED,AUTH_EXPIRED,None
                         # raise AuthenticationError(str(e)) from e
                      
                     return  payload[username_field],userobj['token'],payload
         else:
             if userobj: 
                 return userobj,"",None
             else:
@@ -157,14 +160,16 @@
         auth_type:str = kwargs.get("auth_type")
 
         args = {'username_field':self.username_field, 'key':self.secret_key, 'algorithms': self.algorithm , 'audience':self.audience ,
                                             'options':self.options }
         userobj,token,payload = _casbin_auth.get_user_from_request(request=request,
                                                                  prefix=self.prefix, 
                                                                  is_jwt=True,**args)
+        if token==AUTH_EXPIRED:
+            return False,AUTH_EXPIRED
          
         user = userobj#SimpleUser(userobj['username'])
         request.scope['user'] = user
         if  auth_type.lower()=='public': 
             if userobj:
                 if hasattr(userobj,'token') or token or payload:
                     if payload and token:
```

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/controller_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -294,39 +294,31 @@
 
 def _route_method(path: str, method, *args, **mwargs): 
     if not path.startswith("/"):
         raise "path must start with '/'"
     def wrapper(func ): 
         @wraps(func)
         async def decorator(  *args, **kwargs):
-            # 获取当前方法的名称
-            # method_name = inspect.currentframe().f_code.co_name
-            # # 获取当前方法的对象
-            # method_obj = inspect.currentframe().f_back.f_locals.get(method_name)
-            # print("当前方法名称为：", method_name)
-            # print("当前方法对象为：", method_obj)
             auth_type:str = getattr(func,AUTH_KEY) 
             has_request = kwargs.get("__has_request__")
             has_response = kwargs.get("__has_response__")
             module = inspect.getmodule(func)
-            cls = getattr(module, func.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0])
-            
+            cls = getattr(module, func.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0]) 
             #it's not instanced yet
             #instance = cls.__dict__.get('__wrapped__', None).__self__ #or cls.__dict__.get('__objclass__', None)(obj)
             response:Response = None
             result:Response = None
             
             if 'request' in kwargs and 'response' in kwargs:
                 response  = kwargs["response"]
                 rqst = kwargs['request']  
                 #auth first then call constructor
                 if auth_type and auth_type !="none"  :
                     auth_result,user = await cls._auth__(request=rqst,response=kwargs['response'],auth_type=auth_type)
-                    if isinstance(auth_result,Response):
-                        # __clear_flash(request=rqst)
+                    if isinstance(auth_result,Response): 
                         return auth_result
                     if not auth_result:
                         auth_error()
                 await cls._constructor(cls,request = kwargs['request'],response=kwargs['response'])
 
             if 'request' in kwargs and not has_request:  
                 del kwargs['request']  
@@ -335,23 +327,23 @@
             del kwargs["__has_request__"]
             del kwargs["__has_response__"]
             if inspect.iscoroutinefunction(func):
                 result = await func(*args, **kwargs)
             else:
                 result =  func(*args,**kwargs)
             if isinstance(result,tuple):result = result[0]
-            if response and isinstance(result,Response):
-                
+            if response and isinstance(result,Response): 
                 result.raw_headers.extend(response.raw_headers)
             if isinstance(result,Response):
                 ret = await cls._deconstructor(cls,result)
                 if isinstance(ret,Response):
                     result = ret
-            # __clear_flash(request=rqst)
-            return result
+ 
+            return result #end of decorator
+            
         setattr(decorator, PATH_KEY, path)
         setattr(decorator, METHOD_KEY, method)
         setattr(decorator, ARGS_KEY, args)
         if '__auth_url__' in mwargs: 
             setattr(func,'__auth_url__',mwargs['__auth_url__'])
             del mwargs['__auth_url__']
 
@@ -366,13 +358,13 @@
     return wrapper
 
 def get_docs(doc:str):
     ret = {}
     if doc:
         for line in doc.strip().split("\n"):
             if line.strip().startswith(":"):
-                parts = line.lstrip(":").split(" ")
+                parts = line.lstrip(":").split(" ",maxsplit=1)
                 if len(parts) == 2:
                     key, value = parts 
                     if value: 
                         ret[key] = value
     return ret
```

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 import time,os,inspect,datetime
 from typing import Any,Dict
 
-from fastapi import (FastAPI,
-                     UploadFile,
-                     File,Header, 
-                     Depends,
-                     HTTPException,
+from fastapi import (FastAPI, 
                      Request,
                      Response,
-                     WebSocket,
-                     WebSocketDisconnect, 
-                     Cookie,
                      status as StateCodes)
  
 from .controller import create_controller,MvcRouter as api,   register_controllers_to_app 
 from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
 from .config import config,ROOT_PATH,_log
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
@@ -159,34 +152,39 @@
                 auth_type = kwargs['auth_type'] 
                 
                 if not hasattr(application,'authObj'):
                     return True,None
                 
                 kwargs['session'] = request.session  
                 ret,user = await application.authObj.authenticate(request,**kwargs)
+                if user==auth.AUTH_EXPIRED:
+                    request.session['flash']  = "your authencation has been expired!"  
+                    user = False
                 def add_redirect_param(url: str, redirect_url: str) -> str:
                     if "?" in url:
                         return url + "&redirect=" + redirect_url
                     else:
                         return url + "?redirect=" + redirect_url
                 accept_header = request.headers.get("Accept")
                 if user: #continue singture 
-                    application.authObj.create_access_token(user=user, expires_delta=None,request=request)
+                    if config.get("session").get('auto_refresh_token',True):
+                        application.authObj.create_access_token(user=user, expires_delta=None,request=request)
                 #
                 if not ret and not user: 
                     _log.debug(f'Failed Auth[type:{auth_type}] url:'+str(request.url))
                     if accept_header == "application/json":
                         return  ORJSONResponse(content={"message": "401 UNAUTHORIZED!"},
                                                    status_code=StateCodes.HTTP_401_UNAUTHORIZED),None
                     _auth_url = getattr(application,f"_{auth_type}_auth_url") if hasattr(application,f"_{auth_type}_auth_url") else None
 
                     if _auth_url: 
                         if 'flash' not in request.session:
                             request.session['flash']=''
-                        request.session['flash']  = "you are not authenticated,please login!"  
+                        if request.session['flash']=="":
+                            request.session['flash']  = "you are not authenticated,please login!"  
                         _auth_url = add_redirect_param(_auth_url,str(request.url))
                         return RedirectResponse(_auth_url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
                     else:  
                         return RedirectResponse('/',status_code=StateCodes.HTTP_303_SEE_OTHER),None
                 else:
                     _log.debug(f'Successed Auth[type:{auth_type}] Url:'+str(request.url)+',User:'+str(user))
                     return ret,user
```

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/database.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/database.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/midware.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mvc-framework
-Version: 1.2.3
+Version: 1.2.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -91,32 +91,32 @@
         text = "Hello World! I'm in FastapiMvcFramework"
         routers_map = application.routers_map
         routers = application.routes 
         return self.view()
     
     @api.get("/xml",auth='user')
     def get_legacy_data(self):
-        """:title XML(Protected)"""
+        """:title XML(only bruce)"""
 
         data = """<?xml version="1.0"?>
         <shampoo>
         <Header>
             Apply shampoo here.
         </Header>
         <Body>
             You'll have to use soap here.
         </Body>
         </shampoo>
         """
         return self.view(content=data,media_type="application/xml")
           
-    @api.get("/chatgpt")
+    @api.get("/chatgpt",auth="user")
     def chatgpt(self):
         """
-        :title Chat
+        :title Chat(only alice)
         """
         return self.view()
 
 
  
  
 websockets:Dict[str,WebSocket] = {}
@@ -160,24 +160,28 @@
     <meta charset="utf-8">
     <title>FastApi MVC Framework</title>
     <link rel="stylesheet" href="home.css" />
 
 </head>
 
 <body>
-    <header>
-        <h1>Hello Python</h1>
+    <header style="text-align:left;display: flex;">
+        <h1>Python</h1>
+        <h4>on FastApi</h4>
+
     </header>
     <nav>
-        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
-        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endfor %}
+        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %} {% if routers_map[item]['auth']=='none' or request.session['user'] %}
+        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc']
+                and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endif %} {% endfor %}
 
         <a href="#">About</a>
         <a href="#">Contact</a> {% if request.session['user'] %}
-        <a href="/user/logout"><b>{{request.session['user']['username']}}</b> Logout</a> {% endif %}
+        <a href="/user/logout"><b>{{request.session['user']['username']}}</b>
+                Logout</a> {% endif %}
     </nav>
     <section>
         <h2>Welcome to my website</h2>
         <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
         <p>here is the `text` variable in class method:{{text}}</p>
         <p style="color:red"><b>{{flash}}</b></p>
     </section>
```

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/fastapi_mvc_framework.egg-info/requires.txt` & `fastapi_mvc_framework-1.2.4/fastapi_mvc_framework.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.2.3/setup.py` & `fastapi_mvc_framework-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import chardet
 
-version = "1.2.3"
+version = "1.2.4"
 def update_readme(source,spec,content=""):
     assert source or content
 
     if not content:
         with open(source, 'r') as file:
             content = file.read()
     with open('README.md', 'r') as file:
```

