# Comparing `tmp/structure_py-0.1.1.tar.gz` & `tmp/structure_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structure_py-0.1.1.tar", last modified: Wed Apr 12 16:33:35 2023, max compression
+gzip compressed data, was "structure_py-0.3.0.tar", last modified: Sat Apr 22 00:59:26 2023, max compression
```

## Comparing `structure_py-0.1.1.tar` & `structure_py-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 16:33:26.000000 structure_py-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-12 16:33:35.827948 structure_py-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3377 2023-04-12 16:33:26.000000 structure_py-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:33:35.827948 structure_py-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-12 16:33:26.000000 structure_py-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.823948 structure_py-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4675 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/companies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/enrich_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/enrich_person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/list_employees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/list_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/list_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/login.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/me.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1536 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/search_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/operations/search_people.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2571 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7557 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/shared/person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2756 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/people.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-12 16:33:26.000000 structure_py-0.1.1/src/sdk/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:33:35.827948 structure_py-0.1.1/src/structure_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-12 16:33:35.000000 structure_py-0.1.1/src/structure_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-12 16:33:35.000000 structure_py-0.1.1/src/structure_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:33:35.000000 structure_py-0.1.1/src/structure_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 16:33:35.000000 structure_py-0.1.1/src/structure_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 16:33:35.000000 structure_py-0.1.1/src/structure_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.800268 structure_py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 00:59:17.000000 structure_py-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-22 00:59:26.800268 structure_py-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-04-22 00:59:17.000000 structure_py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:59:26.800268 structure_py-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-22 00:59:17.000000 structure_py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.796268 structure_py-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.796268 structure_py-0.3.0/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4614 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/companies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.796268 structure_py-0.3.0/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.800268 structure_py-0.3.0/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      705 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/enrich_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/enrich_person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/list_employees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1086 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/list_jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/list_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      981 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/login.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      483 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/me.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/search_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1530 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/operations/search_people.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.800268 structure_py-0.3.0/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2653 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7557 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/shared/person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/people.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.800268 structure_py-0.3.0/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-22 00:59:17.000000 structure_py-0.3.0/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:59:26.800268 structure_py-0.3.0/src/structure_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-22 00:59:26.000000 structure_py-0.3.0/src/structure_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-22 00:59:26.000000 structure_py-0.3.0/src/structure_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:59:26.000000 structure_py-0.3.0/src/structure_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-22 00:59:26.000000 structure_py-0.3.0/src/structure_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 00:59:26.000000 structure_py-0.3.0/src/structure_py.egg-info/top_level.txt
```

### Comparing `structure_py-0.1.1/LICENSE.md` & `structure_py-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/PKG-INFO` & `structure_py-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure_py
-Version: 0.1.1
+Version: 0.3.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -47,18 +47,15 @@
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
 
 req = operations.EnrichCompanyRequest(
-    country_code="corrupti",
-    headquarters="provident",
-    id="distinctio",
-    name="quibusdam",
+    id="89bd9d8d-69a6-474e-8f46-7cc8796ed151",
 )
     
 res = s.companies.enrich(req)
 
 if res.body is not None:
     # handle response
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure_py Version: 0.1.1 Summary: Python Client
+Metadata-Version: 2.1 Name: structure_py Version: 0.3.0 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
@@ -18,19 +18,18 @@
 offers authentication for your API requests with a token. ### OAuth2 with
 bearer token Authentication with the Structure API is using OAuth2. When
 establishing a connection using OAuth2, you will need your access token â you
 will find it in the [Structure dashboard](https://www.structure.ac/api_tokens)
 under API settings. ## SDK Example Usage  ```python import sdk from sdk.models
 import operations, shared s = sdk.SDK( security=shared.Security
 ( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), ) req =
-operations.EnrichCompanyRequest( country_code="corrupti",
-headquarters="provident", id="distinctio", name="quibusdam", ) res =
-s.companies.enrich(req) if res.body is not None: # handle response ```   ##
-Available Resources and Operations ### accounts * `list_users` - Show current
-user accounts ### companies * `enrich` - Enrich a company profile *
+operations.EnrichCompanyRequest( id="89bd9d8d-69a6-474e-8f46-7cc8796ed151", )
+res = s.companies.enrich(req) if res.body is not None: # handle response ```
+## Available Resources and Operations ### accounts * `list_users` - Show
+current user accounts ### companies * `enrich` - Enrich a company profile *
 `list_employees` - List company employees * `list_jobs` - List company jobs *
 `search` - Search Companies ### people * `enrich` - Enrich a person profile *
 `search` - Search People ### user * `login` - Login user * `me` - Show current
 user  ### Maturity This SDK is in beta, and there may be breaking changes
 between versions without a major version update. Therefore, we recommend
 pinning usage to a specific package version. This way, you can install the same
 version each time without breaking changes unless you are intentionally looking
```

### Comparing `structure_py-0.1.1/README.md` & `structure_py-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,18 +35,15 @@
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
 
 req = operations.EnrichCompanyRequest(
-    country_code="corrupti",
-    headquarters="provident",
-    id="distinctio",
-    name="quibusdam",
+    id="89bd9d8d-69a6-474e-8f46-7cc8796ed151",
 )
     
 res = s.companies.enrich(req)
 
 if res.body is not None:
     # handle response
 ```
```

#### html2text {}

```diff
@@ -14,19 +14,18 @@
 offers authentication for your API requests with a token. ### OAuth2 with
 bearer token Authentication with the Structure API is using OAuth2. When
 establishing a connection using OAuth2, you will need your access token â you
 will find it in the [Structure dashboard](https://www.structure.ac/api_tokens)
 under API settings. ## SDK Example Usage  ```python import sdk from sdk.models
 import operations, shared s = sdk.SDK( security=shared.Security
 ( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), ) req =
-operations.EnrichCompanyRequest( country_code="corrupti",
-headquarters="provident", id="distinctio", name="quibusdam", ) res =
-s.companies.enrich(req) if res.body is not None: # handle response ```   ##
-Available Resources and Operations ### accounts * `list_users` - Show current
-user accounts ### companies * `enrich` - Enrich a company profile *
+operations.EnrichCompanyRequest( id="89bd9d8d-69a6-474e-8f46-7cc8796ed151", )
+res = s.companies.enrich(req) if res.body is not None: # handle response ```
+## Available Resources and Operations ### accounts * `list_users` - Show
+current user accounts ### companies * `enrich` - Enrich a company profile *
 `list_employees` - List company employees * `list_jobs` - List company jobs *
 `search` - Search Companies ### people * `enrich` - Enrich a person profile *
 `search` - Search People ### user * `login` - Login user * `me` - Show current
 user  ### Maturity This SDK is in beta, and there may be breaking changes
 between versions without a major version update. Therefore, we recommend
 pinning usage to a specific package version. This way, you can install the same
 version each time without breaking changes unless you are intentionally looking
```

### Comparing `structure_py-0.1.1/setup.py` & `structure_py-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="structure_py",
-    version="0.1.1",
+    version="0.3.0",
     author="Structure",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `structure_py-0.1.1/src/sdk/accounts.py` & `structure_py-0.3.0/src/sdk/accounts.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/companies.py` & `structure_py-0.3.0/src/sdk/companies.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,20 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def enrich(self, request: operations.EnrichCompanyRequest) -> operations.EnrichCompanyResponse:
         r"""Enrich a company profile"""
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/companies/enrich'
+        url = utils.generate_url(operations.EnrichCompanyRequest, base_url, '/companies/{id}/enrich', request)
         
-        query_params = utils.get_query_params(operations.EnrichCompanyRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.EnrichCompanyResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
```

### Comparing `structure_py-0.1.1/src/sdk/models/operations/__init__.py` & `structure_py-0.3.0/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/models/operations/enrich_company.py` & `structure_py-0.3.0/src/sdk/models/operations/list_jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
-class EnrichCompanyRequest:
+class ListJobsRequest:
     
-    country_code: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'country_code', 'style': 'form', 'explode': True }})
-    r"""Country code of the company"""  
-    headquarters: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'headquarters', 'style': 'form', 'explode': True }})
-    r"""The headquarters of the company"""  
-    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""ID of the company"""  
-    name: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'name', 'style': 'form', 'explode': True }})
-    r"""Game of the company"""  
+    offset: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
+    r"""The offset number to start at"""  
+    per_page: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'per_page', 'style': 'form', 'explode': True }})
+    r"""Number of results per page (0-100)"""  
     
 
 @dataclasses.dataclass
-class EnrichCompanyResponse:
+class ListJobsResponse:
     
     content_type: str = dataclasses.field()  
     status_code: int = dataclasses.field()  
     body: Optional[bytes] = dataclasses.field(default=None)  
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `structure_py-0.1.1/src/sdk/models/operations/enrich_person.py` & `structure_py-0.3.0/src/sdk/models/operations/enrich_person.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests as requests_http
 from typing import Optional
 
 
 @dataclasses.dataclass
 class EnrichPersonRequest:
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'id', 'style': 'simple', 'explode': False }})
     r"""LinkedIn ID of the person"""  
     
 
 @dataclasses.dataclass
 class EnrichPersonResponse:
     
     content_type: str = dataclasses.field()
```

### Comparing `structure_py-0.1.1/src/sdk/models/operations/list_employees.py` & `structure_py-0.3.0/src/sdk/models/operations/list_employees.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/models/operations/login.py` & `structure_py-0.3.0/src/sdk/models/operations/login.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/models/operations/search_companies.py` & `structure_py-0.3.0/src/sdk/models/operations/search_people.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCompaniesApplicationJSON:
+class SearchPeopleApplicationJSON:
     
     filter: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filter'), 'exclude': lambda f: f is None }})
     r"""Filter for searching"""  
     limit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
     r"""Number of results per page (0-100)"""  
     page: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page'), 'exclude': lambda f: f is None }})
     r"""The offset number to start at"""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
     r"""Query for searching"""  
     
 
 @dataclasses.dataclass
-class SearchCompaniesResponse:
+class SearchPeopleResponse:
     
     content_type: str = dataclasses.field()  
     status_code: int = dataclasses.field()  
     body: Optional[bytes] = dataclasses.field(default=None)  
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `structure_py-0.1.1/src/sdk/models/operations/search_people.py` & `structure_py-0.3.0/src/sdk/models/operations/search_companies.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchPeopleApplicationJSON:
+class SearchCompaniesApplicationJSON:
     
     filter: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filter'), 'exclude': lambda f: f is None }})
     r"""Filter for searching"""  
     limit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
-    r"""Number of results per page (0-100)"""  
+    r"""Number of results per page (0-100) default 10"""  
     page: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page'), 'exclude': lambda f: f is None }})
     r"""The offset number to start at"""  
     query: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
     r"""Query for searching"""  
     
 
 @dataclasses.dataclass
-class SearchPeopleResponse:
+class SearchCompaniesResponse:
     
     content_type: str = dataclasses.field()  
     status_code: int = dataclasses.field()  
     body: Optional[bytes] = dataclasses.field(default=None)  
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `structure_py-0.1.1/src/sdk/models/shared/account.py` & `structure_py-0.3.0/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/models/shared/company.py` & `structure_py-0.3.0/src/sdk/models/shared/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     r"""The company's locations"""  
     logo: str = dataclasses.field()
     r"""URL to the company's logo"""  
     name: str = dataclasses.field()
     r"""The company's name"""  
     organization_type: str = dataclasses.field()
     r"""The type of organization"""  
