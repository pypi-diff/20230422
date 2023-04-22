# Comparing `tmp/ganga-8.6.4.tar.gz` & `tmp/ganga-8.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ganga-8.6.4.tar", last modified: Tue Mar 28 10:36:46 2023, max compression
+gzip compressed data, was "ganga-8.6.5.tar", last modified: Sat Apr 22 09:37:37 2023, max compression
```

## Comparing `ganga-8.6.4.tar` & `ganga-8.6.5.tar`

### file list

```diff
@@ -1,1052 +1,1052 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.366449 ganga-8.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-28 10:36:29.000000 ganga-8.6.4/LICENSE_GPL
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 10:36:29.000000 ganga-8.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-28 10:36:46.366449 ganga-8.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-28 10:36:29.000000 ganga-8.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.226445 ganga-8.6.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3687 2023-03-28 10:36:29.000000 ganga-8.6.4/bin/ganga
--rwxr-xr-x   0 runner    (1001) docker     (123)     2088 2023-03-28 10:36:29.000000 ganga-8.6.4/bin/ganga-gui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.226445 ganga-8.6.4/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.226445 ganga-8.6.4/doc/API/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/API/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.226445 ganga-8.6.4/doc/GPI/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/GPI/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.230445 ganga-8.6.4/doc/UserGuide/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/Configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/GoogleOauth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/InputAndOutputData.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/InstallAndBasicUsage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/JobManipulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/MiscellaneousFunctionality.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/PostProcessors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/Queues.rst
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/RunningExecutables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/Splitters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/Tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/TutorialPlugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/UsingDifferentApplications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/UsingDifferentBackends.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/Virtualization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/WhatIsGanga.rst
--rw-r--r--   0 runner    (1001) docker     (123)   587157 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/first_job.gif
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    65215 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/start_terminal.gif
--rw-r--r--   0 runner    (1001) docker     (123)   515269 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/UserGuide/virtualization.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.230445 ganga-8.6.4/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.230445 ganga-8.6.4/doc/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/dev/credentials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/dev/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     7656 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/fill_gpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.214445 ganga-8.6.4/doc/journal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.250446 ganga-8.6.4/doc/journal/CPC2007/
--rwxr-xr-x   0 runner    (1001) docker     (123)    55839 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/GangaJob.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   310914 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/GangaOverview.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   121579 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/GangaPlugin.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/README
--rwxr-xr-x   0 runner    (1001) docker     (123)   189776 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/avianflu.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   255272 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/avianflu.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     7896 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/camtology.tex
--rw-r--r--   0 runner    (1001) docker     (123)  5151013 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/camtologyfigure.eps
--rwxr-xr-x   0 runner    (1001) docker     (123)   588084 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/camtologyfigure.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   106103 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/camtologytech.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)    54997 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/elsart.cls
--rwxr-xr-x   0 runner    (1001) docker     (123)    13301 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/elsart1p.cls
--rwxr-xr-x   0 runner    (1001) docker     (123)    13505 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/elsart3p.cls
--rwxr-xr-x   0 runner    (1001) docker     (123)    13426 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/elsart5p.cls
--rw-r--r--   0 runner    (1001) docker     (123)  7395300 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-GUI.eps
--rw-r--r--   0 runner    (1001) docker     (123)   127751 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-GUI.png
--rw-r--r--   0 runner    (1001) docker     (123)   102543 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-architecture.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    98876 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-diane-portal.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    87966 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-diane-portal.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    31356 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-diane-portal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-objects.dia
--rw-r--r--   0 runner    (1001) docker     (123)    66244 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-objects.eps
--rw-r--r--   0 runner    (1001) docker     (123)    31406 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga-objects.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    75987 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/ganga.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)    26228 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/instructions-num.tex
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/job-uml.dia
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/job-uml.eps
--rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/job-uml.png
--rw-r--r--   0 runner    (1001) docker     (123)   372567 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/monitoring.eps
--rw-r--r--   0 runner    (1001) docker     (123)   116572 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/monitoring.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   136823 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/journal/CPC2007/monitoring.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.250446 ganga-8.6.4/doc/manuals/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.250446 ganga-8.6.4/doc/manuals/html/
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/about.dat
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.254446 ganga-8.6.4/doc/manuals/html/icons/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/blank.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/blank.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/contents.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/contents.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/index.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      529 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/index.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/modules.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/modules.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/next.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/next.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/previous.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/previous.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/pyfav.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/up.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/icons/up.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4443 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/index.html.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/stdabout.dat
--rwxr-xr-x   0 runner    (1001) docker     (123)     6041 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/html/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.254446 ganga-8.6.4/doc/manuals/perl/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2513 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/SynopsisTable.pm
--rwxr-xr-x   0 runner    (1001) docker     (123)      405 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/distutils.perl
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/howto.perl
--rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/isilo.perl
--rwxr-xr-x   0 runner    (1001) docker     (123)    24053 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/l2hinit.perl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1921 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/ltxmarkup.perl
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/manual.perl
--rwxr-xr-x   0 runner    (1001) docker     (123)    62754 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/perl/python.perl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.254446 ganga-8.6.4/doc/manuals/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)      279 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/script/fiximgpath.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/script/make-doc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/script/makeincl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.214445 ganga-8.6.4/doc/manuals/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.254446 ganga-8.6.4/doc/manuals/src/DocMaker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/DocMaker/DocMaker.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.266446 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Back.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2410 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Copy.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2492 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Delete.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2147 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Download.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1710 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_Generic.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_New.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_Remove.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2297 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2037 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_Rename.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Forward.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    23577 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2490 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/General_Options.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2509 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Go.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Properties.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2433 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Refresh.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Save.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4504 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Search.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Stop.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2452 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/View_Doc.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Write.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1007 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/browse.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1479 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      987 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_text_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_text_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1891 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1563 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2322 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3183 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    10990 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3964 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_6.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2656 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)   120641 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7028 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    10096 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    22429 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    31848 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    37895 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    10919 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4417 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    25440 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2776 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/help.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    23577 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    41244 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5020 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    11470 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    11606 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9174 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    24152 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7218 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9076 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    48083 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    26786 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    13686 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2140 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/open.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/preview.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    62349 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    33800 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    17676 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    29133 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    26485 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/retrieve.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    54473 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    46152 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    70724 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    27847 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GUI_User_Manual/toolbar.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.266446 ganga-8.6.4/doc/manuals/src/GangaIntroduction/
--rwxr-xr-x   0 runner    (1001) docker     (123)    87638 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.266446 ganga-8.6.4/doc/manuals/src/LHCb/
--rwxr-xr-x   0 runner    (1001) docker     (123)    31025 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/LHCb/LHCb.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.266446 ganga-8.6.4/doc/manuals/src/dev_survival/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11822 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/dev_survival/dev_survival.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/dev_survival/makegraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10107 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/dev_survival/transient-states.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)    11362 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/dev_survival/user-states.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.266446 ganga-8.6.4/doc/manuals/src/workbook/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.270446 ganga-8.6.4/doc/manuals/src/workbook/development/
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/architecture.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/cvs.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/dashboard.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/developer.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/development.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/documentation.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/panels.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/release.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/submission.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/test.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/twiki.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/development/webpages.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.270446 ganga-8.6.4/doc/manuals/src/workbook/extension/
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/application.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/backend.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/connector.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/dataset.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/extension.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/logging.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/merger.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/parameters.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/plugins.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/extension/splitter.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.270446 ganga-8.6.4/doc/manuals/src/workbook/installation/
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/installation/afs.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)      185 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/installation/installation.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/installation/local.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/installation/site.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.270446 ganga-8.6.4/doc/manuals/src/workbook/introduction/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/introduction/functionality.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/introduction/introduction.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/introduction/license.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/introduction/mail.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/introduction/website.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.274446 ganga-8.6.4/doc/manuals/src/workbook/usage/
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/bugs.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/configuration.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/credentials.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/gpi.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/gui.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/help.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/jobs.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/model.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/monitoring.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/operations.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/repository.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/scripts.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/startup.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/statistics.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/usage.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/usage/workspace.tex
--rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/src/workbook/workbook.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.274446 ganga-8.6.4/doc/manuals/texinputs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/distutils.sty
--rwxr-xr-x   0 runner    (1001) docker     (123)    14699 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/fancyhdr.sty
--rwxr-xr-x   0 runner    (1001) docker     (123)    10359 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/fncychap.sty
--rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/howto.cls
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/ltxmarkup.sty
--rwxr-xr-x   0 runner    (1001) docker     (123)     4440 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/manual.cls
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/pypaper.sty
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/python.ist
--rwxr-xr-x   0 runner    (1001) docker     (123)    40097 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/texinputs/python.sty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/doc/manuals/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2182 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/anno-api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10526 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/buildindex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/checkargs.pm
--rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/cklatex
--rwxr-xr-x   0 runner    (1001) docker     (123)     2154 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/custlib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2434 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/cvsinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/findacks
--rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/findcsyms
--rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/findmodrefs
--rwxr-xr-x   0 runner    (1001) docker     (123)     3937 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/findsyms
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/fix_hack
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/fix_libaux.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)      441 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/fixinfo.el
--rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/getpagecounts
--rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/getversioninfo
--rwxr-xr-x   0 runner    (1001) docker     (123)    58169 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/html2texi.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2301 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/indfix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/keywords.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5283 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/listmodules
--rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/makesec.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/mkackshtml
--rwxr-xr-x   0 runner    (1001) docker     (123)    24033 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/mkhowto
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/mkinfo
--rwxr-xr-x   0 runner    (1001) docker     (123)     4819 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/mkmodindex
--rwxr-xr-x   0 runner    (1001) docker     (123)     2338 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/mkpkglist
--rwxr-xr-x   0 runner    (1001) docker     (123)     5884 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/mksourcepkg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1944 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/node2label.pl
--rwxr-xr-x   0 runner    (1001) docker     (123)    15832 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/prechm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/push-docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)    31256 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/py2texi.el
--rwxr-xr-x   0 runner    (1001) docker     (123)   786944 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/python
--rwxr-xr-x   0 runner    (1001) docker     (123)     2316 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/refcounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/rewrite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/doc/manuals/tools/sgmlconv/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/README
--rwxr-xr-x   0 runner    (1001) docker     (123)    23495 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/conversion.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)    37241 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/docfixer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7269 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/esis2sgml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9228 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/esistools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19936 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/latex2esis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/sgmlconv/make.rules
--rwxr-xr-x   0 runner    (1001) docker     (123)     6704 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/support.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3949 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/toc2bkm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/undoc_symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/update-docs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/manuals/tools/whichlibs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/doc/sysadmin/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/sysadmin/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/doc/work/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5697 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/work/lifetime.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     6857 2023-03-28 10:36:29.000000 ganga-8.6.4/doc/work/splitting.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/ganga/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/ganga/GangaCore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/ganga/GangaCore/Core/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10903 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/FileWorkspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.286447 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/DStreamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25943 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/FixedLock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11096 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py
--rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54032 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/PickleStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27239 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/Registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    35399 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/SessionLock.py
--rw-r--r--   0 runner    (1001) docker     (123)    19363 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py
--rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17812 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/VStreamer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/container_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.286447 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/GangaThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.286447 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.286447 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/GangaThread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.290447 ganga-8.6.4/ganga/GangaCore/Core/InternalServices/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9702 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/InternalServices/Coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/InternalServices/ShutdownManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/InternalServices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.290447 ganga-8.6.4/ganga/GangaCore/Core/MonitoringComponent/
--rwxr-xr-x   0 runner    (1001) docker     (123)    54936 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4521 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/MonitoringComponent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.290447 ganga-8.6.4/ganga/GangaCore/Core/Sandbox/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5281 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/Sandbox/Sandbox.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4265 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/Sandbox/WNSandbox.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/Sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6128 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.290447 ganga-8.6.4/ganga/GangaCore/GPI/
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.290447 ganga-8.6.4/ganga/GangaCore/GPIDev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.290447 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5528 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IApplication.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23490 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IBackend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3412 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9100 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IMerger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10624 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ISplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7566 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4315 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/Filters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59985 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/Objects.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    53774 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/Proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12619 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/VPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5177 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/VPrinterOld.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/AfsToken.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/
--rwxr-xr-x   0 runner    (1001) docker     (123)    19393 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/GridProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20594 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3369 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Config/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Config/Config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Dataset/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5984 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/Configure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17376 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/File.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24411 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14622 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/LCGSEFile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11200 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3368 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.294447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/GangaList/
--rwxr-xr-x   0 runner    (1001) docker     (123)    26733 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/GangaList/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/
--rwxr-xr-x   0 runner    (1001) docker     (123)   120918 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/Job.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/JobTree/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15970 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/JobTree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8979 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14541 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py
--rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21459 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistryUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12904 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/MonitoringServices/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10221 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Persistency/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7887 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Persistency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/GPIDev/Schema/
--rwxr-xr-x   0 runner    (1001) docker     (123)    32271 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Schema/Schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/TypeCheck.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/GPIDev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.298447 ganga-8.6.4/ganga/GangaCore/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.302447 ganga-8.6.4/ganga/GangaCore/Lib/Batch/
--rwxr-xr-x   0 runner    (1001) docker     (123)    25180 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Batch/Batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.302447 ganga-8.6.4/ganga/GangaCore/Lib/Checkers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Checkers/CustomChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2822 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Checkers/FileChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6964 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Checkers/RootFileChecker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.302447 ganga-8.6.4/ganga/GangaCore/Lib/Condor/
--rwxr-xr-x   0 runner    (1001) docker     (123)    29587 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Condor/Condor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4609 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Condor/CondorRequirements.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Condor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.302447 ganga-8.6.4/ganga/GangaCore/Lib/Executable/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13879 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Executable/Executable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.302447 ganga-8.6.4/ganga/GangaCore/Lib/Interactive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11328 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Interactive/Interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Interactive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/LCG/
--rw-r--r--   0 runner    (1001) docker     (123)    45978 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/ARC.py
--rw-r--r--   0 runner    (1001) docker     (123)    46736 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/CREAM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      908 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/ElapsedTimeProfiler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34355 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/Grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11624 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSandboxCache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8964 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/GridSimulator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/simulator-analyze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2173 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridftpSandboxCache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   101802 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCG.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCGOutputDownloader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5116 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCGRequirements.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10211 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCGSandboxCache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/Utility.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/LCG/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Localhost/
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    17182 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Localhost/Localhost.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Localhost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Mergers/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15780 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Mergers/Merger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Mergers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Notebook/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6557 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Notebook/Notebook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Notifier/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2823 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Notifier/Notifier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Notifier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Remote/
--rw-r--r--   0 runner    (1001) docker     (123)    32668 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Remote/Remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4294 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/ArgSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/ExeSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2450 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5491 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/GenericSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      223 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.306447 ganga-8.6.4/ganga/GangaCore/Lib/Virtualization/
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Virtualization/Docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Virtualization/Singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/Virtualization/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6001 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.310447 ganga-8.6.4/ganga/GangaCore/Runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/GPIFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/GPIexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/GangaCompleter.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/HEAD_CONFIG.INI
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/IPythonMagic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/Repository_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/Workspace_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65291 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/bootstrap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12710 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/eliza.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/ganga_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/gangadoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/gangadoceval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Runtime/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.310447 ganga-8.6.4/ganga/GangaCore/Utility/
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/ColourText.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.314447 ganga-8.6.4/ganga/GangaCore/Utility/Config/
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Config/A.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Config/B.ini
--rw-r--r--   0 runner    (1001) docker     (123)    43719 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Config/Config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Config/ConfigTest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Config/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/GridShell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.314447 ganga-8.6.4/ganga/GangaCore/Utility/Plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Plugin/GangaPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/Virtualization.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.314447 ganga-8.6.4/ganga/GangaCore/Utility/external/
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/external/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26942 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/feedback_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.314447 ganga-8.6.4/ganga/GangaCore/Utility/logging/
--rw-r--r--   0 runner    (1001) docker     (123)    21803 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/logging/message_caching_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/logging/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/stacktracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9868 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/Utility/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    60294 2023-03-28 10:36:44.000000 ganga-8.6.4/ganga/GangaCore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.314447 ganga-8.6.4/ganga/GangaCore/old_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.314447 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.318448 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah10013/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah10013/Savannah10013.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah17638.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.318448 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah23737/
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah23737/Savannah23737.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah32201.ini
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Bugs/Savannah36651.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.318448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/BackendApplicationMatrix.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/CompressOutput.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/ConfigFile.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/ConfigObject.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/ConfigUser.ini
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/LCG.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.318448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/Mergers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/Mergers/TestRootMerger.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/Mergers/TestTextMerger.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/Mergers/TestTextMergerGzip.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.318448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/MigrationFramework/
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass1.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass2.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/MonTest.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/MonitoringServices.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatch.ini
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageAndLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageUpload.ini
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedBatch.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedLocal.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractive.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCGMultipleCompressedFilesForMassStorageAndLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/RegistrySorting.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/ResubmitSubjobs.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/Root/
--rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/Root/TestRoot.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/WorkspaceRemoval.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/GPI/auto_resubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/GPI/auto_resubmit/auto_resubmit.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/Internals/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Internals/TestGridProxyExpandSystemVars.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/Performance/
--rwxr-xr-x   0 runner    (1001) docker     (123)      184 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Performance/PerfStats.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/Performance/TimeJobs.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/XMLRepository/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/XMLRepository/SpecialName.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/old_test/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/config/Schema.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/config/default.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/old_test/config/localxml.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.218445 ganga-8.6.4/ganga/GangaCore/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.218445 ganga-8.6.4/ganga/GangaCore/test/GPI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/test/GPI/Config/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/test/GPI/Config/A.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/test/GPI/Config/B.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/test/GPI/Config/ConfigTest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/test/GPI/Notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/test/GPI/Notebook/Test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaCore/testlib/
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/GangaUnitTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/mark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaCore/testlib/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaDirac/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7272 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/BOOT.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Dirac.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.322448 ganga-8.6.4/ganga/GangaDirac/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/Backends/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Backends/Dirac.py
--rw-r--r--   0 runner    (1001) docker     (123)    77133 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Backends/DiracBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Backends/DiracUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/Credentials/
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Credentials/DiracProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Credentials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/Files/
--rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Files/DiracFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Files/downloadScript.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Files/uploadScript.py.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/Server/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/BlankCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/DiracCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/DiracDefinition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2364 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/DiracProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/InspectionClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/InspectionServer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3253 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24622 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/Lib/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9265 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.218445 ganga-8.6.4/ganga/GangaDirac/old_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.218445 ganga-8.6.4/ganga/GangaDirac/old_test/GPI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/old_test/GPI/Files/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/old_test/GPI/Files/TestDiracFile.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.218445 ganga-8.6.4/ganga/GangaDirac/old_test/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.326448 ganga-8.6.4/ganga/GangaDirac/old_test/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaDirac/old_test/Lib/RTHandlers/TestExeDiracRTHandler.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.330448 ganga-8.6.4/ganga/GangaGUI/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/BOOT.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.330448 ganga-8.6.4/ganga/GangaGUI/api/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33429 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/api/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.330448 ganga-8.6.4/ganga/GangaGUI/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    65122 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.222445 ganga-8.6.4/ganga/GangaGUI/gui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.330448 ganga-8.6.4/ganga/GangaGUI/gui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   164410 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.330448 ganga-8.6.4/ganga/GangaGUI/gui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/cli.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/create.js
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/credentials.js
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/job.js
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/jobs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/login.js
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/queue.js
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/slidecli.js
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/subjob.js
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/subjobs.js
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/static/js/templates.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.334448 ganga-8.6.4/ganga/GangaGUI/gui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/cli.html
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/config_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/credentials.html
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/edit_job.html
--rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/job.html
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/job_dir.html
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/jobs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/plugin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/plugins.html
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/queue.html
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/runfile.html
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/storage.html
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/subjob.html
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/subjob_dir.html
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/subjobs.html
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/gui/templates/templates.html
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/guistate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/start.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGUI/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.334448 ganga-8.6.4/ganga/GangaGaudi/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Gaudi.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.334448 ganga-8.6.4/ganga/GangaGaudi/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/CMTUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/Gaudi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/GaudiBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaGaudi/Lib/Checkers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2848 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaGaudi/Lib/Datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/RunTimeHandlerUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaGaudi/Lib/Splitters/
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Splitters/SplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaGaudi/Lib/XMLSummary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/XMLSummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63863 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/XMLSummary/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24704 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/XMLSummary/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/PACKAGE.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaGaudi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaLHCb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/BOOT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2352 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/LHCb.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.338448 ganga-8.6.4/ganga/GangaLHCb/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.342448 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/AppsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/Bender.py
--rw-r--r--   0 runner    (1001) docker     (123)    24468 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/BenderBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/BenderScript.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/CMTscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/FileFunctions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30814 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/GaudiExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/GaudiPython.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/Ostap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.342448 ganga-8.6.4/ganga/GangaLHCb/Lib/Backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Backends/Dirac.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.342448 ganga-8.6.4/ganga/GangaLHCb/Lib/Checkers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Checkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.342448 ganga-8.6.4/ganga/GangaLHCb/Lib/Files/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Files/LogicalFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Files/PhysicalFile.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.342448 ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19914 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23063 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.342448 ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34906 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/Lib/Server/
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/Lib/XMLSummary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/XMLSummary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64899 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/XMLSummary/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25050 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/XMLSummary/summary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/Utility/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Utility/LHCbDIRACenv.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/Utility/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8967 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.346448 ganga-8.6.4/ganga/GangaLHCb/testlib/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaLHCb/testlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/BOOT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/Highland/
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Highland/Highland.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Highland/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280Checkers/
--rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Checkers/ND280Checker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Checkers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9075 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Checkers/post_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280Control/
--rwxr-xr-x   0 runner    (1001) docker     (123)    26102 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/ND280Configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/runND280.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/runND280CosMC.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/runND280Kin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/runND280RDP.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Control/runND280SandMC.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280Dataset/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8427 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Dataset/ND280Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280Executable/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Executable/ND280Executable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Executable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280Skimmer/
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Skimmer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.350448 ganga-8.6.4/ganga/GangaND280/ND280Splitter/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8589 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Splitter/ND280Splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280Splitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.354449 ganga-8.6.4/ganga/GangaND280/ND280TPCGasInteractions/
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/ND280TPCGasInteractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.354449 ganga-8.6.4/ganga/GangaND280/Tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Tasks/ND280Task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Tasks/ND280Transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Tasks/ND280Unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/Tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaND280/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.358449 ganga-8.6.4/ganga/GangaRelease/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.0
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.1
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.2
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.3
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.4
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.0
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.1
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.10
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.11
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.12
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.13
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.14
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.15
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.2
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.3
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.4
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.5
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.6
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.7
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.8
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.9
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.0
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.1
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.2
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.3
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.1.0
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.0
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.1
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.2
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.3
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.4
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.0
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.1
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.2
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.3
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-28 10:36:44.000000 ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.6.4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.358449 ganga-8.6.4/ganga/GangaRelease/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/tools/check-new-ganga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaRelease/tools/ganga-cvmfs-install.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.358449 ganga-8.6.4/ganga/GangaTest/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/BOOT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Framework/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18555 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/driver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31840 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/htmlizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47550 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11385 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Framework/xmldifferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4013 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/CrashTest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Lib/GListApp/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2803 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/GListApp/GListApp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/GListApp/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/GListApp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3277 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/StoreTestFramework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Lib/TFile/
--rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TFile/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1485 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TFile/TFile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TFile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Lib/TestApplication/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5553 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestApplication/TestApplication.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestApplication/TestDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestApplication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Lib/TestMonitoringService/
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestMonitoringService/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestObjects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3498 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      293 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/Lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/PACKAGE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTest/TestGPIP/
--rwxr-xr-x   0 runner    (1001) docker     (123)      153 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/TestGPIP/TestGPIP.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      405 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.362449 ganga-8.6.4/ganga/GangaTutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/BOOT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.366449 ganga-8.6.4/ganga/GangaTutorial/Lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6800 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/PrimeFactorizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2287 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/PrimeTableDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.366449 ganga-8.6.4/ganga/GangaTutorial/Lib/primes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/primes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/primes/prime_factor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Lib/primes/primes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/PACKAGE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/Tutorial.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/GangaTutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.366449 ganga-8.6.4/ganga/ganga/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/ganga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-28 10:36:29.000000 ganga-8.6.4/ganga/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:36:46.282447 ganga-8.6.4/ganga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-28 10:36:46.000000 ganga-8.6.4/ganga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37743 2023-03-28 10:36:46.000000 ganga-8.6.4/ganga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:36:46.000000 ganga-8.6.4/ganga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-28 10:36:46.000000 ganga-8.6.4/ganga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-28 10:36:46.000000 ganga-8.6.4/ganga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-28 10:36:46.366449 ganga-8.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-28 10:36:44.000000 ganga-8.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.340427 ganga-8.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 09:37:22.000000 ganga-8.6.5/LICENSE_GPL
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-22 09:37:22.000000 ganga-8.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-22 09:37:37.340427 ganga-8.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-22 09:37:22.000000 ganga-8.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.212426 ganga-8.6.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3687 2023-04-22 09:37:22.000000 ganga-8.6.5/bin/ganga
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2088 2023-04-22 09:37:22.000000 ganga-8.6.5/bin/ganga-gui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.212426 ganga-8.6.5/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.212426 ganga-8.6.5/doc/API/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/API/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.212426 ganga-8.6.5/doc/GPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/GPI/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.216426 ganga-8.6.5/doc/UserGuide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/Configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/GoogleOauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/InputAndOutputData.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/InstallAndBasicUsage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/JobManipulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/MiscellaneousFunctionality.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/PostProcessors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/Queues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/RunningExecutables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/Splitters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/Tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/TutorialPlugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/UsingDifferentApplications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/UsingDifferentBackends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/Virtualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/WhatIsGanga.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   587157 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/first_job.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    65215 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/start_terminal.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   515269 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/UserGuide/virtualization.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.216426 ganga-8.6.5/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.216426 ganga-8.6.5/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/dev/credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/dev/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7656 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/fill_gpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.196426 ganga-8.6.5/doc/journal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.236426 ganga-8.6.5/doc/journal/CPC2007/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55839 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/GangaJob.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   310914 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/GangaOverview.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   121579 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/GangaPlugin.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)   189776 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/avianflu.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   255272 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/avianflu.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7896 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/camtology.tex
+-rw-r--r--   0 runner    (1001) docker     (123)  5151013 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/camtologyfigure.eps
+-rwxr-xr-x   0 runner    (1001) docker     (123)   588084 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/camtologyfigure.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106103 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/camtologytech.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54997 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/elsart.cls
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13301 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/elsart1p.cls
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13505 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/elsart3p.cls
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13426 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/elsart5p.cls
+-rw-r--r--   0 runner    (1001) docker     (123)  7395300 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-GUI.eps
+-rw-r--r--   0 runner    (1001) docker     (123)   127751 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-GUI.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102543 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56388 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-architecture.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98876 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-diane-portal.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    87966 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-diane-portal.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31356 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-diane-portal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-objects.dia
+-rw-r--r--   0 runner    (1001) docker     (123)    66244 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-objects.eps
+-rw-r--r--   0 runner    (1001) docker     (123)    31406 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga-objects.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75987 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/ganga.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26228 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/instructions-num.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/job-uml.dia
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/job-uml.eps
+-rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/job-uml.png
+-rw-r--r--   0 runner    (1001) docker     (123)   372567 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/monitoring.eps
+-rw-r--r--   0 runner    (1001) docker     (123)   116572 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/monitoring.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   136823 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/journal/CPC2007/monitoring.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.236426 ganga-8.6.5/doc/manuals/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.236426 ganga-8.6.5/doc/manuals/html/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/about.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.240426 ganga-8.6.5/doc/manuals/html/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/blank.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/blank.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/contents.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/contents.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/index.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      529 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/index.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/modules.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/modules.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/next.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/next.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/previous.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/previous.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/pyfav.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/up.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/icons/up.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4443 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/index.html.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/stdabout.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6041 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/html/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.240426 ganga-8.6.5/doc/manuals/perl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2513 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/SynopsisTable.pm
+-rwxr-xr-x   0 runner    (1001) docker     (123)      405 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/distutils.perl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/howto.perl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/isilo.perl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24053 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/l2hinit.perl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1921 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/ltxmarkup.perl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/manual.perl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62754 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/perl/python.perl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.240426 ganga-8.6.5/doc/manuals/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      279 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/script/fiximgpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/script/make-doc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/script/makeincl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.200425 ganga-8.6.5/doc/manuals/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.240426 ganga-8.6.5/doc/manuals/src/DocMaker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/DocMaker/DocMaker.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.252426 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Back.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2410 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Copy.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2492 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Delete.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2147 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Download.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1710 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_Generic.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_New.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_Remove.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2297 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2037 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_Rename.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Forward.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23577 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2490 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/General_Options.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2509 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Go.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Properties.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2433 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Refresh.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Save.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4504 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Search.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Stop.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2452 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/View_Doc.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Write.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1007 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/browse.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1479 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      987 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_text_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_text_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1891 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1563 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2322 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3183 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10990 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3964 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_6.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2656 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)   120641 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7028 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10096 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22429 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31848 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37895 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10919 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4417 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25440 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2776 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/help.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23577 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41244 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5020 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11470 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11606 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9174 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24152 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7218 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9076 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48083 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26786 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13686 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2140 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/open.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/preview.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62349 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33800 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17676 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29133 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26485 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/retrieve.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54473 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46152 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70724 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27847 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GUI_User_Manual/toolbar.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.252426 ganga-8.6.5/doc/manuals/src/GangaIntroduction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87638 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.252426 ganga-8.6.5/doc/manuals/src/LHCb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31025 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/LHCb/LHCb.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.252426 ganga-8.6.5/doc/manuals/src/dev_survival/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11822 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/dev_survival/dev_survival.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/dev_survival/makegraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10107 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/dev_survival/transient-states.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11362 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/dev_survival/user-states.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.252426 ganga-8.6.5/doc/manuals/src/workbook/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.256426 ganga-8.6.5/doc/manuals/src/workbook/development/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/architecture.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/cvs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/dashboard.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/developer.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/development.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/documentation.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/panels.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/release.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/submission.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/test.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/twiki.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/development/webpages.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.256426 ganga-8.6.5/doc/manuals/src/workbook/extension/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/application.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/backend.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/connector.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/dataset.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/extension.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/logging.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/merger.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/parameters.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/plugins.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/extension/splitter.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.256426 ganga-8.6.5/doc/manuals/src/workbook/installation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/installation/afs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)      185 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/installation/installation.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/installation/local.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/installation/site.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.256426 ganga-8.6.5/doc/manuals/src/workbook/introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/introduction/functionality.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/introduction/introduction.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/introduction/license.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/introduction/mail.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/introduction/website.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.260426 ganga-8.6.5/doc/manuals/src/workbook/usage/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/bugs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/configuration.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/credentials.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/gpi.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/gui.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/help.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/jobs.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/model.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/monitoring.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/operations.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/repository.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/scripts.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/startup.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/statistics.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/usage.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/usage/workspace.tex
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1004 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/src/workbook/workbook.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.260426 ganga-8.6.5/doc/manuals/texinputs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/distutils.sty
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14699 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/fancyhdr.sty
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10359 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/fncychap.sty
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/howto.cls
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/ltxmarkup.sty
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4440 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/manual.cls
+-rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/pypaper.sty
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/python.ist
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40097 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/texinputs/python.sty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.264427 ganga-8.6.5/doc/manuals/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2182 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/anno-api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10526 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/buildindex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/checkargs.pm
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/cklatex
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2154 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/custlib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2434 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/cvsinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/findacks
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/findcsyms
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/findmodrefs
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3937 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/findsyms
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/fix_hack
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/fix_libaux.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)      441 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/fixinfo.el
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/getpagecounts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/getversioninfo
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58169 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/html2texi.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2301 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/indfix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      365 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/keywords.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5283 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/listmodules
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3438 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/makesec.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/mkackshtml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24033 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/mkhowto
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/mkinfo
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4819 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/mkmodindex
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2338 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/mkpkglist
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5884 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/mksourcepkg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1944 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/node2label.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15832 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/prechm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1987 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/push-docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31256 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/py2texi.el
+-rwxr-xr-x   0 runner    (1001) docker     (123)   786944 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/python
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2316 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/refcounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1366 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/rewrite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/doc/manuals/tools/sgmlconv/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23495 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/conversion.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37241 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/docfixer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7269 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/esis2sgml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9228 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/esistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19936 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/latex2esis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/sgmlconv/make.rules
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6704 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/support.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3949 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/toc2bkm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2528 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/undoc_symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/update-docs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/manuals/tools/whichlibs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/doc/sysadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/sysadmin/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/doc/work/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5697 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/work/lifetime.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6857 2023-04-22 09:37:22.000000 ganga-8.6.5/doc/work/splitting.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/ganga/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/ganga/GangaCore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/ganga/GangaCore/Core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10903 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/FileWorkspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/DStreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25943 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/FixedLock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11096 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36287 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54032 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/PickleStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27239 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/Registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35399 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/SessionLock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19363 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26908 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17812 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/VStreamer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1146 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/container_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/GangaThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/GangaThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/InternalServices/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9702 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/InternalServices/Coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/InternalServices/ShutdownManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/InternalServices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/MonitoringComponent/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54936 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4521 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/MonitoringComponent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/Core/Sandbox/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5281 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/Sandbox/Sandbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4265 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/Sandbox/WNSandbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/Sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6128 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/GPI/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.272426 ganga-8.6.5/ganga/GangaCore/GPIDev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1872 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5528 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IApplication.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23490 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IBackend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3412 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9100 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IMerger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10624 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ISplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7566 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4315 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/Filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59985 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/Objects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53774 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/Proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12619 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/VPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5177 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/VPrinterOld.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/AfsToken.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19393 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/GridProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20594 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3369 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11717 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Config/Config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.276427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5984 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.280427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/Configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17376 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/File.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24411 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14622 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/LCGSEFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11200 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12947 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3368 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.280427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.280427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/GangaList/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26733 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/GangaList/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.280427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   120918 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.280427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/JobTree/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15970 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/JobTree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.280427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8979 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14541 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21459 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistryUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12904 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19061 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/GPIDev/MonitoringServices/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10221 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/GPIDev/Persistency/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7887 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Persistency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/GPIDev/Schema/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32271 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Schema/Schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/TypeCheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/GPIDev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/Lib/Batch/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25180 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Batch/Batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Batch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/Lib/Checkers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2335 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Checkers/CustomChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2822 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Checkers/FileChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6964 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Checkers/RootFileChecker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/Lib/Condor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29587 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Condor/Condor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4609 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Condor/CondorRequirements.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Condor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/Lib/Executable/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13879 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Executable/Executable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.284427 ganga-8.6.5/ganga/GangaCore/Lib/Interactive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11328 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Interactive/Interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Interactive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/LCG/
+-rw-r--r--   0 runner    (1001) docker     (123)    45978 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/ARC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46736 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/CREAM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      908 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/ElapsedTimeProfiler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34355 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/Grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11624 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSandboxCache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8964 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/GridSimulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/simulator-analyze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2173 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridftpSandboxCache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   101802 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCG.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3188 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCGOutputDownloader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5116 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCGRequirements.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10211 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCGSandboxCache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/Utility.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/LCG/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Localhost/
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17182 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Localhost/Localhost.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Localhost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Mergers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15780 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Mergers/Merger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Mergers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Notebook/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6557 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Notebook/Notebook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Notifier/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2823 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Notifier/Notifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Notifier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Remote/
+-rw-r--r--   0 runner    (1001) docker     (123)    32668 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Remote/Remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4294 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/ArgSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/ExeSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2450 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5491 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/GenericSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      223 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.288427 ganga-8.6.5/ganga/GangaCore/Lib/Virtualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Virtualization/Docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Virtualization/Singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/Virtualization/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6001 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.292427 ganga-8.6.5/ganga/GangaCore/Runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/GPIFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/GPIexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/GangaCompleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/HEAD_CONFIG.INI
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/IPythonMagic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/Repository_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/Workspace_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65291 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/bootstrap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12710 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/eliza.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/ganga_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/gangadoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/gangadoceval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Runtime/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.292427 ganga-8.6.5/ganga/GangaCore/Utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/ColourText.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/Utility/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       51 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Config/A.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Config/B.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    43719 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Config/Config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Config/ConfigTest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Config/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/GridShell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/Utility/Plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Plugin/GangaPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/Virtualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/Utility/external/
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/external/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26942 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/feedback_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/Utility/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)    21803 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/logging/message_caching_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/logging/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/stacktracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9868 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/Utility/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60294 2023-04-22 09:37:36.000000 ganga-8.6.5/ganga/GangaCore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/old_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah10013/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah10013/Savannah10013.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah17638.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah23737/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah23737/Savannah23737.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah32201.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Bugs/Savannah36651.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/BackendApplicationMatrix.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/CompressOutput.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/ConfigFile.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/ConfigObject.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/ConfigUser.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/LCG.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.296427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/Mergers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/Mergers/TestRootMerger.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/Mergers/TestTextMerger.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/Mergers/TestTextMergerGzip.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/MigrationFramework/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass1.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/MigrationFramework/MigrationFramework.pass2.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/MonTest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/MonitoringServices.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatch.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageAndLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForMassStorageUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedBatch.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesCompressedLocal.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractive.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCGMultipleCompressedFilesForMassStorageAndLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/RegistrySorting.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/ResubmitSubjobs/ResubmitSubjobs.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/Root/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/Root/TestRoot.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/WorkspaceRemoval.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/GPI/auto_resubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/GPI/auto_resubmit/auto_resubmit.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/Internals/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Internals/TestGridProxyExpandSystemVars.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/Performance/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      184 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Performance/PerfStats.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/Performance/TimeJobs.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/XMLRepository/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/XMLRepository/SpecialName.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/old_test/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/config/Schema.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/config/default.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/old_test/config/localxml.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.204426 ganga-8.6.5/ganga/GangaCore/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.204426 ganga-8.6.5/ganga/GangaCore/test/GPI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/test/GPI/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/test/GPI/Config/A.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/test/GPI/Config/B.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/test/GPI/Config/ConfigTest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.300427 ganga-8.6.5/ganga/GangaCore/test/GPI/Notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/test/GPI/Notebook/Test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaCore/testlib/
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/GangaUnitTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/mark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaCore/testlib/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7272 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/BOOT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Dirac.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/Lib/Backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Backends/Dirac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77133 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Backends/DiracBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Backends/DiracUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/Lib/Credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Credentials/DiracProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Credentials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/Lib/Files/
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Files/DiracFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Files/downloadScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Files/uploadScript.py.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.304427 ganga-8.6.5/ganga/GangaDirac/Lib/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/BlankCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/DiracCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/DiracDefinition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2364 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/DiracProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/InspectionClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/InspectionServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3253 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24622 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaDirac/Lib/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9265 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.204426 ganga-8.6.5/ganga/GangaDirac/old_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.204426 ganga-8.6.5/ganga/GangaDirac/old_test/GPI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaDirac/old_test/GPI/Files/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/old_test/GPI/Files/TestDiracFile.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.204426 ganga-8.6.5/ganga/GangaDirac/old_test/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaDirac/old_test/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaDirac/old_test/Lib/RTHandlers/TestExeDiracRTHandler.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaGUI/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/BOOT.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaGUI/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33429 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/api/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaGUI/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65122 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.204426 ganga-8.6.5/ganga/GangaGUI/gui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.308427 ganga-8.6.5/ganga/GangaGUI/gui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   164410 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.312427 ganga-8.6.5/ganga/GangaGUI/gui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/cli.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/create.js
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/credentials.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/job.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/jobs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/login.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/queue.js
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/slidecli.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/subjob.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/subjobs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/static/js/templates.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.312427 ganga-8.6.5/ganga/GangaGUI/gui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/cli.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/config_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/credentials.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/edit_job.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/job.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/job_dir.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/jobs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/plugin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/plugins.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/queue.html
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/runfile.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/storage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/subjob.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/subjob_dir.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/subjobs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/gui/templates/templates.html
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/guistate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGUI/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.312427 ganga-8.6.5/ganga/GangaGaudi/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Gaudi.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.312427 ganga-8.6.5/ganga/GangaGaudi/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/CMTUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/Gaudi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/GaudiBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaGaudi/Lib/Checkers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2848 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaGaudi/Lib/Datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/RunTimeHandlerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaGaudi/Lib/Splitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Splitters/SplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaGaudi/Lib/XMLSummary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/XMLSummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63863 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/XMLSummary/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24704 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/XMLSummary/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/PACKAGE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaGaudi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaLHCb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/BOOT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2352 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/LHCb.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.316427 ganga-8.6.5/ganga/GangaLHCb/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/AppsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/Bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24468 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/BenderBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/BenderScript.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/CMTscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/FileFunctions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30814 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/GaudiExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/GaudiPython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/Ostap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/Backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Backends/Dirac.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/Checkers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/Files/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Files/LogicalFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Files/PhysicalFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19914 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23063 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.320427 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34906 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaLHCb/Lib/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaLHCb/Lib/XMLSummary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/XMLSummary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64899 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/XMLSummary/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25050 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/XMLSummary/summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaLHCb/Utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Utility/LHCbDIRACenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/Utility/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8967 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaLHCb/testlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaLHCb/testlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaND280/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/BOOT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaND280/Highland/
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Highland/Highland.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Highland/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.324427 ganga-8.6.5/ganga/GangaND280/ND280Checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19378 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Checkers/ND280Checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Checkers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9075 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Checkers/post_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280Control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27283 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/ND280Configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/runND280.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/runND280CosMC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/runND280Kin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/runND280RDP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Control/runND280SandMC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280Dataset/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8427 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Dataset/ND280Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280Executable/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Executable/ND280Executable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Executable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280Skimmer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Skimmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280Splitter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8589 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Splitter/ND280Splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280Splitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/ND280TPCGasInteractions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/ND280TPCGasInteractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.328427 ganga-8.6.5/ganga/GangaND280/Tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Tasks/ND280Task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Tasks/ND280Transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Tasks/ND280Unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/Tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaND280/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.332427 ganga-8.6.5/ganga/GangaRelease/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.0
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.2
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.3
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.4
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.0
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.10
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.11
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.12
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.13
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.14
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.15
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.2
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.3
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.4
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.5
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.6
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.7
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.8
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.9
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.2
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.3
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.1.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.1
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.2
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.3
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.4
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.2
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.3
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-22 09:37:36.000000 ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.6.5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.332427 ganga-8.6.5/ganga/GangaRelease/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/tools/check-new-ganga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaRelease/tools/ganga-cvmfs-install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.332427 ganga-8.6.5/ganga/GangaTest/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/BOOT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Framework/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18555 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31840 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/htmlizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47550 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11385 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Framework/xmldifferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4013 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/CrashTest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Lib/GListApp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2803 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/GListApp/GListApp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/GListApp/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/GListApp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3277 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/StoreTestFramework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Lib/TFile/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      485 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TFile/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1485 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TFile/TFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TFile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Lib/TestApplication/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5553 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestApplication/TestApplication.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestApplication/TestDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestApplication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Lib/TestMonitoringService/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestMonitoringService/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestObjects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1363 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3498 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      293 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/Lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/PACKAGE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTest/TestGPIP/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      153 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/TestGPIP/TestGPIP.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      405 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/BOOT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTutorial/Lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6800 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/PrimeFactorizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2287 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/PrimeTableDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.336428 ganga-8.6.5/ganga/GangaTutorial/Lib/primes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/primes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3020 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/primes/prime_factor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Lib/primes/primes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/PACKAGE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/Tutorial.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/GangaTutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.340427 ganga-8.6.5/ganga/ganga/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/ganga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 09:37:22.000000 ganga-8.6.5/ganga/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:37:37.268427 ganga-8.6.5/ganga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-22 09:37:37.000000 ganga-8.6.5/ganga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37743 2023-04-22 09:37:37.000000 ganga-8.6.5/ganga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:37:37.000000 ganga-8.6.5/ganga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-22 09:37:37.000000 ganga-8.6.5/ganga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-22 09:37:37.000000 ganga-8.6.5/ganga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-22 09:37:37.340427 ganga-8.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-22 09:37:36.000000 ganga-8.6.5/setup.py
```

### Comparing `ganga-8.6.4/LICENSE_GPL` & `ganga-8.6.5/LICENSE_GPL`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/PKG-INFO` & `ganga-8.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganga
-Version: 8.6.4
+Version: 8.6.5
 Summary: Job management tool
 Home-page: https://github.com/ganga-devs/ganga
 Author: Ganga Developers
 Author-email: project-ganga-developers@cern.ch
 License: GPL v2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ganga-8.6.4/README.rst` & `ganga-8.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/bin/ganga` & `ganga-8.6.5/bin/ganga`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/bin/ganga-gui` & `ganga-8.6.5/bin/ganga-gui`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/Makefile` & `ganga-8.6.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/Configuration.rst` & `ganga-8.6.5/doc/UserGuide/Configuration.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/GoogleOauth.rst` & `ganga-8.6.5/doc/UserGuide/GoogleOauth.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/InputAndOutputData.rst` & `ganga-8.6.5/doc/UserGuide/InputAndOutputData.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/InstallAndBasicUsage.rst` & `ganga-8.6.5/doc/UserGuide/InstallAndBasicUsage.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/JobManipulation.rst` & `ganga-8.6.5/doc/UserGuide/JobManipulation.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/MiscellaneousFunctionality.rst` & `ganga-8.6.5/doc/UserGuide/MiscellaneousFunctionality.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/PostProcessors.rst` & `ganga-8.6.5/doc/UserGuide/PostProcessors.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/Queues.rst` & `ganga-8.6.5/doc/UserGuide/Queues.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/RunningExecutables.rst` & `ganga-8.6.5/doc/UserGuide/RunningExecutables.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/Splitters.rst` & `ganga-8.6.5/doc/UserGuide/Splitters.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/Tasks.rst` & `ganga-8.6.5/doc/UserGuide/Tasks.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/TutorialPlugin.rst` & `ganga-8.6.5/doc/UserGuide/TutorialPlugin.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/UsingDifferentApplications.rst` & `ganga-8.6.5/doc/UserGuide/UsingDifferentApplications.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/UsingDifferentBackends.rst` & `ganga-8.6.5/doc/UserGuide/UsingDifferentBackends.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/Virtualization.rst` & `ganga-8.6.5/doc/UserGuide/Virtualization.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/WhatIsGanga.rst` & `ganga-8.6.5/doc/UserGuide/WhatIsGanga.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/first_job.gif` & `ganga-8.6.5/doc/UserGuide/first_job.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/index.rst` & `ganga-8.6.5/doc/UserGuide/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/start_terminal.gif` & `ganga-8.6.5/doc/UserGuide/start_terminal.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/UserGuide/virtualization.gif` & `ganga-8.6.5/doc/UserGuide/virtualization.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/_static/favicon.ico` & `ganga-8.6.5/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/_static/logo.svg` & `ganga-8.6.5/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/conf.py` & `ganga-8.6.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/dev/credentials.rst` & `ganga-8.6.5/doc/dev/credentials.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/dev/index.rst` & `ganga-8.6.5/doc/dev/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/fill_gpi.py` & `ganga-8.6.5/doc/fill_gpi.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/GangaJob.pdf` & `ganga-8.6.5/doc/journal/CPC2007/GangaJob.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/GangaOverview.pdf` & `ganga-8.6.5/doc/journal/CPC2007/GangaOverview.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/GangaPlugin.pdf` & `ganga-8.6.5/doc/journal/CPC2007/GangaPlugin.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/README` & `ganga-8.6.5/doc/journal/CPC2007/README`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/avianflu.pdf` & `ganga-8.6.5/doc/journal/CPC2007/avianflu.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/avianflu.png` & `ganga-8.6.5/doc/journal/CPC2007/avianflu.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/camtology.tex` & `ganga-8.6.5/doc/journal/CPC2007/camtology.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/camtologyfigure.eps` & `ganga-8.6.5/doc/journal/CPC2007/camtologyfigure.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/camtologyfigure.pdf` & `ganga-8.6.5/doc/journal/CPC2007/camtologyfigure.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/camtologytech.pdf` & `ganga-8.6.5/doc/journal/CPC2007/camtologytech.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/elsart.cls` & `ganga-8.6.5/doc/journal/CPC2007/elsart.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/elsart1p.cls` & `ganga-8.6.5/doc/journal/CPC2007/elsart1p.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/elsart3p.cls` & `ganga-8.6.5/doc/journal/CPC2007/elsart3p.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/elsart5p.cls` & `ganga-8.6.5/doc/journal/CPC2007/elsart5p.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-GUI.eps` & `ganga-8.6.5/doc/journal/CPC2007/ganga-GUI.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-GUI.png` & `ganga-8.6.5/doc/journal/CPC2007/ganga-GUI.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-architecture.png` & `ganga-8.6.5/doc/journal/CPC2007/ganga-architecture.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-architecture.svg` & `ganga-8.6.5/doc/journal/CPC2007/ganga-architecture.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-diane-portal.pdf` & `ganga-8.6.5/doc/journal/CPC2007/ganga-diane-portal.pdf`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-diane-portal.png` & `ganga-8.6.5/doc/journal/CPC2007/ganga-diane-portal.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-diane-portal.svg` & `ganga-8.6.5/doc/journal/CPC2007/ganga-diane-portal.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-objects.dia` & `ganga-8.6.5/doc/journal/CPC2007/ganga-objects.dia`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-objects.eps` & `ganga-8.6.5/doc/journal/CPC2007/ganga-objects.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga-objects.png` & `ganga-8.6.5/doc/journal/CPC2007/ganga-objects.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/ganga.tex` & `ganga-8.6.5/doc/journal/CPC2007/ganga.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/instructions-num.tex` & `ganga-8.6.5/doc/journal/CPC2007/instructions-num.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/job-uml.dia` & `ganga-8.6.5/doc/journal/CPC2007/job-uml.dia`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/job-uml.eps` & `ganga-8.6.5/doc/journal/CPC2007/job-uml.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/job-uml.png` & `ganga-8.6.5/doc/journal/CPC2007/job-uml.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/monitoring.eps` & `ganga-8.6.5/doc/journal/CPC2007/monitoring.eps`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/monitoring.png` & `ganga-8.6.5/doc/journal/CPC2007/monitoring.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/journal/CPC2007/monitoring.svg` & `ganga-8.6.5/doc/journal/CPC2007/monitoring.svg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/Makefile` & `ganga-8.6.5/doc/manuals/Makefile`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/about.dat` & `ganga-8.6.5/doc/manuals/html/about.dat`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/about.html` & `ganga-8.6.5/doc/manuals/html/about.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/icons/blank.gif` & `ganga-8.6.5/doc/manuals/html/icons/blank.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/icons/blank.png` & `ganga-8.6.5/doc/manuals/html/icons/blank.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/icons/contents.png` & `ganga-8.6.5/doc/manuals/html/icons/contents.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/icons/index.png` & `ganga-8.6.5/doc/manuals/html/icons/index.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/icons/modules.png` & `ganga-8.6.5/doc/manuals/html/icons/modules.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/icons/up.png` & `ganga-8.6.5/doc/manuals/html/icons/up.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/index.html.in` & `ganga-8.6.5/doc/manuals/html/index.html.in`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/stdabout.dat` & `ganga-8.6.5/doc/manuals/html/stdabout.dat`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/html/style.css` & `ganga-8.6.5/doc/manuals/html/style.css`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/perl/SynopsisTable.pm` & `ganga-8.6.5/doc/manuals/perl/SynopsisTable.pm`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/perl/l2hinit.perl` & `ganga-8.6.5/doc/manuals/perl/l2hinit.perl`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/perl/ltxmarkup.perl` & `ganga-8.6.5/doc/manuals/perl/ltxmarkup.perl`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/perl/python.perl` & `ganga-8.6.5/doc/manuals/perl/python.perl`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/script/make-doc.py` & `ganga-8.6.5/doc/manuals/script/make-doc.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/DocMaker/DocMaker.tex` & `ganga-8.6.5/doc/manuals/src/DocMaker/DocMaker.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Back.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Back.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Copy.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Copy.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Delete.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Delete.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Download.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Download.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_AddDocument.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_Generic.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_Generic.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_New.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_New.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_Remove.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_Remove.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_RemoveDocument.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Folder_Rename.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Folder_Rename.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Forward.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Forward.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/GUI_User_Manual.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/General_Options.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/General_Options.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Go.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Go.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Properties.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Properties.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Refresh.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Refresh.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Save.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Save.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/SaveAs_Template.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Search.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Search.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Stop.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Stop.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Kill.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_NewJob.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Remove.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Save.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/ToolBtn_Submit.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/View_Doc.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/View_Doc.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/Write.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/Write.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/browse.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/browse.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_16x16.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_16x16.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_24x24.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_text_16x16.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_text_16x16.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/files_text_24x24.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/files_text_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_24x24.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_32x32.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_32x32.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_down_24x24.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/folder_down_32x32.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_1.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_2.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_3.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_4.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-chapter_5.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui-manual-contents.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/gangagui_default-view_typical.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/genericjob_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/guiconfig_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/help.png` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/help.png`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/index.rst` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/jobbuilder_pic_5.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/menubar_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/menubar_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/menubar_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/monitoring_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/open.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/open.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/preview.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/preview.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_3.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_4.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/quickstart_pic_5.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/retrieve.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/retrieve.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/scriptor_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/splitter_pic_1.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/splitter_pic_2.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GUI_User_Manual/toolbar.jpg` & `ganga-8.6.5/doc/manuals/src/GUI_User_Manual/toolbar.jpg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex` & `ganga-8.6.5/doc/manuals/src/GangaIntroduction/GangaIntroduction.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/LHCb/LHCb.tex` & `ganga-8.6.5/doc/manuals/src/LHCb/LHCb.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/dev_survival/dev_survival.tex` & `ganga-8.6.5/doc/manuals/src/dev_survival/dev_survival.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/dev_survival/makegraph.py` & `ganga-8.6.5/doc/manuals/src/dev_survival/makegraph.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/dev_survival/transient-states.gif` & `ganga-8.6.5/doc/manuals/src/dev_survival/transient-states.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/dev_survival/user-states.gif` & `ganga-8.6.5/doc/manuals/src/dev_survival/user-states.gif`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/workbook/development/development.tex` & `ganga-8.6.5/doc/manuals/src/workbook/development/development.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/workbook/usage/usage.tex` & `ganga-8.6.5/doc/manuals/src/workbook/usage/usage.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/src/workbook/workbook.tex` & `ganga-8.6.5/doc/manuals/src/workbook/workbook.tex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/distutils.sty` & `ganga-8.6.5/doc/manuals/texinputs/distutils.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/fancyhdr.sty` & `ganga-8.6.5/doc/manuals/texinputs/fancyhdr.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/fncychap.sty` & `ganga-8.6.5/doc/manuals/texinputs/fncychap.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/howto.cls` & `ganga-8.6.5/doc/manuals/texinputs/howto.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/ltxmarkup.sty` & `ganga-8.6.5/doc/manuals/texinputs/ltxmarkup.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/manual.cls` & `ganga-8.6.5/doc/manuals/texinputs/manual.cls`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/pypaper.sty` & `ganga-8.6.5/doc/manuals/texinputs/pypaper.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/texinputs/python.sty` & `ganga-8.6.5/doc/manuals/texinputs/python.sty`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/anno-api.py` & `ganga-8.6.5/doc/manuals/tools/anno-api.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/buildindex.py` & `ganga-8.6.5/doc/manuals/tools/buildindex.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/checkargs.pm` & `ganga-8.6.5/doc/manuals/tools/checkargs.pm`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/cklatex` & `ganga-8.6.5/doc/manuals/tools/cklatex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/custlib.py` & `ganga-8.6.5/doc/manuals/tools/custlib.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/cvsinfo.py` & `ganga-8.6.5/doc/manuals/tools/cvsinfo.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/findacks` & `ganga-8.6.5/doc/manuals/tools/findacks`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/findcsyms` & `ganga-8.6.5/doc/manuals/tools/findcsyms`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/findmodrefs` & `ganga-8.6.5/doc/manuals/tools/findmodrefs`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/findsyms` & `ganga-8.6.5/doc/manuals/tools/findsyms`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/getpagecounts` & `ganga-8.6.5/doc/manuals/tools/getpagecounts`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/getversioninfo` & `ganga-8.6.5/doc/manuals/tools/getversioninfo`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/html2texi.pl` & `ganga-8.6.5/doc/manuals/tools/html2texi.pl`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/indfix.py` & `ganga-8.6.5/doc/manuals/tools/indfix.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/listmodules` & `ganga-8.6.5/doc/manuals/tools/listmodules`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/makesec.sh` & `ganga-8.6.5/doc/manuals/tools/makesec.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/mkackshtml` & `ganga-8.6.5/doc/manuals/tools/mkackshtml`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/mkhowto` & `ganga-8.6.5/doc/manuals/tools/mkhowto`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/mkinfo` & `ganga-8.6.5/doc/manuals/tools/mkinfo`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/mkmodindex` & `ganga-8.6.5/doc/manuals/tools/mkmodindex`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/mkpkglist` & `ganga-8.6.5/doc/manuals/tools/mkpkglist`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/mksourcepkg` & `ganga-8.6.5/doc/manuals/tools/mksourcepkg`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/node2label.pl` & `ganga-8.6.5/doc/manuals/tools/node2label.pl`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/prechm.py` & `ganga-8.6.5/doc/manuals/tools/prechm.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/push-docs.sh` & `ganga-8.6.5/doc/manuals/tools/push-docs.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/py2texi.el` & `ganga-8.6.5/doc/manuals/tools/py2texi.el`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/python` & `ganga-8.6.5/doc/manuals/tools/python`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/refcounts.py` & `ganga-8.6.5/doc/manuals/tools/refcounts.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/rewrite.py` & `ganga-8.6.5/doc/manuals/tools/rewrite.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/Makefile` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/Makefile`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/README` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/README`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/conversion.xml` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/conversion.xml`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/docfixer.py` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/docfixer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/esis2sgml.py` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/esis2sgml.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/esistools.py` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/esistools.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/latex2esis.py` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/latex2esis.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/sgmlconv/make.rules` & `ganga-8.6.5/doc/manuals/tools/sgmlconv/make.rules`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/support.py` & `ganga-8.6.5/doc/manuals/tools/support.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/toc2bkm.py` & `ganga-8.6.5/doc/manuals/tools/toc2bkm.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/undoc_symbols.py` & `ganga-8.6.5/doc/manuals/tools/undoc_symbols.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/manuals/tools/update-docs.sh` & `ganga-8.6.5/doc/manuals/tools/update-docs.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/sysadmin/index.rst` & `ganga-8.6.5/doc/sysadmin/index.rst`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/work/lifetime.txt` & `ganga-8.6.5/doc/work/lifetime.txt`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/doc/work/splitting.txt` & `ganga-8.6.5/doc/work/splitting.txt`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/FileWorkspace.py` & `ganga-8.6.5/ganga/GangaCore/Core/FileWorkspace.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/DStreamer.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/DStreamer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/DatabaseRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/FixedLock.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/FixedLock.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepository.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepository.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryCentral.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryDatabase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryImmutableTransient.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/GangaRepositoryXML.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/Registry.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/Registry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/SessionLock.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/SessionLock.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/SubJobJsonList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/SubJobXMLList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/VStreamer.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/VStreamer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/container_controllers.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/container_controllers.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaRepository/migrate.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaRepository/migrate.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/GangaThread.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/GangaThread.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/GangaThreadPool.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/Algorithm.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/Data.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/MTRunner/MTRunner.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/ThreadPoolQueueMonitor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/WorkerThreadPool.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Core/GangaThread/WorkerThreads/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/InternalServices/Coordinator.py` & `ganga-8.6.5/ganga/GangaCore/Core/InternalServices/Coordinator.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/InternalServices/ShutdownManager.py` & `ganga-8.6.5/ganga/GangaCore/Core/InternalServices/ShutdownManager.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py` & `ganga-8.6.5/ganga/GangaCore/Core/MonitoringComponent/Local_GangaMC_Service.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py` & `ganga-8.6.5/ganga/GangaCore/Core/MonitoringComponent/Monitoring.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/Sandbox/Sandbox.py` & `ganga-8.6.5/ganga/GangaCore/Core/Sandbox/Sandbox.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/Sandbox/WNSandbox.py` & `ganga-8.6.5/ganga/GangaCore/Core/Sandbox/WNSandbox.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Core/exceptions.py` & `ganga-8.6.5/ganga/GangaCore/Core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ApplicationRuntimeHandlers.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IApplication.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IApplication.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IBackend.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IBackend.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IChecker.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ICredentialInfo.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ICredentialRequirement.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IGangaFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IMerger.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IMerger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IMonitoringService.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IPostProcessor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IPrepareApp.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IRuntimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/ISplitter.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/ISplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/IVirtualization.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Adapters/StandardJobConfig.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Base/Filters.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Base/Filters.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Base/Objects.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Base/Objects.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Base/Proxy.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Base/Proxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Base/VPrinter.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Base/VPrinter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Base/VPrinterOld.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Base/VPrinterOld.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/AfsToken.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/AfsToken.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/CredentialStore.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/VomsProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials/__init__.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/GridProxy.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/GridProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/ICredential.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Credentials_old/__init__.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Credentials_old/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Config/Config.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Config/Config.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Dataset/Dataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Dataset/GangaDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/File.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/File.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/FileBuffer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/FileUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/GoogleFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/LCGSEFile.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/LCGSEFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/LocalFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/MassStorageFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/OutputFileManager.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/__init__.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/scripts/LCGSEFileWNScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/File/scripts/MassStorageFileWNScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/GangaList/GangaList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/Job.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/Job.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/JobTime.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Job/MetadataDict.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/JobTree/JobTree.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/BoxRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/JobRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/PrepRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySlice.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/RegistrySliceProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Registry/TransientRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreTransform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/CoreUnit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITask.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/ITransform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/IUnit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskChainInput.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskLocalCopy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/TaskRegistry.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Lib/Tasks/common.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Lib/Tasks/common.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/MonitoringServices/Composite.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/MonitoringServices/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Persistency/__init__.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Persistency/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/Schema/Schema.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/Schema/Schema.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/GPIDev/TypeCheck.py` & `ganga-8.6.5/ganga/GangaCore/GPIDev/TypeCheck.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Batch/Batch.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Batch/Batch.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template` & `ganga-8.6.5/ganga/GangaCore/Lib/Batch/BatchScriptTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Checkers/CustomChecker.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Checkers/CustomChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Checkers/FileChecker.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Checkers/FileChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Checkers/MetaDataChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Checkers/RootFileChecker.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Checkers/RootFileChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Condor/Condor.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Condor/Condor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Condor/CondorRequirements.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Condor/CondorRequirements.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Condor/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Condor/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Executable/Executable.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Executable/Executable.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Interactive/Interactive.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Interactive/Interactive.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template` & `ganga-8.6.5/ganga/GangaCore/Lib/Interactive/InteractiveScriptTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Interactive/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/ARC.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/ARC.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/CREAM.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/CREAM.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/ElapsedTimeProfiler.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/ElapsedTimeProfiler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/Grid.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/Grid.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSandboxCache.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSandboxCache.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/GridSimulator.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/GridSimulator.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/simulator-analyze.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/simulator-analyze.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridSimulator/simulator.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridSimulator/simulator.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/GridftpSandboxCache.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/GridftpSandboxCache.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCG.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCG.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCGOutputDownloader.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCGOutputDownloader.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCGRequirements.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCGRequirements.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/LCGSandboxCache.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/LCGSandboxCache.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/Utility.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/Utility.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/LCG/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Lib/LCG/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template` & `ganga-8.6.5/ganga/GangaCore/Lib/Localhost/LocalHostExec.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template` & `ganga-8.6.5/ganga/GangaCore/Lib/Localhost/LocalHostExec_batch.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Localhost/Localhost.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Localhost/Localhost.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Mergers/Merger.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Mergers/Merger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Notebook/Notebook.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Notebook/Notebook.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template` & `ganga-8.6.5/ganga/GangaCore/Lib/Notebook/wrapperNotebookTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Notifier/Notifier.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Notifier/Notifier.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Remote/Remote.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Remote/Remote.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Splitters/ArgSplitter.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Splitters/ArgSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Splitters/DefaultSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Splitters/ExeSplitter.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Splitters/ExeSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Splitters/GangaDatasetSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Splitters/GenericSplitter.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Splitters/GenericSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Virtualization/Docker.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Virtualization/Docker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Lib/Virtualization/Singularity.py` & `ganga-8.6.5/ganga/GangaCore/Lib/Virtualization/Singularity.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/PACKAGE.py` & `ganga-8.6.5/ganga/GangaCore/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/GPIFunctions.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/GPIFunctions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/GPIexport.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/GPIexport.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/GangaCompleter.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/GangaCompleter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/HEAD_CONFIG.INI` & `ganga-8.6.5/ganga/GangaCore/Runtime/HEAD_CONFIG.INI`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/IPythonMagic.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/IPythonMagic.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/Repository_runtime.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/Repository_runtime.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/bootstrap.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/eliza.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/eliza.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/ganga_extension.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/ganga_extension.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/gangadoc.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/gangadoc.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Runtime/plugins.py` & `ganga-8.6.5/ganga/GangaCore/Runtime/plugins.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/ColourText.py` & `ganga-8.6.5/ganga/GangaCore/Utility/ColourText.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Config/Config.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Config/Config.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Config/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Config/tests.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Config/tests.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Decorators.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Decorators.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/GridShell.py` & `ganga-8.6.5/ganga/GangaCore/Utility/GridShell.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Plugin/GangaPlugin.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Plugin/GangaPlugin.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Profiling.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Profiling.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Runtime.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Runtime.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Setup.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Setup.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Shell.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Shell.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/Virtualization.py` & `ganga-8.6.5/ganga/GangaCore/Utility/Virtualization.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/execute.py` & `ganga-8.6.5/ganga/GangaCore/Utility/execute.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/external/OrderedDict.py` & `ganga-8.6.5/ganga/GangaCore/Utility/external/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/feedback_report.py` & `ganga-8.6.5/ganga/GangaCore/Utility/feedback_report.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/files.py` & `ganga-8.6.5/ganga/GangaCore/Utility/files.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/logging/__init__.py` & `ganga-8.6.5/ganga/GangaCore/Utility/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/logging/test.py` & `ganga-8.6.5/ganga/GangaCore/Utility/logging/test.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/root.py` & `ganga-8.6.5/ganga/GangaCore/Utility/root.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/stacktracer.py` & `ganga-8.6.5/ganga/GangaCore/Utility/stacktracer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/strings.py` & `ganga-8.6.5/ganga/GangaCore/Utility/strings.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/threads.py` & `ganga-8.6.5/ganga/GangaCore/Utility/threads.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/Utility/util.py` & `ganga-8.6.5/ganga/GangaCore/Utility/util.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/__init__.py` & `ganga-8.6.5/ganga/GangaCore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return lcg_release_areas['cvmfs']
     else:
         return ''
 
 
 # ------------------------------------------------
 # store Ganga version based on new git tag for this file
