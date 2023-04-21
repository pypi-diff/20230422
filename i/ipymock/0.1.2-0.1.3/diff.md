# Comparing `tmp/ipymock-0.1.2.tar.gz` & `tmp/ipymock-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-0.1.2.tar", last modified: Thu Apr 20 13:46:23 2023, max compression
+gzip compressed data, was "ipymock-0.1.3.tar", last modified: Fri Apr 21 22:21:57 2023, max compression
```

## Comparing `ipymock-0.1.2.tar` & `ipymock-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.317186 ipymock-0.1.2/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.2/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.2/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-20 13:46:23.316864 ipymock-0.1.2/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6837 2023-04-20 13:46:09.000000 ipymock-0.1.2/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.314069 ipymock-0.1.2/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-20 13:44:18.000000 ipymock-0.1.2/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-20 13:44:18.000000 ipymock-0.1.2/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)     9733 2023-04-20 13:44:18.000000 ipymock-0.1.2/ipymock/mock.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.315836 ipymock-0.1.2/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-20 13:46:23.316425 ipymock-0.1.2/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7587 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.2/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-20 13:46:23.000000 ipymock-0.1.2/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-20 13:45:19.000000 ipymock-0.1.2/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-20 13:46:23.317342 ipymock-0.1.2/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.2/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.065845 ipymock-0.1.3/
+-rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-0.1.3/LICENSE
+-rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-0.1.3/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-21 22:21:57.065544 ipymock-0.1.3/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-21 22:21:41.000000 ipymock-0.1.3/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.061982 ipymock-0.1.3/ipymock/
+-rw-r--r--   0 saintway   (501) staff       (20)     1603 2023-04-21 22:21:33.000000 ipymock-0.1.3/ipymock/__init__.py
+-rw-r--r--   0 saintway   (501) staff       (20)     1196 2023-04-21 22:21:33.000000 ipymock-0.1.3/ipymock/_nbdev.py
+-rw-r--r--   0 saintway   (501) staff       (20)     9912 2023-04-21 22:21:33.000000 ipymock-0.1.3/ipymock/mock.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.064025 ipymock-0.1.3/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-21 22:21:57.064887 ipymock-0.1.3/ipymock.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-0.1.3/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-0.1.3/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)      409 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/SOURCES.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/dependency_links.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-0.1.3/ipymock.egg-info/not-zip-safe
+-rw-r--r--   0 saintway   (501) staff       (20)       35 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/requires.txt
+-rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-21 22:21:56.000000 ipymock-0.1.3/ipymock.egg-info/top_level.txt
+-rw-r--r--   0 saintway   (501) staff       (20)     2492 2023-04-21 22:21:24.000000 ipymock-0.1.3/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-21 22:21:57.065964 ipymock-0.1.3/setup.cfg
+-rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-0.1.3/setup.py
```

### Comparing `ipymock-0.1.2/LICENSE` & `ipymock-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.2/PKG-INFO` & `ipymock-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,15 @@
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
 
 ## Pytest the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -44,24 +44,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ## Pytest the Python Testcases within IPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -107,15 +107,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -124,22 +124,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -184,34 +184,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to use the do-pytest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-0.1.2/README.md` & `ipymock-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
 
 ## Pytest the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -24,24 +24,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ## Pytest the Python Testcases within IPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -87,15 +87,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -104,22 +104,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -164,34 +164,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to use the do-pytest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-0.1.2/ipymock/__init__.py` & `ipymock-0.1.3/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.2/ipymock/_nbdev.py` & `ipymock-0.1.3/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-0.1.2/ipymock/mock.py` & `ipymock-0.1.3/ipymock/mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,42 +58,56 @@
     message = conversation_detail['message']
     parts = message['content']['parts']
     if len(parts) > 0 and parts[0] != '':
         if message['author']['role'] == common.role_user:
             common.message_channel.put(message)
 
 def start_conversation(content):
-    if common.parent_message_id == '' or common.conversation_id == '':
+    if common.conversation_id != '' and common.parent_message_id == '':
+        try:
+            # set common.parent_message_id
+            get_conversation(common.conversation_id)
+        except requests.exceptions.ConnectionError as errc:
+            sys.stderr.write(f'Error Connecting: {errc}\n')
+        except RecursionError as errr:
+            sys.stderr.write(f'Error Recursion: {errr}\n')
+
+    if common.conversation_id == '' or common.parent_message_id == '':
         common.conversation_id = ''
         common.parent_message_id = str(uuid.uuid4())
+
+    post_data = {
+        'action': 'next',
+        'messages': [{
+            'id': str(uuid.uuid4()),
+            'author': {
+                'role': common.role_user,
+            },
+            'role': common.role_user,
+            'content': {
+                'content_type': 'text',
+                'parts': [content],
+            },
+        }],
+        'model': common.chat_gpt_model,
+        'continue_text': '',
+    }
+    if common.conversation_id != '':
+        post_data['conversation_id'] = common.conversation_id
+    if common.parent_message_id != '':
+        post_data['parent_message_id'] = common.parent_message_id
+
     response = requests.post(
         f'{chat_gpt_base_url}/conversation',
         headers = {
             'Authorization': access_token,
             'Content-Type': 'application/json',
             'Accept': 'text/event-stream'
         },
-        data = json.dumps({
-            'action': 'next',
-            'messages': [{
-                'id': uuid.uuid4().hex,
-                'author': {
-                    'role': common.role_user
-                },
-                'role': common.role_user,
-                'content': {
-                    'content_type': 'text',
-                    'parts': [content]
-                }
-            }],
-            'parent_message_id': common.parent_message_id,
-            'model': common.chat_gpt_model,
-            'conversation_id': common.conversation_id,
-            'continue_text': ''
-        }),
+        data = json.dumps(post_data),
         stream=True
     )
 
     temp_conversation_id = ''
     for line in response.iter_lines():
         if not line.startswith(b'data: '):
             continue
@@ -180,24 +194,15 @@
 
     common.conversation_id = ''
     common.reload_conversations_channel.put(True)
 
 # Internal Cell
 # open the JSON file and read the conversation_id
 with open(os.path.expanduser('~/.config/revChatGPT/config.json'), 'r') as f:
-    conversation_id = json.load(f).get('conversation_id', None)
-
-# Internal Cell
-try:
-    common.conversation_id = conversation_id
-    get_conversation(conversation_id)
-except requests.exceptions.ConnectionError as errc:
-    sys.stderr.write(f'Error Connecting: {errc}\n')
-except RecursionError as errr:
-    sys.stderr.write(f'Error Recursion: {errr}\n')
+    common.conversation_id = json.load(f).get('conversation_id', None)
 
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
 
 def attributize(obj):
```

### Comparing `ipymock-0.1.2/ipymock.egg-info/PKG-INFO` & `ipymock-0.1.3/ipymock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 0.1.2
+Version: 0.1.3
 Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,15 @@
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
 
 ## Pytest the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -44,24 +44,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ## Pytest the Python Testcases within IPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -107,15 +107,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -124,22 +124,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -184,34 +184,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to use the do-pytest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-0.1.2/settings.ini` & `ipymock-0.1.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 0.1.2
+version = 0.1.3
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `ipymock-0.1.2/setup.py` & `ipymock-0.1.3/setup.py`

 * *Files identical despite different names*