+    profiles: list[str] = dataclasses.field()
+    r"""The company's profiles"""  
     region: str = dataclasses.field()
     r"""The comapny's headquarters region"""  
     similar: list[str] = dataclasses.field()
     r"""Similar companies to this company"""  
     slogan: str = dataclasses.field()
     r"""The company's slogan"""  
     specialities: str = dataclasses.field()
```

### Comparing `structure_py-0.1.1/src/sdk/models/shared/person.py` & `structure_py-0.3.0/src/sdk/models/shared/person.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/people.py` & `structure_py-0.3.0/src/sdk/people.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,20 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def enrich(self, request: operations.EnrichPersonRequest) -> operations.EnrichPersonResponse:
         r"""Enrich a person profile"""
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/people/enrich'
+        url = utils.generate_url(operations.EnrichPersonRequest, base_url, '/people/{id}/enrich', request)
         
-        query_params = utils.get_query_params(operations.EnrichPersonRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.EnrichPersonResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
```

### Comparing `structure_py-0.1.1/src/sdk/sdk.py` & `structure_py-0.3.0/src/sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     user: User
     r"""User"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.1.1"
-    _gen_version: str = "2.17.9"
+    _sdk_version: str = "0.3.0"
+    _gen_version: str = "2.20.1"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `structure_py-0.1.1/src/sdk/user.py` & `structure_py-0.3.0/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/utils/retries.py` & `structure_py-0.3.0/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.1.1/src/sdk/utils/utils.py` & `structure_py-0.3.0/src/sdk/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,70 +148,79 @@
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        if param_metadata.get('style', 'simple') == 'simple':
-            param = getattr(
-                path_params, field.name) if path_params is not None else None
-            param = _populate_from_globals(
-                field.name, param, 'pathParam', gbls)
-
-            if param is None:
-                continue
-
-            if isinstance(param, list):
-                pp_vals: list[str] = []
-                for pp_val in param:
-                    if pp_val is None:
-                        continue
-                    pp_vals.append(_val_to_string(pp_val))
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif isinstance(param, dict):
-                pp_vals: list[str] = []
-                for pp_key in param:
-                    if param[pp_key] is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{pp_key}={_val_to_string(param[pp_key])}")
-                    else:
-                        pp_vals.append(
-                            f"{pp_key},{_val_to_string(param[pp_key])}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif not isinstance(param, (str, int, float, complex, bool)):
-                pp_vals: list[str] = []
-                param_fields: Tuple[Field, ...] = fields(param)
-                for param_field in param_fields:
-                    param_value_metadata = param_field.metadata.get(
-                        'path_param')
-                    if not param_value_metadata:
-                        continue
-
-                    parm_name = param_value_metadata.get(
-                        'field_name', field.name)
-
-                    param_field_val = getattr(param, param_field.name)
-                    if param_field_val is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{parm_name}={_val_to_string(param_field_val)}")
-                    else:
-                        pp_vals.append(
-                            f"{parm_name},{_val_to_string(param_field_val)}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            else:
+        param = getattr(
+            path_params, field.name) if path_params is not None else None
+        param = _populate_from_globals(
+            field.name, param, 'pathParam', gbls)
+
+        if param is None:
+            continue
+
+        f_name = param_metadata.get("field_name", field.name)
+        serialization = param_metadata.get('serialization', '')
+        if serialization != '':
+            serialized_params = _get_serialized_params(
+                param_metadata, f_name, param)
+            for key, value in serialized_params.items():
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + key + '}', value, 1)
+        else:
+            if param_metadata.get('style', 'simple') == 'simple':
+                if isinstance(param, list):
+                    pp_vals: list[str] = []
+                    for pp_val in param:
+                        if pp_val is None:
+                            continue
+                        pp_vals.append(_val_to_string(pp_val))
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif isinstance(param, dict):
+                    pp_vals: list[str] = []
+                    for pp_key in param:
+                        if param[pp_key] is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        else:
+                            pp_vals.append(
+                                f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif not isinstance(param, (str, int, float, complex, bool)):
+                    pp_vals: list[str] = []
+                    param_fields: Tuple[Field, ...] = fields(param)
+                    for param_field in param_fields:
+                        param_value_metadata = param_field.metadata.get(
+                            'path_param')
+                        if not param_value_metadata:
+                            continue
+
+                        parm_name = param_value_metadata.get(
+                            'field_name', field.name)
+
+                        param_field_val = getattr(param, param_field.name)
+                        if param_field_val is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{parm_name}={_val_to_string(param_field_val)}")
+                        else:
+                            pp_vals.append(
+                                f"{parm_name},{_val_to_string(param_field_val)}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                else:
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -242,16 +251,20 @@
             query_params, param_name) if query_params is not None else None
 
         value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            params = params | _get_serialized_query_params(
-                metadata, f_name, value)
+            serialized_parms = _get_serialized_params(metadata, f_name, value)
+            for key, value in serialized_parms.items():
+                if key in params:
+                    params[key].extend(value)
+                else:
+                    params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
                 params = params | _get_form_query_params(
@@ -278,16 +291,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    params: dict[str, list[str]] = {}
+def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
+    params: dict[str, str] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
```

### Comparing `structure_py-0.1.1/src/structure_py.egg-info/PKG-INFO` & `structure_py-0.3.0/src/structure_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure-py
-Version: 0.1.1
+Version: 0.3.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -47,18 +47,15 @@
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
 
 req = operations.EnrichCompanyRequest(
-    country_code="corrupti",
-    headquarters="provident",
-    id="distinctio",
-    name="quibusdam",
+    id="89bd9d8d-69a6-474e-8f46-7cc8796ed151",
 )
     
 res = s.companies.enrich(req)
 
 if res.body is not None:
     # handle response
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure-py Version: 0.1.1 Summary: Python Client
+Metadata-Version: 2.1 Name: structure-py Version: 0.3.0 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
@@ -18,19 +18,18 @@
 offers authentication for your API requests with a token. ### OAuth2 with
 bearer token Authentication with the Structure API is using OAuth2. When
 establishing a connection using OAuth2, you will need your access token â you
 will find it in the [Structure dashboard](https://www.structure.ac/api_tokens)
 under API settings. ## SDK Example Usage  ```python import sdk from sdk.models
 import operations, shared s = sdk.SDK( security=shared.Security
 ( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), ) req =
-operations.EnrichCompanyRequest( country_code="corrupti",
-headquarters="provident", id="distinctio", name="quibusdam", ) res =
-s.companies.enrich(req) if res.body is not None: # handle response ```   ##
-Available Resources and Operations ### accounts * `list_users` - Show current
-user accounts ### companies * `enrich` - Enrich a company profile *
+operations.EnrichCompanyRequest( id="89bd9d8d-69a6-474e-8f46-7cc8796ed151", )
+res = s.companies.enrich(req) if res.body is not None: # handle response ```
+## Available Resources and Operations ### accounts * `list_users` - Show
+current user accounts ### companies * `enrich` - Enrich a company profile *
 `list_employees` - List company employees * `list_jobs` - List company jobs *
 `search` - Search Companies ### people * `enrich` - Enrich a person profile *
 `search` - Search People ### user * `login` - Login user * `me` - Show current
 user  ### Maturity This SDK is in beta, and there may be breaking changes
 between versions without a major version update. Therefore, we recommend
 pinning usage to a specific package version. This way, you can install the same
 version each time without breaking changes unless you are intentionally looking
```

### Comparing `structure_py-0.1.1/src/structure_py.egg-info/SOURCES.txt` & `structure_py-0.3.0/src/structure_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

