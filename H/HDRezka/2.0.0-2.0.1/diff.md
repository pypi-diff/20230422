# Comparing `tmp/HDRezka-2.0.0.tar.gz` & `tmp/HDRezka-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HDRezka-2.0.0.tar", last modified: Wed Apr 19 13:13:51 2023, max compression
+gzip compressed data, was "HDRezka-2.0.1.tar", last modified: Sat Apr 22 04:07:34 2023, max compression
```

## Comparing `HDRezka-2.0.0.tar` & `HDRezka-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:13:51.768142 HDRezka-2.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-19 13:13:51.759143 HDRezka-2.0.0/HDRezka.egg-info/
--rw-rw-rw-   0        0        0     4410 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 13:13:51.000000 HDRezka-2.0.0/HDRezka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     4410 2023-04-19 13:13:51.767142 HDRezka-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      812 2023-04-19 13:06:04.000000 HDRezka-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:13:51.765144 HDRezka-2.0.0/hdrezka/
--rw-rw-rw-   0        0        0      901 2023-04-19 13:04:35.000000 HDRezka-2.0.0/hdrezka/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-04-19 10:05:55.000000 HDRezka-2.0.0/hdrezka/_antiobfuscation.py
--rw-rw-rw-   0        0        0      299 2023-04-08 03:54:33.000000 HDRezka-2.0.0/hdrezka/_bs4.py
--rw-rw-rw-   0        0        0      365 2023-04-19 12:27:06.000000 HDRezka-2.0.0/hdrezka/errors.py
--rw-rw-rw-   0        0        0      387 2023-04-06 11:53:59.000000 HDRezka-2.0.0/hdrezka/translators.py
--rw-rw-rw-   0        0        0       42 2023-04-19 13:13:51.768142 HDRezka-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1992 2023-04-19 13:06:04.000000 HDRezka-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.498551 HDRezka-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.438351 HDRezka-2.0.1/HDRezka.egg-info/
+-rw-rw-rw-   0        0        0     4446 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 04:07:34.000000 HDRezka-2.0.1/HDRezka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4446 2023-04-22 04:07:34.497551 HDRezka-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-04-19 13:06:04.000000 HDRezka-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.465246 HDRezka-2.0.1/hdrezka/
+-rw-rw-rw-   0        0        0      901 2023-04-19 13:04:35.000000 HDRezka-2.0.1/hdrezka/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-04-19 10:05:55.000000 HDRezka-2.0.1/hdrezka/_antiobfuscation.py
+-rw-rw-rw-   0        0        0      299 2023-04-08 03:54:33.000000 HDRezka-2.0.1/hdrezka/_bs4.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.470365 HDRezka-2.0.1/hdrezka/api/
+-rw-rw-rw-   0        0        0       42 2023-04-06 11:57:13.000000 HDRezka-2.0.1/hdrezka/api/__init__.py
+-rw-rw-rw-   0        0        0     1363 2023-04-19 13:10:55.000000 HDRezka-2.0.1/hdrezka/api/ajax.py
+-rw-rw-rw-   0        0        0      315 2023-04-06 11:55:17.000000 HDRezka-2.0.1/hdrezka/api/http.py
+-rw-rw-rw-   0        0        0     1164 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/api/search.py
+-rw-rw-rw-   0        0        0      365 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.478696 HDRezka-2.0.1/hdrezka/post/
+-rw-rw-rw-   0        0        0       40 2023-04-06 11:11:48.000000 HDRezka-2.0.1/hdrezka/post/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-04-06 11:12:40.000000 HDRezka-2.0.1/hdrezka/post/_dataclass.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.481697 HDRezka-2.0.1/hdrezka/post/info/
+-rw-rw-rw-   0        0        0       42 2023-04-02 10:26:20.000000 HDRezka-2.0.1/hdrezka/post/info/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-04-06 11:53:58.000000 HDRezka-2.0.1/hdrezka/post/info/fields.py
+-rw-rw-rw-   0        0        0     5313 2023-04-19 12:59:55.000000 HDRezka-2.0.1/hdrezka/post/info/info.py
+-rw-rw-rw-   0        0        0     3154 2023-04-19 12:53:06.000000 HDRezka-2.0.1/hdrezka/post/page.py
+-rw-rw-rw-   0        0        0     2444 2023-04-06 11:57:13.000000 HDRezka-2.0.1/hdrezka/post/post.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.490583 HDRezka-2.0.1/hdrezka/post/urls/
+-rw-rw-rw-   0        0        0       61 2023-04-19 12:43:33.000000 HDRezka-2.0.1/hdrezka/post/urls/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/post/urls/_regexes.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.494551 HDRezka-2.0.1/hdrezka/post/urls/kind/
+-rw-rw-rw-   0        0        0       68 2023-04-19 10:43:34.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/__init__.py
+-rw-rw-rw-   0        0        0      739 2023-04-19 11:56:29.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/quality.py
+-rw-rw-rw-   0        0        0     1448 2023-04-19 12:37:33.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/subtitle.py
+-rw-rw-rw-   0        0        0     1975 2023-04-19 12:09:56.000000 HDRezka-2.0.1/hdrezka/post/urls/kind/video.py
+-rw-rw-rw-   0        0        0      528 2023-04-19 10:30:04.000000 HDRezka-2.0.1/hdrezka/post/urls/short.py
+-rw-rw-rw-   0        0        0      455 2023-04-19 12:43:14.000000 HDRezka-2.0.1/hdrezka/post/urls/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-22 04:07:34.496553 HDRezka-2.0.1/hdrezka/stream/
+-rw-rw-rw-   0        0        0       22 2023-04-03 14:41:41.000000 HDRezka-2.0.1/hdrezka/stream/__init__.py
+-rw-rw-rw-   0        0        0     2535 2023-04-19 12:27:06.000000 HDRezka-2.0.1/hdrezka/stream/player.py
+-rw-rw-rw-   0        0        0      387 2023-04-06 11:53:59.000000 HDRezka-2.0.1/hdrezka/translators.py
+-rw-rw-rw-   0        0        0       42 2023-04-22 04:07:34.498551 HDRezka-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2007 2023-04-22 04:06:12.000000 HDRezka-2.0.1/setup.py
```

### Comparing `HDRezka-2.0.0/HDRezka.egg-info/PKG-INFO` & `HDRezka-2.0.1/HDRezka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 2.0.0
+Version: 2.0.1
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -62,14 +62,18 @@
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 2.0.1
+
+- Fixed bug with PIP
+
 ## 2.0.0
 
 Backward incompatible changes have been made
 
 - #### New submodules `urls.short`, `urls.kind`, `urls.kind.quality`, `urls.kind.subtitles`, `urls.kind.video`
 - Optimizations
 - `Ajax` renamed to `AJAX` (PEP-8)
