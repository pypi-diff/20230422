# Comparing `tmp/fgo_api_types-2023.4.1.4.0.49.tar.gz` & `tmp/fgo_api_types-2023.4.22.17.7.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.4.1.4.0.49.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.4.22.17.7.38.tar", max compression
```

## Comparing `fgo_api_types-2023.4.1.4.0.49.tar` & `fgo_api_types-2023.4.22.17.7.38.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-04-01 04:00:22.826368 fgo_api_types-2023.4.1.4.0.49/LICENSE
--rw-r--r--   0        0        0      449 2023-04-01 04:00:22.826368 fgo_api_types-2023.4.1.4.0.49/README.md
--rw-r--r--   0        0        0        0 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/common.py
--rw-r--r--   0        0        0    37431 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/enums.py
--rw-r--r--   0        0        0   155624 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    73973 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/nice.py
--rw-r--r--   0        0        0    49669 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18464 2023-04-01 04:00:49.790625 fgo_api_types-2023.4.1.4.0.49/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-04-01 04:00:50.218628 fgo_api_types-2023.4.1.4.0.49/pyproject.toml
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.1.4.0.49/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-22 17:07:16.505451 fgo_api_types-2023.4.22.17.7.38/LICENSE
+-rw-r--r--   0        0        0      449 2023-04-22 17:07:16.505451 fgo_api_types-2023.4.22.17.7.38/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37431 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   155624 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74299 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    49669 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18464 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-04-22 17:07:38.509731 fgo_api_types-2023.4.22.17.7.38/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.22.17.7.38/PKG-INFO
```

### Comparing `fgo_api_types-2023.4.1.4.0.49/LICENSE` & `fgo_api_types-2023.4.22.17.7.38/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/basic.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/common.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/enums.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/gameenums.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/nice.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/nice.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,14 +638,30 @@
     arts: list[int]
     quick: list[int]
     extra: list[int]
     defence: list[int]
     np: list[int]
 
 
+class NiceTdSvt(BaseModelORJson):
+    svtId: int
+    num: int
+    priority: int
+    damage: list[int]
+    strengthStatus: int
+    flag: int
+    imageIndex: int
+    condQuestId: int
+    condQuestPhase: int
+    condLv: int = 0
+    condFriendshipRank: int = 0
+    motion: int
+    card: NiceCardType
+
+
 class NiceTd(BaseModelORJson):
     id: int
     num: int
     card: NiceCardType
     name: str
     originalName: str
     ruby: str
@@ -658,14 +674,15 @@
     npGain: NpGain
     npDistribution: list[int]
     strengthStatus: int
     priority: int
     condQuestId: int
     condQuestPhase: int
     individuality: list[NiceTrait]
+    npSvts: list[NiceTdSvt]
     script: NiceSkillScript
     functions: list[NiceFunction]
 
 
 class ExtraMCAssets(BaseModel):
     item: MCAssets
     masterFace: MCAssets
```

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/raw.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/rayshift.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/fgo_api_types/search.py` & `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.1.4.0.49/pyproject.toml` & `fgo_api_types-2023.4.22.17.7.38/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.04.01.04.00.49"
+version = "2023.04.22.17.07.38"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.4.1.4.0.49/PKG-INFO` & `fgo_api_types-2023.4.22.17.7.38/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.4.1.4.0.49
+Version: 2023.4.22.17.7.38
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

