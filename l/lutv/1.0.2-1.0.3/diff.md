# Comparing `tmp/lutv-1.0.2.tar.gz` & `tmp/lutv-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lutv-1.0.2.tar", last modified: Fri Apr 21 11:42:59 2023, max compression
+gzip compressed data, was "lutv-1.0.3.tar", last modified: Sat Apr 22 15:30:32 2023, max compression
```

## Comparing `lutv-1.0.2.tar` & `lutv-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:42:59.350758 lutv-1.0.2/
--rw-rw-rw-   0        0        0     1075 2022-11-06 02:47:18.000000 lutv-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1445 2023-04-21 11:42:59.348622 lutv-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      734 2022-11-06 09:00:39.000000 lutv-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:42:59.346642 lutv-1.0.2/lutv/
--rw-rw-rw-   0        0        0        0 2022-11-06 08:49:22.000000 lutv-1.0.2/lutv/__init__.py
--rw-rw-rw-   0        0        0      916 2023-04-21 11:33:56.000000 lutv-1.0.2/lutv/gpt.py
--rw-rw-rw-   0        0        0    17148 2022-11-06 08:49:06.000000 lutv-1.0.2/lutv/random.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:42:59.348622 lutv-1.0.2/lutv.egg-info/
--rw-rw-rw-   0        0        0     1445 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 11:42:59.000000 lutv-1.0.2/lutv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:42:59.350758 lutv-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-04-21 11:38:21.000000 lutv-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:30:32.567787 lutv-1.0.3/
+-rw-rw-rw-   0        0        0     1075 2022-11-06 02:47:18.000000 lutv-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1445 2023-04-22 15:30:32.567787 lutv-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2022-11-06 09:00:39.000000 lutv-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 15:30:32.565794 lutv-1.0.3/lutv/
+-rw-rw-rw-   0        0        0        0 2022-11-06 08:49:22.000000 lutv-1.0.3/lutv/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-04-22 15:27:12.000000 lutv-1.0.3/lutv/gpt.py
+-rw-rw-rw-   0        0        0    17148 2022-11-06 08:49:06.000000 lutv-1.0.3/lutv/random.py
+drwxrwxrwx   0        0        0        0 2023-04-22 15:30:32.566790 lutv-1.0.3/lutv.egg-info/
+-rw-rw-rw-   0        0        0     1445 2023-04-22 15:30:32.000000 lutv-1.0.3/lutv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-22 15:30:32.000000 lutv-1.0.3/lutv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 15:30:32.000000 lutv-1.0.3/lutv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-22 15:30:32.000000 lutv-1.0.3/lutv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 15:30:32.567787 lutv-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-04-22 15:30:24.000000 lutv-1.0.3/setup.py
```

### Comparing `lutv-1.0.2/LICENSE` & `lutv-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lutv-1.0.2/PKG-INFO` & `lutv-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lutv
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is my personal project
 Author: Trần Xuân Lợi
 Author-email: tranxuanloi2007@gmail.com
 Keywords: LuTV,lutv,random,random_uer,lutvrandom,LuTV Random User,Tranxuanloi,TranXuanLoi,tranxuanloi,tranxuanloi2007
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lutv-1.0.2/README.md` & `lutv-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lutv-1.0.2/lutv/gpt.py` & `lutv-1.0.3/lutv/gpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,8 +12,17 @@
         response = requests.post('https://api.openai.com/v1/chat/completions', headers=headers, json=json_data).json()
         print('____\n\n',response["choices"][0]['message']['content'],'\n\n____')
         if n =='':
             break
 def chat(noidung):
     json_data = {'model': 'gpt-3.5-turbo','messages': [{'role': 'user','content': noidung,},],}
     response = requests.post('https://api.openai.com/v1/chat/completions', headers=headers, json=json_data).json()
-    print('____\n\n',response["choices"][0]['message']['content'],'\n\n____')
+    print('____\n\n',response["choices"][0]['message']['content'],'\n\n____')
+def save(text):
+    json_data = {'model': 'gpt-3.5-turbo','messages': [{'role': 'user','content': text,},],}
+    response = requests.post('https://api.openai.com/v1/chat/completions', headers=headers, json=json_data).json()
+    a=response["choices"][0]['message']['content']
+    try:parts = a.split("```")[1].split('python')[1]
+    except:parts = a.split("```")[1]
+    with open("filename.py", "w", encoding='utf-8') as f:
+        f.write(parts)
+    print('Done')
```

### Comparing `lutv-1.0.2/lutv/random.py` & `lutv-1.0.3/lutv/random.py`

 * *Files identical despite different names*

### Comparing `lutv-1.0.2/lutv.egg-info/PKG-INFO` & `lutv-1.0.3/lutv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lutv
-Version: 1.0.2
+Version: 1.0.3
 Summary: This is my personal project
 Author: Trần Xuân Lợi
 Author-email: tranxuanloi2007@gmail.com
 Keywords: LuTV,lutv,random,random_uer,lutvrandom,LuTV Random User,Tranxuanloi,TranXuanLoi,tranxuanloi,tranxuanloi2007
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lutv-1.0.2/setup.py` & `lutv-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'This is my personal project'
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
```