-_gangaVersion = '8.6.4'
+_gangaVersion = '8.6.5'
 _development = False
 
 # store a path to Ganga libraries
 _gangaPythonPath = os.path.dirname(os.path.dirname(__file__))
 
 
 # grab the hostname
```

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/ConfigObject.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/ConfigObject.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/ConfigUser.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/ConfigUser.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesBatchMultipleFilesForLCGUpload.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesInteractiveMultipleFilesForPattern.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLCG.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocal.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForLCGUpload.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesLocalMultipleFilesForPattern.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/GPI/OutputFiles/OutputFilesMixedBatch.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/__init__.py` & `ganga-8.6.5/ganga/GangaCore/old_test/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/config/Schema.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/config/Schema.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/config/default.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/config/default.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/old_test/config/localxml.ini` & `ganga-8.6.5/ganga/GangaCore/old_test/config/localxml.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/test/GPI/Notebook/Test.ipynb` & `ganga-8.6.5/ganga/GangaCore/test/GPI/Notebook/Test.ipynb`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/testlib/GangaUnitTest.py` & `ganga-8.6.5/ganga/GangaCore/testlib/GangaUnitTest.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/testlib/decorators.py` & `ganga-8.6.5/ganga/GangaCore/testlib/decorators.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/testlib/file_utils.py` & `ganga-8.6.5/ganga/GangaCore/testlib/file_utils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/testlib/fixtures.py` & `ganga-8.6.5/ganga/GangaCore/testlib/fixtures.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/testlib/mark.py` & `ganga-8.6.5/ganga/GangaCore/testlib/mark.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaCore/testlib/monitoring.py` & `ganga-8.6.5/ganga/GangaCore/testlib/monitoring.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/BOOT.py` & `ganga-8.6.5/ganga/GangaDirac/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Dirac.ini` & `ganga-8.6.5/ganga/GangaDirac/Dirac.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Backends/Dirac.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Backends/Dirac.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Backends/DiracBase.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Backends/DiracBase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Backends/DiracUtils.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Backends/DiracUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Credentials/DiracProxy.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Credentials/DiracProxy.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Files/DiracFile.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Files/DiracFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template` & `ganga-8.6.5/ganga/GangaDirac/Lib/Files/WNInjectTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Files/uploadScript.py.template` & `ganga-8.6.5/ganga/GangaDirac/Lib/Files/uploadScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template` & `ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/DiracRTHUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/ExeDiracRTHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/RTHandlers/RunTimeHandlerUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Server/DiracCommands.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Server/DiracCommands.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Server/DiracDefinition.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Server/DiracDefinition.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Server/DiracProcess.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Server/DiracProcess.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Server/InspectionClient.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Server/InspectionClient.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Server/InspectionServer.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Server/InspectionServer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/GangaSplitterUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/OfflineGangaDiracSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Splitters/SplitterUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py` & `ganga-8.6.5/ganga/GangaDirac/Lib/Utilities/DiracUtilities.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/PACKAGE.py` & `ganga-8.6.5/ganga/GangaDirac/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaDirac/__init__.py` & `ganga-8.6.5/ganga/GangaDirac/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/api/routes.py` & `ganga-8.6.5/ganga/GangaGUI/api/routes.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/config.py` & `ganga-8.6.5/ganga/GangaGUI/gui/config.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/routes.py` & `ganga-8.6.5/ganga/GangaGUI/gui/routes.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/css/style.css` & `ganga-8.6.5/ganga/GangaGUI/gui/static/css/style.css`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/cli.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/cli.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/create.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/create.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/credentials.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/credentials.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/dashboard.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/job.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/job.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/jobs.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/jobs.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/login.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/login.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/main.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/queue.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/queue.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/style.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/style.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/subjob.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/subjob.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/subjobs.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/subjobs.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/static/js/templates.js` & `ganga-8.6.5/ganga/GangaGUI/gui/static/js/templates.js`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/base.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/cli.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/cli.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/config.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/config.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/config_edit.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/config_edit.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/create.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/create.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/credentials.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/credentials.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/dashboard.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/edit_job.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/edit_job.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/job.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/job.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/job_dir.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/job_dir.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/jobs.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/jobs.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/login.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/login.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/logs.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/logs.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/plugins.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/plugins.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/queue.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/queue.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/runfile.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/runfile.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/storage.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/storage.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/subjob.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/subjob.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/subjob_dir.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/subjob_dir.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/subjobs.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/subjobs.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/gui/templates/templates.html` & `ganga-8.6.5/ganga/GangaGUI/gui/templates/templates.html`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGUI/start.py` & `ganga-8.6.5/ganga/GangaGUI/start.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/CMTUtils.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/CMTUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/Gaudi.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/Gaudi.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/GaudiBase.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/GaudiBase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/GaudiUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/GaudiXMLSummary.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Applications/cmakeUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Checkers/GaudiMetaDataChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Datasets/GaudiDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiDiracRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/RTHandlers/GaudiRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/Splitters/GaudiInputDataSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/XMLSummary/schema.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/XMLSummary/schema.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/Lib/XMLSummary/summary.py` & `ganga-8.6.5/ganga/GangaGaudi/Lib/XMLSummary/summary.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/PACKAGE.py` & `ganga-8.6.5/ganga/GangaGaudi/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaGaudi/__init__.py` & `ganga-8.6.5/ganga/GangaGaudi/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/BOOT.py` & `ganga-8.6.5/ganga/GangaLHCb/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/LHCb.ini` & `ganga-8.6.5/ganga/GangaLHCb/LHCb.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/AppsBase.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/AppsBase.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/AppsBaseUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/Bender.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/Bender.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/BenderBox.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/BenderBox.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/BenderScript.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/BenderScript.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/CMTscript.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/CMTscript.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/EnvironFunctions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/FileFunctions.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/FileFunctions.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/GaudiExec.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/GaudiExec.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/GaudiExecUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/GaudiPython.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/GaudiPython.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/Ostap.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/Ostap.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/PythonOptionsParser.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/PythonOptsCmakeParser.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/XMLPostProcessor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Applications/__init__.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Applications/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Backends/Bookkeeping.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Backends/Dirac.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Backends/Dirac.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Checkers/LHCbMetadataChecker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Files/LogicalFile.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Files/LogicalFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Files/PhysicalFile.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Files/PhysicalFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/BKQuery.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbCompressedDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/LHCbDataset/LHCbDatasetUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/CMTVersion.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/GaudiExecMerger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Mergers/LHCbFileMerger.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/ExeDiracRTHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiExecRTHandlers.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/GaudiTemplate.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiDiracRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/LHCbGaudiRunTimeHandler.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/RTHUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/WorkerScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template` & `ganga-8.6.5/ganga/GangaLHCb/Lib/RTHandlers/XMLWorkerScript.py.template`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Server/DiracLHCbCommands.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Server/DiracLHCbDefinition.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/GaussSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/LHCbSplitterUtils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/OptionsFileSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/SplitByFiles.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/SplitFilesBySize.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Splitters/TestSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/BKTestQuery.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbTask.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbTaskDummySplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbTransform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/Tasks/LHCbUnit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/XMLSummary/schema.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/XMLSummary/schema.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Lib/XMLSummary/summary.py` & `ganga-8.6.5/ganga/GangaLHCb/Lib/XMLSummary/summary.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/PACKAGE.py` & `ganga-8.6.5/ganga/GangaLHCb/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/Utility/LHCbDIRACenv.py` & `ganga-8.6.5/ganga/GangaLHCb/Utility/LHCbDIRACenv.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaLHCb/__init__.py` & `ganga-8.6.5/ganga/GangaLHCb/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/Highland/Highland.py` & `ganga-8.6.5/ganga/GangaND280/Highland/Highland.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280.ini` & `ganga-8.6.5/ganga/GangaND280/ND280.ini`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Checkers/ND280Checker.py` & `ganga-8.6.5/ganga/GangaND280/ND280Checkers/ND280Checker.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Checkers/post_status.py` & `ganga-8.6.5/ganga/GangaND280/ND280Checkers/post_status.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/ND280Configs.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/ND280Configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 #!/usr/bin/env python
 
-import sys
-import re
-import tempfile
-import os
-import optparse
-import shutil
 import random
 
 from GangaCore.Utility.logging import getLogger
 logger = getLogger()
 
-class ND280Config:
 
+class ND280Config:
 
     """
     This is an adaptation of ND280Computing/tools/ND280Configs.py.
     A class to handle automatically creating nd280Control config info.
 
     Types
 
@@ -67,25 +61,25 @@
     >>> cfg.options['production'] = 'True'
     >>> cfg.options['save_geometry'] = '1'
 
     >>> cfg_str = cfg.CreateConfig()
     >>> print cfg_str # prints configuration file info
     """
 
-    def __init__(self, cfgtype,extra_opts):
-        self.cfgtype=cfgtype.lower()
-        self.options=self.common_options
-        self.options_ignore=self.common_options_ignore
+    def __init__(self, cfgtype, extra_opts):
+        self.cfgtype = cfgtype.lower()
+        self.options = self.common_options
+        self.options_ignore = self.common_options_ignore
 
         if self.cfgtype == 'gnsetup':
             self.options.update(self.genieSetup_options)
-            self.options['genie_setup_script']=self.t2ksoftdir + '/GENIE/setup.sh'
+            self.options['genie_setup_script'] = self.t2ksoftdir + '/GENIE/setup.sh'
         elif self.cfgtype == 'gnmc':
             self.options.update(self.genieMC_options)
-            self.options['genie_setup_script']=self.t2ksoftdir + '/GENIE/setup.sh'
+            self.options['genie_setup_script'] = self.t2ksoftdir + '/GENIE/setup.sh'
         elif self.cfgtype == 'raw':
             self.options.update(self.raw_options)
             self.options_ignore.update(self.raw_options_ignore)
         elif self.cfgtype == 'cosmicmc':
             self.options.update(self.cosmicmc_options)
             self.options_ignore.update(self.cosmicmc_options_ignore)
         elif self.cfgtype == 'sandmc':
@@ -96,292 +90,291 @@
         elif self.cfgtype == 'MC':
             self.options.update(self.mc_options)
         elif self.cfgtype == 'PG':
             self.options.update(self.pg_options)
         else:
             raise RuntimeError('ND280Configs: {} Not a reconised config type.'.format(self.cfgtype))
 
-
         self.options.update(extra_opts)
 
-    ### Global
-    cfgtype=''
-    config_filename=''
-    t2ksoftdir=''
-    options={}
+    # Global
+    cfgtype = ''
+    config_filename = ''
+    t2ksoftdir = ''
+    options = {}
     ##################
-    ### Options
-    ### Common Options: Dictionary of common options amongst all config files
-    common_options={'cmtpath':'environment',
-                    'cmtroot':'environment',
-                    'nd280ver':'',
-                    'custom_list':'',
-                    'db_time':'',
-                    'database_P6':''}
-
-    ## Ignore options - options that are not essential and can be overlooked
-    common_options_ignore={'comment':'','midas_file':'',
-                           'event_select':'',
-                           'inputfile':'',
-                           'version_number':'',
-                           'custom_list':'',
-                           'db_time':'',
-                           'database_P6':''}
-
-    ### Raw Data Options: Dictionary of options specific to Raw data processing cfg files
-    raw_options={ 'midas_file':'',
-                  'comment':'',
-                  'event_select':'',
-                  'module_list_cmt':'oaCalib oaRecon oaAnalysis',
-                  'module_list_git':'eventCalib eventRecon eventAnalysis',
-                  'version_number':'',
-                  'inputfile':'',
-                  'enable_modules':'',
-                  'disable_modules':'',
-                  'process_truncated':'',
-                  'num_events':'',
-                  'production':'',
-                  'save_geometry':''}
-
-    raw_options_ignore={'enable_modules':'',
-                        'disable_modules':'',
-                        'process_truncated':'',
-                        'num_events':'',
-                        'production':'',
-                        'save_geometry':''}
-
-    cosmicmc_options={   'stage':'base',
-                         'nd280ver':'v11r31',
-                         'module_list_cmt':'cosmic nd280MC elecSim oaCalibMC oaCosmicTrigger',
-                         'module_list_git':'cosmic nd280Geant4Sim detResponseSim eventCalibMC cosmicTriggerGeant4Sim',
-                         'run_number':'0',
-                         'subrun':'0',
-                         'baseline':'2010-11',
-                         'p0d_water_fill':'1',
-                         'replace_comment':'1',
-                         'comment':'basecosmiccorsika5F',
-                         'mc_type':'Cosmic',
-                         'random_seed':'123456789',
-                         'num_events':'1000000000',
-                         'mc_full_spill':'0',
-                         'mc_position':'Free',
-                         'kinfile':'REPLACE_KINFILE',
-                         'inputfile':'REPLACE_INPUTFILE',
-                         'randomize_kinfile':'false',
-                         'save_digits':'true' }
-
-    cosmicmc_options_ignore={'random_seed':''}
-
-    #### Sand MC
-    sandmc_options={'stage':'neutMC',
-                'module_list_cmt':'sandPropagate nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
-                'module_list_git':'sandPropagate nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
-                'neut_setup_script':'REPLACE_NEUTSETUP',
-                'neut_card':'REPLACE_NEUTCARD',
-                'flux_file':'REPLACE_FLUXFILE',
-                'maxint_file':'REPLACE_MAXINT',
-                'inputfile':'REPLACE_INPUTFILE',
-                'run_number':'0',
-                'subrun':'0',
-                'baseline':'2010-11',
-                'p0d_water_fill':'0',
-                'num_events':'10000000',
-                'mc_type':'Neut_RooTracker',
-                'nd280mc_random_seed':'3456532423',
-                #'nd280mc_random_seed':str(random.getrandbits(29)),
-                'pot':'2.5e17',
-                'neutrino_type':'beam',
-                'flux_region':'SAND',
-                'master_volume':'World',
-                'force_volume_name':'true',
-                'tpc_periods_to_activate':'runs2-3',
-                'ecal_periods_to_activate':'3-4',
-                'random_start':'1',
-                'nbunches':'8',
-                'interactions_per_spill':'1',
-                'pot_per_spill':'1',
-                'mc_full_spill':'1',
-                'time_offset':'50',
-                'count_type':'MEAN',
-		'mc_position':'free',
-                'bunch_duration':'19',
-                'elmc_random_seed':'317075105',
-                #'elmc_random_seed':str(random.getrandbits(28)),
-                'production':'True',
-                'save_geometry':'1',
-                'comment':'prod6sand201011airrun3'}
-
-    sandmc_options_ignore={}
-
-    #### MC
-    mc_options={'module_list_cmt':'nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
-                'module_list_git':'nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
-                'inputfile':'/lustre/ific.uv.es/sw/t2k.org/nd280Soft/nd280computing/processing_scripts/oa_nt_beam_90210013-0100_3ravbul66rum_numc_000_prod004magnet201011waterb.root',
-                'run_number':'90210000',
-                'subrun':'0',
-                'baseline':'2010-11',
-                'p0d_water_fill':'1',
-                'num_events':'100000000',
-                'mc_type':'Neut_RooTracker',
-#                'nd280mc_random_seed':'3456532423',
-                'nd280mc_random_seed':str(random.getrandbits(29)),
-                'nbunches':'8',
-                # for production 5
-                'interactions_per_spill':'9.2264889',
-                'pot_per_spill':'7.9891e+13',
-                'mc_full_spill':'1',
-                'time_offset':'50',
-                'count_type':'MEAN',
-		'mc_position':'free',
-                'bunch_duration':'19',
-#                'elmc_random_seed':'317075105',
-                'elmc_random_seed':str(random.getrandbits(28)),
-                'production':'1',
-                'comment':'prod004magnet201011waterb'}
-
-    ### GENIE Setup Options: Dictionary of options specific to GENIE setup cfg files
-    genieSetup_options={'baseline':'',
-                        'p0d_water_fill':'',
-                        'genie_xs_table':'',
-                        'master_volume':'',
-                        'genie_setup_script':''}
-
-    ### GENIE MC Options: Dictionary of options specific to GENIE MC cfg files
-    genieMC_options={'baseline':'',
-                     'p0d_water_fill':'',
-                     'genie_xs_table':'',
-                     'master_volume':'',
-                     'genie_setup_script':'',
-                     'run_number':'',
-                     'subrun':'',
-                     'comment':'',
-                     'neutrino_type':'beam',
-                     'flux_file':'',
-                     'flux_tree':'h3002',
-                     'pot':'',
-                     'genie_paths':'',
-                     'random_seed':''}
-
-    gncp_options = {'module_list_cmt':'oaCherryPicker nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
-                    'module_list_git':'selectEventSim nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
-                    'run_number':'',
-                    'subrun':'',
-                    'comment':'',
-                    'baseline':'',
-                    'p0d_water_fill':'',
-                    'num_events':'999999999',
-                    'nd280mc_random_seed':'',
-                    'mc_full_spill':'0',
-                    'time_offset':'50',
-                    'mc_position':'free',
-                    'interactions_per_spill':'1',
-                    'count_type':'FIXED',
-                    'elmc_random_seed':'',
-                    'cherry_picker_type':''}
-
-    ### GRID options are not considered compulsory but I include here for totality.
-    grid_options = {'use_grid':'0',
-                    'storage_address':'',
-                    'register_address':'',
-                    'register_files':'1',
-                    'register_catalogue_files':'0'}
-
-    ### Particle Gun options
-    pg_options = {'geo_baseline':'2010-02',
-                  'p0d_water':'1',
-                  'module_list_cmt':'nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
-                  'module_list_git':'nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
-                  'comment':'',
-                  'num_events':'10000',
-                  'mc_particle':'mu-',
-                  'mc_position':'SUBDETECTOR p0d',
-                  'mc_energy':'uniform 500 1000',
-                  'mc_direction':'ISOTROPIC',
-                  'nd280mc_random_seed':'999',
-                  'interactions_per_spill':'1',
-                  'nbunches':'1',
-                  'elmc_random_seed':'999'}
-
+    # Options
+    # Common Options: Dictionary of common options amongst all config files
+    common_options = {'cmtpath': 'environment',
+                      'cmtroot': 'environment',
+                      'nd280ver': '',
+                      'custom_list': '',
+                      'db_time': '',
+                      'database_P6': '',
+                      'magnet_ecal_production6': ''}
+
+    # Ignore options - options that are not essential and can be overlooked
+    common_options_ignore = {'comment': '', 'midas_file': '',
+                             'event_select': '',
+                             'inputfile': '',
+                             'version_number': '',
+                             'custom_list': '',
+                             'db_time': '',
+                             'database_P6': '',
+                             'magnet_ecal_production6': ''}
+
+    # Raw Data Options: Dictionary of options specific to Raw data processing cfg files
+    raw_options = {'midas_file': '',
+                   'comment': '',
+                   'event_select': '',
+                   'module_list_cmt': 'oaCalib oaRecon oaAnalysis',
+                   'module_list_git': 'eventCalib eventRecon eventAnalysis',
+                   'version_number': '',
+                   'inputfile': '',
+                   'enable_modules': '',
+                   'disable_modules': '',
+                   'process_truncated': '',
+                   'num_events': '',
+                   'production': '',
+                   'save_geometry': ''}
+
+    raw_options_ignore = {'enable_modules': '',
+                          'disable_modules': '',
+                          'process_truncated': '',
+                          'num_events': '',
+                          'production': '',
+                          'save_geometry': ''}
+
+    cosmicmc_options = {'stage': 'base',
+                        'nd280ver': 'v11r31',
+                        'module_list_cmt': 'cosmic nd280MC elecSim oaCalibMC oaCosmicTrigger',
+                        'module_list_git': 'cosmic nd280Geant4Sim detResponseSim eventCalibMC cosmicTriggerGeant4Sim',
+                        'run_number': '0',
+                        'subrun': '0',
+                        'baseline': '2010-11',
+                        'p0d_water_fill': '1',
+                        'replace_comment': '1',
+                        'comment': 'basecosmiccorsika5F',
+                        'mc_type': 'Cosmic',
+                        'random_seed': '123456789',
+                        'num_events': '1000000000',
+                        'mc_full_spill': '0',
+                        'mc_position': 'Free',
+                        'kinfile': 'REPLACE_KINFILE',
+                        'inputfile': 'REPLACE_INPUTFILE',
+                        'randomize_kinfile': 'false',
+                        'save_digits': 'true'}
+
+    cosmicmc_options_ignore = {'random_seed': ''}
+
+    # Sand MC
+    sandmc_options = {'stage': 'neutMC',
+                      'module_list_cmt': 'sandPropagate nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
+                      'module_list_git': 'sandPropagate nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
+                      'neut_setup_script': 'REPLACE_NEUTSETUP',
+                      'neut_card': 'REPLACE_NEUTCARD',
+                      'flux_file': 'REPLACE_FLUXFILE',
+                      'maxint_file': 'REPLACE_MAXINT',
+                      'inputfile': 'REPLACE_INPUTFILE',
+                      'run_number': '0',
+                      'subrun': '0',
+                      'baseline': '2010-11',
+                      'p0d_water_fill': '0',
+                      'num_events': '10000000',
+                      'mc_type': 'Neut_RooTracker',
+                      'nd280mc_random_seed': '3456532423',
+                      # 'nd280mc_random_seed':str(random.getrandbits(29)),
+                      'pot': '2.5e17',
+                      'neutrino_type': 'beam',
+                      'flux_region': 'SAND',
+                      'master_volume': 'World',
+                      'force_volume_name': 'true',
+                      'tpc_periods_to_activate': 'runs2-3',
+                      'ecal_periods_to_activate': '3-4',
+                      'random_start': '1',
+                      'nbunches': '8',
+                      'interactions_per_spill': '1',
+                      'pot_per_spill': '1',
+                      'mc_full_spill': '1',
+                      'time_offset': '50',
+                      'count_type': 'MEAN',
+                      'mc_position': 'free',
+                      'bunch_duration': '19',
+                      'elmc_random_seed': '317075105',
+                      # 'elmc_random_seed':str(random.getrandbits(28)),
+                      'production': 'True',
+                      'save_geometry': '1',
+                      'comment': 'prod6sand201011airrun3'}
+
+    sandmc_options_ignore = {}
+
+    # MC
+    mc_options = {'module_list_cmt': 'nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
+                  'module_list_git': 'nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
+                  'inputfile': ('/lustre/ific.uv.es/sw/t2k.org/nd280Soft/nd280computing/processing_scripts/'
+                                'oa_nt_beam_90210013-0100_3ravbul66rum_numc_000_prod004magnet201011waterb.root'),
+                  'run_number': '90210000',
+                  'subrun': '0',
+                  'baseline': '2010-11',
+                  'p0d_water_fill': '1',
+                  'num_events': '100000000',
+                  'mc_type': 'Neut_RooTracker',
+                  #                'nd280mc_random_seed':'3456532423',
+                  'nd280mc_random_seed': str(random.getrandbits(29)),
+                  'nbunches': '8',
+                  # for production 5
+                  'interactions_per_spill': '9.2264889',
+                  'pot_per_spill': '7.9891e+13',
+                  'mc_full_spill': '1',
+                  'time_offset': '50',
+                  'count_type': 'MEAN',
+                  'mc_position': 'free',
+                  'bunch_duration': '19',
+                  #                'elmc_random_seed':'317075105',
+                  'elmc_random_seed': str(random.getrandbits(28)),
+                  'production': '1',
+                  'comment': 'prod004magnet201011waterb'}
+
+    # GENIE Setup Options: Dictionary of options specific to GENIE setup cfg files
+    genieSetup_options = {'baseline': '',
+                          'p0d_water_fill': '',
+                          'genie_xs_table': '',
+                          'master_volume': '',
+                          'genie_setup_script': ''}
+
+    # GENIE MC Options: Dictionary of options specific to GENIE MC cfg files
+    genieMC_options = {'baseline': '',
+                       'p0d_water_fill': '',
+                       'genie_xs_table': '',
+                       'master_volume': '',
+                       'genie_setup_script': '',
+                       'run_number': '',
+                       'subrun': '',
+                       'comment': '',
+                       'neutrino_type': 'beam',
+                       'flux_file': '',
+                       'flux_tree': 'h3002',
+                       'pot': '',
+                       'genie_paths': '',
+                       'random_seed': ''}
+
+    gncp_options = {'module_list_cmt': 'oaCherryPicker nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
+                    'module_list_git': 'selectEventSim nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
+                    'run_number': '',
+                    'subrun': '',
+                    'comment': '',
+                    'baseline': '',
+                    'p0d_water_fill': '',
+                    'num_events': '999999999',
+                    'nd280mc_random_seed': '',
+                    'mc_full_spill': '0',
+                    'time_offset': '50',
+                    'mc_position': 'free',
+                    'interactions_per_spill': '1',
+                    'count_type': 'FIXED',
+                    'elmc_random_seed': '',
+                    'cherry_picker_type': ''}
+
+    # GRID options are not considered compulsory but I include here for totality.
+    grid_options = {'use_grid': '0',
+                    'storage_address': '',
+                    'register_address': '',
+                    'register_files': '1',
+                    'register_catalogue_files': '0'}
+
+    # Particle Gun options
+    pg_options = {'geo_baseline': '2010-02',
+                  'p0d_water': '1',
+                  'module_list_cmt': 'nd280MC elecSim oaCalibMC oaRecon oaAnalysis',
+                  'module_list_git': 'nd280Geant4Sim detResponseSim eventCalibMC eventRecon eventAnalysis',
+                  'comment': '',
+                  'num_events': '10000',
+                  'mc_particle': 'mu-',
+                  'mc_position': 'SUBDETECTOR p0d',
+                  'mc_energy': 'uniform 500 1000',
+                  'mc_direction': 'ISOTROPIC',
+                  'nd280mc_random_seed': '999',
+                  'interactions_per_spill': '1',
+                  'nbunches': '1',
+                  'elmc_random_seed': '999'}
 
     def CheckOptions(self):
-        allOK=1
-        ## Quick check to see if there are any blank options, only allowed for comment.
-        for k,v in self.options.items():
+        allOK = 1
+        # Quick check to see if there are any blank options, only allowed for comment.
+        for k, v in self.options.items():
             if not v:
                 if k in self.options_ignore:
                     continue
                 else:
                     logger.info('Please ensure a value for ' + k + ' using the object.options[\'' + k + '\']')
-                    allOK=0
+                    allOK = 0
 
         return allOK
 
     def ListOptions(self):
-        for k,v in self.options.items():
+        for k, v in self.options.items():
             logger.info(k + ' = ' + v)
         return
 
-    def SetOptions(self,options_in):
-        for k,v in options_in.items():
+    def SetOptions(self, options_in):
+        for k, v in options_in.items():
             if k in self.options:
-                self.options[k]=v
+                self.options[k] = v
             else:
                 logger.info('Option ' + k + ' not in list, ignoring.')
 
     def CreateConfig(self):
         map = {
-            'gnsetup' : self.CreateGENIEsetupCF,
-            'raw'     : self.CreateRawCF,
+            'gnsetup': self.CreateGENIEsetupCF,
+            'raw': self.CreateRawCF,
             'cosmicmc': self.CreateCosmicMCCF,
             'sandmc': self.CreateSandMCCF
-            }
+        }
         if map.get(self.cfgtype):
             creator = map[self.cfgtype]
             return creator()
         else:
             raise RuntimeError('ND280Configs: {} Not a reconised config type.'.format(self.cfgtype))
 
+    # GENIE Setup
 
-
-    ######################## GENIE Setup
     def CreateGENIEsetupCF(self):
         pass
 
+    # Raw Data Processing Config file
 
-    ######################## Raw Data Processing Config file
     def CreateRawCF(self):
 
         if not self.CheckOptions():
             logger.error('Please make sure all options stated above are entered')
             return ''
 
         configfile = ''
         configfile += "# Automatically generated config file\n\n"
 
-        ### Software Setup
+        # Software Setup
         configfile += "[software]\n"
         if 'cmtpath' in self.options:
             configfile += "cmtpath = " + self.options['cmtpath'] + "\n"
 
         if 'cmtroot' in self.options:
             configfile += "cmtroot = " + self.options['cmtroot'] + "\n"
 
         configfile += "nd280ver = " + self.options['nd280ver'] + "\n\n"
 
-        ### File naming
-        if not  self.options['comment']:
-             self.options['comment'] =  self.options['nd280ver']
+        # File naming
+        if not self.options['comment']:
+            self.options['comment'] = self.options['nd280ver']
         configfile += "[filenaming]\n"
         if self.options['inputfile']:
             logger.info("version_number = " + self.options['version_number'] + "\n")
             configfile += "version_number = " + self.options['version_number'] + "\n"
         configfile += "comment = " + self.options['comment'] + "\n\n"
 
-
-        ### Module list
+        # Module list
         configfile += "[configuration]\n"
         if not self.options['midas_file']:
             configfile += "inputfile = " + self.options['inputfile'] + "\n"
 
         if self.options['nd280ver'][0] == 'v':
             configfile += "module_list = " + self.options['module_list_cmt'] + "\n"
         else:
@@ -392,257 +385,269 @@
             configfile += "dq_database_rollback_date = " + self.options['db_time'] + "\n"
 
         if self.options['database_P6']:
             configfile += 'database_P6 = %s\n' % self.options['database_P6']
 
         configfile += "\n"
 
-        ### Unpack - only if this is a midas file
+        # Unpack - only if this is a midas file
         if self.options['midas_file']:
             configfile += "[unpack]\n"
             configfile += "midas_file = " + self.options['midas_file'] + "\n"
             configfile += "event_select = " + self.options['event_select'] + "\n"
 
             if self.options['process_truncated']:
                 configfile += "process_truncated = " + self.options['process_truncated'] + "\n"
                 configfile += "\n"
             if self.options['num_events']:
                 configfile += "num_events = " + self.options['num_events'] + "\n"
             configfile += "\n"
 
-        ### Analysis if corresponding options are present
+        # Geometry - if needed
+        if self.options['magnet_ecal_production6']:
+            configfile += '[geometry]\n'
+            configfile += 'magnet_ecal_production6 = ' + self.options['magnet_ecal_production6'] + '\n'
+            configfile += "\n"
+
+        # Analysis if corresponding options are present
         if self.options['enable_modules'] or self.options['disable_modules'] or \
-               self.options['production'] or self.options['save_geometry']:
+                self.options['production'] or self.options['save_geometry']:
             configfile += "[analysis]\n"
             if self.options['enable_modules']:
                 configfile += "enable_modules = " + self.options['enable_modules'] + "\n"
             if self.options['disable_modules']:
                 configfile += "disable_modules = " + self.options['disable_modules'] + "\n"
             if self.options['production']:
-                 configfile += "production = " +  self.options['production'] + "\n"
+                configfile += "production = " + self.options['production'] + "\n"
             if self.options['save_geometry']:
-                 configfile += "save_geometry = " +  self.options['save_geometry'] + "\n"
+                configfile += "save_geometry = " + self.options['save_geometry'] + "\n"
             configfile += "\n"
 
-
-        ### GRID Tools
-        if 'use_grid' in self.options and self.options['use_grid']=='1':
+        # GRID Tools
+        if 'use_grid' in self.options and self.options['use_grid'] == '1':
             configfile += "[grid_tools]\n"
             configfile += "use_grid = " + self.options['use_grid'] + "\n"
             configfile += "storage_address = " + self.options['storage_address'] + "\n"
             configfile += "register_files = " + self.options['register_files'] + "\n"
             configfile += "register_catalogue_files = " + self.options['register_catalogue_files'] + "\n"
             configfile += "register_address = " + self.options['register_address'] + "\n"
 
-        ### Custom options
+        # Custom options
         if self.options['custom_list']:
             configfile += '\n'
             configlist = self.options['custom_list'].split(',')
             for confline in configlist:
-                configfile += str(confline)+"\n"
+                configfile += str(confline) + "\n"
             configfile += '\n'
 
         return configfile
 
-    ######################## Cosmic Processing Config file
+    # Cosmic Processing Config file
     def CreateCosmicMCCF(self):
 
         if not self.CheckOptions():
             logger.error('Please make sure all options stated above are entered')
             return ''
 
-        if not self.options['stage'] in ['base','fgd','tript','all']:
-            logger.error('"stage" options should be one of',['base','fgd','tript','all'])
+        if not self.options['stage'] in ['base', 'fgd', 'tript', 'all']:
+            logger.error('"stage" options should be one of', ['base', 'fgd', 'tript', 'all'])
             return ''
 
         configfile = ''
         configfile += "# Automatically generated config file\n\n"
 
-
-        ### Software Setup
+        # Software Setup
         configfile += "[software]\n"
         if 'cmtpath' in self.options:
             configfile += "cmtpath = " + self.options['cmtpath'] + "\n"
 
         if 'cmtroot' in self.options:
             configfile += "cmtroot = " + self.options['cmtroot'] + "\n"
 
         configfile += "nd280ver = " + self.options['nd280ver'] + "\n\n"
 
-        ### Module list
+        # Module list
         configfile += "[configuration]\n"
         if self.options['stage'] != 'base':
             if self.options['nd280ver'][0] == 'v':
                 configfile += "module_list = oaRecon oaAnalysis\n"
             else:
                 configfile += "module_list = eventRecon eventAnalysis\n"
 
-            configfile += "inputfile = " +  self.options['inputfile'] + "\n\n"
+            configfile += "inputfile = " + self.options['inputfile'] + "\n\n"
 
         else:
             if self.options['nd280ver'][0] == 'v':
                 configfile += "module_list = " + self.options['module_list_cmt'] + "\n\n"
             else:
                 configfile += "module_list = " + self.options['module_list_git'] + "\n\n"
 
-        ### File naming
-        if not  self.options['comment']:
-             self.options['comment'] =  self.options['nd280ver']
+        # File naming
+        if not self.options['comment']:
+            self.options['comment'] = self.options['nd280ver']
         configfile += "[filenaming]\n"
         configfile += "run_number = " + self.options['run_number'] + "\n"
         configfile += "subrun = " + self.options['subrun'] + "\n"
         configfile += "replace_comment = " + self.options['replace_comment'] + "\n"
         configfile += "comment = " + self.options['stage'] + "cosmiccorsika5F\n\n"
 
-
-        ### Geometry
+        # Geometry
         configfile += "[geometry]\n"
         configfile += "baseline = " + self.options['baseline'] + "\n"
-        configfile += "p0d_water_fill = " + self.options['p0d_water_fill'] + "\n\n"
+        configfile += "p0d_water_fill = " + self.options['p0d_water_fill'] + "\n"
+        if self.options['magnet_ecal_production6']:
+            configfile += 'magnet_ecal_production6 = ' \
+                + self.options['magnet_ecal_production6'] + "\n"
+
+        configfile += "\n"
 
-        ### nd280mc
+        # nd280mc
         configfile += "[nd280mc]\n"
         configfile += "mc_type = " + self.options['mc_type'] + "\n"
-        configfile += "random_seed = " + str(random.randint(1,999999999)) + "\n"
+        configfile += "random_seed = " + str(random.randint(1, 999999999)) + "\n"
         configfile += "num_events = " + self.options['num_events'] + "\n"
         configfile += "mc_full_spill = " + self.options['mc_full_spill'] + "\n"
         configfile += "mc_position = " + self.options['mc_position'] + "\n\n"
 
-        ### Cosmic
+        # Cosmic
         configfile += "[cosmics]\n"
         configfile += "kinfile = " + self.options['kinfile'] + "\n"
         configfile += "randomize_kinfile = " + self.options['randomize_kinfile'] + "\n\n"
 
-        ### Electronics
+        # Electronics
         configfile += "[electronics]\n"
-        configfile += "random_seed = " + str(random.randint(1,999999999)) + "\n\n"
+        configfile += "random_seed = " + str(random.randint(1, 999999999)) + "\n\n"
 
-         ### Calibrate
+        # Calibrate
         configfile += "[calibrate]\n"
         configfile += "save_digits = " + self.options['save_digits'] + "\n\n"
 
-         ### Reconstruction
+        # Reconstruction
         configfile += "[reconstruction]\n"
-        if  self.options['stage'] != 'all':
+        if self.options['stage'] != 'all':
             configfile += "event_select = " + self.options['stage'] + "cosmic\n"
         else:
             configfile += "event_select = all\n"
 
         return configfile
 
-    ######################## Sand MC Processing Config file
+    # Sand MC Processing Config file
     def CreateSandMCCF(self):
 
         if not self.CheckOptions():
             logger.error('Please make sure all options stated above are entered')
             return ''
 
-        if not self.options['stage'] in ['neutMC','g4anal','neutSetup']:
-            logger.error('"stage" options should be one of',['neutMC','g4anal','neutSetup'])
+        if not self.options['stage'] in ['neutMC', 'g4anal', 'neutSetup']:
+            logger.error('"stage" options should be one of', ['neutMC', 'g4anal', 'neutSetup'])
             return ''
 
         configfile = ''
         configfile += "# Automatically generated config file\n\n"
 
-
-        ### Software Setup
+        # Software Setup
         configfile += "[software]\n"
         configfile += "neut_setup_script = " + self.options['neut_setup_script'] + "\n\n"
 
-        ### Module list
+        # Module list
         configfile += "[configuration]\n"
         if self.options['stage'] == 'g4anal':
             if self.options['nd280ver'][0] == 'v':
                 configfile += "module_list = sandPropagate nd280MC elecSim oaCalibMC  oaRecon oaAnalysis\n"
             else:
-                configfile += "module_list = sandPropagate nd280Geant4Sim detResponseSim eventCalibMC  eventRecon eventAnalysis\n"
+                configfile += ("module_list = sandPropagate nd280Geant4Sim detResponseSim eventCalibMC  "
+                               "eventRecon eventAnalysis\n")
 
-            configfile += "inputfile = " +  self.options['inputfile'] + "\n\n"
+            configfile += "inputfile = " + self.options['inputfile'] + "\n\n"
         else:
             configfile += "module_list = neutMC\n\n"
 
-        ### File naming
-        if not  self.options['comment']:
-             self.options['comment'] =  self.options['nd280ver']
+        # File naming
+        if not self.options['comment']:
+            self.options['comment'] = self.options['nd280ver']
         configfile += "[filenaming]\n"
 
         thisrun = 90007000
         if self.options['generator'] == "old-neut":
             thisrun += 2000000
         if self.options['generator'] == "anti-neut":
             thisrun = 80007000
-        if self.options['generator'] == "genie" :
+        if self.options['generator'] == "genie":
             thisrun += 1000000
 
         if self.options['beam'] == "beamc":
             thisrun += 300000
         else:
             logger.error("self.beam = " + self.beam + " is not supported!!!")
             return ''
 
-        if self.options['p0d_water_fill']: # water
+        if self.options['p0d_water_fill']:  # water
             thisrun += 10000
 
-        configfile += "run_number = %d\n" % (thisrun+int(self.options['run_number']))
+        configfile += "run_number = %d\n" % (thisrun + int(self.options['run_number']))
         configfile += "subrun = " + self.options['subrun'] + "\n"
         configfile += "comment = " + self.options['comment'] + "\n\n"
 
-
-        ### Geometry
+        # Geometry
         configfile += "[geometry]\n"
         configfile += "baseline = " + self.options['baseline'] + "\n"
-        configfile += "p0d_water_fill = " + self.options['p0d_water_fill'] + "\n\n"
+        configfile += "p0d_water_fill = " + self.options['p0d_water_fill'] + "\n"
+        if self.options['magnet_ecal_production6']:
+            configfile += 'magnet_ecal_production6 = ' \
+                + self.options['magnet_ecal_production6'] + "\n"
+
+        configfile += "\n"
 
-        ### Neutrino
+        # Neutrino
         configfile += "[neutrino]\n"
         configfile += "neut_card = " + self.options['neut_card'] + "\n"
         configfile += "flux_file = " + self.options['flux_file'] + "\n"
         configfile += "maxint_file = " + self.options['maxint_file'] + "\n"
 
         configfile += "pot = " + self.options['pot'] + "\n"
-        #configfile += "num_events = 5000\n" # DVtmp
+        # configfile += "num_events = 5000\n" # DVtmp
         configfile += "neutrino_type = " + self.options['neutrino_type'] + "\n"
         configfile += "flux_region = " + self.options['flux_region'] + "\n"
         configfile += "master_volume = " + self.options['master_volume'] + "\n"
         configfile += "force_volume_name = " + self.options['force_volume_name'] + "\n"
         configfile += "random_start = " + self.options['random_start'] + "\n"
-        configfile += "random_seed = " + str(random.randint(1,999999999)) + "\n"
-        configfile += "neut_seed1 = "  + str(random.randint(1,999999999)) + "\n"
-        configfile += "neut_seed2 = "  + str(random.randint(1,999999999)) + "\n"
-        configfile += "neut_seed3 = "  + str(random.randint(1,999999999)) + "\n\n"
+        configfile += "random_seed = " + str(random.randint(1, 999999999)) + "\n"
+        configfile += "neut_seed1 = " + str(random.randint(1, 999999999)) + "\n"
+        configfile += "neut_seed2 = " + str(random.randint(1, 999999999)) + "\n"
+        configfile += "neut_seed3 = " + str(random.randint(1, 999999999)) + "\n\n"
 
-        ### Dead channels
+        # Dead channels
         configfile += "[dead_channels]\n"
         configfile += "tpc_periods_to_activate = " + self.options['tpc_periods_to_activate'] + "\n"
         configfile += "ecal_periods_to_activate = " + self.options['ecal_periods_to_activate'] + "\n\n"
 
-        ### Sand propagate
+        # Sand propagate
         configfile += "[sandPropagate]\n"
         configfile += "num_events = " + self.options['num_events'] + "\n\n"
 
-        ### nd280mc
+        # nd280mc
         configfile += "[nd280mc]\n"
         configfile += "num_events = " + self.options['num_events'] + "\n"
         configfile += "mc_type = " + self.options['mc_type'] + "\n"
         configfile += "nbunches = " + self.options['nbunches'] + "\n"
 
         configfile += "interactions_per_spill = " + self.options['interactions_per_spill'] + "\n"
         configfile += "pot_per_spill = " + self.options['pot_per_spill'] + "\n"
         configfile += "bunch_duration = " + self.options['bunch_duration'] + "\n"
         configfile += "mc_full_spill = " + self.options['mc_full_spill'] + "\n"
         configfile += "time_offset = " + self.options['time_offset'] + "\n"
         configfile += "count_type = " + self.options['count_type'] + "\n"
         configfile += "mc_position = " + self.options['mc_position'] + "\n"
-        configfile += "random_seed = " + str(random.randint(1,999999999)) + "\n\n"
+        configfile += "random_seed = " + str(random.randint(1, 999999999)) + "\n\n"
 
-        ### Electronics
+        # Electronics
         configfile += "[electronics]\n"
-        configfile += "random_seed = " + str(random.randint(1,999999999)) + "\n\n"
+        configfile += "random_seed = " + str(random.randint(1, 999999999)) + "\n\n"
 
-        ### Analysis
+        # Analysis
         configfile += "[analysis]\n"
-        configfile += "production = " +  self.options['production'] + "\n"
-        configfile += "save_geometry = " +  self.options['save_geometry'] + "\n"
+        configfile += "production = " + self.options['production'] + "\n"
+        configfile += "save_geometry = " + self.options['save_geometry'] + "\n"
 
         return configfile
 
     ########################################################################################################################
```

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/runND280.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/runND280.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/runND280CosMC.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/runND280CosMC.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/runND280CtrlSmpl.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/runND280Kin.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/runND280Kin.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/runND280RDP.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/runND280RDP.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Control/runND280SandMC.py` & `ganga-8.6.5/ganga/GangaND280/ND280Control/runND280SandMC.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Dataset/ND280Dataset.py` & `ganga-8.6.5/ganga/GangaND280/ND280Dataset/ND280Dataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Executable/ND280Executable.py` & `ganga-8.6.5/ganga/GangaND280/ND280Executable/ND280Executable.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py` & `ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/RecoPlusVFT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py` & `ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/VFT_make_ana.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py` & `ganga-8.6.5/ganga/GangaND280/ND280RecoValidation/oaReconPlusoaAnalysis.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py` & `ganga-8.6.5/ganga/GangaND280/ND280Skimmer/ND280Skimmer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280Splitter/ND280Splitter.py` & `ganga-8.6.5/ganga/GangaND280/ND280Splitter/ND280Splitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py` & `ganga-8.6.5/ganga/GangaND280/ND280TPCGasInteractions/TRExPlusOAAnalysis.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/PACKAGE.py` & `ganga-8.6.5/ganga/GangaND280/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/Tasks/ND280Task.py` & `ganga-8.6.5/ganga/GangaND280/Tasks/ND280Task.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/Tasks/ND280Transform.py` & `ganga-8.6.5/ganga/GangaND280/Tasks/ND280Transform.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py` & `ganga-8.6.5/ganga/GangaND280/Tasks/ND280Transform_CSVEvtList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/Tasks/ND280Unit.py` & `ganga-8.6.5/ganga/GangaND280/Tasks/ND280Unit.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py` & `ganga-8.6.5/ganga/GangaND280/Tasks/ND280Unit_CSVEvtList.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaND280/__init__.py` & `ganga-8.6.5/ganga/GangaND280/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.0` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.0`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.1` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.1`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.2` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.2`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.3` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.3`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.0.4` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.0.4`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.0` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.0`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.1` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.1`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.10` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.10`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.11` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.11`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.12` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.12`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.13` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.13`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.14` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.14`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.15` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.15`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.2` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.2`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.3` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.3`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.4` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.4`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.5` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.5`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.6` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.6`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.7` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.7`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.8` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.8`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-7.1.9` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-7.1.9`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.0` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.0`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.1` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.1`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.2` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.2`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.0.3` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.0.3`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.1.0` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.1.0`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.0` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.0`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.1` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.1`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.2` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.2`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.3` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.3`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.2.4` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.2.4`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.0` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.0`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.1` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.1`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.2` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.2`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/ReleaseNotes-8.3.3` & `ganga-8.6.5/ganga/GangaRelease/ReleaseNotes-8.3.3`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/tools/check-new-ganga.py` & `ganga-8.6.5/ganga/GangaRelease/tools/check-new-ganga.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh` & `ganga-8.6.5/ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaRelease/tools/ganga-cvmfs-install.sh` & `ganga-8.6.5/ganga/GangaRelease/tools/ganga-cvmfs-install.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/bin/bash
 
 cvmfs_server transaction ganga.cern.ch
 
-export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/cvmfs/sft.cern.ch/lcg/releases/LCG_100/Python/3.8.6/x86_64-centos7-gcc9-opt/lib
+export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/cvmfs/sft.cern.ch/lcg/releases/LCG_103/Python/3.9.12/x86_64-centos7-gcc11-opt/lib
 
 cd /cvmfs/ganga.cern.ch/Ganga/install
 
-/cvmfs/sft.cern.ch/lcg/releases/LCG_100/Python/3.8.6/x86_64-centos7-gcc9-opt/bin/python3 -m venv $1
+/cvmfs/sft.cern.ch/lcg/views/LCG_103/x86_64-centos7-gcc11-opt/bin/python -m venv $1
 
 . $1/bin/activate
 
 pip install --upgrade pip setuptools
 
 pip install git+https://github.com/ganga-devs/ganga.git@$1#egg=ganga[LHCb] 
 
 sed -i "23i\
-lib_string = '/cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc9-opt/lib64:/cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc9-opt/lib:/cvmfs/sft.cern.ch/lcg/releases/gcc/9.2.0-afc57/x86_64-centos7/lib:/cvmfs/sft.cern.ch/lcg/releases/gcc/9.2.0-afc57/x86_64-centos7/lib64'\n\
-sys.path.append('/cvmfs/sft.cern.ch/lcg/views/LCG_100/x86_64-centos7-gcc9-opt/lib/python3.8/site-packages')\n\
+lib_string = '/cvmfs/sft.cern.ch/lcg/views/LCG_103/x86_64-centos7-gcc11-opt/lib64:/cvmfs/sft.cern.ch/lcg/views/LCG_103/x86_64-centos7-gcc11-opt/lib:/cvmfs/sft.cern.ch/lcg/releases/gcc/11.3.0-ad0f5/x86_64-centos7/lib:/cvmfs/sft.cern.ch/lcg/releases/gcc/11.3.0-ad0f5/x86_64-centos7/lib64'\n\
+sys.path.append('/cvmfs/sft.cern.ch/lcg/views/LCG_103/x86_64-centos7-gcc11-opt/lib/python3.9/site-packages')\n\
 if not 'LD_LIBRARY_PATH' in os.environ.keys():\n\
     os.environ['LD_LIBRARY_PATH'] = lib_string\n\
     os.execv(sys.argv[0], sys.argv)\n\
 elif not lib_string in os.environ['LD_LIBRARY_PATH']:\n\
     os.environ['LD_LIBRARY_PATH'] += ':'+lib_string\n\
     os.execv(sys.argv[0], sys.argv)" $1/bin/ganga
```

