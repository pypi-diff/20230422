# Comparing `tmp/colorist-1.4.0.tar.gz` & `tmp/colorist-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorist-1.4.0.tar", last modified: Mon Apr 10 22:26:56 2023, max compression
+gzip compressed data, was "colorist-1.5.1.tar", last modified: Sat Apr 22 10:28:26 2023, max compression
```

## Comparing `colorist-1.4.0.tar` & `colorist-1.5.1.tar`

### file list

```diff
@@ -1,70 +1,75 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.478059 colorist-1.4.0/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1687 2023-04-02 10:14:25.000000 colorist-1.4.0/INSTALLATION.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.4.0/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 10:14:25.000000 colorist-1.4.0/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    22625 2023-04-10 22:26:56.478197 colorist-1.4.0/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    18625 2023-04-10 22:24:39.000000 colorist-1.4.0/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.4.0/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1436 2023-04-10 22:26:56.478548 colorist-1.4.0/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.467869 colorist-1.4.0/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.470110 colorist-1.4.0/src/colorist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2456 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.472041 colorist-1.4.0/src/colorist/constants/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/constants/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2229 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/constants/ansi.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/constants/ascii.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.473784 colorist-1.4.0/src/colorist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.4.0/src/colorist/helper/.coverage
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.474492 colorist-1.4.0/src/colorist/helper/.pytest_cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/.gitignore
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/README.md
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.468147 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.474941 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.4.0/src/colorist/helper/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1399 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/convert.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      564 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/error.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/generate.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/helper/print.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      316 2023-04-09 23:12:39.000000 colorist-1.4.0/src/colorist/helper/validate.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.475481 colorist-1.4.0/src/colorist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1508 2023-04-09 22:59:24.000000 colorist-1.4.0/src/colorist/model/README.MD
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.476001 colorist-1.4.0/src/colorist/model/abc/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-10 22:22:29.000000 colorist-1.4.0/src/colorist/model/abc/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-10 22:22:29.000000 colorist-1.4.0/src/colorist/model/abc/effect.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/abc/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/abc/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.476439 colorist-1.4.0/src/colorist/model/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      417 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      412 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.476884 colorist-1.4.0/src/colorist/model/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      420 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      415 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/model/foreground/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.477012 colorist-1.4.0/src/colorist/print/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.477469 colorist-1.4.0/src/colorist/print/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2509 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1320 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      518 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      355 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1395 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.477933 colorist-1.4.0/src/colorist/print/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2331 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1142 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      498 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      335 2023-04-10 22:24:37.000000 colorist-1.4.0/src/colorist/print/foreground/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.4.0/src/colorist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2023-04-10 22:24:39.000000 colorist-1.4.0/src/colorist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-10 22:26:56.471135 colorist-1.4.0/src/colorist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    22625 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1756 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.4.0/src/colorist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-04-10 22:26:56.000000 colorist-1.4.0/src/colorist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.357324 colorist-1.5.1/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1759 2023-04-22 10:25:29.000000 colorist-1.5.1/INSTALLATION.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.5.1/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 10:14:25.000000 colorist-1.5.1/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    24114 2023-04-22 10:28:26.357447 colorist-1.5.1/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    19992 2023-04-22 10:25:30.000000 colorist-1.5.1/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.5.1/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1475 2023-04-22 10:28:26.357783 colorist-1.5.1/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.344629 colorist-1.5.1/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.346742 colorist-1.5.1/src/colorist/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2666 2023-04-22 08:37:25.000000 colorist-1.5.1/src/colorist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.348273 colorist-1.5.1/src/colorist/constants/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/constants/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2181 2023-04-11 11:49:16.000000 colorist-1.5.1/src/colorist/constants/ansi.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/constants/ascii.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.350350 colorist-1.5.1/src/colorist/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.5.1/src/colorist/helper/.coverage
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.351033 colorist-1.5.1/src/colorist/helper/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.344910 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.351449 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.5.1/src/colorist/helper/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1973 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/helper/convert.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      733 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/helper/error.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.5.1/src/colorist/helper/generate.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/helper/print.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      492 2023-04-21 23:37:48.000000 colorist-1.5.1/src/colorist/helper/validate.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.351890 colorist-1.5.1/src/colorist/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1789 2023-04-22 08:37:25.000000 colorist-1.5.1/src/colorist/model/README.MD
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.353402 colorist-1.5.1/src/colorist/model/abc/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/effect.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1329 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/model/abc/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/abc/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.354374 colorist-1.5.1/src/colorist/model/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      428 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/model/background/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      417 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      412 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.355101 colorist-1.5.1/src/colorist/model/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      431 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/model/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      420 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      415 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/model/foreground/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.355239 colorist-1.5.1/src/colorist/print/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.356133 colorist-1.5.1/src/colorist/print/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2509 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1320 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      418 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/print/background/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      518 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      355 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1395 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.357181 colorist-1.5.1/src/colorist/print/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2331 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1142 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      382 2023-04-22 10:25:27.000000 colorist-1.5.1/src/colorist/print/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      498 2023-04-21 23:04:21.000000 colorist-1.5.1/src/colorist/print/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      335 2023-04-11 07:01:26.000000 colorist-1.5.1/src/colorist/print/foreground/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.5.1/src/colorist/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2023-04-22 10:25:30.000000 colorist-1.5.1/src/colorist/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-22 10:28:26.347634 colorist-1.5.1/src/colorist.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    24114 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1934 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.5.1/src/colorist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-04-22 10:28:26.000000 colorist-1.5.1/src/colorist.egg-info/top_level.txt
```

### Comparing `colorist-1.4.0/INSTALLATION.md` & `colorist-1.5.1/INSTALLATION.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.3.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 How to Install Colorist for Python 🌈
 ## Prerequisites
