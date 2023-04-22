# Comparing `tmp/erscipcard-1.18.1.tar.gz` & `tmp/erscipcard-1.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.18.1.tar", last modified: Sat Apr 22 19:56:30 2023, max compression
+gzip compressed data, was "erscipcard-1.18.2.tar", last modified: Sat Apr 22 20:08:38 2023, max compression
```

## Comparing `erscipcard-1.18.1.tar` & `erscipcard-1.18.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.662840 erscipcard-1.18.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-22 19:56:21.000000 erscipcard-1.18.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-22 19:56:21.000000 erscipcard-1.18.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1371 2023-04-22 19:56:30.662840 erscipcard-1.18.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1053 2023-04-22 19:56:21.000000 erscipcard-1.18.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.645840 erscipcard-1.18.1/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.647840 erscipcard-1.18.1/erscipcard/migrations/
--rw-r--r--   0 root         (0) root         (0)     2100 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.649840 erscipcard-1.18.1/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    11041 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    11792 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/BTITR.TTF
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.642840 erscipcard-1.18.1/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.651840 erscipcard-1.18.1/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.653840 erscipcard-1.18.1/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.654840 erscipcard-1.18.1/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.655840 erscipcard-1.18.1/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.660840 erscipcard-1.18.1/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/static/spinners.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.661840 erscipcard-1.18.1/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      241 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.661840 erscipcard-1.18.1/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    12711 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/erscipcard/ou.html
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templates/replace_re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.661840 erscipcard-1.18.1/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    11853 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-04-22 19:56:21.000000 erscipcard-1.18.1/erscipcard/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 19:56:30.646840 erscipcard-1.18.1/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1371 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 19:56:30.000000 erscipcard-1.18.1/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      769 2023-04-22 19:56:30.663840 erscipcard-1.18.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-22 19:56:21.000000 erscipcard-1.18.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.527780 erscipcard-1.18.2/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-22 20:08:30.000000 erscipcard-1.18.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-22 20:08:30.000000 erscipcard-1.18.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-04-22 20:08:38.528780 erscipcard-1.18.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-22 20:08:30.000000 erscipcard-1.18.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.507780 erscipcard-1.18.2/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.509780 erscipcard-1.18.2/erscipcard/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.511780 erscipcard-1.18.2/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/BTITR.TTF
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.504780 erscipcard-1.18.2/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.514780 erscipcard-1.18.2/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.515780 erscipcard-1.18.2/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.518780 erscipcard-1.18.2/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.519780 erscipcard-1.18.2/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.525780 erscipcard-1.18.2/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/static/spinners.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.526780 erscipcard-1.18.2/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.527780 erscipcard-1.18.2/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12711 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/templates/erscipcard/ou.html
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/templates/replace_re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.527780 erscipcard-1.18.2/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    11847 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-04-22 20:08:30.000000 erscipcard-1.18.2/erscipcard/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 20:08:38.508780 erscipcard-1.18.2/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-04-22 20:08:38.000000 erscipcard-1.18.2/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-04-22 20:08:38.000000 erscipcard-1.18.2/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 20:08:38.000000 erscipcard-1.18.2/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-22 20:08:38.000000 erscipcard-1.18.2/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 20:08:38.000000 erscipcard-1.18.2/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      769 2023-04-22 20:08:38.529780 erscipcard-1.18.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-22 20:08:30.000000 erscipcard-1.18.2/setup.py
```

### Comparing `erscipcard-1.18.1/LICENSE` & `erscipcard-1.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/PKG-INFO` & `erscipcard-1.18.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18.1
+Version: 1.18.2
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `erscipcard-1.18.1/README.md` & `erscipcard-1.18.2/README.md`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/migrations/0001_initial.py` & `erscipcard-1.18.2/erscipcard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/models.py` & `erscipcard-1.18.2/erscipcard/models.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/1.docx` & `erscipcard-1.18.2/erscipcard/static/1.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/2.docx` & `erscipcard-1.18.2/erscipcard/static/2.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.18.2/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/BTITR.TTF` & `erscipcard-1.18.2/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.18.2/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.18.2/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.18.2/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.18.2/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/css/style.css` & `erscipcard-1.18.2/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/css/util.css` & `erscipcard-1.18.2/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.18.2/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.18.2/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.18.2/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.18.2/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.18.2/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.18.2/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.18.2/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.18.2/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.18.2/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.18.2/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.18.2/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/favicon.ico` & `erscipcard-1.18.2/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/logo.png` & `erscipcard-1.18.2/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/main.css` & `erscipcard-1.18.2/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/atebits.css` & `erscipcard-1.18.2/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/ball.css` & `erscipcard-1.18.2/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/circles.css` & `erscipcard-1.18.2/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/dots.css` & `erscipcard-1.18.2/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/echo.css` & `erscipcard-1.18.2/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/flower.css` & `erscipcard-1.18.2/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/gauge.css` & `erscipcard-1.18.2/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.18.2/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.18.2/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.18.2/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.18.2/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.18.2/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/plus.css` & `erscipcard-1.18.2/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/pong.css` & `erscipcard-1.18.2/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/pulse.css` & `erscipcard-1.18.2/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.18.2/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/spinner.css` & `erscipcard-1.18.2/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.18.2/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.18.2/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/throbber.css` & `erscipcard-1.18.2/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/timer.css` & `erscipcard-1.18.2/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/whirly.css` & `erscipcard-1.18.2/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.18.2/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/static/spinners.css` & `erscipcard-1.18.2/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.18.2/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.18.2/erscipcard/templates/erscipcard/ou.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/urls.py` & `erscipcard-1.18.2/erscipcard/urls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard/views.py` & `erscipcard-1.18.2/erscipcard/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,17 @@
 		response = HttpResponse(pdf_contents, content_type='application/pdf')
 		return response
 	except:
 		pass
 	return redirect("/erscipcard")
 ####################################################################
 def printcard2(request):
-	#if not request.user.is_authenticated:
-	#	return render (request,'erscipcard/login.html' )
-	#try:
+	if not request.user.is_authenticated:
+		return render (request,'erscipcard/login.html' )
+	try:
 		doc=DocxTemplate("1.docx") if os.path.isfile("1.docx") else DocxTemplate(finders.find("1.docx"))
 		picwidth = "30"
 		if os.path.isfile("picwidth"):
 			f = open("picwidth", "r")
 			picwidth = f.read()
 			f.close()
 		user = User1.objects.all()
@@ -171,17 +171,17 @@
 			response = HttpResponse(pdf_contents, content_type='application/pdf')
 			return response
 		if chk == "2" :
 			response = HttpResponse(pdf_contents, content_type='application/docx')
 			response['Content-Disposition'] = 'inline;filename=erscipcard.docx'
 			return response
 		return redirect("/erscipcard")
-	#except:
-	#	pass
-	#return redirect("/erscipcard")
+	except:
+		pass
+	return redirect("/erscipcard")
 ####################################################################
 def userlist(request):
 	if not request.user.is_authenticated:
 		return render (request,'erscipcard/login.html' )
 	try:
 	    if request.method == 'POST':
 	        data = request.POST['idnum']
```

### Comparing `erscipcard-1.18.1/erscipcard/widget.py` & `erscipcard-1.18.2/erscipcard/widget.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/erscipcard.egg-info/PKG-INFO` & `erscipcard-1.18.2/erscipcard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18.1
+Version: 1.18.2
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `erscipcard-1.18.1/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.18.2/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.1/setup.cfg` & `erscipcard-1.18.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.18.1
+version = 1.18.2
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