### Comparing `ganga-8.6.4/ganga/GangaTest/BOOT.py` & `ganga-8.6.5/ganga/GangaTest/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/driver.py` & `ganga-8.6.5/ganga/GangaTest/Framework/driver.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/htmlizer.py` & `ganga-8.6.5/ganga/GangaTest/Framework/htmlizer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/loader.py` & `ganga-8.6.5/ganga/GangaTest/Framework/loader.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/runner.py` & `ganga-8.6.5/ganga/GangaTest/Framework/runner.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/tests.py` & `ganga-8.6.5/ganga/GangaTest/Framework/tests.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/utils.py` & `ganga-8.6.5/ganga/GangaTest/Framework/utils.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Framework/xmldifferencer.py` & `ganga-8.6.5/ganga/GangaTest/Framework/xmldifferencer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/CrashTest.py` & `ganga-8.6.5/ganga/GangaTest/Lib/CrashTest.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/GListApp/GListApp.py` & `ganga-8.6.5/ganga/GangaTest/Lib/GListApp/GListApp.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/StoreTestFramework.py` & `ganga-8.6.5/ganga/GangaTest/Lib/StoreTestFramework.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TFile/TFile.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TFile/TFile.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestApplication/TestApplication.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestApplication/TestApplication.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestApplication/TestDataset.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestApplication/TestDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestMonitoringService/TestMonitoringService.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestObjects.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestObjects.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestConfig2.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py` & `ganga-8.6.5/ganga/GangaTest/Lib/TestSubmitter/TestSubmitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTest/PACKAGE.py` & `ganga-8.6.5/ganga/GangaTest/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/BOOT.py` & `ganga-8.6.5/ganga/GangaTutorial/BOOT.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/Lib/PrimeFactorizer.py` & `ganga-8.6.5/ganga/GangaTutorial/Lib/PrimeFactorizer.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py` & `ganga-8.6.5/ganga/GangaTutorial/Lib/PrimeFactorizerSplitter.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/Lib/PrimeTableDataset.py` & `ganga-8.6.5/ganga/GangaTutorial/Lib/PrimeTableDataset.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/Lib/primes/prime_factor.py` & `ganga-8.6.5/ganga/GangaTutorial/Lib/primes/prime_factor.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/Lib/primes/primes.py` & `ganga-8.6.5/ganga/GangaTutorial/Lib/primes/primes.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/GangaTutorial/PACKAGE.py` & `ganga-8.6.5/ganga/GangaTutorial/PACKAGE.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga/ganga/__init__.py` & `ganga-8.6.5/ganga/ganga/__init__.py`

 * *Files identical despite different names*