-* Python 3.10 or higher
+* Python version:
+    * 2.7
+    * 3.10, 3.11 or higher
 * Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
 
 ## Installation
 ### PyPI
 Assuming that Python is installed already, execute this command in the terminal:
 
 ```shell
-pip3 install colorist
+pip install colorist
 ```
 
 If you already have installed Colorist for Python, use this command to upgrade to latest version:
 
 ```shell
-pip3 install --upgrade colorist
+pip install --upgrade colorist
 ```
 
 ### Homebrew
 If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Colorist for Python:
 
 ```shell
 brew tap jakob-bagterp/colorist
```

### Comparing `colorist-1.4.0/LICENSE.md` & `colorist-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/PKG-INFO` & `colorist-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.4.0
+Version: 1.5.1
 Summary: Colorist for Python
 Home-page: https://github.com/jakob-bagterp/colorist-for-python
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: 3-Clause BSD License
 Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
 Keywords: python,colors,terminal
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
@@ -129,16 +130,16 @@
 print("I want " + Color.RED + "red" + Color.OFF + " color inside this paragraph")
 ```
 
 Both options appear the same in the terminal:
 
 ![Example of terminal message with red text color](/assets/images/examples/color_custom_text_red.png)
 
-### Print RGB and HSL Colors
-Note that not all terminals support RGB or HSL colors. If your terminal does support such advanced colors, read on.
+### Print RGB, HSL and Hex Colors
+Note that not all terminals support RGB, HSL or Hex colors. If your terminal does support such advanced colors, read on.
 
 #### RGB Colors
 Try the `rgb` and `bg_rgb` methods for a full line of colored text. The values for red, green, blue can be an integer between `0-255`.
 
 ```python
 from colorist import rgb, bg_rgb
 