```

### Comparing `HDRezka-2.0.0/LICENSE` & `HDRezka-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HDRezka-2.0.0/PKG-INFO` & `HDRezka-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 2.0.0
+Version: 2.0.1
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -62,14 +62,18 @@
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 2.0.1
+
+- Fixed bug with PIP
+
 ## 2.0.0
 
 Backward incompatible changes have been made
 
 - #### New submodules `urls.short`, `urls.kind`, `urls.kind.quality`, `urls.kind.subtitles`, `urls.kind.video`
 - Optimizations
 - `Ajax` renamed to `AJAX` (PEP-8)
```

### Comparing `HDRezka-2.0.0/README.md` & `HDRezka-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `HDRezka-2.0.0/hdrezka/__init__.py` & `HDRezka-2.0.1/hdrezka/__init__.py`

 * *Files identical despite different names*

### Comparing `HDRezka-2.0.0/hdrezka/_antiobfuscation.py` & `HDRezka-2.0.1/hdrezka/_antiobfuscation.py`

 * *Files identical despite different names*

### Comparing `HDRezka-2.0.0/setup.py` & `HDRezka-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 with open('README.md', encoding='UTF-8') as f:
     long_description = f.read().strip()
 with open('CHANGELOG.md', encoding='UTF-8') as f:
     long_description += f'\n\n---\n\n{f.read().strip()}\n'
 
 setuptools.setup(
     name='HDRezka',
-    version='2.0.0',
+    version='2.0.1',
 
     author='Nikita (NIKDISSV)',
     author_email='nikdissv@proton.me',
 
     description='HDRezka (rezka.ag) Python API',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/NIKDISSV-Forever/HDRezka',
     project_urls={
         'GitHub': 'https://github.com/NIKDISSV-Forever/HDRezka',
         'Documentation': 'https://nikdissv-forever.github.io/HDRezka/hdrezka'
     },
-    packages=['hdrezka'],
+    packages=setuptools.find_packages(),
     install_requires=install_requires,
 
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: End Users/Desktop',
```