### Comparing `ganga-8.6.4/ganga.egg-info/PKG-INFO` & `ganga-8.6.5/ganga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganga
-Version: 8.6.4
+Version: 8.6.5
 Summary: Job management tool
 Home-page: https://github.com/ganga-devs/ganga
 Author: Ganga Developers
 Author-email: project-ganga-developers@cern.ch
 License: GPL v2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ganga-8.6.4/ganga.egg-info/SOURCES.txt` & `ganga-8.6.5/ganga.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -824,15 +824,15 @@
 ganga/GangaRelease/ReleaseNotes-8.2.2
 ganga/GangaRelease/ReleaseNotes-8.2.3
 ganga/GangaRelease/ReleaseNotes-8.2.4
 ganga/GangaRelease/ReleaseNotes-8.3.0
 ganga/GangaRelease/ReleaseNotes-8.3.1
 ganga/GangaRelease/ReleaseNotes-8.3.2
 ganga/GangaRelease/ReleaseNotes-8.3.3
-ganga/GangaRelease/ReleaseNotes-8.6.4
+ganga/GangaRelease/ReleaseNotes-8.6.5
 ganga/GangaRelease/tools/check-new-ganga.py
 ganga/GangaRelease/tools/ganga-cvmfs-install-dev.sh
 ganga/GangaRelease/tools/ganga-cvmfs-install.sh
 ganga/GangaTest/BOOT.py
 ganga/GangaTest/PACKAGE.py
 ganga/GangaTest/__init__.py
 ganga/GangaTest/Framework/__init__.py
```

### Comparing `ganga-8.6.4/setup.py` & `ganga-8.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import Command
 import subprocess
 import os
 import sys
 
 file_path = os.path.dirname(os.path.realpath(__file__))
 
-_gangaVersion = '8.6.4'
+_gangaVersion = '8.6.5'
 
 def version():
     return _gangaVersion
 
 
 def readme():
     filename = os.path.abspath(os.path.join(file_path, 'README.rst'))
```

