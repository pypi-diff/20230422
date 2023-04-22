# Comparing `tmp/osrs-lib-0.1.1.tar.gz` & `tmp/osrs-lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osrs-lib-0.1.1.tar", last modified: Sat Apr 22 21:08:37 2023, max compression
+gzip compressed data, was "osrs-lib-0.1.2.tar", last modified: Sat Apr 22 21:17:00 2023, max compression
```

## Comparing `osrs-lib-0.1.1.tar` & `osrs-lib-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/
--rw-r--r--   0 peter     (1000) peter     (1000)    11357 2023-02-22 21:55:07.000000 osrs-lib-0.1.1/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)      509 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1249 2023-02-23 03:26:10.000000 osrs-lib-0.1.1/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/osrs_lib/
--rw-r--r--   0 peter     (1000) peter     (1000)      794 2023-02-23 03:38:15.000000 osrs-lib-0.1.1/osrs_lib/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      887 2023-02-23 03:26:08.000000 osrs-lib-0.1.1/osrs_lib/errors.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4465 2023-04-22 21:02:59.000000 osrs-lib-0.1.1/osrs_lib/hiscores.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1217 2023-02-22 21:55:36.000000 osrs-lib-0.1.1/osrs_lib/utils.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/osrs_lib.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      509 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      264 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       20 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        9 2023-04-22 21:08:37.000000 osrs-lib-0.1.1/osrs_lib.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-22 21:08:37.841650 osrs-lib-0.1.1/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)      722 2023-04-22 21:08:35.000000 osrs-lib-0.1.1/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:17:00.781588 osrs-lib-0.1.2/
+-rw-r--r--   0 peter     (1000) peter     (1000)    11357 2023-02-22 21:55:07.000000 osrs-lib-0.1.2/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)      509 2023-04-22 21:17:00.781588 osrs-lib-0.1.2/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1249 2023-02-23 03:26:10.000000 osrs-lib-0.1.2/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:17:00.781588 osrs-lib-0.1.2/osrs_lib/
+-rw-r--r--   0 peter     (1000) peter     (1000)      794 2023-04-22 21:16:32.000000 osrs-lib-0.1.2/osrs_lib/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      887 2023-02-23 03:26:08.000000 osrs-lib-0.1.2/osrs_lib/errors.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4488 2023-04-22 21:16:25.000000 osrs-lib-0.1.2/osrs_lib/hiscores.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1217 2023-02-22 21:55:36.000000 osrs-lib-0.1.2/osrs_lib/utils.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-22 21:17:00.781588 osrs-lib-0.1.2/osrs_lib.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      509 2023-04-22 21:17:00.000000 osrs-lib-0.1.2/osrs_lib.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      264 2023-04-22 21:17:00.000000 osrs-lib-0.1.2/osrs_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-22 21:17:00.000000 osrs-lib-0.1.2/osrs_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       20 2023-04-22 21:17:00.000000 osrs-lib-0.1.2/osrs_lib.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        9 2023-04-22 21:17:00.000000 osrs-lib-0.1.2/osrs_lib.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-22 21:17:00.781588 osrs-lib-0.1.2/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)      722 2023-04-22 21:16:39.000000 osrs-lib-0.1.2/setup.py
```

### Comparing `osrs-lib-0.1.1/LICENSE` & `osrs-lib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.1/README.md` & `osrs-lib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.1/osrs_lib/__init__.py` & `osrs-lib-0.1.2/osrs_lib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 __author__ = 'shumatepf'
```

### Comparing `osrs-lib-0.1.1/osrs_lib/errors.py` & `osrs-lib-0.1.2/osrs_lib/errors.py`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.1/osrs_lib/hiscores.py` & `osrs-lib-0.1.2/osrs_lib/hiscores.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import math
 
 from bs4 import BeautifulSoup
 import asyncio
 import aiohttp
 import logging
 
-from errors import BadHiScoresPage
-import utils
+from osrs_lib.errors import BadHiScoresPage
+from osrs_lib import utils
 
 
 def get_stats(users):
     """
     Get users' stats concurrently
     """
     return asyncio.run(__get_users_sync(users))
```

### Comparing `osrs-lib-0.1.1/osrs_lib/utils.py` & `osrs-lib-0.1.2/osrs_lib/utils.py`

 * *Files identical despite different names*

### Comparing `osrs-lib-0.1.1/setup.py` & `osrs-lib-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='osrs-lib',
-    version='0.1.1',
+    version='0.1.2',
     description='An OSRS library',
     url='https://github.com/shumatepf/osrs-lib',
     author='shumatepf',
     author_email='shumatepfs@gmail.com',
     license='Apache 2.0',
     packages=['osrs_lib'],
     install_requires=['bs4',
```

