# Comparing `tmp/mpb_lib-0.1.80.tar.gz` & `tmp/mpb_lib-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpb_lib-0.1.80.tar", last modified: Thu Feb  2 06:35:55 2023, max compression
+gzip compressed data, was "mpb_lib-0.1.81.tar", last modified: Sat Apr 22 02:35:03 2023, max compression
```

## Comparing `mpb_lib-0.1.80.tar` & `mpb_lib-0.1.81.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.148071 mpb_lib-0.1.80/
--rw-r--r--   0 ats        (501) staff       (20)      336 2023-02-02 06:35:55.147828 mpb_lib-0.1.80/PKG-INFO
--rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:33.000000 mpb_lib-0.1.80/README.md
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.120468 mpb_lib-0.1.80/mpb_lib/
--rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:46.000000 mpb_lib-0.1.80/mpb_lib/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.121946 mpb_lib-0.1.80/mpb_lib/apis/
--rw-r--r--   0 ats        (501) staff       (20)     4928 2023-02-01 23:02:29.000000 mpb_lib-0.1.80/mpb_lib/apis/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.124037 mpb_lib-0.1.80/mpb_lib/cannon/
--rw-r--r--   0 ats        (501) staff       (20)      319 2023-02-01 23:04:45.000000 mpb_lib-0.1.80/mpb_lib/cannon/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     2050 2023-02-01 23:05:23.000000 mpb_lib-0.1.80/mpb_lib/cannon/cannon.py
--rw-r--r--   0 ats        (501) staff       (20)     9060 2023-02-01 23:05:06.000000 mpb_lib-0.1.80/mpb_lib/cannon/cannon_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.125859 mpb_lib-0.1.80/mpb_lib/face/
--rw-r--r--   0 ats        (501) staff       (20)      157 2023-02-01 23:06:06.000000 mpb_lib-0.1.80/mpb_lib/face/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     4435 2023-02-01 23:06:15.000000 mpb_lib-0.1.80/mpb_lib/face/face.py
--rw-r--r--   0 ats        (501) staff       (20)     4304 2023-02-01 23:06:36.000000 mpb_lib-0.1.80/mpb_lib/face/face_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.126664 mpb_lib-0.1.80/mpb_lib/maze/
--rw-r--r--   0 ats        (501) staff       (20)     2633 2023-02-02 01:03:43.000000 mpb_lib-0.1.80/mpb_lib/maze/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.128604 mpb_lib-0.1.80/mpb_lib/rpg/
--rw-r--r--   0 ats        (501) staff       (20)      185 2021-07-20 02:03:49.000000 mpb_lib-0.1.80/mpb_lib/rpg/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     9880 2022-06-01 08:47:58.000000 mpb_lib-0.1.80/mpb_lib/rpg/rpg.py
--rw-r--r--   0 ats        (501) staff       (20)     2996 2021-11-26 23:16:54.000000 mpb_lib-0.1.80/mpb_lib/rpg/rpg_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.130598 mpb_lib-0.1.80/mpb_lib/rythmbox/
--rw-r--r--   0 ats        (501) staff       (20)       29 2021-09-06 05:02:03.000000 mpb_lib-0.1.80/mpb_lib/rythmbox/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     2419 2021-12-27 01:25:09.000000 mpb_lib-0.1.80/mpb_lib/rythmbox/rythmbox.py
--rw-r--r--   0 ats        (501) staff       (20)     5044 2021-09-02 04:33:49.000000 mpb_lib-0.1.80/mpb_lib/rythmbox/rythmbox_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.131252 mpb_lib-0.1.80/mpb_lib/sound/
--rw-r--r--   0 ats        (501) staff       (20)      881 2023-02-01 23:07:24.000000 mpb_lib-0.1.80/mpb_lib/sound/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.140880 mpb_lib-0.1.80/mpb_lib/sound/wavs/
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:51.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/a.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:15.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/b.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:23.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/c.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:30.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/d.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:35.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/e.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:40.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/f.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:46.000000 mpb_lib-0.1.80/mpb_lib/sound/wavs/g.wav
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.143996 mpb_lib-0.1.80/mpb_lib/tictactoe/
--rw-r--r--   0 ats        (501) staff       (20)      170 2023-02-01 23:08:05.000000 mpb_lib-0.1.80/mpb_lib/tictactoe/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)      950 2023-02-01 23:08:32.000000 mpb_lib-0.1.80/mpb_lib/tictactoe/tictactoe.py
--rw-r--r--   0 ats        (501) staff       (20)     2415 2023-02-01 23:08:24.000000 mpb_lib-0.1.80/mpb_lib/tictactoe/tictactoe_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.147099 mpb_lib-0.1.80/mpb_lib/vowelgen/
--rw-r--r--   0 ats        (501) staff       (20)     2350 2022-08-18 22:51:31.000000 mpb_lib-0.1.80/mpb_lib/vowelgen/HPF.py
--rw-r--r--   0 ats        (501) staff       (20)      946 2023-02-01 23:02:22.000000 mpb_lib-0.1.80/mpb_lib/vowelgen/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     3277 2022-08-18 22:51:27.000000 mpb_lib-0.1.80/mpb_lib/vowelgen/glottal.py
--rw-r--r--   0 ats        (501) staff       (20)     6059 2022-08-18 10:39:56.000000 mpb_lib-0.1.80/mpb_lib/vowelgen/threetube.py
--rw-r--r--   0 ats        (501) staff       (20)     5291 2022-08-18 10:39:53.000000 mpb_lib-0.1.80/mpb_lib/vowelgen/twotube.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-02-02 06:35:55.121624 mpb_lib-0.1.80/mpb_lib.egg-info/
--rw-r--r--   0 ats        (501) staff       (20)      336 2023-02-02 06:35:54.000000 mpb_lib-0.1.80/mpb_lib.egg-info/PKG-INFO
--rw-r--r--   0 ats        (501) staff       (20)      962 2023-02-02 06:35:55.000000 mpb_lib-0.1.80/mpb_lib.egg-info/SOURCES.txt
--rw-r--r--   0 ats        (501) staff       (20)        1 2023-02-02 06:35:54.000000 mpb_lib-0.1.80/mpb_lib.egg-info/dependency_links.txt
--rw-r--r--   0 ats        (501) staff       (20)        8 2023-02-02 06:35:54.000000 mpb_lib-0.1.80/mpb_lib.egg-info/top_level.txt
--rw-r--r--   0 ats        (501) staff       (20)       38 2023-02-02 06:35:55.148143 mpb_lib-0.1.80/setup.cfg
--rw-r--r--   0 ats        (501) staff       (20)     1043 2023-02-02 01:04:10.000000 mpb_lib-0.1.80/setup.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.205654 mpb_lib-0.1.81/
+-rw-r--r--   0 ats        (501) staff       (20)      336 2023-04-22 02:35:03.204734 mpb_lib-0.1.81/PKG-INFO
+-rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:33.000000 mpb_lib-0.1.81/README.md
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.170646 mpb_lib-0.1.81/mpb_lib/
+-rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:46.000000 mpb_lib-0.1.81/mpb_lib/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.172791 mpb_lib-0.1.81/mpb_lib/apis/
+-rw-r--r--   0 ats        (501) staff       (20)     4931 2023-04-22 02:23:02.000000 mpb_lib-0.1.81/mpb_lib/apis/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.175797 mpb_lib-0.1.81/mpb_lib/cannon/
+-rw-r--r--   0 ats        (501) staff       (20)      319 2023-02-01 23:04:45.000000 mpb_lib-0.1.81/mpb_lib/cannon/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     2050 2023-02-01 23:05:23.000000 mpb_lib-0.1.81/mpb_lib/cannon/cannon.py
+-rw-r--r--   0 ats        (501) staff       (20)     9060 2023-02-01 23:05:06.000000 mpb_lib-0.1.81/mpb_lib/cannon/cannon_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.178175 mpb_lib-0.1.81/mpb_lib/face/
+-rw-r--r--   0 ats        (501) staff       (20)      157 2023-02-01 23:06:06.000000 mpb_lib-0.1.81/mpb_lib/face/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     4435 2023-02-01 23:06:15.000000 mpb_lib-0.1.81/mpb_lib/face/face.py
+-rw-r--r--   0 ats        (501) staff       (20)     4304 2023-02-01 23:06:36.000000 mpb_lib-0.1.81/mpb_lib/face/face_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.179102 mpb_lib-0.1.81/mpb_lib/maze/
+-rw-r--r--   0 ats        (501) staff       (20)     2633 2023-02-02 01:03:43.000000 mpb_lib-0.1.81/mpb_lib/maze/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.181212 mpb_lib-0.1.81/mpb_lib/rpg/
+-rw-r--r--   0 ats        (501) staff       (20)      185 2021-07-20 02:03:49.000000 mpb_lib-0.1.81/mpb_lib/rpg/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     9880 2022-06-01 08:47:58.000000 mpb_lib-0.1.81/mpb_lib/rpg/rpg.py
+-rw-r--r--   0 ats        (501) staff       (20)     2996 2021-11-26 23:16:54.000000 mpb_lib-0.1.81/mpb_lib/rpg/rpg_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.183756 mpb_lib-0.1.81/mpb_lib/rythmbox/
+-rw-r--r--   0 ats        (501) staff       (20)       29 2021-09-06 05:02:03.000000 mpb_lib-0.1.81/mpb_lib/rythmbox/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     2419 2021-12-27 01:25:09.000000 mpb_lib-0.1.81/mpb_lib/rythmbox/rythmbox.py
+-rw-r--r--   0 ats        (501) staff       (20)     5044 2021-09-02 04:33:49.000000 mpb_lib-0.1.81/mpb_lib/rythmbox/rythmbox_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.184793 mpb_lib-0.1.81/mpb_lib/sound/
+-rw-r--r--   0 ats        (501) staff       (20)      881 2023-02-01 23:07:24.000000 mpb_lib-0.1.81/mpb_lib/sound/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.195863 mpb_lib-0.1.81/mpb_lib/sound/wavs/
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:51.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/a.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:15.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/b.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:23.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/c.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:30.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/d.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:35.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/e.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:40.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/f.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:46.000000 mpb_lib-0.1.81/mpb_lib/sound/wavs/g.wav
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.199471 mpb_lib-0.1.81/mpb_lib/tictactoe/
+-rw-r--r--   0 ats        (501) staff       (20)      170 2023-02-01 23:08:05.000000 mpb_lib-0.1.81/mpb_lib/tictactoe/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)      950 2023-02-01 23:08:32.000000 mpb_lib-0.1.81/mpb_lib/tictactoe/tictactoe.py
+-rw-r--r--   0 ats        (501) staff       (20)     2415 2023-02-01 23:08:24.000000 mpb_lib-0.1.81/mpb_lib/tictactoe/tictactoe_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.203939 mpb_lib-0.1.81/mpb_lib/vowelgen/
+-rw-r--r--   0 ats        (501) staff       (20)     2350 2022-08-18 22:51:31.000000 mpb_lib-0.1.81/mpb_lib/vowelgen/HPF.py
+-rw-r--r--   0 ats        (501) staff       (20)      946 2023-02-01 23:02:22.000000 mpb_lib-0.1.81/mpb_lib/vowelgen/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     3277 2022-08-18 22:51:27.000000 mpb_lib-0.1.81/mpb_lib/vowelgen/glottal.py
+-rw-r--r--   0 ats        (501) staff       (20)     6059 2022-08-18 10:39:56.000000 mpb_lib-0.1.81/mpb_lib/vowelgen/threetube.py
+-rw-r--r--   0 ats        (501) staff       (20)     5291 2022-08-18 10:39:53.000000 mpb_lib-0.1.81/mpb_lib/vowelgen/twotube.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-22 02:35:03.172184 mpb_lib-0.1.81/mpb_lib.egg-info/
+-rw-r--r--   0 ats        (501) staff       (20)      336 2023-04-22 02:35:02.000000 mpb_lib-0.1.81/mpb_lib.egg-info/PKG-INFO
+-rw-r--r--   0 ats        (501) staff       (20)      962 2023-04-22 02:35:03.000000 mpb_lib-0.1.81/mpb_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 ats        (501) staff       (20)        1 2023-04-22 02:35:02.000000 mpb_lib-0.1.81/mpb_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 ats        (501) staff       (20)        8 2023-04-22 02:35:02.000000 mpb_lib-0.1.81/mpb_lib.egg-info/top_level.txt
+-rw-r--r--   0 ats        (501) staff       (20)       38 2023-04-22 02:35:03.205742 mpb_lib-0.1.81/setup.cfg
+-rw-r--r--   0 ats        (501) staff       (20)     1043 2023-04-22 02:23:31.000000 mpb_lib-0.1.81/setup.py
```

### Comparing `mpb_lib-0.1.80/mpb_lib/apis/__init__.py` & `mpb_lib-0.1.81/mpb_lib/apis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     直近の気温予測を返す
     """
     d = get_wf_json(code)
     c = int(d[0]["timeSeries"][2]["areas"][0]["temps"][0])
     return int(1.8*c+32)
 
 
-def f2c(f):
+def f_to_c(f):
     """
     華氏(Fahrenheit)から摂氏(Celsius)に変換
     """
     return int((f-32)*(5/9))
 
 
 def get_rpl(code=13):
```

### Comparing `mpb_lib-0.1.80/mpb_lib/cannon/cannon.py` & `mpb_lib-0.1.81/mpb_lib/cannon/cannon.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/cannon/cannon_html.py` & `mpb_lib-0.1.81/mpb_lib/cannon/cannon_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/face/face.py` & `mpb_lib-0.1.81/mpb_lib/face/face.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/face/face_html.py` & `mpb_lib-0.1.81/mpb_lib/face/face_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/maze/__init__.py` & `mpb_lib-0.1.81/mpb_lib/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/rpg/rpg.py` & `mpb_lib-0.1.81/mpb_lib/rpg/rpg.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/rpg/rpg_html.py` & `mpb_lib-0.1.81/mpb_lib/rpg/rpg_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/rythmbox/rythmbox.py` & `mpb_lib-0.1.81/mpb_lib/rythmbox/rythmbox.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/rythmbox/rythmbox_html.py` & `mpb_lib-0.1.81/mpb_lib/rythmbox/rythmbox_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/__init__.py` & `mpb_lib-0.1.81/mpb_lib/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/a.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/a.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/b.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/b.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/c.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/c.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/d.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/d.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/e.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/e.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/f.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/f.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/sound/wavs/g.wav` & `mpb_lib-0.1.81/mpb_lib/sound/wavs/g.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/tictactoe/tictactoe.py` & `mpb_lib-0.1.81/mpb_lib/tictactoe/tictactoe.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/tictactoe/tictactoe_html.py` & `mpb_lib-0.1.81/mpb_lib/tictactoe/tictactoe_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/vowelgen/HPF.py` & `mpb_lib-0.1.81/mpb_lib/vowelgen/HPF.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/vowelgen/__init__.py` & `mpb_lib-0.1.81/mpb_lib/vowelgen/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/vowelgen/glottal.py` & `mpb_lib-0.1.81/mpb_lib/vowelgen/glottal.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/vowelgen/threetube.py` & `mpb_lib-0.1.81/mpb_lib/vowelgen/threetube.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib/vowelgen/twotube.py` & `mpb_lib-0.1.81/mpb_lib/vowelgen/twotube.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/mpb_lib.egg-info/SOURCES.txt` & `mpb_lib-0.1.81/mpb_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.80/setup.py` & `mpb_lib-0.1.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                        'sound/wavs/d.wav',
                        'sound/wavs/e.wav',
                        'sound/wavs/f.wav',
                        'sound/wavs/g.wav',
                        'sound/wavs/a.wav',
                        'sound/wavs/b.wav' ]},
 
-    version='0.1.80', # バージョン
+    version='0.1.81', # バージョン
 
     license='MIT', # ライセンス
 
     install_requires=[],
 
     author='Atsushi Shibata',
     author_email='shibata@m-info.co.jp',
```

