# Comparing `tmp/vprikol_api_python-1.3.tar.gz` & `tmp/vprikol_api_python-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vprikol_api_python-1.3.tar", max compression
+gzip compressed data, was "vprikol_api_python-1.4.tar", max compression
```

## Comparing `vprikol_api_python-1.3.tar` & `vprikol_api_python-1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/README.md
--rw-r--r--   0        0        0      349 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/__init__.py
--rw-r--r--   0        0        0      921 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/api.py
--rw-r--r--   0        0        0     5567 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/main.py
--rw-r--r--   0        0        0     3704 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/model.py
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.3/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/README.md
+-rw-r--r--   0        0        0      349 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/__init__.py
+-rw-r--r--   0        0        0      921 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/api.py
+-rw-r--r--   0        0        0     5567 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/main.py
+-rw-r--r--   0        0        0     3703 2023-04-22 08:22:24.844596 vprikol_api_python-1.4/vprikol_api/model.py
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.4/PKG-INFO
```

### Comparing `vprikol_api_python-1.3/vprikol_api/api.py` & `vprikol_api_python-1.4/vprikol_api/api.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.3/vprikol_api/main.py` & `vprikol_api_python-1.4/vprikol_api/main.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.3/vprikol_api/model.py` & `vprikol_api_python-1.4/vprikol_api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class FastApiErrorResponse(BaseModel):
     detail: FastAPIErrorDetail | str
 
 
 class APIErrorResponse(BaseModel):
     error_code: int
-    message: str
+    detail: str
 
 
 class Response(GenericModel):
     data: DataT | None
     error: APIErrorResponse | FastApiErrorResponse | None
     success: bool = True
```

