# Comparing `tmp/cooldfa-1.0.1.tar.gz` & `tmp/cooldfa-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cooldfa-1.0.1.tar", last modified: Sat Apr  8 14:17:43 2023, max compression
+gzip compressed data, was "cooldfa-1.0.2.tar", last modified: Sat Apr 22 15:49:51 2023, max compression
```

## Comparing `cooldfa-1.0.1.tar` & `cooldfa-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.1/LICENSE
--rw-r--r--   0        0        0     2016 2023-04-08 14:13:20.647390 cooldfa-1.0.1/README.md
--rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.1/cooldfa/__init__.py
--rw-r--r--   0        0        0     3696 2023-04-03 17:08:12.751910 cooldfa-1.0.1/cooldfa/_cooldfa.py
--rw-r--r--   0        0        0   478756 2023-04-03 17:12:39.903738 cooldfa-1.0.1/cooldfa/_words/others.json
--rw-r--r--   0        0        0    23166 2023-04-03 17:12:39.906737 cooldfa-1.0.1/cooldfa/_words/politics.json
--rw-r--r--   0        0        0    10325 2023-04-03 17:12:39.909739 cooldfa-1.0.1/cooldfa/_words/sex.json
--rw-r--r--   0        0        0   262857 2023-04-07 01:51:58.429386 cooldfa-1.0.1/cooldfa/_words/url.json
--rw-r--r--   0        0        0     4015 2023-04-03 17:12:39.929739 cooldfa-1.0.1/cooldfa/_words/violence.json
--rw-r--r--   0        0        0      547 2023-04-08 14:02:30.796255 cooldfa-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 cooldfa-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 cooldfa-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1985 2023-04-19 04:33:25.482492 cooldfa-1.0.2/README.md
+-rw-r--r--   0        0        0       39 2023-04-03 14:28:11.266714 cooldfa-1.0.2/cooldfa/__init__.py
+-rw-r--r--   0        0        0     3692 2023-04-19 04:33:25.482492 cooldfa-1.0.2/cooldfa/_cooldfa.py
+-rw-r--r--   0        0        0   478756 2023-04-03 17:12:39.903738 cooldfa-1.0.2/cooldfa/_words/others.json
+-rw-r--r--   0        0        0    23166 2023-04-03 17:12:39.906737 cooldfa-1.0.2/cooldfa/_words/politics.json
+-rw-r--r--   0        0        0    10325 2023-04-03 17:12:39.909739 cooldfa-1.0.2/cooldfa/_words/sex.json
+-rw-r--r--   0        0        0   262857 2023-04-07 01:51:58.429386 cooldfa-1.0.2/cooldfa/_words/url.json
+-rw-r--r--   0        0        0     4015 2023-04-03 17:12:39.929739 cooldfa-1.0.2/cooldfa/_words/violence.json
+-rw-r--r--   0        0        0      547 2023-04-22 15:46:27.072378 cooldfa-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 cooldfa-1.0.2/PKG-INFO
```

### Comparing `cooldfa-1.0.1/LICENSE` & `cooldfa-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.1/README.md` & `cooldfa-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,25 +50,24 @@
 example.find_all('1--2--3--4--5--6--7--8--9--end--')
 # >>> ['1--2--3', '5--6', 'end']
 ```
 
 替换所有敏感词：
 
 ```python
-example.sub_all('1--2--3--4--5--6--7--8--9--end--', '*')
+example.sub('1--2--3--4--5--6--7--8--9--end--', '*')
 # >>> '*******--4--****--7--8--9--***--'
 ```
 
 使用预置的敏感词库：
 
 ```python
 from cooldfa import dfa, preset_words
 
 example = dfa(
-    ['123', '56', 'end'],
     preset_words.politics,  # 政治类
     preset_words.sex,  # 色情类
     preset_words.violence,  # 暴力类
     preset_words.url,  # 网址
     preset_words.others,  # 其它
 )
 ```
```

### Comparing `cooldfa-1.0.1/cooldfa/_cooldfa.py` & `cooldfa-1.0.2/cooldfa/_cooldfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         for x in word.lower():
             if x not in self.ignore_words:
                 tree = tree.setdefault(x, {})
         tree['__'] = 0
         # '__'必须大于1个字符
         # 这样才能使<if treeSon := tree.get(s):>判断为False, 否则在添加空敏感词''后, 查找时会报错
     
-    def sub_all(self, text:str, repl:str='*', compress=False):
+    def sub(self, text:str, repl:str='*', compress=False):
         last_i = -1
         new_text = []
         content = text.lower()
         if compress:
             for start_i, t in enumerate(content):
                 if t not in self.ignore_words:
                     if indexs := self._find_base(content, start_i):
```

### Comparing `cooldfa-1.0.1/cooldfa/_words/others.json` & `cooldfa-1.0.2/cooldfa/_words/others.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.1/cooldfa/_words/politics.json` & `cooldfa-1.0.2/cooldfa/_words/politics.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.1/cooldfa/_words/sex.json` & `cooldfa-1.0.2/cooldfa/_words/sex.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.1/cooldfa/_words/url.json` & `cooldfa-1.0.2/cooldfa/_words/url.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.1/cooldfa/_words/violence.json` & `cooldfa-1.0.2/cooldfa/_words/violence.json`

 * *Files identical despite different names*

### Comparing `cooldfa-1.0.1/pyproject.toml` & `cooldfa-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "cooldfa"
-version = "1.0.1"
+version = "1.0.2"
 description = "一个基于DFA算法的敏感词检测器"
 dependencies = []
 keywords = ["cooldfa", "dfa"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `cooldfa-1.0.1/PKG-INFO` & `cooldfa-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cooldfa
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一个基于DFA算法的敏感词检测器
 Keywords: cooldfa,dfa
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/cooldfa
@@ -61,25 +61,24 @@
 example.find_all('1--2--3--4--5--6--7--8--9--end--')
 # >>> ['1--2--3', '5--6', 'end']
 ```
 
 替换所有敏感词：
 
 ```python
-example.sub_all('1--2--3--4--5--6--7--8--9--end--', '*')
+example.sub('1--2--3--4--5--6--7--8--9--end--', '*')
 # >>> '*******--4--****--7--8--9--***--'
 ```
 
 使用预置的敏感词库：
 
 ```python
 from cooldfa import dfa, preset_words
 
 example = dfa(
-    ['123', '56', 'end'],
     preset_words.politics,  # 政治类
     preset_words.sex,  # 色情类
     preset_words.violence,  # 暴力类
     preset_words.url,  # 网址
     preset_words.others,  # 其它
 )
 ```
```