@@ -190,14 +191,43 @@
 print(f"I want to use {mustard_green}mustard green{mustard_green.OFF} and {bg_steel_gray}steel blue{bg_steel_gray.OFF} colors inside this paragraph")
 ```
 
 How it appears in the terminal:
 
 ![Another example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_custom_text.png)
 
+#### Hex Colors
+Try the `hex` and `bg_hex` methods for a full line of colored text. Allowed Hex values are, for instance, `#00aaff` or `#0af`, alternatively without the hash sign as `00aaff` or `0af`.
+
+```python
+from colorist import hex, bg_hex
+
+hex("I want this text in coral Hex colors", "#ff7f50")
+bg_hex("I want this background in coral Hex colors", "#ff7f50")
+```
+
+How it appears in the terminal:
+
+![Example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_full_text.png)
+
+Or customize the styling of text and background with the `ColorHex` and `BgColorHex` classes:
+
+```python
+from colorist import ColorHex, BgColorHex
+
+watermelon_red = ColorHex("#ff5733")
+bg_mint_green = BgColorHex("#99ff99")
+
+print(f"I want to use {watermelon_red}watermelon pink{watermelon_red.OFF} and {bg_mint_green}mint green{bg_mint_green.OFF} colors inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Another example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_custom_text.png)
+
 ### Print Effects and Other Styles
 In addition to colors, Colorist can also add effects when you print text in the terminal. How to print a full line of text with effects:
 
 ```python
 from colorist import effect_blink
 
 effect_blink("This is BLINKING!")
@@ -246,62 +276,66 @@
 ![Example of terminal message with red and blinking text](/assets/images/examples/effect_custom_text_blink_red.gif)
 
 Similar to `Color.OFF`, remember to turn off an effect with the relevant reset option (e.g `Effect.BOLD_OFF`, `Effect.DIM_OFF`, etc. or even just `Effect.OFF`) every time you want to revert back to the default terminal text style. Otherwise the effect may spill over and into other terminal messages.
 
 # Supported Colors and Styles
 Colorist is based on [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code), a standard that defines colors, styling and effects for text in terminal windows. Note that most terminals support all color options, but not all:
 
-| Category                                               | Color Options                                      |
-| ------------------------------------------------------ | -------------------------------------------------- |
-| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                       |
-| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                     |
-| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL` |
+| Category                                               | Color Options                                                                |
+| ------------------------------------------------------ | ---------------------------------------------------------------------------- |
+| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                                                 |
+| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                                               |
+| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL`, `ColorHex`, `BgColorHex` |
 
 ## Foreground Text
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
 | ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
 | ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
 | ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
 | ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
 | ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
 | ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
 | ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
 | ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
+| - | - | `Color.DEFAULT` | - |
 | - | - | `Color.OFF` | - |
 | ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
 | ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
 | ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
 | ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
 | ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
 | ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
 | ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
 | ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
+| - | - | `BrightColor.DEFAULT` | - |
 | - | - | `BrightColor.OFF` | - |
 
 ## Background
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
 | ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
 | ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
 | ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
 | ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
 | ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
 | ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
 | ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
 | ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
+| - | - | `BgColor.DEFAULT` | - |
 | - | - | `BgColor.OFF` | - |
 | ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
 | ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
 | ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
 | ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
 | ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
 | ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
 | ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
 | ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
+| - | - |`BgBrightColor.DEFAULT` | - |
 | - | - | `BgBrightColor.OFF` | - |
 
 ## Effects
 | Effect           | Full Text Function         | Custom             | Reset                  | Example    |
 | ---------------- | -------------------------- | ------------------ | ---------------------- | ---------- |
 | **Bold**         | `effect_bold("text")`      | `Effect.BOLD`      | `Effect.BOLD_OFF`      | ![Example of terminal message with bold text](/assets/images/examples/effect_map/bold_full_text_140x16.png) |
 | Dim              | `effect_dim("text")`       | `Effect.DIM`       | `Effect.DIM_OFF`       | ![Example of terminal message with dimmed text](/assets/images/examples/effect_map/dim_full_text_140x16.png) |
@@ -317,37 +351,39 @@
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.3.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 How to Install Colorist for Python 🌈
 ## Prerequisites
-* Python 3.10 or higher
+* Python version:
+    * 2.7
+    * 3.10, 3.11 or higher
 * Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
 
 ## Installation
 ### PyPI
 Assuming that Python is installed already, execute this command in the terminal:
 
 ```shell
-pip3 install colorist
+pip install colorist
 ```
 
 If you already have installed Colorist for Python, use this command to upgrade to latest version:
 
 ```shell
-pip3 install --upgrade colorist
+pip install --upgrade colorist
 ```
 
 ### Homebrew
 If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Colorist for Python:
 
 ```shell
 brew tap jakob-bagterp/colorist
```

