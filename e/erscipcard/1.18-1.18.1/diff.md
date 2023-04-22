# Comparing `tmp/erscipcard-1.18.tar.gz` & `tmp/erscipcard-1.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.18.tar", last modified: Fri Apr 21 11:26:29 2023, max compression
+gzip compressed data, was "erscipcard-1.18.1.tar", last modified: Sat Apr 22 19:56:30 2023, max compression
```

## Comparing `erscipcard-1.18.tar` & `erscipcard-1.18.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.247776 erscipcard-1.18/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-21 11:26:21.000000 erscipcard-1.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-21 11:26:21.000000 erscipcard-1.18/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-21 11:26:29.247776 erscipcard-1.18/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1053 2023-04-21 11:26:21.000000 erscipcard-1.18/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.233775 erscipcard-1.18/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)      313 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.234775 erscipcard-1.18/erscipcard/migrations/
--rw-r--r--   0 root         (0) root         (0)     1503 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.236775 erscipcard-1.18/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    11002 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    14825 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/BTITR.TTF
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.230775 erscipcard-1.18/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.238775 erscipcard-1.18/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.239776 erscipcard-1.18/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.241776 erscipcard-1.18/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.241776 erscipcard-1.18/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.246776 erscipcard-1.18/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/static/spinners.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.246776 erscipcard-1.18/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      241 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.246776 erscipcard-1.18/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    12726 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/templates/erscipcard/ou.html
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/templates/replace_re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.247776 erscipcard-1.18/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    11871 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-04-21 11:26:21.000000 erscipcard-1.18/erscipcard/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:26:29.234775 erscipcard-1.18/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-21 11:26:28.000000 erscipcard-1.18/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-21 11:26:28.000000 erscipcard-1.18/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 11:26:28.000000 erscipcard-1.18/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 11:26:28.000000 erscipcard-1.18/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-21 11:26:28.000000 erscipcard-1.18/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      767 2023-04-21 11:26:29.248776 erscipcard-1.18/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-21 11:26:21.000000 erscipcard-1.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.662840 erscipcard-1.18.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-22 19:56:21.000000 erscipcard-1.18.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-22 19:56:21.000000 erscipcard-1.18.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-04-22 19:56:30.662840 erscipcard-1.18.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-22 19:56:21.000000 erscipcard-1.18.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.645840 erscipcard-1.18.1/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.647840 erscipcard-1.18.1/erscipcard/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.649840 erscipcard-1.18.1/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/BTITR.TTF
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.642840 erscipcard-1.18.1/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.651840 erscipcard-1.18.1/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.653840 erscipcard-1.18.1/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.654840 erscipcard-1.18.1/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.655840 erscipcard-1.18.1/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.660840 erscipcard-1.18.1/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinners.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.661840 erscipcard-1.18.1/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.661840 erscipcard-1.18.1/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12711 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/erscipcard/ou.html
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/replace_re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.661840 erscipcard-1.18.1/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    11853 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.646840 erscipcard-1.18.1/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-22 19:56:30.663840 erscipcard-1.18.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-22 19:56:21.000000 erscipcard-1.18.1/setup.py
```

### Comparing `erscipcard-1.18/LICENSE` & `erscipcard-1.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/PKG-INFO` & `erscipcard-1.18.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18
+Version: 1.18.1
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `erscipcard-1.18/README.md` & `erscipcard-1.18.1/README.md`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/models.py` & `erscipcard-1.18.1/erscipcard/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,19 +19,25 @@
 class PassType(models.Model):
     name = models.CharField(max_length=30)
     def __str__(self):
         return self.name
 '''
 class User1(models.Model):
 	name = models.CharField(max_length=100 ,verbose_name='نام و نام خانوادگی')
+	fathername = models.CharField(max_length=30,verbose_name='نام پدر')
 	personeli = models.CharField(max_length=20,unique=True,verbose_name='شماره پرسنلی')
 	etebar = models.CharField(max_length=10,validators=[valid_date] ,verbose_name='تاريخ اعتبار')
-	pic = models.ImageField(upload_to='images/', blank=True, null=True ,verbose_name='تصویر')
-	number = models.IntegerField(default = 1 , unique=True ,verbose_name='شماره کارت')
 	melli = models.CharField(max_length=10,unique=True,verbose_name='کد ملی')
-	postal = models.CharField(max_length=10,unique=False,null=True,blank=True,verbose_name='کد‍پستی')
-	position = models.CharField(max_length=30,unique=False,null=True,blank=True,verbose_name='محل کار')
-	gharardad = models.CharField(max_length=20,unique=False,null=True,blank=True,verbose_name='نوع قرارداد')
+	pic = models.ImageField(upload_to='images/', blank=True, null=True ,verbose_name='تصویر')
+	shenasname = models.CharField(max_length=10,verbose_name='شماره شناسنامه')
+	postal = models.CharField(max_length=10,null=True,blank=True,verbose_name='کدپستی')
+	position = models.CharField(max_length=30,null=True,blank=True,verbose_name='محل کار')
+	gharardad = models.CharField(max_length=20,null=True,blank=True,verbose_name='نوع قرارداد')
+	address = models.TextField(null=True,blank=True,verbose_name='آدرس')
+	reserv1 = models.CharField(max_length=30,null=True,blank=True,verbose_name='')
+	reserv2 = models.CharField(max_length=30,null=True,blank=True,verbose_name='')
+	reserv3 = models.CharField(max_length=30,null=True,blank=True,verbose_name='')
+	reserv4 = models.TextField(null=True,blank=True,verbose_name='توضیحات')
 	
 	def __str__(self):
 	    return self.name
```

### Comparing `erscipcard-1.18/erscipcard/static/1.docx` & `erscipcard-1.18.1/erscipcard/static/1.docx`

 * *Files 19% similar despite different names*

#### docx2txt

```diff
@@ -1,13 +1,13 @@
 {%p for u in user %}
 
                                کارت تردد
 {{ pic[u.id] }}
                               شماره کارت
-                                {{ u.number }}
+                                  {{ u.id }}
 
 
 نام و نام خانوادگی : {{ u.name }}
 شماره : {{ u.personeli }}
 تاریخ انقضا :  {{ u.etebar }}
```

### Comparing `erscipcard-1.18/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.18.1/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/BTITR.TTF` & `erscipcard-1.18.1/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.18.1/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.18.1/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.18.1/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.18.1/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/css/style.css` & `erscipcard-1.18.1/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/css/util.css` & `erscipcard-1.18.1/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.18.1/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.18.1/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.18.1/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.18.1/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.18.1/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.18.1/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.18.1/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.18.1/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.18.1/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.18.1/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.18.1/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/favicon.ico` & `erscipcard-1.18.1/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/logo.png` & `erscipcard-1.18.1/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/main.css` & `erscipcard-1.18.1/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/atebits.css` & `erscipcard-1.18.1/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/ball.css` & `erscipcard-1.18.1/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/circles.css` & `erscipcard-1.18.1/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/dots.css` & `erscipcard-1.18.1/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/echo.css` & `erscipcard-1.18.1/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/flower.css` & `erscipcard-1.18.1/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/gauge.css` & `erscipcard-1.18.1/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.18.1/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.18.1/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.18.1/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.18.1/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.18.1/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/plus.css` & `erscipcard-1.18.1/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/pong.css` & `erscipcard-1.18.1/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/pulse.css` & `erscipcard-1.18.1/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.18.1/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/spinner.css` & `erscipcard-1.18.1/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.18.1/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.18.1/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/throbber.css` & `erscipcard-1.18.1/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/timer.css` & `erscipcard-1.18.1/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/whirly.css` & `erscipcard-1.18.1/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.18.1/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/static/spinners.css` & `erscipcard-1.18.1/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.18.1/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.18.1/erscipcard/templates/erscipcard/ou.html`

 * *Files 2% similar despite different names*

```diff
@@ -133,28 +133,28 @@
 					</div>
 				</form>
 				
 			
 				<div class="table-responsive">
 					<table class="table table-bordered table-striped table-hover" id="userTable">
 						<tr>
-						<th  onclick="sortTable(0)" >نام و نام خانوادگی</th>
-						<th  onclick="sortTable(1)" >شماره پرسنلی</th>
-						<th  onclick="sortTable(2)" >شماره کارت</th>
+						<th  onclick="sortTable(0)" >شماره کارت</th>
+						<th  onclick="sortTable(1)" >نام و نام خانوادگی</th>
+						<th  onclick="sortTable(2)" >شماره پرسنلی</th>
 						<th>کد ملی</th>
 						<th> تاریخ اعتبار </th>
 						<th>تصویر</th>
 						<th></th>
 						<th></th>
 						</tr>
 						{% for i in userlist %}
 						<tr>
+						<td>{{i.id}}</td>
 						<td>{{i.name}}</td>
 						<td>{{i.personeli}}</td>
-						<td>{{i.number}}</td>
 						<td>{{i.melli}}</td>
 						<td>{{i.etebar}}</td>
 						<td><a href="#" onclick="showpic({{i.id}});" ><i class="fa fa-picture-o" aria-hidden="true"></i></a></td>
 						<td><a class="btn btn-primary" href="#" onclick="loadershow();window.open('/erscipcard/edituser?id={{i.id}}','_self');">ویرایش</a></td>
 						<td><a class="btn btn-danger" href="#" onclick="loadershow();window.open('/erscipcard/deluser?id={{i.id}}','_self');">پاک شود</a></td>
 						</tr>
 						{% endfor %}
@@ -191,23 +191,23 @@
     <div class="modal bottom fade" id="cardpn" tabindex="-1" data-backdrop="static" data-keyboard="false">
       <div class="modal-dialog modal-frame modal-bottom ">
         <div class="modal-content">
           <div class="modal-header">
             <h5 class="modal-title" id="exampleModalLabel">چاپ یک یا چند کارت</h5>            
           </div>
           <div class="modal-body">
-			<form  class="row" id="login" method="GET" enctype="multipart/form-data" action="/erscipcard/printcard2/" >
+			<form  id="login" method="GET" enctype="multipart/form-data" action="/erscipcard/printcard2/" >
 				{% csrf_token %}
 				<div class="col-md-12 mb-3" >
 					<input type="input" class="form-control" name="fromprn" id="fromprn"  />
 				</div>
 				<div class="col-md-12 mb-3" >
 					<input type="input" class="form-control" name="toprn" id="toprn"  />
 				</div>
-				<div class="col-md-8 mb-3" >
+				<div class="col-md-12 mb-3" >
                     <input type="radio" id="wordfile" name="ftype" value="2"/>
                     <label for="wordfile">فایل Word</label>
                     <input type="radio" id="pdffile" name="ftype" value="1"/>
                     <label for="pdffile">فایل Pdf</label>
                 </div>
 				<div class="col-md-12 mb-3" >
 					<input type="submit" class="btn btn-primary ml-3"   value="ارسال" />
```

#### html2text {}

```diff
@@ -39,18 +39,18 @@
 {{ field}}
 {% endfor %}
 ذخیره
 {% elif var1 == 3 %}
 {% csrf_token %}
 [{{data}}            ]
 [جستجو]
-نام و ناشماره پرشماره �کد ملیتاریخ  تصویر
-خانوادگی                                    اعتبار
-{{i.name}}    {              {           {          {                 ویر�پاک
-              {i.personeli}} {i.number}} {i.melli}} {i.etebar}}              شود
+شمار�نام و �شماره پرکد ملیتاریخ  تصویر
+کارت خانوادگی                     اعتبار
+{{i.id}} {{i.name}} {              {          {                 ویر�پاک_شود
+                    {i.personeli}} {i.melli}} {i.etebar}}
 {% elif var1 == 7 %}
 {% csrf_token %}
 آپلود فایل نمونه کارت: [File]
 آپلود فایل نمونه لیست کاربران: [File]
 آپلود
 {% endif %} {% else %}
 ****** خوش آمدید ******
```

### Comparing `erscipcard-1.18/erscipcard/urls.py` & `erscipcard-1.18.1/erscipcard/urls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard/views.py` & `erscipcard-1.18.1/erscipcard/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,30 +128,30 @@
 		response = HttpResponse(pdf_contents, content_type='application/pdf')
 		return response
 	except:
 		pass
 	return redirect("/erscipcard")
 ####################################################################
 def printcard2(request):
-	if not request.user.is_authenticated:
-		return render (request,'erscipcard/login.html' )
-	try:
+	#if not request.user.is_authenticated:
+	#	return render (request,'erscipcard/login.html' )
+	#try:
 		doc=DocxTemplate("1.docx") if os.path.isfile("1.docx") else DocxTemplate(finders.find("1.docx"))
 		picwidth = "30"
 		if os.path.isfile("picwidth"):
 			f = open("picwidth", "r")
 			picwidth = f.read()
 			f.close()
 		user = User1.objects.all()
 		if request.GET['fromprn'] == '' and request.GET['toprn'] == '' :
 			user = User1.objects.all()
 		if request.GET['fromprn'] != '' or request.GET['toprn'] != '' :
-			user = User1.objects.filter(number=request.GET['fromprn'])
+			user = User1.objects.filter(id=request.GET['fromprn'])
 		if request.GET['fromprn'] != '' and request.GET['toprn'] != '' :
-			user = User1.objects.filter(number__gte=request.GET['fromprn'],number__lte=request.GET['toprn'])
+			user = User1.objects.filter(id__gte=request.GET['fromprn'],id__lte=request.GET['toprn'])
 		pic = {}
 		for u in user:
 			if u.pic.name != '' :
 				pic[u.id] = InlineImage(doc, image_descriptor = u.pic.path , width=Mm(int(picwidth)))
 		context = {"user" : user  , "pic" : pic }
 		doc.render(context)
 		doc.save("aa.docx")
@@ -171,29 +171,29 @@
 			response = HttpResponse(pdf_contents, content_type='application/pdf')
 			return response
 		if chk == "2" :
 			response = HttpResponse(pdf_contents, content_type='application/docx')
 			response['Content-Disposition'] = 'inline;filename=erscipcard.docx'
 			return response
 		return redirect("/erscipcard")
-	except:
-		pass
-	return redirect("/erscipcard")
+	#except:
+	#	pass
+	#return redirect("/erscipcard")
 ####################################################################
 def userlist(request):
 	if not request.user.is_authenticated:
 		return render (request,'erscipcard/login.html' )
 	try:
 	    if request.method == 'POST':
 	        data = request.POST['idnum']
-	        userlist=User1.objects.filter(name__contains = data ).order_by('number')
+	        userlist=User1.objects.filter(name__contains = data ).order_by('id')
 	        return render(request, 'erscipcard/ou.html', {'data': data , 'userlist' : userlist , 'var1' : 3 })
 	    else:
 	        data = ""
-	        userlist=User1.objects.all().order_by('number')
+	        userlist=User1.objects.all().order_by('id')
 	        return render(request, 'erscipcard/ou.html', {'data': data , 'userlist' : userlist , 'var1' : 3 })
 	except:
 		pass
 	return redirect("/erscipcard")
 ####################################################################
 def edituser(request):
 	if not request.user.is_authenticated:
@@ -263,15 +263,15 @@
 	return render(request, 'erscipcard/ou.html', {'memo': 'خطا در سرور' , 'var1' : 1 })
 ###################################################################
 def printalluser(request):
 	if not request.user.is_authenticated:
 		return render (request,'erscipcard/login.html' )
 	try:
 		doc=DocxTemplate("2.docx") if os.path.isfile("2.docx") else DocxTemplate(finders.find("2.docx"))
-		user = User1.objects.all().order_by('number')
+		user = User1.objects.all().order_by('id')
 		context = {"user" : user }
 		doc.render(context)
 		doc.save("aa.docx")
 		del doc
 		if platform.system() == "Windows":
 			os.system("docx2pdf {}".format('aa.docx'))
 		if platform.system() == "Linux":
```

### Comparing `erscipcard-1.18/erscipcard/widget.py` & `erscipcard-1.18.1/erscipcard/widget.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/erscipcard.egg-info/PKG-INFO` & `erscipcard-1.18.1/erscipcard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18
+Version: 1.18.1
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `erscipcard-1.18/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.18.1/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18/setup.cfg` & `erscipcard-1.18.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.18
+version = 1.18.1
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