### Comparing `colorist-1.4.0/README.md` & `colorist-1.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
@@ -106,16 +106,16 @@
 print("I want " + Color.RED + "red" + Color.OFF + " color inside this paragraph")
 ```
 
 Both options appear the same in the terminal:
 
 ![Example of terminal message with red text color](/assets/images/examples/color_custom_text_red.png)
 
-### Print RGB and HSL Colors
-Note that not all terminals support RGB or HSL colors. If your terminal does support such advanced colors, read on.
+### Print RGB, HSL and Hex Colors
+Note that not all terminals support RGB, HSL or Hex colors. If your terminal does support such advanced colors, read on.
 
 #### RGB Colors
 Try the `rgb` and `bg_rgb` methods for a full line of colored text. The values for red, green, blue can be an integer between `0-255`.
 
 ```python
 from colorist import rgb, bg_rgb
 
@@ -167,14 +167,43 @@
 print(f"I want to use {mustard_green}mustard green{mustard_green.OFF} and {bg_steel_gray}steel blue{bg_steel_gray.OFF} colors inside this paragraph")
 ```
 
 How it appears in the terminal:
 
 ![Another example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_custom_text.png)
 
+#### Hex Colors
+Try the `hex` and `bg_hex` methods for a full line of colored text. Allowed Hex values are, for instance, `#00aaff` or `#0af`, alternatively without the hash sign as `00aaff` or `0af`.
+
+```python
+from colorist import hex, bg_hex
+
+hex("I want this text in coral Hex colors", "#ff7f50")
+bg_hex("I want this background in coral Hex colors", "#ff7f50")
+```
+
+How it appears in the terminal:
+
+![Example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_full_text.png)
+
+Or customize the styling of text and background with the `ColorHex` and `BgColorHex` classes:
+
+```python
+from colorist import ColorHex, BgColorHex
+
+watermelon_red = ColorHex("#ff5733")
+bg_mint_green = BgColorHex("#99ff99")
+
+print(f"I want to use {watermelon_red}watermelon pink{watermelon_red.OFF} and {bg_mint_green}mint green{bg_mint_green.OFF} colors inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Another example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_custom_text.png)
+
 ### Print Effects and Other Styles
 In addition to colors, Colorist can also add effects when you print text in the terminal. How to print a full line of text with effects:
 
 ```python
 from colorist import effect_blink
 
 effect_blink("This is BLINKING!")
@@ -223,62 +252,66 @@
 ![Example of terminal message with red and blinking text](/assets/images/examples/effect_custom_text_blink_red.gif)
 
 Similar to `Color.OFF`, remember to turn off an effect with the relevant reset option (e.g `Effect.BOLD_OFF`, `Effect.DIM_OFF`, etc. or even just `Effect.OFF`) every time you want to revert back to the default terminal text style. Otherwise the effect may spill over and into other terminal messages.
 
 # Supported Colors and Styles
 Colorist is based on [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code), a standard that defines colors, styling and effects for text in terminal windows. Note that most terminals support all color options, but not all:
 
-| Category                                               | Color Options                                      |
-| ------------------------------------------------------ | -------------------------------------------------- |
-| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                       |
-| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                     |
-| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL` |
+| Category                                               | Color Options                                                                |
+| ------------------------------------------------------ | ---------------------------------------------------------------------------- |
+| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                                                 |
+| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                                               |
+| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL`, `ColorHex`, `BgColorHex` |
 
 ## Foreground Text
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
 | ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
 | ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
 | ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
 | ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
 | ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
 | ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
 | ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
 | ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
+| - | - | `Color.DEFAULT` | - |
 | - | - | `Color.OFF` | - |
 | ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
 | ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
 | ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
 | ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
 | ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
 | ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
 | ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
 | ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
+| - | - | `BrightColor.DEFAULT` | - |
 | - | - | `BrightColor.OFF` | - |
 
 ## Background
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
 | ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
 | ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
 | ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
 | ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
 | ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
 | ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
 | ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
 | ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
+| - | - | `BgColor.DEFAULT` | - |
 | - | - | `BgColor.OFF` | - |
 | ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
 | ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
 | ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
 | ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
 | ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
 | ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
 | ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
 | ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
+| - | - |`BgBrightColor.DEFAULT` | - |
 | - | - | `BgBrightColor.OFF` | - |
 
 ## Effects
 | Effect           | Full Text Function         | Custom             | Reset                  | Example    |
 | ---------------- | -------------------------- | ------------------ | ---------------------- | ---------- |
 | **Bold**         | `effect_bold("text")`      | `Effect.BOLD`      | `Effect.BOLD_OFF`      | ![Example of terminal message with bold text](/assets/images/examples/effect_map/bold_full_text_140x16.png) |
 | Dim              | `effect_dim("text")`       | `Effect.DIM`       | `Effect.DIM_OFF`       | ![Example of terminal message with dimmed text](/assets/images/examples/effect_map/dim_full_text_140x16.png) |
```

### Comparing `colorist-1.4.0/setup.cfg` & `colorist-1.5.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	python
 	colors
 	terminal
 url = https://github.com/jakob-bagterp/colorist-for-python
 project_urls = 
 	Bug Tracker = https://github.com/jakob-bagterp/colorist-for-python/issues
 classifiers = 
+	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 license = 3-Clause BSD License
 license_files = LICENSE.md
@@ -33,17 +34,17 @@
 include_package_data = True
 
 [options.extras_require]
 testing = 
 	coverage ==7.2.3
 	flake8 ==6.0.0
 	mypy ==1.2.0
-	pytest ==7.3.0
+	pytest ==7.3.1
 	pytest-cov ==4.0.0
-	tox ==4.4.11
+	tox ==4.4.12
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `colorist-1.4.0/src/colorist/__init__.py` & `colorist-1.5.1/src/colorist/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 # Copyright 2022 – present, Jakob Bagterp. BSD 3-Clause license and refer to LICENSE file.
 
 __all__ = [
-    "Color", "BrightColor", "BgColor", "BgBrightColor", "ColorRGB", "BgColorRGB", "ColorHSL", "BgColorHSL", "Effect",
+    "Color", "BrightColor", "BgColor", "BgBrightColor", "ColorHex", "BgColorHex", "ColorRGB", "BgColorRGB", "ColorHSL", "BgColorHSL", "Effect",
     "black", "red", "green", "yellow", "blue", "magenta", "cyan", "white",
     "bright_black", "bright_red", "bright_green", "bright_yellow", "bright_blue", "bright_magenta", "bright_cyan", "bright_white",
     "bg_black", "bg_red", "bg_green", "bg_yellow", "bg_blue", "bg_magenta", "bg_cyan", "bg_white",
     "bg_bright_black", "bg_bright_red", "bg_bright_green", "bg_bright_yellow", "bg_bright_blue", "bg_bright_magenta", "bg_bright_cyan", "bg_bright_white",
     "effect_bold", "effect_dim", "effect_underline", "effect_blink", "effect_reverse", "effect_hide",
-    "rgb", "hsl",
-    "bg_rgb", "bg_hsl"
+    "hex", "rgb", "hsl",
+    "bg_hex", "bg_rgb", "bg_hsl"
 ]
 
 from .model.background.bright_color import BgBrightColor
 from .model.background.color import BgColor
+from .model.background.hex import BgColorHex
 from .model.background.hsl import BgColorHSL
 from .model.background.rgb import BgColorRGB
 from .model.effect import Effect
 from .model.foreground.bright_color import BrightColor
 from .model.foreground.color import Color
+from .model.foreground.hex import ColorHex
 from .model.foreground.hsl import ColorHSL
 from .model.foreground.rgb import ColorRGB
 from .print.background.bright_color import (bg_bright_black, bg_bright_blue,
                                             bg_bright_cyan, bg_bright_green,
                                             bg_bright_magenta, bg_bright_red,
                                             bg_bright_white, bg_bright_yellow)
 from .print.background.color import (bg_black, bg_blue, bg_cyan, bg_green,
                                      bg_magenta, bg_red, bg_white, bg_yellow)
+from .print.background.hex import bg_hex
 from .print.background.hsl import bg_hsl
 from .print.background.rgb import bg_rgb
 from .print.effect import (effect_blink, effect_bold, effect_dim, effect_hide,
                            effect_reverse, effect_underline)
 from .print.foreground.bright_color import (bright_black, bright_blue,
                                             bright_cyan, bright_green,
                                             bright_magenta, bright_red,
                                             bright_white, bright_yellow)
 from .print.foreground.color import (black, blue, cyan, green, magenta, red,
                                      white, yellow)
+from .print.foreground.hex import hex
 from .print.foreground.hsl import hsl
 from .print.foreground.rgb import rgb
 from .version import __version__  # noqa
```

### Comparing `colorist-1.4.0/src/colorist/constants/ansi.py` & `colorist-1.5.1/src/colorist/constants/ansi.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 @unique
 class AnsiRgbColorSelector(Enum):
-    """ANSI RGB color selector to be mixed with AnsiColor for foreground (30-37), background (40-47) and other combinations."""
+    """ANSI RGB color selector to be mixed with values for red, green, blue."""
 
     FOREGROUND = "38;2"
     """Parameter for RGB foreground color sequence: 38;2;r;g;b."""
 
     BACKGROUND = "48;2"
     """Parameter for RGB background color sequence: 48;2;r;g;b."""
```

### Comparing `colorist-1.4.0/src/colorist/helper/.coverage` & `colorist-1.5.1/src/colorist/helper/.coverage`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/helper/error.py` & `colorist-1.5.1/src/colorist/helper/error.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,7 +6,11 @@
 
 def message_for_hsl_hue_value_error(value: float) -> str:
     return f"Value for \"hue\" is {value}, but should be number between 0 and 360."
 
 
 def message_for_hsl_percentage_value_error(param: str, value: float) -> str:
     return f"Value for \"{param}\" is {value}, but should be number between 0(%) and 100(%)."
+
+
+def message_for_hex_value_error(value: str) -> str:
+    return f"Value {value} isn't valid Hex color code, and should be for instance #B4FBB8 or B4FBB8, #B4F or B4F."
```

### Comparing `colorist-1.4.0/src/colorist/helper/generate.py` & `colorist-1.5.1/src/colorist/helper/generate.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/helper/print.py` & `colorist-1.5.1/src/colorist/helper/print.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/README.MD` & `colorist-1.5.1/src/colorist/model/README.MD`

 * *Files 11% similar despite different names*

```diff
@@ -93,7 +93,26 @@
 }
 class ColorHSL
 class BgColorHSL
 
 HSL_ABC <|-- ColorHSL
 HSL_ABC <|-- BgColorHSL
 ```
+
+## Hex Color Classes
+```mermaid
+classDiagram
+class Hex_ABC {
+    <<abstract>>
+    +str hex
+    +ColorRGB _rgb
+    +str _ansi_code
+    +str OFF
+    +convert_hex_to_rgb()
+    +generate_ansi_code()
+}
+class ColorHex
+class BgColorHex
+
+Hex_ABC <|-- ColorHex
+Hex_ABC <|-- BgColorHex
+```
```

### Comparing `colorist-1.4.0/src/colorist/model/abc/color.py` & `colorist-1.5.1/src/colorist/model/abc/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/abc/hsl.py` & `colorist-1.5.1/src/colorist/model/abc/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/abc/rgb.py` & `colorist-1.5.1/src/colorist/model/abc/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/background/bright_color.py` & `colorist-1.5.1/src/colorist/model/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/background/color.py` & `colorist-1.5.1/src/colorist/model/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/effect.py` & `colorist-1.5.1/src/colorist/model/effect.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/foreground/bright_color.py` & `colorist-1.5.1/src/colorist/model/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/model/foreground/color.py` & `colorist-1.5.1/src/colorist/model/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/print/background/bright_color.py` & `colorist-1.5.1/src/colorist/print/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/print/background/color.py` & `colorist-1.5.1/src/colorist/print/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/print/background/hsl.py` & `colorist-1.5.1/src/colorist/print/background/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/print/effect.py` & `colorist-1.5.1/src/colorist/print/effect.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/print/foreground/bright_color.py` & `colorist-1.5.1/src/colorist/print/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist/print/foreground/color.py` & `colorist-1.5.1/src/colorist/print/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.4.0/src/colorist.egg-info/PKG-INFO` & `colorist-1.5.1/src/colorist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.4.0
+Version: 1.5.1
 Summary: Colorist for Python
 Home-page: https://github.com/jakob-bagterp/colorist-for-python
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: 3-Clause BSD License
 Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
 Keywords: python,colors,terminal
 Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
@@ -129,16 +130,16 @@
 print("I want " + Color.RED + "red" + Color.OFF + " color inside this paragraph")
 ```
 
 Both options appear the same in the terminal:
 
 ![Example of terminal message with red text color](/assets/images/examples/color_custom_text_red.png)
 
-### Print RGB and HSL Colors
-Note that not all terminals support RGB or HSL colors. If your terminal does support such advanced colors, read on.
+### Print RGB, HSL and Hex Colors
+Note that not all terminals support RGB, HSL or Hex colors. If your terminal does support such advanced colors, read on.
 
 #### RGB Colors
 Try the `rgb` and `bg_rgb` methods for a full line of colored text. The values for red, green, blue can be an integer between `0-255`.
 
 ```python
 from colorist import rgb, bg_rgb
 
@@ -190,14 +191,43 @@
 print(f"I want to use {mustard_green}mustard green{mustard_green.OFF} and {bg_steel_gray}steel blue{bg_steel_gray.OFF} colors inside this paragraph")
 ```
 
 How it appears in the terminal:
 
 ![Another example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_custom_text.png)
 
+#### Hex Colors
+Try the `hex` and `bg_hex` methods for a full line of colored text. Allowed Hex values are, for instance, `#00aaff` or `#0af`, alternatively without the hash sign as `00aaff` or `0af`.
+
+```python
+from colorist import hex, bg_hex
+
+hex("I want this text in coral Hex colors", "#ff7f50")
+bg_hex("I want this background in coral Hex colors", "#ff7f50")
+```
+
+How it appears in the terminal:
+
+![Example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_full_text.png)
+
+Or customize the styling of text and background with the `ColorHex` and `BgColorHex` classes:
+
+```python
+from colorist import ColorHex, BgColorHex
+
+watermelon_red = ColorHex("#ff5733")
+bg_mint_green = BgColorHex("#99ff99")
+
+print(f"I want to use {watermelon_red}watermelon pink{watermelon_red.OFF} and {bg_mint_green}mint green{bg_mint_green.OFF} colors inside this paragraph")
+```
+
+How it appears in the terminal:
+
+![Another example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_custom_text.png)
+
 ### Print Effects and Other Styles
 In addition to colors, Colorist can also add effects when you print text in the terminal. How to print a full line of text with effects:
 
 ```python
 from colorist import effect_blink
 
 effect_blink("This is BLINKING!")
@@ -246,62 +276,66 @@
 ![Example of terminal message with red and blinking text](/assets/images/examples/effect_custom_text_blink_red.gif)
 
 Similar to `Color.OFF`, remember to turn off an effect with the relevant reset option (e.g `Effect.BOLD_OFF`, `Effect.DIM_OFF`, etc. or even just `Effect.OFF`) every time you want to revert back to the default terminal text style. Otherwise the effect may spill over and into other terminal messages.
 
 # Supported Colors and Styles
 Colorist is based on [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code), a standard that defines colors, styling and effects for text in terminal windows. Note that most terminals support all color options, but not all:
 
-| Category                                               | Color Options                                      |
-| ------------------------------------------------------ | -------------------------------------------------- |
-| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                       |
-| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                     |
-| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL` |
+| Category                                               | Color Options                                                                |
+| ------------------------------------------------------ | ---------------------------------------------------------------------------- |
+| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                                                 |
+| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                                               |
+| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL`, `ColorHex`, `BgColorHex` |
 
 ## Foreground Text
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
 | ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
 | ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
 | ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
 | ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
 | ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
 | ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
 | ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
 | ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
+| - | - | `Color.DEFAULT` | - |
 | - | - | `Color.OFF` | - |
 | ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
 | ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
 | ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
 | ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
 | ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
 | ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
 | ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
 | ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
+| - | - | `BrightColor.DEFAULT` | - |
 | - | - | `BrightColor.OFF` | - |
 
 ## Background
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
 | ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
 | ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
 | ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
 | ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
 | ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
 | ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
 | ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
 | ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
+| - | - | `BgColor.DEFAULT` | - |
 | - | - | `BgColor.OFF` | - |
 | ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
 | ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
 | ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
 | ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
 | ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
 | ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
 | ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
 | ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
+| - | - |`BgBrightColor.DEFAULT` | - |
 | - | - | `BgBrightColor.OFF` | - |
 
 ## Effects
 | Effect           | Full Text Function         | Custom             | Reset                  | Example    |
 | ---------------- | -------------------------- | ------------------ | ---------------------- | ---------- |
 | **Bold**         | `effect_bold("text")`      | `Effect.BOLD`      | `Effect.BOLD_OFF`      | ![Example of terminal message with bold text](/assets/images/examples/effect_map/bold_full_text_140x16.png) |
 | Dim              | `effect_dim("text")`       | `Effect.DIM`       | `Effect.DIM_OFF`       | ![Example of terminal message with dimmed text](/assets/images/examples/effect_map/dim_full_text_140x16.png) |
@@ -317,37 +351,39 @@
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.3.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+![Python 2.7 | 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=2.7%20|%203.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 
 # 🌈 How to Install Colorist for Python 🌈
 ## Prerequisites
-* Python 3.10 or higher
+* Python version:
+    * 2.7
+    * 3.10, 3.11 or higher
 * Terminal that supports color (i.e. [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code))
 
 ## Installation
 ### PyPI
 Assuming that Python is installed already, execute this command in the terminal:
 
 ```shell
-pip3 install colorist
+pip install colorist
 ```
 
 If you already have installed Colorist for Python, use this command to upgrade to latest version:
 
 ```shell
-pip3 install --upgrade colorist
+pip install --upgrade colorist
 ```
 
 ### Homebrew
 If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Colorist for Python:
 
 ```shell
 brew tap jakob-bagterp/colorist
```

### Comparing `colorist-1.4.0/src/colorist.egg-info/SOURCES.txt` & `colorist-1.5.1/src/colorist.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,31 @@
 src/colorist/helper/.pytest_cache/README.md
 src/colorist/helper/.pytest_cache/v/cache/nodeids
 src/colorist/helper/.pytest_cache/v/cache/stepwise
 src/colorist/model/README.MD
 src/colorist/model/effect.py
 src/colorist/model/abc/color.py
 src/colorist/model/abc/effect.py
+src/colorist/model/abc/hex.py
 src/colorist/model/abc/hsl.py
 src/colorist/model/abc/rgb.py
 src/colorist/model/background/bright_color.py
 src/colorist/model/background/color.py
+src/colorist/model/background/hex.py
 src/colorist/model/background/hsl.py
 src/colorist/model/background/rgb.py
 src/colorist/model/foreground/bright_color.py
 src/colorist/model/foreground/color.py
+src/colorist/model/foreground/hex.py
 src/colorist/model/foreground/hsl.py
 src/colorist/model/foreground/rgb.py
 src/colorist/print/effect.py
 src/colorist/print/background/bright_color.py
 src/colorist/print/background/color.py
+src/colorist/print/background/hex.py
 src/colorist/print/background/hsl.py
 src/colorist/print/background/rgb.py
 src/colorist/print/foreground/bright_color.py
 src/colorist/print/foreground/color.py
+src/colorist/print/foreground/hex.py
 src/colorist/print/foreground/hsl.py
 src/colorist/print/foreground/rgb.py
```

