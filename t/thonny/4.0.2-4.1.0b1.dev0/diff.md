# Comparing `tmp/thonny-4.0.2.tar.gz` & `tmp/thonny-4.1.0b1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-4.0.2.tar", last modified: Sat Jan 14 19:40:37 2023, max compression
+gzip compressed data, was "thonny-4.1.0b1.dev0.tar", last modified: Sat Apr 22 07:29:17 2023, max compression
```

## Comparing `thonny-4.0.2.tar` & `thonny-4.1.0b1.dev0.tar`

### file list

```diff
@@ -1,683 +1,703 @@
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.968244 thonny-4.0.2/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    74167 2023-01-14 19:36:51.000000 thonny-4.0.2/CHANGELOG.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4875 2023-01-07 08:26:22.000000 thonny-4.0.2/CREDITS.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1081 2023-01-14 19:35:19.000000 thonny-4.0.2/LICENSE.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      317 2022-08-15 15:16:42.000000 thonny-4.0.2/MANIFEST.in
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1650 2023-01-14 19:40:37.968244 thonny-4.0.2/PKG-INFO
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      742 2022-08-15 15:16:42.000000 thonny-4.0.2/README.rst
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.900244 thonny-4.0.2/licenses/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    11347 2022-08-15 15:16:42.000000 thonny-4.0.2/licenses/ECLIPSE-ICONS-LICENSE.txt
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.888244 thonny-4.0.2/packaging/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.900244 thonny-4.0.2/packaging/icons/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1591 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-128x128.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      214 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-16x16.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3077 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-192x192.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      324 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-2.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      542 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-22x22.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3823 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-256x256.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      624 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-32x32.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      914 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-48x48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      933 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/icons/thonny-64x64.png
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.904244 thonny-4.0.2/packaging/linux/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3099 2022-09-11 13:29:37.000000 thonny-4.0.2/packaging/linux/org.thonny.Thonny.appdata.xml
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      339 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/linux/org.thonny.Thonny.desktop
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      976 2022-08-15 15:16:42.000000 thonny-4.0.2/packaging/linux/thonny.1
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      305 2022-08-15 15:16:42.000000 thonny-4.0.2/pyproject.toml
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      180 2022-08-18 04:24:24.000000 thonny-4.0.2/requirements.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       38 2023-01-14 19:40:37.968244 thonny-4.0.2/setup.cfg
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3407 2023-01-07 08:26:22.000000 thonny-4.0.2/setup.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)        5 2023-01-14 19:36:36.000000 thonny-4.0.2/thonny/VERSION
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    16330 2022-10-07 18:12:57.000000 thonny-4.0.2/thonny/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       78 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/__main__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    34913 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/assistance.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6202 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/ast_utils.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    32932 2022-09-11 04:35:27.000000 thonny-4.0.2/thonny/backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    53672 2022-10-14 06:30:41.000000 thonny-4.0.2/thonny/base_file_browser.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    21847 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/codeview.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    23396 2022-10-14 06:30:41.000000 thonny-4.0.2/thonny/common.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6423 2022-09-10 18:15:45.000000 thonny-4.0.2/thonny/config.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5700 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/config_ui.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      335 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/defaults.ini
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    12742 2022-08-17 17:37:21.000000 thonny-4.0.2/thonny/editor_helpers.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    42737 2022-10-18 19:34:51.000000 thonny-4.0.2/thonny/editors.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1554 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/export.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3503 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/first_run.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     9415 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/gridtable.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     9899 2022-08-18 04:22:13.000000 thonny-4.0.2/thonny/jedi_utils.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2411 2023-01-14 19:35:19.000000 thonny-4.0.2/thonny/languages.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/ar_AR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/ar_AR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    37201 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    55586 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ar_AR/LC_MESSAGES/thonny.po
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       77 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/compile_mo.bat
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/cs_CZ/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/cs_CZ/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    28884 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    52358 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/de_DE/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/de_DE/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    35927 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/de_DE/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    58829 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/de_DE/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/el_GR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/el_GR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    45499 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/el_GR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    64554 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/el_GR/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/en_US/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/en_US/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      471 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/en_US/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    29903 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/en_US/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/es_ES/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4610 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5448 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/debugging.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2156 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/errors.rst
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny/locale/es_ES/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    35880 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/es_ES/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    56087 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/es_ES/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/et_EE/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/et_EE/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    33577 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/et_EE/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    53876 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/et_EE/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/fa_IR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/fa_IR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    38874 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    57261 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fa_IR/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/fi_FI/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/fi_FI/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    27028 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    51530 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/fi_FI/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/fr_FR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1739 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4885 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5999 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1272 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/dock.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2364 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/errors.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1558 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/flask.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      781 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/index.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1009 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/modes.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2955 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/packages.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2556 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1293 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4026 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/shell.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      646 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/fr_FR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    34584 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    56604 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/fr_FR/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/hu_HU/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/hu_HU/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    29029 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    52830 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/hu_HU/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/hy_AM/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/hy_AM/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    41398 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    59817 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/hy_AM/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/it_IT/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.912244 thonny-4.0.2/thonny/locale/it_IT/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    29164 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/it_IT/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    52783 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/it_IT/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/ja_JP/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.916244 thonny-4.0.2/thonny/locale/ja_JP/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    39069 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    59722 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/ja_JP/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/ko_KR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.916244 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1744 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4901 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6151 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1292 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/dock.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2503 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/errors.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2108 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/flask.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      886 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/index.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1142 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/modes.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2719 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/packages.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2482 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1245 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4213 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/shell.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      646 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.916244 thonny-4.0.2/thonny/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    29558 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    51805 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ko_KR/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/lt_LT/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.916244 thonny-4.0.2/thonny/locale/lt_LT/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    26421 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    40681 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/lt_LT/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/nb_NO/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.916244 thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6043 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2084 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/errors.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      754 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/index.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3988 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/shell.rst
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.916244 thonny-4.0.2/thonny/locale/nb_NO/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    23574 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    49831 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/nb_NO/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/nl_NL/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/nl_NL/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    27734 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    48672 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/nl_NL/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/nn_NO/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/nn_NO/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    21613 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    49202 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/nn_NO/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/pl_PL/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/pl_PL/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    28441 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    52478 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/pl_PL/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/pt_BR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    35547 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    55866 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/pt_BR/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/pt_PT/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/pt_PT/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    26955 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    40981 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/pt_PT/LC_MESSAGES/thonny.po
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1513 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/register_updates.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/ro_RO/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/ro_RO/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    32776 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    51239 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ro_RO/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.892244 thonny-4.0.2/thonny/locale/ru_RU/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/ru_RU/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    46239 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    66723 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/ru_RU/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/sk_SK/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/sk_SK/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    34201 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    55163 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/sk_SK/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/sl_SI/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/sl_SI/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    33078 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    54237 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/sl_SI/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/sq_AL/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/sq_AL/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    34380 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    54032 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/sq_AL/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/sv_SE/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.920244 thonny-4.0.2/thonny/locale/sv_SE/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     9758 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    33357 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/sv_SE/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/ta_IN/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/ta_IN/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    61109 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    80796 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/ta_IN/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/th_TH/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/th_TH/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    50299 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/th_TH/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    69932 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/th_TH/LC_MESSAGES/thonny.po
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    41047 2022-09-11 13:31:36.000000 thonny-4.0.2/thonny/locale/thonny.pot
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/tr_TR/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    26908 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    41183 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/tr_TR/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/uk_UA/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/uk_UA/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    34630 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    48861 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/uk_UA/LC_MESSAGES/thonny.po
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      108 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/locale/update_pot.bat
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/vi_VN/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/vi_VN/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    35515 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    57308 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/vi_VN/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/zh_CN/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    31548 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    54185 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/locale/zh_CN/LC_MESSAGES/thonny.po
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.896244 thonny-4.0.2/thonny/locale/zh_TW/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.924244 thonny-4.0.2/thonny/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    32353 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    52653 2022-09-11 13:42:12.000000 thonny-4.0.2/thonny/locale/zh_TW/LC_MESSAGES/thonny.po
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4244 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/memory.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    17132 2023-01-09 10:14:19.000000 thonny-4.0.2/thonny/misc_utils.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.932244 thonny-4.0.2/thonny/plugins/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       17 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5208 2022-08-28 04:32:54.000000 thonny-4.0.2/thonny/plugins/about.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2652 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/assistant_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     7503 2022-09-09 10:03:27.000000 thonny-4.0.2/thonny/plugins/ast_view.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    18561 2022-08-17 17:16:04.000000 thonny-4.0.2/thonny/plugins/autocomplete.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.932244 thonny-4.0.2/thonny/plugins/backend/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       17 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1494 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend/birdseye_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2145 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend/dock_user_windows_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1762 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend/flask_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1117 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend/matplotlib_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2802 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend/pgzero_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    11572 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/backend_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    19598 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/base_syntax_themes.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    23891 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/base_ui_themes.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2483 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/birdseye_frontend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5647 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/calltip.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6277 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cells.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.932244 thonny-4.0.2/thonny/plugins/circuitpython/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      396 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/circuitpython/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4215 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/circuitpython/cirpy_back.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3699 2022-08-21 12:11:24.000000 thonny-4.0.2/thonny/plugins/circuitpython/cirpy_front.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    14107 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/clean_ui_themes.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    12566 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/coloring.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5562 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/commenting_indenting.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2683 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/common_editing_commands.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.932244 thonny-4.0.2/thonny/plugins/cpython_backend/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      226 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_backend/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    48944 2022-10-30 19:26:04.000000 thonny-4.0.2/thonny/plugins/cpython_backend/cp_back.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1484 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_backend/cp_launcher.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    57899 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_backend/cp_tracers.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.932244 thonny-4.0.2/thonny/plugins/cpython_frontend/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      920 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_frontend/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    17745 2022-09-10 18:15:45.000000 thonny-4.0.2/thonny/plugins/cpython_frontend/cp_front.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1926 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_frontend/cp_pip_gui.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.932244 thonny-4.0.2/thonny/plugins/cpython_ssh/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      808 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_ssh/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     7070 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_ssh/cps_back.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5401 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_ssh/cps_front.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      361 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/cpython_ssh/cps_pip_gui.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    49639 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/plugins/debugger.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      812 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/dock_user_windows_frontend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3703 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/editor_config_page.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.936244 thonny-4.0.2/thonny/plugins/esp/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    13291 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/esp/__init__.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.936244 thonny-4.0.2/thonny/plugins/esp/esp32_api_stubs/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    18158 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/esp/esp32_api_stubs/esp32.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      555 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      743 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/esp/esp_back.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.936244 thonny-4.0.2/thonny/plugins/ev3/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4254 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/ev3/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      701 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/ev3/ev3_back.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6623 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/event_logging.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1535 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/event_view.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    20730 2022-10-30 19:17:09.000000 thonny-4.0.2/thonny/plugins/files.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    18119 2023-01-07 09:04:16.000000 thonny-4.0.2/thonny/plugins/find_replace.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5383 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/general_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4520 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/goto_definition.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2987 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/heap.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.936244 thonny-4.0.2/thonny/plugins/help/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2508 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1365 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/assistant.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1403 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/birdseye.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4006 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/debuggers.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5114 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/debugging.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1132 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/dock.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1969 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/errors.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1760 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/flask.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      677 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/index.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      878 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/modes.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2646 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/packages.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2183 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/plotter.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1041 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/program_arguments.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3643 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/shell.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      569 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/help/turtle.rst
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4105 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/highlight_names.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4178 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/locals_marker.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.936244 thonny-4.0.2/thonny/plugins/microbit/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6674 2022-08-21 12:11:24.000000 thonny-4.0.2/thonny/plugins/microbit/__init__.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.940244 thonny-4.0.2/thonny/plugins/microbit/api_stubs/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       20 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/antigravity.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      184 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/array.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1299 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/audio.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5665 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/builtins.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      402 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/collections.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      186 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/gc.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       68 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/love.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      204 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/machine.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      617 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/math.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    33816 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/microbit.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      218 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/micropython.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     8815 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/music.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3287 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/neopixel.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      916 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/os.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6453 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/radio.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1486 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/random.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1676 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/speech.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       66 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/struct.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4365 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/sys.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       85 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/this.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      187 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/time.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     7935 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/uarray.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      402 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/ucollections.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2138 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/ustruct.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     9148 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/api_stubs/utime.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      635 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/microbit/microbit_back.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.940244 thonny-4.0.2/thonny/plugins/micropython/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1882 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    63203 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/bare_metal_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6269 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      345 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/miniterm_wrapper.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    50760 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/plugins/micropython/mp_back.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       88 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/mp_common.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    36253 2023-01-14 19:35:19.000000 thonny-4.0.2/thonny/plugins/micropython/mp_front.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    13082 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/os_mp_backend.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4819 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/pip_gui.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6517 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/serial_connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1621 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/ssh_connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1862 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/subprocess_connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    23704 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/plugins/micropython/uf2dialog.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4562 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/micropython/webrepl_connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6308 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/misc_analyzers.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.940244 thonny-4.0.2/thonny/plugins/mypy/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4134 2022-10-07 18:04:54.000000 thonny-4.0.2/thonny/plugins/mypy/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2102 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/notes.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    26583 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/object_inspector.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5194 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/outline.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     8058 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/paren_matcher.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      734 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pgzero_frontend.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.940244 thonny-4.0.2/thonny/plugins/pi/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    12210 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/__init__.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.948244 thonny-4.0.2/thonny/plugins/pi/res/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      206 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/Ukraine.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      328 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/Ukraine48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1525 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run-cursor.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1525 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      668 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1012 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      590 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-into.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      894 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-into48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      586 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-out.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      882 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-out48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      577 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-over.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      861 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-over48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      403 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-new.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      530 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-new48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      731 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-open.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1221 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-open48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      691 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-save.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1082 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-save48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1146 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_media-playback-start.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1806 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_media-playback-start48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      993 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_process-stop.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1476 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_process-stop48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1082 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_quit.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1741 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_quit48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1133 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_resume.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1763 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_resume48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      177 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-down-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      208 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-down.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      160 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-left-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      207 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-left.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      173 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-right-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      202 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-right.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      175 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-up-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      187 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_scrollbar-button-up.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      633 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_window-close-act.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      423 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_window-close.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1488 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_zoom.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2349 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/_disabled_zoom48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1589 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-run-cursor.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1589 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-run-cursor48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      746 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-run.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1150 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-run48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      659 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-step-into.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      980 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-step-into48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      644 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-step-out.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      976 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-step-out48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      637 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-step-over.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      962 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/debug-step-over48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      445 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/document-new.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      611 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/document-new48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      800 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/document-open.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1354 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/document-open48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      770 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/document-save.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1223 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/document-save48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1337 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/media-playback-start.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2072 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/media-playback-start48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1139 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/process-stop.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1663 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/process-stop48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1207 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/quit.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1988 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/quit48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1258 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/resume.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1977 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/resume48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2866 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-down-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2857 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-down.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2857 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-left-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2834 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-left.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2865 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-right-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2858 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-right.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2859 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-up-insens.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2862 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-up.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    16273 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/window-close-act.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      505 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/window-close.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1513 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/zoom.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2561 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pi/res/zoom48.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    55551 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/plugins/pip_gui.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/prime_inventor/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1832 2022-08-22 16:15:29.000000 thonny-4.0.2/thonny/plugins/prime_inventor/__init__.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/prime_inventor/api_stubs/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    19398 2022-08-21 11:09:27.000000 thonny-4.0.2/thonny/plugins/prime_inventor/api_stubs/hub.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      663 2022-08-21 12:21:17.000000 thonny-4.0.2/thonny/plugins/prime_inventor/prime_inventor_back.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/printing/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2778 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/printing/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1382 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/printing/template.html
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/pylint/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6186 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pylint/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)   155507 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pylint/messages.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1131 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/pythontutor.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1514 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/remove_old_data_dir.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    13492 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/replayer.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/rp2040/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1605 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/rp2040/__init__.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/rp2040/api_stubs/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      344 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/rp2040/api_stubs/mp-1.18-pico.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     9549 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/rp2040/api_stubs/rp2.pyi
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      646 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/rp2040/rp2040_back.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/rpi_pico/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2003 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/rpi_pico/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2679 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/run_debug_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2564 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/shell_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3498 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/shell_macro.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     8452 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/statement_boxes.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    25884 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/stdlib_error_helpers.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.952244 thonny-4.0.2/thonny/plugins/system_shell/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2183 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/system_shell/__init__.py
--rwxrwxr-x   0 annamaa   (1000) annamaa   (1000)     5369 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/system_shell/explain_environment.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1375 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/terminal_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     9268 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/theme_and_font_config_page.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      763 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/thonny_folders.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4599 2022-08-16 15:07:41.000000 thonny-4.0.2/thonny/plugins/todo_view.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6327 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/tomorrow_syntax_theme.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5411 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/plugins/variables.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.968244 thonny-4.0.2/thonny/res/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      832 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/16x16-blank.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      807 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/1x1-white.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      270 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/PrintLnkTarget.vbs
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      171 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/Ukraine.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5430 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/Ukraine_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      682 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_create_disabled_variants.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      832 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_16x16-blank.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      807 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_1x1-white.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      837 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_arrow-down.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      734 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_birdseye.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      199 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxdot.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      169 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxdot_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      192 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxminus.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      160 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxminus_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      212 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxplus.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      176 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxplus_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      224 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxx.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      179 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_boxx_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      908 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_broken.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      917 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_closed-folder.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      577 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_debug-current-script.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1320 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_debug-current-script_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      877 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_delete.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      907 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_folder.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      881 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_generic-file.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      895 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_hard-drive.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      553 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_harddisk.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1177 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_harddisk_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      745 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_help.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1897 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_help_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      654 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_information.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1555 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_information_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      428 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_nav-backward.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      756 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_nav-backward_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      420 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_nav-forward.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      749 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_nav-forward_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      320 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_new-file.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      376 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_new-file_Linux.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      868 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_new-file_Linux_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      502 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_open-file.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      495 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_open-file_Linux.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1217 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_open-file_Linux_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      935 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_open_folder.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      613 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_outline-class.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1324 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_outline-class_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      928 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_outline-method.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      929 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_python-file.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      945 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_python-icon.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      461 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_quit.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      780 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_quit_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      469 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_resume.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      885 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_resume_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      620 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_run-current-script.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1281 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_run-current-script_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      339 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_run-to-cursor.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      612 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_run-to-cursor_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      460 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_save-file.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      944 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_save-file_2x_alt.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      604 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_save-file_Linux.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1611 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_save-file_Linux_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      518 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_save-file_alt.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      615 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_star.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1489 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_star_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      421 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_step-into.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      760 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_step-into_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      404 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_step-out.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      726 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_step-out_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      530 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_step-over.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1034 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_step-over_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      630 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_stop.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1888 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_stop_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      837 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_tab-close-active-clam-dark.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      837 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_tab-close-active-clam.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      837 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_tab-close-active.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      842 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_tab-close-clam.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      842 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_tab-close.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      511 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_terminal.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1255 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_terminal_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      934 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_text-file.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5186 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_thonny.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      469 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/_disabled_zoom.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      837 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/arrow-down.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1225 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/birdseye.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      282 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxdot.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      258 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxdot_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      272 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxminus.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1170 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxminus_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      288 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxplus.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1179 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxplus_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      312 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxx.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      264 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/boxx_light.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1535 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/broken.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1111 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/closed-folder.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      563 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/debug-current-script.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1453 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/debug-current-script_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      900 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/delete.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      386 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/folder.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      238 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/generic-file.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1019 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/hard-drive.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      847 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/harddisk.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1519 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/harddisk_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      932 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/help.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2231 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/help_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      863 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/information.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1910 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/information_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      347 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/nav-backward.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      652 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/nav-backward_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      344 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/nav-forward.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      644 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/nav-forward_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      299 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/new-file.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      477 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/new-file_Linux.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1008 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/new-file_Linux_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      567 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/open-file.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      672 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/open-file_Linux.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1550 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/open-file_Linux_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1108 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/open_folder.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      628 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/outline-class.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1129 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/outline-class_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      578 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/outline-method.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      626 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/python-file.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1049 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/python-icon.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2430 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/python-icon_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      561 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/quit.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      984 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/quit_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      539 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/resume.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1046 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/resume_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      620 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/run-current-script.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1226 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/run-current-script_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      252 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/run-to-cursor.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      492 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/run-to-cursor_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      543 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/save-file.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1151 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/save-file_2x_alt.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      911 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/save-file_Linux.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1971 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/save-file_Linux_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      617 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/save-file_alt.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      950 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/star.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1800 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/star_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      356 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/step-into.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      761 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/step-into_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      379 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/step-out.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      798 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/step-out_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      457 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/step-over.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1014 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/step-over_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      718 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/stop.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3595 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/stop_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       58 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/tab-close-active-clam-dark.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       58 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/tab-close-active-clam.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       58 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/tab-close-active.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      842 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/tab-close-clam.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      842 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/tab-close.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      668 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/terminal.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1488 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/terminal_2x.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      627 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/text-file.gif
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    16652 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/thonny.ico
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     5134 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/thonny.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      894 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/thonny_small.ico
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      468 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/res/zoom.png
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    33753 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/roughparse.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    17498 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/rst_utils.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    56073 2023-01-14 19:35:19.000000 thonny-4.0.2/thonny/running.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    80012 2023-01-14 19:35:19.000000 thonny-4.0.2/thonny/shell.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     8048 2022-12-30 12:56:52.000000 thonny-4.0.2/thonny/terminal.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.968244 thonny-4.0.2/thonny/test/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       17 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/test/__init__.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.968244 thonny-4.0.2/thonny/test/plugins/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       17 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/test/plugins/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      599 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/test/plugins/test_locals_marker.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     3360 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/test/plugins/test_name_highlighter.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      336 2022-09-09 11:18:06.000000 thonny-4.0.2/thonny/test/plugins/test_pip_gui.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1173 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/test/test_common.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    45327 2022-09-10 09:29:26.000000 thonny-4.0.2/thonny/tktextext.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2262 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/token_utils.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    83012 2023-01-07 08:54:47.000000 thonny-4.0.2/thonny/ui_utils.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.900244 thonny-4.0.2/thonny/vendored_libs/
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.968244 thonny-4.0.2/thonny/vendored_libs/filelock/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1315 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/filelock/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     8896 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/filelock/_api.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      399 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/filelock/_error.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1650 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/filelock/_soft.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1578 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/filelock/_unix.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      594 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/filelock/_util.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1890 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/filelock/_windows.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)        0 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/filelock/py.typed
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      160 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/filelock/version.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.968244 thonny-4.0.2/thonny/vendored_libs/pipkin/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1738 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/__init__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     2137 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/__main__.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    16912 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/adapters.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    33595 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/bare_metal.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      355 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/common.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6235 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    10546 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/parser.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    18969 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/proxy.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6599 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/serial_connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    27862 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/session.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     6702 2023-01-07 08:26:22.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/util.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     4580 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/vendored_libs/pipkin/webrepl_connection.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    98549 2022-10-14 06:30:41.000000 thonny-4.0.2/thonny/workbench.py
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    15323 2022-08-15 15:16:42.000000 thonny-4.0.2/thonny/workdlg.py
-drwxrwxr-x   0 annamaa   (1000) annamaa   (1000)        0 2023-01-14 19:40:37.908244 thonny-4.0.2/thonny.egg-info/
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)     1650 2023-01-14 19:40:37.000000 thonny-4.0.2/thonny.egg-info/PKG-INFO
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)    21029 2023-01-14 19:40:37.000000 thonny-4.0.2/thonny.egg-info/SOURCES.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)        1 2023-01-14 19:40:37.000000 thonny-4.0.2/thonny.egg-info/dependency_links.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)       38 2023-01-14 19:40:37.000000 thonny-4.0.2/thonny.egg-info/entry_points.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)      120 2023-01-14 19:40:37.000000 thonny-4.0.2/thonny.egg-info/requires.txt
--rw-rw-r--   0 annamaa   (1000) annamaa   (1000)        7 2023-01-14 19:40:37.000000 thonny-4.0.2/thonny.egg-info/top_level.txt
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.883777 thonny-4.1.0b1.dev0/
+-rw-r--r--   0 aivar      (501) staff       (20)    74167 2023-01-14 19:52:25.000000 thonny-4.1.0b1.dev0/CHANGELOG.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4974 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/CREDITS.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1081 2023-01-14 19:52:25.000000 thonny-4.1.0b1.dev0/LICENSE.txt
+-rw-r--r--   0 aivar      (501) staff       (20)      317 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/MANIFEST.in
+-rw-r--r--   0 aivar      (501) staff       (20)     1759 2023-04-22 07:29:17.883102 thonny-4.1.0b1.dev0/PKG-INFO
+-rw-r--r--   0 aivar      (501) staff       (20)      742 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/README.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.031992 thonny-4.1.0b1.dev0/licenses/
+-rw-r--r--   0 aivar      (501) staff       (20)    11347 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/licenses/ECLIPSE-ICONS-LICENSE.txt
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.942441 thonny-4.1.0b1.dev0/packaging/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.046904 thonny-4.1.0b1.dev0/packaging/icons/
+-rw-r--r--   0 aivar      (501) staff       (20)     1591 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-128x128.png
+-rw-r--r--   0 aivar      (501) staff       (20)      214 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-16x16.png
+-rw-r--r--   0 aivar      (501) staff       (20)     3077 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-192x192.png
+-rw-r--r--   0 aivar      (501) staff       (20)      324 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-2.png
+-rw-r--r--   0 aivar      (501) staff       (20)      542 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-22x22.png
+-rw-r--r--   0 aivar      (501) staff       (20)     3823 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-256x256.png
+-rw-r--r--   0 aivar      (501) staff       (20)      624 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-32x32.png
+-rw-r--r--   0 aivar      (501) staff       (20)      914 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-48x48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      933 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/icons/thonny-64x64.png
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.051037 thonny-4.1.0b1.dev0/packaging/linux/
+-rw-r--r--   0 aivar      (501) staff       (20)     3099 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.appdata.xml
+-rw-r--r--   0 aivar      (501) staff       (20)      339 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.desktop
+-rw-r--r--   0 aivar      (501) staff       (20)      976 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/packaging/linux/thonny.1
+-rw-r--r--   0 aivar      (501) staff       (20)      305 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/pyproject.toml
+-rw-r--r--   0 aivar      (501) staff       (20)      180 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/requirements.txt
+-rw-r--r--   0 aivar      (501) staff       (20)       38 2023-04-22 07:29:17.883965 thonny-4.1.0b1.dev0/setup.cfg
+-rw-r--r--   0 aivar      (501) staff       (20)     3517 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/setup.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.140302 thonny-4.1.0b1.dev0/thonny/
+-rw-r--r--   0 aivar      (501) staff       (20)       11 2023-04-22 07:29:07.000000 thonny-4.1.0b1.dev0/thonny/VERSION
+-rw-r--r--   0 aivar      (501) staff       (20)    16347 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)       78 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/__main__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    34909 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/assistance.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6202 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/ast_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)    33389 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)    53486 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/base_file_browser.py
+-rw-r--r--   0 aivar      (501) staff       (20)    21845 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/codeview.py
+-rw-r--r--   0 aivar      (501) staff       (20)    23478 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/common.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6423 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/config.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5700 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/config_ui.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.155650 thonny-4.1.0b1.dev0/thonny/dbus/
+-rw-r--r--   0 aivar      (501) staff       (20)      691 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/dbus/org.freedesktop.DBus.ObjectManager.xml
+-rw-r--r--   0 aivar      (501) staff       (20)    11220 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/dbus/org.freedesktop.UDisks2.xml
+-rw-r--r--   0 aivar      (501) staff       (20)      335 2020-11-02 17:21:06.000000 thonny-4.1.0b1.dev0/thonny/defaults.ini
+-rw-r--r--   0 aivar      (501) staff       (20)    12741 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/editor_helpers.py
+-rw-r--r--   0 aivar      (501) staff       (20)    42942 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/editors.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1554 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/export.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3503 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/first_run.py
+-rw-r--r--   0 aivar      (501) staff       (20)     9415 2020-09-03 11:18:16.000000 thonny-4.1.0b1.dev0/thonny/gridtable.py
+-rw-r--r--   0 aivar      (501) staff       (20)    10702 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/jedi_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2411 2023-01-14 19:52:25.000000 thonny-4.1.0b1.dev0/thonny/languages.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.163535 thonny-4.1.0b1.dev0/thonny/locale/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.946627 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.165002 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    37201 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    55586 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)       77 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/compile_mo.bat
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.947342 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.177380 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    28884 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52358 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.948052 thonny-4.1.0b1.dev0/thonny/locale/de_DE/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.180001 thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35927 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    58829 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.948567 thonny-4.1.0b1.dev0/thonny/locale/el_GR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.193640 thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    45499 2021-02-22 20:19:16.000000 thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    64554 2021-02-22 20:19:16.000000 thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.949041 thonny-4.1.0b1.dev0/thonny/locale/en_US/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.197870 thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)      471 2020-02-18 07:08:34.000000 thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    29903 2020-02-18 07:08:34.000000 thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.950076 thonny-4.1.0b1.dev0/thonny/locale/es_ES/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.210270 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     4610 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5448 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2156 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/errors.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.213051 thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35880 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    56087 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.951250 thonny-4.1.0b1.dev0/thonny/locale/et_EE/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.218666 thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    33577 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    53876 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.953802 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.222327 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    38874 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    57261 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.954704 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.224882 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    27028 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    51530 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.956207 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.240167 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     1739 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4885 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5999 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1272 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2364 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1558 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      781 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1009 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2955 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2556 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1293 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4026 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      646 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.243114 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34584 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    56604 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.957019 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.245907 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    29029 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52830 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.957700 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.247658 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    41398 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    59817 2021-01-06 13:30:09.000000 thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.958458 thonny-4.1.0b1.dev0/thonny/locale/it_IT/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.251834 thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    29164 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52783 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.959156 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.255297 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    39069 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    59722 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.960212 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.271644 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     1744 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4901 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     6151 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1292 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2503 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2108 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      886 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1142 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2719 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2482 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1245 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4213 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      646 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.275312 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    29558 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    51805 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.960874 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.278391 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    26421 2019-11-03 18:24:01.000000 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    40681 2021-01-14 21:04:27.000000 thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.962410 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.283596 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     6043 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2084 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      754 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     3988 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/shell.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.285107 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    23574 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    49831 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.963317 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.288007 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    27734 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    48672 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.963899 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.290718 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    21613 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    49202 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.964463 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.292611 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    28441 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52478 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.965430 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.310047 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/
+-rw-r--r--   0 aivar      (501) staff       (20)     1528 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/assistant.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1558 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4485 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5245 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1330 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2096 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2003 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      740 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      920 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2977 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2308 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1230 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4024 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      649 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/HELP_CONTENT/turtle.rst
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.312904 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35547 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    55866 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.966538 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.314839 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    26955 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    40981 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)     1512 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/locale/register_updates.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.967303 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.316738 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    32776 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    51239 2021-02-17 13:22:04.000000 thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.968158 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.320814 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    46239 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    66723 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.968792 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.324152 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34201 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    55163 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.970134 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.328139 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    33078 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    54237 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.973340 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.330738 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34380 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    54032 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.976378 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.332374 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)     9758 2020-07-06 19:08:58.000000 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    33357 2020-07-06 19:08:58.000000 thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.979226 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.333951 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    61109 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    80796 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.980766 thonny-4.1.0b1.dev0/thonny/locale/th_TH/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.339321 thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    50299 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    69932 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)    42558 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/locale/thonny.pot
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.981948 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.342940 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    26908 2019-11-18 18:57:56.000000 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    41183 2019-11-18 18:57:56.000000 thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.982927 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.347207 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    34630 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    48861 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)      108 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/locale/update_pot.bat
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.985003 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.349322 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    35515 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    57308 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.986907 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.351057 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    31548 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    54185 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.po
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:16.987942 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.354466 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 aivar      (501) staff       (20)    32353 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo
+-rw-r--r--   0 aivar      (501) staff       (20)    52653 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.po
+-rw-r--r--   0 aivar      (501) staff       (20)     4243 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/memory.py
+-rw-r--r--   0 aivar      (501) staff       (20)    17771 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/misc_utils.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.422508 thonny-4.1.0b1.dev0/thonny/plugins/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5075 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/about.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2652 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/assistant_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     7502 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/ast_view.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18878 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/autocomplete.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.430244 thonny-4.1.0b1.dev0/thonny/plugins/backend/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1494 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/birdseye_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2145 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/dock_user_windows_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1604 2023-04-22 07:29:07.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/flask_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1116 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/matplotlib_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2802 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend/pgzero_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)    11570 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/backend_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)    19598 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/base_syntax_themes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    23891 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/base_ui_themes.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2483 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/birdseye_frontend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5647 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/calltip.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6276 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/cells.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.432920 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/
+-rw-r--r--   0 aivar      (501) staff       (20)      396 2023-01-05 10:46:57.000000 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4461 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4238 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)    14106 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/clean_ui_themes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    12566 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/coloring.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5561 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/commenting_indenting.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2683 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/common_editing_commands.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.437427 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/
+-rw-r--r--   0 aivar      (501) staff       (20)      226 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    51717 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1883 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_launcher.py
+-rw-r--r--   0 aivar      (501) staff       (20)    57896 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_tracers.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.444018 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/
+-rw-r--r--   0 aivar      (501) staff       (20)      920 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18540 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1926 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_pip_gui.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.449771 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/
+-rw-r--r--   0 aivar      (501) staff       (20)      808 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     7613 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5685 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)      361 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_pip_gui.py
+-rw-r--r--   0 aivar      (501) staff       (20)    49636 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/debugger.py
+-rw-r--r--   0 aivar      (501) staff       (20)      812 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/dock_user_windows_frontend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3703 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/editor_config_page.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.451084 thonny-4.1.0b1.dev0/thonny/plugins/esp/
+-rw-r--r--   0 aivar      (501) staff       (20)     2446 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.453171 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)    18158 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/esp32.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      555 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt
+-rw-r--r--   0 aivar      (501) staff       (20)      988 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/esp/esp_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.455284 thonny-4.1.0b1.dev0/thonny/plugins/ev3/
+-rw-r--r--   0 aivar      (501) staff       (20)     4254 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/ev3/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)      996 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/ev3/ev3_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6623 2021-07-25 16:05:48.000000 thonny-4.1.0b1.dev0/thonny/plugins/event_logging.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1535 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/event_view.py
+-rw-r--r--   0 aivar      (501) staff       (20)    20730 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/files.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18116 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/find_replace.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5383 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/general_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4520 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/goto_definition.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2987 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/plugins/heap.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.472442 thonny-4.1.0b1.dev0/thonny/plugins/help/
+-rw-r--r--   0 aivar      (501) staff       (20)     2508 2020-12-04 16:41:08.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1366 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/assistant.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1410 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/birdseye.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4009 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/debuggers.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     5114 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/debugging.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1131 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/dock.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1969 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/errors.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1764 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/flask.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      677 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/index.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      816 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/modes.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2633 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/packages.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     2183 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/plotter.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     1038 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/program_arguments.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     3650 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/shell.rst
+-rw-r--r--   0 aivar      (501) staff       (20)      569 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/help/turtle.rst
+-rw-r--r--   0 aivar      (501) staff       (20)     4104 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/highlight_names.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4178 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/locals_marker.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.475282 thonny-4.1.0b1.dev0/thonny/plugins/microbit/
+-rw-r--r--   0 aivar      (501) staff       (20)     7039 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.502717 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)       20 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/antigravity.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      184 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/array.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     1299 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/audio.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      402 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/collections.py
+-rw-r--r--   0 aivar      (501) staff       (20)      186 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/gc.py
+-rw-r--r--   0 aivar      (501) staff       (20)       68 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/love.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      204 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/machine.py
+-rw-r--r--   0 aivar      (501) staff       (20)      617 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/math.py
+-rw-r--r--   0 aivar      (501) staff       (20)    33816 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/microbit.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      218 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/micropython.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8815 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/music.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     3287 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/neopixel.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      916 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/os.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     6453 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/radio.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     1486 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/random.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     1676 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/speech.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)       66 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/struct.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     4365 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/sys.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)       85 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/this.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      187 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/time.py
+-rw-r--r--   0 aivar      (501) staff       (20)     7935 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/uarray.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      402 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/ucollections.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2138 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/ustruct.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)     9148 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/utime.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      880 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/microbit/microbit_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.525368 thonny-4.1.0b1.dev0/thonny/plugins/micropython/
+-rw-r--r--   0 aivar      (501) staff       (20)     1914 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    64546 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/bare_metal_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)    21237 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/base_flashing_dialog.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6269 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    20159 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/esptool_dialog.py
+-rw-r--r--   0 aivar      (501) staff       (20)      345 2020-11-02 17:21:06.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/miniterm_wrapper.py
+-rw-r--r--   0 aivar      (501) staff       (20)    52302 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_back.py
+-rw-r--r--   0 aivar      (501) staff       (20)       88 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_common.py
+-rw-r--r--   0 aivar      (501) staff       (20)    36776 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_front.py
+-rw-r--r--   0 aivar      (501) staff       (20)    13352 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/os_mp_backend.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4819 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/pip_gui.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6515 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/serial_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1621 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/ssh_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1862 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/subprocess_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     9964 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/uf2dialog.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4561 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/micropython/webrepl_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6307 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/misc_analyzers.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.526981 thonny-4.1.0b1.dev0/thonny/plugins/mypy/
+-rw-r--r--   0 aivar      (501) staff       (20)     4134 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/mypy/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2102 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/notes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    26582 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/object_inspector.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5194 2021-04-30 13:51:14.000000 thonny-4.1.0b1.dev0/thonny/plugins/outline.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8057 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/paren_matcher.py
+-rw-r--r--   0 aivar      (501) staff       (20)      734 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/pgzero_frontend.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.527966 thonny-4.1.0b1.dev0/thonny/plugins/pi/
+-rw-r--r--   0 aivar      (501) staff       (20)    12209 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.625185 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/
+-rw-r--r--   0 aivar      (501) staff       (20)      206 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/Ukraine.png
+-rw-r--r--   0 aivar      (501) staff       (20)      328 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/Ukraine48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1525 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1525 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      668 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1012 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      590 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      894 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      586 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      882 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      577 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)      861 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      403 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-new.png
+-rw-r--r--   0 aivar      (501) staff       (20)      530 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-new48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      731 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1221 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      691 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1082 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1146 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1806 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      993 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1476 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1082 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1741 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1133 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1763 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      177 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-down-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      208 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-down.png
+-rw-r--r--   0 aivar      (501) staff       (20)      160 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-left-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      207 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-left.png
+-rw-r--r--   0 aivar      (501) staff       (20)      173 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-right-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      202 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-right.png
+-rw-r--r--   0 aivar      (501) staff       (20)      175 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-up-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)      187 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_scrollbar-button-up.png
+-rw-r--r--   0 aivar      (501) staff       (20)      633 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_window-close-act.png
+-rw-r--r--   0 aivar      (501) staff       (20)      423 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_window-close.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1488 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2349 2019-12-06 15:56:03.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1589 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1589 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      746 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1150 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      659 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      980 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      644 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      976 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      637 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)      962 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      445 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-new.png
+-rw-r--r--   0 aivar      (501) staff       (20)      611 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-new48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      800 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1354 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open48.png
+-rw-r--r--   0 aivar      (501) staff       (20)      770 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1223 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1337 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2072 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1139 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1663 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1207 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1988 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1258 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1977 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume48.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2866 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2857 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2857 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2834 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2865 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2858 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2859 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up-insens.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2862 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up.png
+-rw-r--r--   0 aivar      (501) staff       (20)    16273 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/window-close-act.png
+-rw-r--r--   0 aivar      (501) staff       (20)      505 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/window-close.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1513 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2561 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom48.png
+-rw-r--r--   0 aivar      (501) staff       (20)    55548 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/pip_gui.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.626815 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/
+-rw-r--r--   0 aivar      (501) staff       (20)     1774 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.629023 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)    19398 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/api_stubs/hub.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      663 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/prime_inventor_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.631280 thonny-4.1.0b1.dev0/thonny/plugins/printing/
+-rw-r--r--   0 aivar      (501) staff       (20)     2778 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/printing/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1382 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/printing/template.html
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.633208 thonny-4.1.0b1.dev0/thonny/plugins/pylint/
+-rw-r--r--   0 aivar      (501) staff       (20)     6186 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pylint/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)   155507 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pylint/messages.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1131 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/pythontutor.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1514 2020-09-29 16:35:00.000000 thonny-4.1.0b1.dev0/thonny/plugins/remove_old_data_dir.py
+-rw-r--r--   0 aivar      (501) staff       (20)    13491 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/replayer.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.635136 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/
+-rw-r--r--   0 aivar      (501) staff       (20)     1692 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.641796 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/
+-rw-r--r--   0 aivar      (501) staff       (20)      344 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/mp-1.18-pico.txt
+-rw-r--r--   0 aivar      (501) staff       (20)     9549 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/rp2.pyi
+-rw-r--r--   0 aivar      (501) staff       (20)      891 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/rp2040/rp2040_back.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.643267 thonny-4.1.0b1.dev0/thonny/plugins/rpi_pico/
+-rw-r--r--   0 aivar      (501) staff       (20)     2003 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/rpi_pico/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3051 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/run_debug_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2564 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/shell_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3497 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/shell_macro.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8449 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/statement_boxes.py
+-rw-r--r--   0 aivar      (501) staff       (20)    25880 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/stdlib_error_helpers.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.647794 thonny-4.1.0b1.dev0/thonny/plugins/system_shell/
+-rw-r--r--   0 aivar      (501) staff       (20)     2183 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/system_shell/__init__.py
+-rwxr-xr-x   0 aivar      (501) staff       (20)     5377 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/plugins/system_shell/explain_environment.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1375 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/terminal_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)     9267 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/plugins/theme_and_font_config_page.py
+-rw-r--r--   0 aivar      (501) staff       (20)      763 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/plugins/thonny_folders.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4599 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/plugins/todo_view.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6327 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/tomorrow_syntax_theme.py
+-rw-r--r--   0 aivar      (501) staff       (20)     5411 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/plugins/variables.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.848070 thonny-4.1.0b1.dev0/thonny/res/
+-rw-r--r--   0 aivar      (501) staff       (20)      832 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/16x16-blank.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      807 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/1x1-white.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      270 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/PrintLnkTarget.vbs
+-rw-r--r--   0 aivar      (501) staff       (20)      171 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/Ukraine.png
+-rw-r--r--   0 aivar      (501) staff       (20)     5430 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/Ukraine_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      682 2020-09-02 21:27:22.000000 thonny-4.1.0b1.dev0/thonny/res/_create_disabled_variants.py
+-rw-r--r--   0 aivar      (501) staff       (20)      832 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_16x16-blank.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      807 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_1x1-white.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_arrow-down.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      734 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_birdseye.png
+-rw-r--r--   0 aivar      (501) staff       (20)      199 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxdot.png
+-rw-r--r--   0 aivar      (501) staff       (20)      169 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxdot_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      192 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxminus.png
+-rw-r--r--   0 aivar      (501) staff       (20)      160 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxminus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      212 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxplus.png
+-rw-r--r--   0 aivar      (501) staff       (20)      176 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxplus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      224 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxx.png
+-rw-r--r--   0 aivar      (501) staff       (20)      179 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_boxx_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      908 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_broken.png
+-rw-r--r--   0 aivar      (501) staff       (20)      917 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_closed-folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      577 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1320 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      877 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_delete.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      907 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      881 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_generic-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      895 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_hard-drive.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      553 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1177 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      745 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_help.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1897 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_help_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      654 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_information.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1555 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_information_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      428 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-backward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      756 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-backward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      420 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-forward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      749 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-forward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      320 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      376 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)      868 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      502 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      495 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1217 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      935 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_open_folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      613 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1324 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      928 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-method.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      929 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_python-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      945 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_python-icon.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      461 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)      780 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_quit_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      469 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)      885 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_resume_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      620 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1281 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      339 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-to-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)      612 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_run-to-cursor_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      460 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      944 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_2x_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      604 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1611 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      518 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      615 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_star.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1489 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_star_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      421 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      760 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-into_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      404 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      726 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-out_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      530 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1034 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      630 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1888 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_stop_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam-dark.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      511 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_terminal.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1255 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_terminal_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      934 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_text-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     5186 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_thonny.png
+-rw-r--r--   0 aivar      (501) staff       (20)      469 2019-12-06 15:52:43.000000 thonny-4.1.0b1.dev0/thonny/res/_disabled_zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)      837 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/arrow-down.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     1225 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/birdseye.png
+-rw-r--r--   0 aivar      (501) staff       (20)      282 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxdot.png
+-rw-r--r--   0 aivar      (501) staff       (20)      258 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxdot_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      272 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxminus.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1170 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxminus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      288 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxplus.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1179 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxplus_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)      312 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxx.png
+-rw-r--r--   0 aivar      (501) staff       (20)      264 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/boxx_light.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1535 2020-11-15 16:51:08.000000 thonny-4.1.0b1.dev0/thonny/res/broken.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1111 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/closed-folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      563 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/debug-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1453 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/debug-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      900 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/delete.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      386 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      238 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/generic-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     1019 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/hard-drive.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      847 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/harddisk.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1519 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/harddisk_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      932 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/help.png
+-rw-r--r--   0 aivar      (501) staff       (20)     2231 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/help_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      863 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/information.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1910 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/information_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      347 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-backward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      652 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-backward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      344 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-forward.png
+-rw-r--r--   0 aivar      (501) staff       (20)      644 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/nav-forward_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      299 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/new-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      477 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/new-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1008 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/new-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      567 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)      672 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1550 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1108 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/open_folder.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      628 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/outline-class.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1129 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/outline-class_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      578 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/outline-method.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      626 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/python-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     1049 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/python-icon.gif
+-rw-r--r--   0 aivar      (501) staff       (20)     2430 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/python-icon_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      561 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/quit.png
+-rw-r--r--   0 aivar      (501) staff       (20)      984 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/quit_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      539 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/resume.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1046 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/resume_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      620 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-current-script.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1226 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-current-script_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      252 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-to-cursor.png
+-rw-r--r--   0 aivar      (501) staff       (20)      492 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/run-to-cursor_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      543 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1151 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_2x_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      911 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_Linux.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1971 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_Linux_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      617 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/save-file_alt.png
+-rw-r--r--   0 aivar      (501) staff       (20)      950 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/star.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1800 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/star_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      356 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-into.png
+-rw-r--r--   0 aivar      (501) staff       (20)      761 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-into_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      379 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-out.png
+-rw-r--r--   0 aivar      (501) staff       (20)      798 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-out_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      457 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-over.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1014 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/step-over_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      718 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/stop.png
+-rw-r--r--   0 aivar      (501) staff       (20)     3595 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/res/stop_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)       58 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-active-clam-dark.gif
+-rw-r--r--   0 aivar      (501) staff       (20)       58 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-active-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)       58 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-active.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close-clam.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      842 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/tab-close.gif
+-rw-r--r--   0 aivar      (501) staff       (20)      668 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/terminal.png
+-rw-r--r--   0 aivar      (501) staff       (20)     1488 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/terminal_2x.png
+-rw-r--r--   0 aivar      (501) staff       (20)      627 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/text-file.gif
+-rw-r--r--   0 aivar      (501) staff       (20)    16652 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/thonny.ico
+-rw-r--r--   0 aivar      (501) staff       (20)     5134 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/thonny.png
+-rw-r--r--   0 aivar      (501) staff       (20)      894 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/thonny_small.ico
+-rw-r--r--   0 aivar      (501) staff       (20)      468 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/res/zoom.png
+-rw-r--r--   0 aivar      (501) staff       (20)    33753 2020-09-03 11:18:16.000000 thonny-4.1.0b1.dev0/thonny/roughparse.py
+-rw-r--r--   0 aivar      (501) staff       (20)    17497 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/rst_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)    57393 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/running.py
+-rw-r--r--   0 aivar      (501) staff       (20)    80009 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/shell.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8048 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/terminal.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.851479 thonny-4.1.0b1.dev0/thonny/test/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/test/__init__.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.856958 thonny-4.1.0b1.dev0/thonny/test/plugins/
+-rw-r--r--   0 aivar      (501) staff       (20)       17 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)      598 2023-02-15 20:40:24.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/test_locals_marker.py
+-rw-r--r--   0 aivar      (501) staff       (20)     3360 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/test_name_highlighter.py
+-rw-r--r--   0 aivar      (501) staff       (20)      336 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/test/plugins/test_pip_gui.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1173 2019-10-01 19:35:52.000000 thonny-4.1.0b1.dev0/thonny/test/test_common.py
+-rw-r--r--   0 aivar      (501) staff       (20)    45325 2023-02-15 20:47:32.000000 thonny-4.1.0b1.dev0/thonny/tktextext.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2262 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/token_utils.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4914 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/udisks.py
+-rw-r--r--   0 aivar      (501) staff       (20)    83339 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/ui_utils.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.014799 thonny-4.1.0b1.dev0/thonny/vendored_libs/
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.866424 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/
+-rw-r--r--   0 aivar      (501) staff       (20)     1315 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     8896 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_api.py
+-rw-r--r--   0 aivar      (501) staff       (20)      399 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_error.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1650 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_soft.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1578 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_unix.py
+-rw-r--r--   0 aivar      (501) staff       (20)      594 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_util.py
+-rw-r--r--   0 aivar      (501) staff       (20)     1890 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_windows.py
+-rw-r--r--   0 aivar      (501) staff       (20)        0 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/py.typed
+-rw-r--r--   0 aivar      (501) staff       (20)      160 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/version.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.882086 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/
+-rw-r--r--   0 aivar      (501) staff       (20)     1738 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__init__.py
+-rw-r--r--   0 aivar      (501) staff       (20)     2114 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__main__.py
+-rw-r--r--   0 aivar      (501) staff       (20)    16912 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/adapters.py
+-rw-r--r--   0 aivar      (501) staff       (20)    33595 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/bare_metal.py
+-rw-r--r--   0 aivar      (501) staff       (20)      355 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/common.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6235 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    10546 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/parser.py
+-rw-r--r--   0 aivar      (501) staff       (20)    18946 2023-04-15 09:35:35.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/proxy.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6599 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/serial_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    27862 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/session.py
+-rw-r--r--   0 aivar      (501) staff       (20)     6702 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/util.py
+-rw-r--r--   0 aivar      (501) staff       (20)     4580 2023-01-05 10:46:58.000000 thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/webrepl_connection.py
+-rw-r--r--   0 aivar      (501) staff       (20)    98557 2023-04-22 07:29:07.000000 thonny-4.1.0b1.dev0/thonny/workbench.py
+-rw-r--r--   0 aivar      (501) staff       (20)    16632 2023-03-26 18:51:25.000000 thonny-4.1.0b1.dev0/thonny/workdlg.py
+drwxr-xr-x   0 aivar      (501) staff       (20)        0 2023-04-22 07:29:17.151038 thonny-4.1.0b1.dev0/thonny.egg-info/
+-rw-r--r--   0 aivar      (501) staff       (20)     1759 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/PKG-INFO
+-rw-r--r--   0 aivar      (501) staff       (20)    21822 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/SOURCES.txt
+-rw-r--r--   0 aivar      (501) staff       (20)        1 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/dependency_links.txt
+-rw-r--r--   0 aivar      (501) staff       (20)       38 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/entry_points.txt
+-rw-r--r--   0 aivar      (501) staff       (20)      120 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/requires.txt
+-rw-r--r--   0 aivar      (501) staff       (20)        7 2023-04-22 07:29:16.000000 thonny-4.1.0b1.dev0/thonny.egg-info/top_level.txt
```

### Comparing `thonny-4.0.2/CHANGELOG.rst` & `thonny-4.1.0b1.dev0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/CREDITS.rst` & `thonny-4.1.0b1.dev0/CREDITS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 * send2trash (https://github.com/hsoft/send2trash) is used by the Files view.
 * certifi (https://pypi.python.org/pypi/certifi) provides SSL certs for bundled Python in Linux and Mac.
 * distro (https://pypi.python.org/pypi/distro) is optionally used for detecting Linux version in About dialog.
 * paramiko (https://pypi.org/project/paramiko) is optionally used for writing and running code on remote machines.
 * websockets (https://pypi.org/project/websockets) is optionally used for communicating with MicroPython devices over WebREPL.
 * Most icons are taken from Eclipse project (https://www.eclipse.org/, https://github.com/eclipse/eclipse.platform.debug/tree/master/org.eclipse.debug.ui/icons/full/, https://github.com/eclipse/eclipse.platform.ui/tree/master/bundles/org.eclipse.ui/icons/full/, https://github.com/eclipse/eclipse.jdt.ui/tree/master/org.eclipse.jdt.ui/icons/full/), on Linux, some are overridden by Tango icons (http://tango.freedesktop.org/)
 * POEditor (https://poeditor.com/) is used for managing translations of UI strings.
+* https://github.com/hlovatt/PyBoardTypeshed
 
 Source contributors, sponsors, advisors, translators and frequent bug-reporters
 -------------------------------------------------------------------------------
 * adzierzanowski
 * Aivar Annamaa
 * Albin
 * Alar Leemet
@@ -98,14 +99,15 @@
 * Ivanhercaz
 * Ivan.schamann
 * Илья Кругликов
 * Jarek Miszczak
 * Jens Diemer
 * jharris1993
 * Juan Falgueras
+* Juhan Oskar Hennoste (@FeldrinH)
 * Jonathan Campbell
 * Jordan Williams
 * jose1711
 * José Carlos García
 * Kaspar Papli
 * Kauri Raba
 * kr-g
@@ -130,14 +132,15 @@
 * Radim
 * Rene Lehtma
 * Rune Langøy
 * Saishen, Inc.
 * Sam Warmuth
 * Sami Almuhammady
 * sailslack
+* Scott Blackledge
 * segalion
 * Simon Gijsen
 * Simon Long
 * sourceperl
 * speedy-10
 * Stefan Rothe
 * Stewart Russell (@scruss)
```

### Comparing `thonny-4.0.2/LICENSE.txt` & `thonny-4.1.0b1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/PKG-INFO` & `thonny-4.1.0b1.dev0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny
-Version: 4.0.2
+Version: 4.1.0b1.dev0
 Summary: Python IDE for beginners
 Home-page: https://thonny.org
 Author: Aivar Annamaa and others
 Author-email: thonny@googlegroups.com
 License: MIT
 Project-URL: Source code, https://github.com/thonny/thonny
 Project-URL: Bug tracker, https://github.com/thonny/thonny/issues
@@ -28,14 +28,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Text Editors
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

### Comparing `thonny-4.0.2/README.rst` & `thonny-4.1.0b1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/licenses/ECLIPSE-ICONS-LICENSE.txt` & `thonny-4.1.0b1.dev0/licenses/ECLIPSE-ICONS-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-128x128.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-128x128.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-192x192.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-192x192.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-22x22.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-22x22.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-256x256.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-256x256.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-32x32.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-32x32.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-48x48.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-48x48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/icons/thonny-64x64.png` & `thonny-4.1.0b1.dev0/packaging/icons/thonny-64x64.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/linux/org.thonny.Thonny.appdata.xml` & `thonny-4.1.0b1.dev0/packaging/linux/org.thonny.Thonny.appdata.xml`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/packaging/linux/thonny.1` & `thonny-4.1.0b1.dev0/packaging/linux/thonny.1`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/setup.py` & `thonny-4.1.0b1.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     paths = []
     for (path, _, filenames) in os.walk(directory):
         for filename in filenames:
             if not filename.endswith(".pyc") and filename != "registered.json":
                 paths.append(os.path.join('..', path, filename))
     return paths
 
-if sys.version_info < (3, 6):
-    raise RuntimeError("Thonny requires Python 3.6 or later")
+if sys.version_info < (3, 8):
+    raise RuntimeError("Thonny requires Python 3.8 or later")
 
 setupdir = os.path.dirname(__file__)
 
 with open(os.path.join(setupdir, "thonny", "VERSION"), encoding="ASCII") as f:
     version = f.read().strip()
 
 requirements = []
@@ -51,14 +51,16 @@
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Education",
         "Topic :: Software Development",
         "Topic :: Software Development :: Debuggers",
         "Topic :: Text Editors",
     ],
     keywords="IDE education debugger",
     project_urls={
@@ -66,15 +68,15 @@
         "Bug tracker": "https://github.com/thonny/thonny/issues",
     },
     platforms=["Windows", "macOS", "Linux"],
     install_requires=requirements,
     python_requires=">=3.8",
     packages=find_packages(),
     package_data={
-        "": ["VERSION", "defaults.ini", "res/*"]
+        "": ["VERSION", "defaults.ini", "res/*", "dbus/*"]
             + recursive_files("thonny/locale")
             + recursive_files("thonny/vendored_libs"),
         "thonny.plugins.help": ["*.rst"],
         "thonny.plugins.pi": ["res/*.*"],
         "thonny.plugins.printing": ["*.html"],
         "thonny.plugins.micropython": ["api_stubs/*.*"],
         "thonny.plugins.circuitpython": ["api_stubs/*.*"],
```

### Comparing `thonny-4.0.2/thonny/__init__.py` & `thonny-4.1.0b1.dev0/thonny/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,15 @@
             arguments.append(argv[i])
 
         return arguments
 
 
 def _configure_logging(log_file, console_level=None):
     logFormatter = logging.Formatter(
-        "%(asctime)s.%(msecs)03d %(levelname)-7s %(name)s: %(message)s", "%H:%M:%S"
+        "%(asctime)s.%(msecs)03d [%(threadName)s] %(levelname)-7s %(name)s: %(message)s", "%H:%M:%S"
     )
 
     file_handler = logging.FileHandler(log_file, encoding="UTF-8", mode="w")
     file_handler.setFormatter(logFormatter)
 
     main_logger = logging.getLogger("thonny")
     contrib_logger = logging.getLogger("thonnycontrib")
```

### Comparing `thonny-4.0.2/thonny/assistance.py` & `thonny-4.1.0b1.dev0/thonny/assistance.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,14 @@
         self._accepted_warning_sets.clear()
         for wp in self._analyzer_instances:
             wp.cancel_analysis()
         self._analyzer_instances = []
         self.text.clear()
 
     def _start_program_analyses(self, main_file_path, main_file_source, imported_file_paths):
-
         for cls in _program_analyzer_classes:
             analyzer = cls(self._accept_warnings)
             if analyzer.is_enabled():
                 self._analyzer_instances.append(analyzer)
 
         if not self._analyzer_instances:
             return
@@ -283,15 +282,14 @@
 
         self._accepted_warning_sets.append(warnings)
         if len(self._accepted_warning_sets) == len(self._analyzer_instances):
             self._present_warnings()
             self._present_conclusion()
 
     def _present_conclusion(self):
-
         if not self.text.get("1.0", "end").strip():
             if self.main_file_path is not None and os.path.exists(self.main_file_path):
                 self._append_text("\n")
                 self.text.append_rst(
                     "The code in `%s <%s>`__ looks good.\n\n"
                     % (
                         os.path.basename(self.main_file_path),
@@ -398,15 +396,14 @@
     def _append_feedback_link(self):
         self._append_text("Was it helpful or confusing?\n", ("a", "feedback_link"))
 
     def _format_file_url(self, atts):
         return format_file_url(atts["filename"], atts.get("lineno"), atts.get("col_offset"))
 
     def _ask_feedback(self, event=None):
-
         all_snapshots = self._snapshots_per_main_file[self._current_snapshot["main_file_path"]]
 
         # TODO: select only snapshots which are not sent yet
         snapshots = all_snapshots
 
         ui_utils.show_dialog(FeedbackDialog(get_workbench(), self.main_file_path, snapshots))
 
@@ -440,15 +437,14 @@
 
     def get_suggestions(self) -> Iterable[Suggestion]:
         raise NotImplementedError()
 
 
 class ErrorHelper(Helper):
     def __init__(self, error_info):
-
         # TODO: don't repeat all this for all error helpers
         self.error_info = error_info
 
         self.last_frame = error_info["stack"][-1]
         self.last_frame_ast = None
         if self.last_frame.source:
             try:
```

### Comparing `thonny-4.0.2/thonny/ast_utils.py` & `thonny-4.1.0b1.dev0/thonny/ast_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/backend.py` & `thonny-4.1.0b1.dev0/thonny/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 import warnings
 from abc import ABC, abstractmethod
 from logging import getLogger
 from typing import Any, BinaryIO, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import thonny
 from thonny import report_time
-from thonny.common import BackendEvent  # TODO: try to get rid of this
-from thonny.common import (
+from thonny.common import (  # TODO: try to get rid of this
     IGNORED_FILES_AND_DIRS,
+    PROCESS_ACK,
+    BackendEvent,
     CommandToBackend,
     EOFCommand,
     ImmediateCommand,
     InlineCommand,
     InlineResponse,
     InputSubmission,
     MessageFromBackend,
     ToplevelCommand,
     ToplevelResponse,
     UserError,
+    is_local_path,
     parse_message,
     read_one_incoming_message_str,
     serialize_message,
     try_load_modules_with_frontend_sys_path,
     universal_dirname,
 )
 
@@ -349,21 +351,30 @@
 
     def _cmd_editor_autocomplete(self, cmd):
         logger.debug("Starting _cmd_editor_autocomplete")
         error = None
         try:
             from thonny import jedi_utils
 
+            sys_path = self._get_sys_path_for_analysis()
+
+            # add current dir for local files
+            """
+            if cmd.filename and is_local_path(cmd.filename):
+                sys_path.insert(0, os.getcwd())
+                logger.debug("editor autocomplete with %r", sys_path)
+            """
+
             with warnings.catch_warnings():
                 completions = jedi_utils.get_script_completions(
                     cmd.source,
                     cmd.row,
                     cmd.column,
                     cmd.filename,
-                    sys_path=self._get_sys_path_for_analysis(),
+                    sys_path=sys_path,
                 )
         except ImportError:
             completions = []
             error = "Could not import jedi"
 
         return dict(
             source=cmd.source,
@@ -584,15 +595,14 @@
         self,
         items: Iterable[Dict],
         ensure_dir_fun: Callable[[str], None],
         transfer_file_fun: Callable,
         cmd,
         target_path_class,
     ) -> List[str]:
-
         total_cost = 0
         for item in items:
             if item["kind"] == "file":
                 total_cost += item["size"] + self._get_file_fixed_cost()
             else:
                 total_cost += self._get_dir_transfer_cost()
 
@@ -795,14 +805,17 @@
         )
         stdin, stdout, _ = self._client.exec_command(
             cmd_line_str, bufsize=0, get_pty=True, environment=env
         )
 
         # stderr gets directed to stdout because of pty
         pid = stdout.readline().strip()
+        ack = stdout.readline().strip()
+        if ack != PROCESS_ACK:
+            raise RuntimeError(f"Got {ack!r} instead of expected {PROCESS_ACK!r}")
         channel = stdout.channel
 
         return RemoteProcess(self._client, channel, stdin, stdout, pid)
 
     def _handle_immediate_command(self, cmd: ImmediateCommand) -> None:
         if cmd.name == "kill":
             self._kill()
@@ -817,15 +830,14 @@
 
         self._proc.kill()
 
     def _interrupt(self):
         pass
 
     def _get_sftp(self, fresh: bool):
-
         if fresh and self._sftp is not None:
             self._sftp.close()
             self._sftp = None
 
         if self._sftp is None:
             import paramiko
 
@@ -920,15 +932,14 @@
     path: str, stat_mode_fun: Callable[[str], Optional[int]], mkdir_fun: Callable[[str], None]
 ) -> None:
     assert path.startswith("/")
     if path == "/":
         return
 
     for step in list(reversed(list(map(str, pathlib.PurePosixPath(path).parents)))) + [path]:
-
         if step != "/":
             mode = stat_mode_fun(step)
             if mode is None:
                 mkdir_fun(step)
             elif not stat.S_ISDIR(mode):
                 raise AssertionError("'%s' is file, not a directory" % step)
```

### Comparing `thonny-4.0.2/thonny/base_file_browser.py` & `thonny-4.1.0b1.dev0/thonny/base_file_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     CommonDialog,
     ask_one_from_choices,
     ask_string,
     create_string_var,
     ems_to_pixels,
     get_hyperlink_cursor,
     lookup_style_option,
+    open_with_default_app,
     scrollbar_style,
     show_dialog,
 )
 
 _dummy_node_text = "..."
 
 _LOCAL_FILES_ROOT_TEXT = ""  # needs to be initialized later
@@ -1570,22 +1571,13 @@
     if not _LOCAL_FILES_ROOT_TEXT:
         # translation can't be done in module load time
         _LOCAL_FILES_ROOT_TEXT = tr("This computer")
 
     return _LOCAL_FILES_ROOT_TEXT
 
 
-def open_with_default_app(path):
-    if running_on_windows():
-        os.startfile(path)
-    elif running_on_mac_os():
-        subprocess.run(["open", path])
-    else:
-        subprocess.run(["xdg-open", path])
-
-
 def get_file_handler_conf_key(extension):
     return "file_default_handlers.%s" % extension
 
 
 def show_hidden_files():
     return get_workbench().get_option(HIDDEN_FILES_OPTION)
```

### Comparing `thonny-4.0.2/thonny/codeview.py` & `thonny-4.1.0b1.dev0/thonny/codeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         self.configure(tabs=tabs, tabstyle="wordprocessor")
 
 
 class CodeViewText(EnhancedTextWithLogging, SyntaxText):
     """Provides opportunities for monkey-patching by plugins"""
 
     def __init__(self, master=None, cnf={}, **kw):
-
         super().__init__(
             master=master,
             tag_current_line=get_workbench().get_option("view.highlight_current_line"),
             cnf=cnf,
             **kw,
         )
         # Allow binding to events of all CodeView texts
@@ -229,15 +228,14 @@
         content = OLD_MAC_LINEBREAK.sub(self._original_newlines, content)
         content = WINDOWS_LINEBREAK.sub(self._original_newlines, content)
         content = UNIX_LINEBREAK.sub(self._original_newlines, content)
 
         return content.encode(self.detect_encoding(content.encode("ascii", errors="replace")))
 
     def set_content_as_bytes(self, data, keep_undo=False):
-
         encoding = self.detect_encoding(data)
         logger.debug("Detected encoding %s", encoding)
         while True:
             try:
                 chars = data.decode(encoding)
                 if self.looks_like_text(chars):
                     self.set_content(chars, keep_undo)
```

### Comparing `thonny-4.0.2/thonny/common.py` & `thonny-4.1.0b1.dev0/thonny/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 logger = getLogger(__name__)
 
 STRING_PSEUDO_FILENAME = "<string>"
 REPL_PSEUDO_FILENAME = "<stdin>"
 MESSAGE_MARKER = "\x02"
 OBJECT_LINK_START = "[object_link_for_thonny=%d]"
 OBJECT_LINK_END = "[/object_link_for_thonny]"
+REMOTE_PATH_MARKER = " :: "
+PROCESS_ACK = "OK"
 
 IGNORED_FILES_AND_DIRS = [
     "System Volume Information",
     "._.Trashes",
     ".Trashes",
     "__MACOSX",
     ".DS_Store",
@@ -438,14 +440,16 @@
     name: str
     name_with_symbols: str
     full_name: str
     type: str
     prefix_length: int  # the number of chars to be deleted before inserting name
     signatures: Optional[List[SignatureInfo]]
     docstring: Optional[str]
+    module_name: Optional[str]
+    module_path: Optional[str]
 
 
 @dataclass
 class NameReference:
     module_name: str
     module_path: str
     row: int
@@ -717,21 +721,19 @@
             return str(p.relative_to(context))
         except ValueError:
             return path
     else:
         return os.path.relpath(path, context)
 
 
-def get_python_version_string(version_info: Optional[Tuple] = None, maxsize=None):
-    result = ".".join(map(str, sys.version_info[:3]))
-    if sys.version_info[3] != "final":
-        result += "-" + sys.version_info[3]
+def get_python_version_string():
+    result = sys.version.split()[0]
 
-    if maxsize is not None:
-        result += " (" + ("64" if sys.maxsize > 2**32 else "32") + " bit)"
+    if sys.maxsize <= 2**32:
+        result += ", 32-bit"
 
     return result
 
 
 def execute_with_frontend_sys_path(function: Callable) -> Any:
     import ast
 
@@ -791,7 +793,15 @@
     )
 
 
 def is_private_python(executable):
     result = os.path.exists(os.path.join(os.path.dirname(executable), "thonny_python.ini"))
     logger.debug("is_private_python(%r) == %r", executable, result)
     return result
+
+
+def is_remote_path(s: str) -> bool:
+    return REMOTE_PATH_MARKER in s
+
+
+def is_local_path(s: str) -> bool:
+    return not is_remote_path(s) and not s.startswith("<")
```

### Comparing `thonny-4.0.2/thonny/config.py` & `thonny-4.1.0b1.dev0/thonny/config.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/config_ui.py` & `thonny-4.1.0b1.dev0/thonny/config_ui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/editor_helpers.py` & `thonny-4.1.0b1.dev0/thonny/editor_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,14 @@
         self._append_chars(")")
 
         if sig.return_type and not only_params:
             self._append_chars(" -> ", ["marker"])
             self._append_chars(sig.return_type, ["annotation"])
 
     def render_parameter(self, param: SignatureParameter, active: bool) -> None:
-
         if active:
             base_tags = ["active"]
         else:
             base_tags = []
 
         if param.kind == "VAR_POSITIONAL":
             self._append_chars("*", base_tags)
```

### Comparing `thonny-4.0.2/thonny/editors.py` & `thonny-4.1.0b1.dev0/thonny/editors.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 
 from _tkinter import TclError
 
 from thonny import get_runner, get_workbench, ui_utils
 from thonny.base_file_browser import ask_backend_path, choose_node_for_file_operations
 from thonny.codeview import BinaryFileException, CodeView, CodeViewText
 from thonny.common import (
+    REMOTE_PATH_MARKER,
     InlineCommand,
     TextRange,
     ToplevelResponse,
+    is_local_path,
+    is_remote_path,
     is_same_path,
     normpath_with_actual_case,
     universal_dirname,
 )
 from thonny.languages import tr
 from thonny.misc_utils import running_on_mac_os, running_on_windows
 from thonny.tktextext import rebind_control_a
@@ -31,26 +34,24 @@
     select_sequence,
     windows_known_extensions_are_hidden,
 )
 
 PYTHON_FILES_STR = tr("Python files")
 _dialog_filetypes = [(PYTHON_FILES_STR, ".py .pyw .pyi"), (tr("all files"), ".*")]
 
-REMOTE_PATH_MARKER = " :: "
 PYTHON_EXTENSIONS = {"py", "pyw", "pyi"}
 PYTHONLIKE_EXTENSIONS = set()
 
 logger = getLogger(__name__)
 
 
 class EditorCodeViewText(CodeViewText):
     """Allows separate class binding for CodeViewTexts which are inside editors"""
 
     def __init__(self, master=None, cnf={}, **kw):
-
         super().__init__(
             master=master,
             cnf=cnf,
             **kw,
         )
         self.bindtags(self.bindtags() + ("EditorCodeViewText",))
 
@@ -180,15 +181,14 @@
                     self.see_line(int(prev_location.split(".")[0]))
                 except Exception:
                     logger.exception("Could not restore previous location")
 
             self._last_known_mtime = os.path.getmtime(self._filename)
 
     def get_long_description(self):
-
         if self._filename is None:
             result = tr("<untitled>")
         else:
             result = self._filename
 
         try:
             index = self._code_view.text.index("insert")
@@ -206,23 +206,25 @@
                 result = self._load_remote_file(filename)
             else:
                 result = self._load_local_file(filename, keep_undo)
                 if not result:
                     return False
         except BinaryFileException:
             messagebox.showerror(
-                "Problem", "%s doesn't look like a text file" % filename, master=self
+                tr("Problem"), tr("%s doesn't look like a text file") % (filename,), master=self
             )
             return False
         except SyntaxError as e:
             assert "encoding" in str(e).lower()
             messagebox.showerror(
-                "Problem loading file",
-                "This file seems to have problems with encoding.\n\n"
-                + "Make sure it is in UTF-8 or contains proper encoding hint.",
+                tr("Problem loading file"),
+                tr(
+                    "This file seems to have problems with encoding.\n\n"
+                    "Make sure it is in UTF-8 or contains proper encoding hint."
+                ),
                 master=self,
             )
             return False
 
         self.update_appearance()
         return True
 
@@ -286,18 +288,20 @@
             save_filename = self.ask_new_path(node)
 
             if not save_filename:
                 return None
 
             if self.notebook.get_editor(save_filename) is not None:
                 messagebox.showerror(
-                    "File is open",
-                    "This file is already open in Thonny.\n\n"
-                    "If you want to save with this name,\n"
-                    "close the existing editor first!",
+                    tr("File is open"),
+                    tr(
+                        "This file is already open in Thonny.\n\n"
+                        "If you want to save with this name,\n"
+                        "close the existing editor first!"
+                    ),
                     master=get_workbench(),
                 )
                 return None
 
             get_workbench().event_generate(
                 "SaveAs", editor=self, filename=save_filename, save_copy=save_copy
             )
@@ -338,15 +342,17 @@
             if not save_copy or save_filename == self._filename:
                 self._last_known_mtime = os.path.getmtime(save_filename)
             get_workbench().event_generate(
                 "LocalFileOperation", path=save_filename, operation="save"
             )
         except PermissionError:
             messagebox.showerror(
-                "Permission Error", "Looks like this file or folder is not writable.", master=self
+                tr("Permission Error"),
+                tr("Looks like this file or folder is not writable."),
+                master=self,
             )
             return False
 
         if not save_copy or save_filename == self._filename:
             self.master.remember_recent_file(save_filename)
 
         if not save_copy or save_filename == self._filename:
@@ -401,20 +407,20 @@
             # NB! edit_modified is not falsed yet!
             get_workbench().event_generate(
                 "RemoteFileOperation", path=target_filename, operation="save"
             )
             get_workbench().event_generate("RemoteFilesChanged")
             return True
         else:
-            messagebox.showerror(tr("Could not save"), "Back-end is not ready")
+            messagebox.showerror(tr("Could not save"), tr("Back-end is not ready"))
             return False
 
     def ask_new_path(self, node=None):
         if node is None:
-            node = choose_node_for_file_operations(self.winfo_toplevel(), "Where to save to?")
+            node = choose_node_for_file_operations(self.winfo_toplevel(), tr("Where to save to?"))
         if not node:
             return None
 
         if node == "local":
             return self.ask_new_local_path()
         else:
             assert node == "remote"
@@ -475,22 +481,24 @@
                 "turtle",
                 "random",
                 "statistics",
                 "pygame",
                 "matplotlib",
                 "numpy",
             ]:
-
                 # More proper name analysis will be performed by ProgramNamingAnalyzer
                 if not tk.messagebox.askyesno(
-                    "Potential problem",
-                    "If you name your script '%s', " % base
-                    + "you won't be able to import the library module named '%s'" % mod_name
+                    tr("Potential problem"),
+                    tr(
+                        "If you name your script '%s', "
+                        "you won't be able to import the library module named '%s'"
+                    )
+                    % (base, mod_name)
                     + ".\n\n"
-                    + "Do you still want to use this name for your script?",
+                    + tr("Do you still want to use this name for your script?"),
                     master=self,
                 ):
                     return self.ask_new_local_path()
 
         return new_filename
 
     def show(self):
@@ -630,18 +638,18 @@
         get_workbench().bind("ToplevelResponse", self.check_for_external_changes, True)
         self.bind("<<NotebookTabChanged>>", self.on_tab_changed, True)
 
     def on_tab_changed(self, *args):
         if sys.platform == "darwin":
             # Since Tk 8.6.11, after closing an editor, the previous editor re-appeared with
             # widgets disappeared, at least on Aivar's machine.
-            child = self.get_current_child()
-            if child:
+            for child in self.get_all_editors():
                 assert isinstance(child, Editor)
                 child.get_code_view().grid_main_widgets()
+            self.update_idletasks()
 
     def _init_commands(self):
         # TODO: do these commands have to be in EditorNotebook ??
         # Create a module level function install_editor_notebook ??
         # Maybe add them separately, when notebook has been installed ??
 
         get_workbench().add_command(
@@ -892,15 +900,14 @@
 
     def _control_o(self, event):
         # http://stackoverflow.com/questions/22907200/remap-default-keybinding-in-tkinter
         self._cmd_open_file()
         return "break"
 
     def _close_files(self, except_index=None):
-
         for tab_index in reversed(range(len(self.winfo_children()))):
             if except_index is not None and tab_index == except_index:
                 continue
             else:
                 editor = self.get_child_by_index(tab_index)
                 if self.check_allow_closing(editor):
                     self.forget(editor)
@@ -1039,19 +1046,19 @@
 
     def show_file(self, filename, text_range=None, set_focus=True, propose_dialog=True):
         # self.close_single_untitled_unmodified_editor()
         try:
             editor = self.get_editor(filename, True)
         except PermissionError:
             logger.exception("Loading " + filename)
-            msg = "Got permission error when trying to load\n" + filename
+            msg = tr("Got permission error when trying to load\n%s") % (filename,)
             if running_on_mac_os() and propose_dialog:
-                msg += "\n\nTry opening it with File => Open."
+                msg += "\n\n" + tr("Try opening it with File => Open.")
 
-            messagebox.showerror("Permission error", msg, master=self)
+            messagebox.showerror(tr("Permission error"), msg, master=self)
             return None
 
         if editor is None:
             return
 
         self.select(editor)
         if set_focus:
@@ -1207,22 +1214,14 @@
 
     if editor.is_modified():
         filename = editor.save_file()
 
     return filename
 
 
-def is_remote_path(s):
-    return REMOTE_PATH_MARKER in s
-
-
-def is_local_path(s):
-    return not is_remote_path(s)
-
-
 def get_target_dirname_from_editor_filename(s):
     if is_local_path(s):
         return os.path.dirname(s)
     else:
         return universal_dirname(extract_target_path(s))
```

### Comparing `thonny-4.0.2/thonny/export.py` & `thonny-4.1.0b1.dev0/thonny/export.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/first_run.py` & `thonny-4.1.0b1.dev0/thonny/first_run.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/gridtable.py` & `thonny-4.1.0b1.dev0/thonny/gridtable.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/jedi_utils.py` & `thonny-4.1.0b1.dev0/thonny/jedi_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """
 Utils to handle different jedi versions
 """
+import os.path
 from logging import getLogger
 from typing import Dict, List, Optional
 
 import jedi.api.classes
 from jedi.api.classes import BaseSignature, ParamName
 
-from thonny.common import CompletionInfo, NameReference, SignatureInfo, SignatureParameter
+from thonny.common import (
+    CompletionInfo,
+    NameReference,
+    SignatureInfo,
+    SignatureParameter,
+    is_local_path,
+)
 
 logger = getLogger(__name__)
 
 _last_jedi_completions: Optional[List[jedi.api.classes.Completion]] = None
 
 
 def get_script_completions(
@@ -68,14 +75,16 @@
                     name=completion.name,
                     name_with_symbols=_get_completion_name_with_symbols(completion, signatures),
                     full_name=completion.full_name,
                     type=completion.type,
                     prefix_length=completion.get_completion_prefix_length(),
                     signatures=signatures,
                     docstring=completion.docstring(raw=raw_docstring),
+                    module_name=completion.module_name,
+                    module_path=completion.module_path and str(completion.module_path),
                 )
     except Exception:
         logger.exception("Jedi error")
 
     return None
 
 
@@ -144,44 +153,48 @@
     # some refs (e.g. in Jedi 0.16) may lack line and column
     references = [ref for ref in references if ref.line is not None and ref.column is not None]
 
     return [_export_reference(ref) for ref in references]
 
 
 def _create_script(source: str, filename: str, sys_path: List[str]) -> jedi.api.Script:
-    if sys_path:
-        project = jedi.Project(path=sys_path[0], sys_path=sys_path, smart_sys_path=False)
+    # Beside local scripts, this is also used for MicroPython remote scripts and also in MP shell
+    if filename and is_local_path(filename) or filename is None:
+        # local and unnamed files
+        project_path = os.getcwd()
+        smart_sys_path = True
     else:
-        project = None
+        # remote files and shell
+        project_path = None
+        smart_sys_path = False
+
+    project = jedi.Project(path=project_path, sys_path=sys_path, smart_sys_path=smart_sys_path)
 
     return jedi.Script(
         code=source,
         path=filename,
         project=project,
     )
 
 
 def _create_interpreter(
     source: str, namespaces: List[Dict], sys_path: Optional[List[str]]
 ) -> jedi.api.Interpreter:
-    if sys_path:
-        project = jedi.Project(path=sys_path[0], sys_path=sys_path, smart_sys_path=False)
-    else:
-        project = None
+    # not using this method for remote MicroPython, therefore it's OK to use cwd as project path
+    project = jedi.Project(path=os.getcwd(), sys_path=sys_path)
     return jedi.Interpreter(source, namespaces, project=project)
 
 
 def _export_completions(completions: List[jedi.api.classes.Completion]) -> List[CompletionInfo]:
     return [_export_completion(comp) for comp in completions]
 
 
 def _filter_completions(
     completions: List[jedi.api.classes.Completion], sys_path: Optional[List[str]]
 ) -> List[jedi.api.classes.Completion]:
-
     if sys_path is None:
         return completions
 
     result = []
     for completion in completions:
         if completion.name.startswith("__"):
             continue
@@ -189,24 +202,29 @@
         result.append(completion)
 
     return result
 
 
 def _export_completion(completion: jedi.api.classes.Completion) -> CompletionInfo:
     # In jedi before 0.16, the name attribute did not contain trailing '=' for argument completions,
-    # since 0.16 it does. Need to ensure similar result for all supported versions.
+    # since 0.16 it does.
+    # When older jedi versions were supported, I needed to ensure similar result for all supported
+    # versions.
+    # Also, for MicroPython there are some completions which are not created by jedi.
 
     return CompletionInfo(
         name=completion.name and completion.name.strip("="),
         name_with_symbols=_get_completion_name_with_symbols(completion),
         full_name=completion.full_name and completion.full_name.strip("="),
         type=completion.type,
         prefix_length=completion.get_completion_prefix_length(),
         signatures=None,  # must be queried separately
         docstring=None,  # must be queried separately
+        module_name=completion.module_name,
+        module_path=completion.module_path and str(completion.module_path),
     )
 
 
 def _export_signature(sig: BaseSignature) -> SignatureInfo:
     as_string = sig.to_string()
     if "->" in as_string:
         # No documented API for getting the return type in 0.18
```

### Comparing `thonny-4.0.2/thonny/languages.py` & `thonny-4.1.0b1.dev0/thonny/languages.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ar_AR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ar_AR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/cs_CZ/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/de_DE/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/de_DE/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/de_DE/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/el_GR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/el_GR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/el_GR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/en_US/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/en_US/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/es_ES/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/es_ES/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/es_ES/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/es_ES/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/et_EE/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/et_EE/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/et_EE/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fa_IR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/fa_IR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fi_FI/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/fi_FI/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/birdseye.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/dock.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/dock.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/flask.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/flask.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/modes.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/modes.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/packages.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/packages.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/program_arguments.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/HELP_CONTENT/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/fr_FR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/fr_FR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/hu_HU/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/hu_HU/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/hy_AM/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/hy_AM/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/it_IT/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/it_IT/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/it_IT/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ja_JP/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ja_JP/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/birdseye.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debuggers.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/dock.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/dock.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/flask.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/flask.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/modes.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/modes.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/packages.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/packages.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/program_arguments.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/HELP_CONTENT/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ko_KR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ko_KR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/lt_LT/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/lt_LT/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/errors.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/index.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nb_NO/HELP_CONTENT/shell.rst` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/HELP_CONTENT/shell.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nb_NO/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/nb_NO/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nl_NL/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/nl_NL/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/nn_NO/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/nn_NO/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/pl_PL/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/pl_PL/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/pt_BR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/pt_BR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/pt_PT/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/pt_PT/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/register_updates.py` & `thonny-4.1.0b1.dev0/thonny/locale/register_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
     review_messages = []
 
     for entry in po:
         if entry.msgstr and (
             entry.msgid not in registered or registered[entry.msgid] != entry.msgstr
         ):
-
             msg = entry.msgstr.strip().replace("\n", " ")
             if not msg.endswith("."):
                 msg = msg + "."
 
             review_messages.append(msg)
 
         if entry.msgstr:
```

### Comparing `thonny-4.0.2/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ro_RO/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ro_RO/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ru_RU/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ru_RU/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sk_SK/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sk_SK/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sl_SI/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sl_SI/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sq_AL/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sq_AL/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/sv_SE/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/sv_SE/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/ta_IN/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/ta_IN/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/th_TH/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/th_TH/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/th_TH/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/thonny.pot` & `thonny-4.1.0b1.dev0/thonny/locale/thonny.pot`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Translations template for PROJECT.
-# Copyright (C) 2022 ORGANIZATION
+# Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-09-11 16:31+0300\n"
+"POT-Creation-Date: 2023-03-14 22:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: thonny/assistance.py:985 thonny/plugins/assistant_config_page.py:74
+#: thonny/assistance.py:981 thonny/plugins/assistant_config_page.py:74
 msgid "Assistant"
 msgstr ""
 
 #: thonny/base_file_browser.py:91 thonny/memory.py:63
 msgid "Name"
 msgstr ""
 
@@ -111,25 +111,25 @@
 msgstr ""
 
 #: thonny/base_file_browser.py:721 thonny/base_file_browser.py:874
 msgid "New directory"
 msgstr ""
 
 #: thonny/base_file_browser.py:724 thonny/plugins/common_editing_commands.py:49
-#: thonny/ui_utils.py:2295
+#: thonny/ui_utils.py:2331
 msgid "Cut"
 msgstr ""
 
 #: thonny/base_file_browser.py:725 thonny/plugins/common_editing_commands.py:61
-#: thonny/ui_utils.py:2296
+#: thonny/ui_utils.py:2332
 msgid "Copy"
 msgstr ""
 
 #: thonny/base_file_browser.py:727 thonny/base_file_browser.py:733
-#: thonny/plugins/common_editing_commands.py:73 thonny/ui_utils.py:2297
+#: thonny/plugins/common_editing_commands.py:73 thonny/ui_utils.py:2333
 msgid "Paste"
 msgstr ""
 
 #: thonny/base_file_browser.py:736
 msgid "Rename"
 msgstr ""
 
@@ -220,15 +220,15 @@
 msgid "There are conflicting folders"
 msgstr ""
 
 #: thonny/base_file_browser.py:1140
 msgid "File already exists"
 msgstr ""
 
-#: thonny/base_file_browser.py:1205 thonny/plugins/pip_gui.py:1516
+#: thonny/base_file_browser.py:1205 thonny/plugins/pip_gui.py:1515
 msgid "Not supported"
 msgstr ""
 
 #: thonny/base_file_browser.py:1206
 msgid "Opening remote files in external app is not supported."
 msgstr ""
 
@@ -240,15 +240,15 @@
 
 #: thonny/base_file_browser.py:1213
 msgid ""
 "If the file needs to be opened in external app, then download it to a "
 "local directory and open it from there!"
 msgstr ""
 
-#: thonny/base_file_browser.py:1254 thonny/editors.py:979 thonny/editors.py:981
+#: thonny/base_file_browser.py:1254 thonny/editors.py:982 thonny/editors.py:984
 msgid "Deleting"
 msgstr ""
 
 #: thonny/base_file_browser.py:1261
 msgid "Creating directory"
 msgstr ""
 
@@ -263,28 +263,28 @@
 msgstr ""
 
 #: thonny/base_file_browser.py:1347
 msgid "File name:"
 msgstr ""
 
 #: thonny/base_file_browser.py:1369 thonny/config_ui.py:41 thonny/export.py:25
-#: thonny/plugins/about.py:111 thonny/plugins/backend_config_page.py:285
-#: thonny/ui_utils.py:154 thonny/ui_utils.py:1816 thonny/workdlg.py:206
+#: thonny/plugins/about.py:111 thonny/plugins/backend_config_page.py:283
+#: thonny/ui_utils.py:157 thonny/ui_utils.py:1817 thonny/workdlg.py:206
 msgid "OK"
 msgstr ""
 
 #: thonny/base_file_browser.py:1378 thonny/config_ui.py:42 thonny/export.py:28
-#: thonny/plugins/backend_config_page.py:290 thonny/plugins/pip_gui.py:1256
-#: thonny/ui_utils.py:157 thonny/ui_utils.py:1733 thonny/ui_utils.py:1819
+#: thonny/plugins/backend_config_page.py:288 thonny/plugins/pip_gui.py:1256
+#: thonny/ui_utils.py:160 thonny/ui_utils.py:1734 thonny/ui_utils.py:1820
 #: thonny/workdlg.py:164 thonny/workdlg.py:209
 msgid "Cancel"
 msgstr ""
 
 #: thonny/base_file_browser.py:1407 thonny/base_file_browser.py:1419
-#: thonny/plugins/autocomplete.py:300 thonny/plugins/highlight_names.py:87
+#: thonny/plugins/autocomplete.py:303 thonny/plugins/highlight_names.py:86
 msgid "Error"
 msgstr ""
 
 #: thonny/base_file_browser.py:1407 thonny/base_file_browser.py:1419
 msgid "You need to select a file!"
 msgstr ""
 
@@ -310,221 +310,299 @@
 msgstr ""
 
 #: thonny/editors.py:36 thonny/plugins/cpython_frontend/cp_front.py:270
 #: thonny/plugins/pip_gui.py:789 thonny/plugins/pip_gui.py:802
 msgid "all files"
 msgstr ""
 
-#: thonny/editors.py:122 thonny/editors.py:189
+#: thonny/editors.py:121 thonny/editors.py:187
 msgid "<untitled>"
 msgstr ""
 
-#: thonny/editors.py:149
+#: thonny/editors.py:148
 msgid "File is gone"
 msgstr ""
 
-#: thonny/editors.py:150
+#: thonny/editors.py:149
 #, python-format
 msgid "Looks like '%s' was deleted or moved."
 msgstr ""
 
-#: thonny/editors.py:152
+#: thonny/editors.py:151
 msgid "Do you want to also close the editor?"
 msgstr ""
 
-#: thonny/editors.py:168
+#: thonny/editors.py:167
 msgid "External modification"
 msgstr ""
 
-#: thonny/editors.py:169
+#: thonny/editors.py:168
 #, python-format
 msgid "Looks like '%s' was modified outside of the editor."
 msgstr ""
 
-#: thonny/editors.py:171
+#: thonny/editors.py:170
 msgid ""
 "Do you want to discard current editor content and reload the file from "
 "disk?"
 msgstr ""
 
+#: thonny/editors.py:211 thonny/plugins/goto_definition.py:58
+msgid "Problem"
+msgstr ""
+
+#: thonny/editors.py:212
+#, python-format
+msgid "%s doesn't look like a text file"
+msgstr ""
+
+#: thonny/editors.py:219
+msgid "Problem loading file"
+msgstr ""
+
+#: thonny/editors.py:220
+msgid ""
+"This file seems to have problems with encoding.\n"
+"\n"
+"Make sure it is in UTF-8 or contains proper encoding hint."
+msgstr ""
+
 #: thonny/editors.py:258
 #, python-format
 msgid "Loading %s"
 msgstr ""
 
 #: thonny/editors.py:260
 msgid "Loading"
 msgstr ""
 
-#: thonny/editors.py:384
+#: thonny/editors.py:293
+msgid "File is open"
+msgstr ""
+
+#: thonny/editors.py:294
+msgid ""
+"This file is already open in Thonny.\n"
+"\n"
+"If you want to save with this name,\n"
+"close the existing editor first!"
+msgstr ""
+
+#: thonny/editors.py:345
+msgid "Permission Error"
+msgstr ""
+
+#: thonny/editors.py:346
+msgid "Looks like this file or folder is not writable."
+msgstr ""
+
+#: thonny/editors.py:386
 #, python-format
 msgid "Saving to %s"
 msgstr ""
 
-#: thonny/editors.py:389
+#: thonny/editors.py:391
 msgid "Saving"
 msgstr ""
 
-#: thonny/editors.py:393 thonny/editors.py:408
+#: thonny/editors.py:395 thonny/editors.py:410
 msgid "Could not save"
 msgstr ""
 
-#: thonny/editors.py:579 thonny/plugins/micropython/pip_gui.py:23
-#: thonny/plugins/pip_gui.py:953
+#: thonny/editors.py:411
+msgid "Back-end is not ready"
+msgstr ""
+
+#: thonny/editors.py:417
+msgid "Where to save to?"
+msgstr ""
+
+#: thonny/editors.py:488
+msgid "Potential problem"
+msgstr ""
+
+#: thonny/editors.py:489
+#, python-format
+msgid ""
+"If you name your script '%s', you won't be able to import the library "
+"module named '%s'"
+msgstr ""
+
+#: thonny/editors.py:493
+msgid "Do you still want to use this name for your script?"
+msgstr ""
+
+#: thonny/editors.py:583 thonny/plugins/micropython/pip_gui.py:23
+#: thonny/plugins/pip_gui.py:952
 msgid "Confirmation"
 msgstr ""
 
-#: thonny/editors.py:580
+#: thonny/editors.py:584
 msgid "Python files usually have .py extension."
 msgstr ""
 
-#: thonny/editors.py:582
+#: thonny/editors.py:586
 #, python-format
 msgid "Did you mean '%s'?"
 msgstr ""
 
-#: thonny/editors.py:650 thonny/editors.py:652
+#: thonny/editors.py:654 thonny/editors.py:656
 msgid "New"
 msgstr ""
 
-#: thonny/editors.py:663
+#: thonny/editors.py:667
 msgid "Open..."
 msgstr ""
 
-#: thonny/editors.py:665
+#: thonny/editors.py:669
 msgid "Load"
 msgstr ""
 
-#: thonny/editors.py:674
+#: thonny/editors.py:678
 msgid "Recent files"
 msgstr ""
 
-#: thonny/editors.py:685 thonny/plugins/pip_gui.py:251 thonny/ui_utils.py:491
-#: thonny/ui_utils.py:1872 thonny/workdlg.py:162
+#: thonny/editors.py:689 thonny/plugins/pip_gui.py:251 thonny/ui_utils.py:494
+#: thonny/ui_utils.py:1873 thonny/workdlg.py:162
 msgid "Close"
 msgstr ""
 
-#: thonny/editors.py:696 thonny/ui_utils.py:493
+#: thonny/editors.py:700 thonny/ui_utils.py:496
 msgid "Close all"
 msgstr ""
 
-#: thonny/editors.py:706 thonny/editors.py:708
+#: thonny/editors.py:710 thonny/editors.py:712
 msgid "Save"
 msgstr ""
 
-#: thonny/editors.py:720 thonny/editors.py:722
+#: thonny/editors.py:724 thonny/editors.py:726
 msgid "Save All files"
 msgstr ""
 
-#: thonny/editors.py:731
+#: thonny/editors.py:735
 msgid "Save as..."
 msgstr ""
 
-#: thonny/editors.py:742
+#: thonny/editors.py:746
 msgid "Save copy..."
 msgstr ""
 
-#: thonny/editors.py:751
+#: thonny/editors.py:755
 msgid "Move / rename..."
 msgstr ""
 
-#: thonny/editors.py:760
+#: thonny/editors.py:764
 msgid "Go to line..."
 msgstr ""
 
-#: thonny/editors.py:1003
+#: thonny/editors.py:1006
 msgid "Go to line"
 msgstr ""
 
-#: thonny/editors.py:1003
+#: thonny/editors.py:1006
 msgid "Line number"
 msgstr ""
 
-#: thonny/editors.py:1149
+#: thonny/editors.py:1049
+#, python-format
+msgid ""
+"Got permission error when trying to load\n"
+"%s"
+msgstr ""
+
+#: thonny/editors.py:1051
+msgid "Try opening it with File => Open."
+msgstr ""
+
+#: thonny/editors.py:1053
+msgid "Permission error"
+msgstr ""
+
+#: thonny/editors.py:1152
 msgid "Do you want to save files before closing?"
 msgstr ""
 
-#: thonny/editors.py:1151
+#: thonny/editors.py:1154
 msgid "Do you want to save file before closing?"
 msgstr ""
 
-#: thonny/editors.py:1154
+#: thonny/editors.py:1157
 msgid "Save On Close"
 msgstr ""
 
-#: thonny/memory.py:64 thonny/plugins/object_inspector.py:539
-#: thonny/plugins/object_inspector.py:618
+#: thonny/memory.py:64 thonny/plugins/object_inspector.py:538
+#: thonny/plugins/object_inspector.py:617
 msgid "Value ID"
 msgstr ""
 
 #: thonny/memory.py:65 thonny/plugins/heap.py:23
-#: thonny/plugins/object_inspector.py:540
-#: thonny/plugins/object_inspector.py:619
+#: thonny/plugins/object_inspector.py:539
+#: thonny/plugins/object_inspector.py:618
 msgid "Value"
 msgstr ""
 
-#: thonny/misc_utils.py:151
+#: thonny/misc_utils.py:154
 #, python-format
 msgid "Could not find disk '%s'. Do you want to locate it yourself?"
 msgstr ""
 
-#: thonny/misc_utils.py:154
+#: thonny/misc_utils.py:157
 #, python-format
 msgid "Found several '%s' disks. Do you want to choose one yourself?"
 msgstr ""
 
-#: thonny/misc_utils.py:170
+#: thonny/misc_utils.py:173
 msgid "Can't find suitable disk"
 msgstr ""
 
-#: thonny/misc_utils.py:513
+#: thonny/misc_utils.py:516
 msgid "Command not available"
 msgstr ""
 
-#: thonny/misc_utils.py:514
+#: thonny/misc_utils.py:517
 msgid "This command is not available if Thonny is run via Flatpak"
 msgstr ""
 
-#: thonny/running.py:115
+#: thonny/running.py:124
 msgid "Run current script"
 msgstr ""
 
-#: thonny/running.py:116 thonny/workbench.py:372
+#: thonny/running.py:125 thonny/workbench.py:372
 msgid "Run"
 msgstr ""
 
-#: thonny/running.py:146
+#: thonny/running.py:155
 msgid "Run current script in terminal"
 msgstr ""
 
-#: thonny/running.py:159
+#: thonny/running.py:168
 msgid "Stop/Restart backend"
 msgstr ""
 
-#: thonny/running.py:160
+#: thonny/running.py:169
 msgid "Stop"
 msgstr ""
 
-#: thonny/running.py:171
+#: thonny/running.py:180
 msgid "Interrupt execution"
 msgstr ""
 
-#: thonny/running.py:184
+#: thonny/running.py:193
 msgid "Send EOF / Soft reboot"
 msgstr ""
 
-#: thonny/running.py:195
+#: thonny/running.py:204
 msgid "Disconnect"
 msgstr ""
 
-#: thonny/running.py:338
+#: thonny/running.py:356
 msgid "Information"
 msgstr ""
 
-#: thonny/running.py:339
+#: thonny/running.py:357
 msgid "For debugging the program must be saved first."
 msgstr ""
 
 #: thonny/shell.py:101
 msgid "Clear shell"
 msgstr ""
 
@@ -541,62 +619,62 @@
 msgid "Clear"
 msgstr ""
 
 #: thonny/shell.py:330
 msgid "Show Plotter"
 msgstr ""
 
-#: thonny/shell.py:1659
+#: thonny/shell.py:1660
 msgid ""
 "For performance reasons, Shell avoids showing very long lines in full "
 "(see Tools => Options => Shell).\n"
 "Here you can interact with the original text fragment."
 msgstr ""
 
-#: thonny/shell.py:1670
+#: thonny/shell.py:1671
 msgid "Wrap text (may be slow)"
 msgstr ""
 
-#: thonny/shell.py:1712
+#: thonny/shell.py:1713
 #, python-format
 msgid "Squeezed text (%d characters)"
 msgstr ""
 
-#: thonny/shell.py:1882
+#: thonny/shell.py:1883
 msgid ""
 "Plotter visualizes series of\n"
 "numbers printed to the Shell."
 msgstr ""
 
-#: thonny/shell.py:1884
+#: thonny/shell.py:1885
 msgid "See Help for details."
 msgstr ""
 
-#: thonny/ui_utils.py:492
+#: thonny/ui_utils.py:495
 msgid "Close others"
 msgstr ""
 
-#: thonny/ui_utils.py:1722
+#: thonny/ui_utils.py:1723
 msgid "Copying"
 msgstr ""
 
-#: thonny/ui_utils.py:1725
+#: thonny/ui_utils.py:1726
 #, python-format
 msgid ""
 "Copying\n"
 "  %s\n"
 "to\n"
 "  %s"
 msgstr ""
 
-#: thonny/ui_utils.py:1867
+#: thonny/ui_utils.py:1868
 msgid "Copy to clipboard"
 msgstr ""
 
-#: thonny/ui_utils.py:2301
+#: thonny/ui_utils.py:2337
 msgid "Select All"
 msgstr ""
 
 #: thonny/workbench.py:369
 msgid "File"
 msgstr ""
 
@@ -612,115 +690,115 @@
 msgid "Tools"
 msgstr ""
 
 #: thonny/plugins/help/__init__.py:80 thonny/workbench.py:374
 msgid "Help"
 msgstr ""
 
-#: thonny/workbench.py:591
+#: thonny/workbench.py:590
 msgid "Exit"
 msgstr ""
 
-#: thonny/workbench.py:601
+#: thonny/workbench.py:600
 msgid "Options..."
 msgstr ""
 
-#: thonny/workbench.py:608
+#: thonny/workbench.py:607
 msgid "Increase font size"
 msgstr ""
 
-#: thonny/workbench.py:618
+#: thonny/workbench.py:617
 msgid "Decrease font size"
 msgstr ""
 
-#: thonny/workbench.py:630
+#: thonny/workbench.py:629
 msgid "Focus editor"
 msgstr ""
 
-#: thonny/workbench.py:639
+#: thonny/workbench.py:638
 msgid "Focus shell"
 msgstr ""
 
-#: thonny/workbench.py:650
+#: thonny/workbench.py:648
 msgid "Maximize view"
 msgstr ""
 
-#: thonny/workbench.py:662
+#: thonny/workbench.py:660
 msgid "Full screen"
 msgstr ""
 
-#: thonny/workbench.py:673
+#: thonny/workbench.py:671
 msgid "Change font size"
 msgstr ""
 
-#: thonny/workbench.py:674
+#: thonny/workbench.py:672
 msgid "Zoom"
 msgstr ""
 
-#: thonny/workbench.py:683
+#: thonny/workbench.py:681
 msgid "Exit Thonny"
 msgstr ""
 
-#: thonny/workbench.py:686
+#: thonny/workbench.py:684
 msgid "Quit"
 msgstr ""
 
-#: thonny/workbench.py:694 thonny/workbench.py:794
+#: thonny/workbench.py:692 thonny/workbench.py:791
 msgid "Support Ukraine"
 msgstr ""
 
-#: thonny/workbench.py:697
+#: thonny/workbench.py:695
 msgid "Support"
 msgstr ""
 
-#: thonny/workbench.py:867
+#: thonny/workbench.py:863
 msgid "Install MicroPython"
 msgstr ""
 
-#: thonny/workbench.py:871
+#: thonny/workbench.py:867
 msgid "Install CircuitPython"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:340 thonny/workbench.py:877
+#: thonny/plugins/backend_config_page.py:338 thonny/workbench.py:873
 msgid "Configure interpreter..."
 msgstr ""
 
-#: thonny/workbench.py:1244 thonny/workbench.py:1252
+#: thonny/workbench.py:1240 thonny/workbench.py:1248
 #, python-format
 msgid "Overwriting theme '%s'"
 msgstr ""
 
-#: thonny/workbench.py:1436
+#: thonny/workbench.py:1431
 msgid "Program arguments:"
 msgstr ""
 
-#: thonny/workbench.py:1465
+#: thonny/workbench.py:1460
 msgid "Program arguments"
 msgstr ""
 
-#: thonny/workbench.py:1479
+#: thonny/workbench.py:1474
 msgid ""
 "Switch to\n"
 "regular\n"
 "mode"
 msgstr ""
 
-#: thonny/workbench.py:1490
+#: thonny/workbench.py:1485
 msgid "Regular mode"
 msgstr ""
 
-#: thonny/workbench.py:1491
+#: thonny/workbench.py:1486
 msgid ""
 "Configuration has been updated. Restart Thonny to start working in "
 "regular mode.\n"
 "\n"
 "(See 'Tools → Options → General' if you change your mind later.)"
 msgstr ""
 
-#: thonny/workbench.py:1589
+#: thonny/workbench.py:1584
 msgid "Device"
 msgstr ""
 
 #: thonny/workdlg.py:193
 msgid "Cancelling"
 msgstr ""
 
@@ -776,55 +854,55 @@
 msgid "Perform MyPy checks"
 msgstr ""
 
 #: thonny/plugins/assistant_config_page.py:36
 msgid "Disabled checks (one id per line)"
 msgstr ""
 
-#: thonny/plugins/ast_view.py:212
+#: thonny/plugins/ast_view.py:211
 msgid "Program tree"
 msgstr ""
 
-#: thonny/plugins/autocomplete.py:522
+#: thonny/plugins/autocomplete.py:524
 msgid "Auto-complete"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:91
+#: thonny/plugins/backend_config_page.py:90
 msgid "Which kind of interpreter should Thonny use for running your code?"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:110
+#: thonny/plugins/backend_config_page.py:109
 msgid "Details"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:212
+#: thonny/plugins/backend_config_page.py:210
 msgid "Make uploaded shebang scripts executable"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:251
+#: thonny/plugins/backend_config_page.py:249
 msgid "Authentication"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:253
+#: thonny/plugins/backend_config_page.py:251
 msgid ""
 "Enter the passphrase of your private key for\n"
 "{}"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:256
+#: thonny/plugins/backend_config_page.py:254
 msgid ""
 "Enter your password for\n"
 "{}"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:274
+#: thonny/plugins/backend_config_page.py:272
 msgid "Save password"
 msgstr ""
 
-#: thonny/plugins/backend_config_page.py:337
+#: thonny/plugins/backend_config_page.py:335
 msgid "Interpreter"
 msgstr ""
 
 #: thonny/plugins/birdseye_frontend.py:55
 msgid "About Birdseye"
 msgstr ""
 
@@ -839,35 +917,35 @@
 msgid "Debug current script (birdseye)"
 msgstr ""
 
 #: thonny/plugins/calltip.py:159
 msgid "Show parameter info"
 msgstr ""
 
-#: thonny/plugins/commenting_indenting.py:143
+#: thonny/plugins/commenting_indenting.py:142
 msgid "Indent selected lines"
 msgstr ""
 
-#: thonny/plugins/commenting_indenting.py:153
+#: thonny/plugins/commenting_indenting.py:152
 msgid "Dedent selected lines"
 msgstr ""
 
-#: thonny/plugins/commenting_indenting.py:163
+#: thonny/plugins/commenting_indenting.py:162
 msgid "Replace tabs with spaces"
 msgstr ""
 
-#: thonny/plugins/commenting_indenting.py:172
+#: thonny/plugins/commenting_indenting.py:171
 msgid "Toggle comment"
 msgstr ""
 
-#: thonny/plugins/commenting_indenting.py:182
+#: thonny/plugins/commenting_indenting.py:181
 msgid "Comment out"
 msgstr ""
 
-#: thonny/plugins/commenting_indenting.py:192
+#: thonny/plugins/commenting_indenting.py:191
 msgid "Uncomment"
 msgstr ""
 
 #: thonny/plugins/common_editing_commands.py:21
 msgid "Undo"
 msgstr ""
 
@@ -875,114 +953,114 @@
 msgid "Redo"
 msgstr ""
 
 #: thonny/plugins/common_editing_commands.py:85 thonny/plugins/debugger.py:152
 msgid "Select all"
 msgstr ""
 
-#: thonny/plugins/debugger.py:145 thonny/plugins/debugger.py:1401
+#: thonny/plugins/debugger.py:145 thonny/plugins/debugger.py:1402
 msgid "Run to cursor"
 msgstr ""
 
-#: thonny/plugins/debugger.py:553
+#: thonny/plugins/debugger.py:557
 #, python-format
 msgid "Function call at %s"
 msgstr ""
 
-#: thonny/plugins/debugger.py:961
+#: thonny/plugins/debugger.py:964
 msgid "Source code"
 msgstr ""
 
-#: thonny/plugins/debugger.py:982
+#: thonny/plugins/debugger.py:985
 msgid "Can't close yet"
 msgstr ""
 
-#: thonny/plugins/debugger.py:983
+#: thonny/plugins/debugger.py:986
 msgid "Use \"Stop\" command if you want to cancel debugging"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1003
+#: thonny/plugins/debugger.py:1006
 msgid "Local variables"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1035
+#: thonny/plugins/debugger.py:1038
 msgid "Function"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1036
+#: thonny/plugins/debugger.py:1039
 msgid "Location"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1112
+#: thonny/plugins/debugger.py:1115
 msgid ""
 "If last command raised an exception then this view will show the "
 "stacktrace."
 msgstr ""
 
-#: thonny/plugins/debugger.py:1283
+#: thonny/plugins/debugger.py:1284
 msgid "Resume"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1299
+#: thonny/plugins/debugger.py:1300
 msgid "Run / resume"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1314
+#: thonny/plugins/debugger.py:1315
 msgid "Debug current script"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1316
+#: thonny/plugins/debugger.py:1317
 msgid "Debug"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1327
+#: thonny/plugins/debugger.py:1328
 msgid "Debug current script (nicer)"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1339
+#: thonny/plugins/debugger.py:1340
 msgid "Debug current script (faster)"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1350
+#: thonny/plugins/debugger.py:1351
 msgid "Step over"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1352
+#: thonny/plugins/debugger.py:1353
 msgid "Over"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1363
+#: thonny/plugins/debugger.py:1364
 msgid "Step into"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1365
+#: thonny/plugins/debugger.py:1366
 msgid "Into"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1376
+#: thonny/plugins/debugger.py:1377
 msgid "Step out"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1378
+#: thonny/plugins/debugger.py:1379
 msgid "Out"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1413
+#: thonny/plugins/debugger.py:1414
 msgid "Step back"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1415
+#: thonny/plugins/debugger.py:1416
 msgid "Back"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1421
+#: thonny/plugins/debugger.py:1422
 msgid "Stack"
 msgstr ""
 
-#: thonny/plugins/debugger.py:1422
+#: thonny/plugins/debugger.py:1423
 msgid "Exception"
 msgstr ""
 
 #: thonny/plugins/dock_user_windows_frontend.py:28
 msgid "Dock user windows"
 msgstr ""
 
@@ -1079,59 +1157,59 @@
 msgid "Downloading %s to %s"
 msgstr ""
 
 #: thonny/plugins/files.py:609
 msgid "Files"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:60 thonny/plugins/find_replace.py:437
+#: thonny/plugins/find_replace.py:60 thonny/plugins/find_replace.py:438
 msgid "Find & Replace"
 msgstr ""
 
 #: thonny/plugins/find_replace.py:66
 msgid "Find:"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:87
+#: thonny/plugins/find_replace.py:90
 msgid "Replace with:"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:105
+#: thonny/plugins/find_replace.py:108
 msgid "Case sensitive"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:112
+#: thonny/plugins/find_replace.py:115
 msgid "Up"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:116
+#: thonny/plugins/find_replace.py:119
 msgid "Down"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:125
+#: thonny/plugins/find_replace.py:128
 msgid "Find"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:135
+#: thonny/plugins/find_replace.py:138
 msgid "Replace"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:143
+#: thonny/plugins/find_replace.py:146
 msgid "Replace+Find"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:153
+#: thonny/plugins/find_replace.py:156
 msgid "Replace all"
 msgstr ""
 
-#: thonny/plugins/find_replace.py:253
+#: thonny/plugins/find_replace.py:254
 msgid "Enter string to be replaced."
 msgstr ""
 
-#: thonny/plugins/find_replace.py:338
+#: thonny/plugins/find_replace.py:339
 msgid "The specified text was not found!"
 msgstr ""
 
 #: thonny/plugins/general_config_page.py:15
 msgid "Allow only single Thonny instance"
 msgstr ""
 
@@ -1195,18 +1273,14 @@
 msgstr ""
 
 #: thonny/plugins/general_config_page.py:148
 msgid "General"
 msgstr ""
 
 #: thonny/plugins/goto_definition.py:58
-msgid "Problem"
-msgstr ""
-
-#: thonny/plugins/goto_definition.py:58
 msgid "Could not find definition"
 msgstr ""
 
 #: thonny/plugins/heap.py:22
 msgid "ID"
 msgstr ""
 
@@ -1247,59 +1321,59 @@
 msgid "Previous object"
 msgstr ""
 
 #: thonny/plugins/object_inspector.py:119
 msgid "Next object"
 msgstr ""
 
-#: thonny/plugins/object_inspector.py:487
+#: thonny/plugins/object_inspector.py:486
 #, python-format
 msgid ""
 "The representation above is an approximate value of this float. The exact"
 " stored value is %s which is about %s"
 msgstr ""
 
-#: thonny/plugins/object_inspector.py:538
+#: thonny/plugins/object_inspector.py:537
 msgid "Index"
 msgstr ""
 
-#: thonny/plugins/object_inspector.py:616
+#: thonny/plugins/object_inspector.py:615
 msgid "Key ID"
 msgstr ""
 
-#: thonny/plugins/object_inspector.py:617
+#: thonny/plugins/object_inspector.py:616
 msgid "Key"
 msgstr ""
 
-#: thonny/plugins/object_inspector.py:733
+#: thonny/plugins/object_inspector.py:732
 msgid "Object inspector"
 msgstr ""
 
 #: thonny/plugins/outline.py:148
 msgid "Outline"
 msgstr ""
 
 #: thonny/plugins/pgzero_frontend.py:27
 msgid "Pygame Zero mode"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:70
+#: thonny/plugins/pip_gui.py:71
 msgid "Search on PyPI"
 msgstr ""
 
 #: thonny/plugins/esp/__init__.py:349
-#: thonny/plugins/micropython/uf2dialog.py:410 thonny/plugins/pip_gui.py:73
+#: thonny/plugins/micropython/uf2dialog.py:417 thonny/plugins/pip_gui.py:74
 msgid "Install"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:76
+#: thonny/plugins/pip_gui.py:77
 msgid "Upgrade"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:79
+#: thonny/plugins/pip_gui.py:80
 msgid "Uninstall"
 msgstr ""
 
 #: thonny/plugins/pip_gui.py:142
 msgid "INSTALL"
 msgstr ""
 
@@ -1486,20 +1560,20 @@
 msgid "Installing"
 msgstr ""
 
 #: thonny/plugins/pip_gui.py:789
 msgid "Package"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:902
+#: thonny/plugins/pip_gui.py:901
 #, python-format
 msgid "Manage packages for %s"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:954
+#: thonny/plugins/pip_gui.py:953
 #, python-format
 msgid ""
 "Looks like you are installing a Thonny-related package.\n"
 "If you meant to install a Thonny plugin, then you should\n"
 "choose 'Tools → Manage plugins...' instead\n"
 "\n"
 "Are you sure you want to install %s for the back-end?"
@@ -1561,89 +1635,93 @@
 msgid "Requires:"
 msgstr ""
 
 #: thonny/plugins/pip_gui.py:1328
 msgid "Error:"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:1502
+#: thonny/plugins/pip_gui.py:1501
 msgid "Package manager is not available for this interpreter"
 msgstr ""
 
-#: thonny/plugins/micropython/pip_gui.py:100 thonny/plugins/pip_gui.py:1521
+#: thonny/plugins/micropython/pip_gui.py:100 thonny/plugins/pip_gui.py:1520
 msgid "Not available"
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:1522
+#: thonny/plugins/pip_gui.py:1521
 msgid "You need to stop your program before launching the package manager."
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:1541
+#: thonny/plugins/pip_gui.py:1540
 msgid "Manage packages..."
 msgstr ""
 
-#: thonny/plugins/pip_gui.py:1547
+#: thonny/plugins/pip_gui.py:1546
 msgid "Manage plug-ins..."
 msgstr ""
 
 #: thonny/plugins/pythontutor.py:41
 msgid "Visualize current script at Python Tutor"
 msgstr ""
 
-#: thonny/plugins/replayer.py:365
+#: thonny/plugins/replayer.py:364
 msgid "Open replayer..."
 msgstr ""
 
 #: thonny/plugins/run_debug_config_page.py:14
+msgid "Allow running unnamed programs"
+msgstr ""
+
+#: thonny/plugins/run_debug_config_page.py:21
 msgid "Change working directory to script directory on Run / Debug"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:22
+#: thonny/plugins/run_debug_config_page.py:29
 msgid "Show function calls (frames) in separate windows"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:23
+#: thonny/plugins/run_debug_config_page.py:30
 msgid "Uncheck if you want more traditional experience."
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:29
+#: thonny/plugins/run_debug_config_page.py:36
 msgid "Open and close Stack view automatically"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:30
+#: thonny/plugins/run_debug_config_page.py:37
 msgid ""
 "Opens the Stack view on first call and closes it when program returns to "
 "main frame."
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:39
+#: thonny/plugins/run_debug_config_page.py:46
 msgid "Allow stepping into libraries (ie. outside of main script directory)"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:40
+#: thonny/plugins/run_debug_config_page.py:47
 msgid "May make debugging slower."
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:45
+#: thonny/plugins/run_debug_config_page.py:52
 msgid "Preferred debugger"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:57
+#: thonny/plugins/run_debug_config_page.py:64
 msgid "(used when clicking Debug toolbar button)"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:62
+#: thonny/plugins/run_debug_config_page.py:69
 msgid "Birdseye port"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:66
+#: thonny/plugins/run_debug_config_page.py:73
 msgid "(restart Thonny after changing this)"
 msgstr ""
 
-#: thonny/plugins/run_debug_config_page.py:74
+#: thonny/plugins/run_debug_config_page.py:81
 msgid "Run & Debug"
 msgstr ""
 
 #: thonny/plugins/shell_config_page.py:17
 msgid "Clear Shell before starting new process (Run, Debug, Stop/Restart, ...)"
 msgstr ""
 
@@ -1689,83 +1767,83 @@
 "(Profiles → Shell → When the shell exits)"
 msgstr ""
 
 #: thonny/plugins/terminal_config_page.py:41
 msgid "Terminal"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:40
+#: thonny/plugins/theme_and_font_config_page.py:39
 msgid "UI theme"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:53
+#: thonny/plugins/theme_and_font_config_page.py:52
 msgid "Syntax theme"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:85
+#: thonny/plugins/theme_and_font_config_page.py:84
 msgid "Editor font"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:108
+#: thonny/plugins/theme_and_font_config_page.py:107
 msgid "IO font"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:133
+#: thonny/plugins/theme_and_font_config_page.py:132
 msgid "Preview"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:151
+#: thonny/plugins/theme_and_font_config_page.py:150
 msgid "This is a comment"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:154
+#: thonny/plugins/theme_and_font_config_page.py:153
 msgid "The answer is"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:158
+#: thonny/plugins/theme_and_font_config_page.py:157
 msgid "unclosed_string"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:160
+#: thonny/plugins/theme_and_font_config_page.py:159
 msgid "blah, blah"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:184
+#: thonny/plugins/theme_and_font_config_page.py:183
 msgid "NB! Some style elements change only after restarting Thonny!"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:223
+#: thonny/plugins/theme_and_font_config_page.py:222
 msgid "Enter an integer"
 msgstr ""
 
-#: thonny/plugins/theme_and_font_config_page.py:236
+#: thonny/plugins/theme_and_font_config_page.py:235
 msgid "Theme & Font"
 msgstr ""
 
 #: thonny/plugins/thonny_folders.py:19
 msgid "Open Thonny program folder..."
 msgstr ""
 
 #: thonny/plugins/thonny_folders.py:24
 msgid "Open Thonny data folder..."
 msgstr ""
 
-#: thonny/plugins/todo_view.py:44
+#: thonny/plugins/todo_view.py:43
 msgid "Line"
 msgstr ""
 
-#: thonny/plugins/todo_view.py:45
+#: thonny/plugins/todo_view.py:44
 msgid "Info"
 msgstr ""
 
-#: thonny/plugins/todo_view.py:123
+#: thonny/plugins/todo_view.py:121
 msgid "No line marked with #todo found"
 msgstr ""
 
-#: thonny/plugins/todo_view.py:143
+#: thonny/plugins/todo_view.py:141
 msgid "TODO"
 msgstr ""
 
 #: thonny/plugins/variables.py:22
 msgid ""
 "Back to\n"
 "current frame"
@@ -1940,15 +2018,15 @@
 msgid "look for your device name, \"USB Serial\" or \"UART\""
 msgstr ""
 
 #: thonny/plugins/micropython/mp_front.py:552
 msgid "If you can't find it, you may need to install proper USB driver first."
 msgstr ""
 
-#: thonny/plugins/micropython/mp_front.py:589
+#: thonny/plugins/micropython/mp_front.py:588
 msgid "Password"
 msgstr ""
 
 #: thonny/plugins/micropython/pip_gui.py:24
 msgid ""
 "This doesn't look like MicroPython/CircuitPython package.\n"
 "Are you sure you want to install it?"
```

### Comparing `thonny-4.0.2/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/tr_TR/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/tr_TR/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/uk_UA/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/uk_UA/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/vi_VN/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/vi_VN/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/zh_CN/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/zh_CN/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo` & `thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.mo`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/locale/zh_TW/LC_MESSAGES/thonny.po` & `thonny-4.1.0b1.dev0/thonny/locale/zh_TW/LC_MESSAGES/thonny.po`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/memory.py` & `thonny-4.1.0b1.dev0/thonny/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 
         for group_title, variables in groups:
             if group_title:
                 node_id = self.tree.insert("", "end", tags=("group_title",))
                 self.tree.set(node_id, "name", group_title)
 
             for name in sorted(variables.keys()):
-
                 if not name.startswith("__"):
                     node_id = self.tree.insert("", "end", tags="item")
                     self.tree.set(node_id, "name", name)
                     if isinstance(variables[name], ValueInfo):
                         description = variables[name].repr
                         id_str = variables[name].id
                     else:
```

### Comparing `thonny-4.0.2/thonny/misc_utils.py` & `thonny-4.1.0b1.dev0/thonny/misc_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,16 +91,31 @@
                 path = "{}:\\".format(disk)
                 if os.path.exists(path):
                     volumes.append(path)
 
             return volumes
         finally:
             ctypes.windll.kernel32.SetErrorMode(old_mode)  # @UndefinedVariable
+    if sys.platform == "linux":
+        from dbus_next.errors import DBusError
+
+        from thonny.udisks import list_volumes_sync
+
+        mount_points = []
+        try:
+            mount_points = list_volumes_sync()
+        except DBusError as error:
+            # Fallback to using the 'mount' command on Linux if the Udisks D-Bus service is unavailable.
+            if "org.freedesktop.DBus.Error.ServiceUnknown" not in error.text:
+                raise
+            mount_output = subprocess.check_output("mount").splitlines()
+            mount_points = [x.split()[2].decode("utf-8") for x in mount_output]
+        return mount_points
     else:
-        # 'posix' means we're on Linux or OSX (Mac).
+        # 'posix' means we're on *BSD or OSX (Mac).
         # Call the unix "mount" command to list the mounted volumes.
         mount_output = subprocess.check_output("mount").splitlines()
         return [x.split()[2].decode("utf-8") for x in mount_output]
 
 
 def get_win_volume_name(path: str) -> str:
     """
```

### Comparing `thonny-4.0.2/thonny/plugins/about.py` & `thonny-4.1.0b1.dev0/thonny/plugins/about.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,35 +40,35 @@
                 import distro  # distro don't need to be installed
 
                 system_desc = distro.name(True)
             except ImportError:
                 system_desc = "Linux"
 
             if "32" not in system_desc and "64" not in system_desc:
-                system_desc += " " + self.get_os_word_size_guess()
+                system_desc += self.get_os_word_size_suffix()
         else:
             release = platform.release()
             if sys.platform == "win32":
                 # Win 10 and 11 both give 10 as release
                 try:
                     build = int(platform.version().split(".")[2])
                     if release == "10" and build >= 22000:
                         release = "11"
                 except Exception:
                     logger.exception("Could not determine Windows version")
 
-            system_desc = platform.system() + " " + release + " " + self.get_os_word_size_guess()
+            system_desc = platform.system() + " " + release + self.get_os_word_size_suffix()
 
         platform_label = ttk.Label(
             self.main_frame,
             justify=tk.CENTER,
             text=system_desc
             + "\n"
             + "Python "
-            + get_python_version_string(maxsize=sys.maxsize)
+            + get_python_version_string()
             + "\n"
             + "Tk "
             + ui_utils.get_tk_version_str(),
         )
         platform_label.grid(pady=self.get_medium_padding())
 
         credits_label = create_url_label(
@@ -111,19 +111,17 @@
             self.main_frame, text=tr("OK"), command=self.on_close, default="active"
         )
         ok_button.grid(pady=(0, self.get_large_padding()))
         ok_button.focus_set()
 
         self.bind("<Return>", self.on_close, True)
 
-    def get_os_word_size_guess(self):
+    def get_os_word_size_suffix(self):
         if "32" in platform.machine() and "64" not in platform.machine():
-            return "(32-bit)"
-        elif "64" in platform.machine() and "32" not in platform.machine():
-            return "(64-bit)"
+            return " (32-bit)"
         else:
             return ""
 
 
 def load_plugin() -> None:
     def open_about():
         ui_utils.show_dialog(AboutDialog(get_workbench()))
```

### Comparing `thonny-4.0.2/thonny/plugins/assistant_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/assistant_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/ast_view.py` & `thonny-4.1.0b1.dev0/thonny/plugins/ast_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 
         except Exception as e:
             self.tree.insert("", "end", text=str(e), open=True)
             logger.exception("Could not select AST node", exc_info=e)
             return
 
         def _format(key, node, parent_id):
-
             if isinstance(node, ast.AST):
                 fields = list(ast.iter_fields(node))
 
                 value_label = node.__class__.__name__
 
             elif isinstance(node, list):
                 fields = list(enumerate(node))
```

### Comparing `thonny-4.0.2/thonny/plugins/autocomplete.py` & `thonny-4.1.0b1.dev0/thonny/plugins/autocomplete.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,18 @@
     def _on_select_item_via_event(self, event=None) -> None:
         if self._tweaking_listbox_selection:
             return
 
         self._check_request_details()
 
     def _check_request_details(self) -> None:
-        assert self.winfo_ismapped()
+        if not self.winfo_ismapped():
+            # can happen, see https://github.com/thonny/thonny/issues/2162
+            return
+
         if (
             self._details_box
             and self._details_box.is_visible()
             or get_workbench().get_option("edit.automatic_completion_details")
         ):
             self.request_details()
 
@@ -372,14 +375,19 @@
             get_workbench().bell()
 
     def _should_open_box_automatically(self, event):
         assert isinstance(event.widget, tk.Text)
         if not get_workbench().get_option("edit.automatic_completions"):
             return False
 
+        # Don't autocomplete in remote shells
+        proxy = get_runner().get_backend_proxy()
+        if isinstance(event.widget, ShellText) and (not proxy or not proxy.has_local_interpreter()):
+            return False
+
         # Don't autocomplete inside comments
         line_prefix = event.widget.get("insert linestart", "insert")
         if "#" in line_prefix:
             # not very precise (eg. when inside a string), but good enough
             return False
 
         return True
@@ -505,15 +513,14 @@
 
 
 def _is_python_name_char(c: str) -> bool:
     return c.isalnum() or c == "_"
 
 
 def load_plugin() -> None:
-
     completer = Completer()
 
     def can_complete():
         runner = get_runner()
         return runner and not runner.is_running()
 
     get_workbench().add_command(
```

### Comparing `thonny-4.0.2/thonny/plugins/backend/birdseye_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/birdseye_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/backend/dock_user_windows_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/dock_user_windows_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/backend/flask_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/flask_backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,19 +39,14 @@
         return source
     else:
         return (
             source
             + """
 
 if "{app_name}" in globals():
-    import os as __temp_os__
-    if "FLASK_ENV" not in __temp_os__.environ:
-        __temp_os__.environ["FLASK_ENV"] = "development"
-    del __temp_os__
-    
     # Conservative options for minimum technical risks.
     # Users who need more control should call run explicitly.
     print(" # Running the app with options chosen by Thonny. See Help for details.")
     {app_name}.run(threaded=False, debug=False, use_reloader=False)
 """.format(
                 app_name=var_name
             )
```

### Comparing `thonny-4.0.2/thonny/plugins/backend/matplotlib_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/matplotlib_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         or os.path.exists(local_conf_file)
         or os.path.exists(user_conf_file1)
         or os.path.exists(user_conf_file2)
     ):
         # done or the user knows what (s)he's doing
         pass
     else:
-
         try:
             import tkinter  # @UnusedImport
 
             os.environ["MPLBACKEND"] = "TkAgg"
         except ImportError:
             pass
```

### Comparing `thonny-4.0.2/thonny/plugins/backend/pgzero_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend/pgzero_backend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/backend_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/backend_config_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         variable_name,
         row,
         show=None,
         pady: Union[int, tuple] = 0,
         width=None,
         **kwargs,
     ):
-
         if isinstance(pady, int):
             pady = (pady, pady)
 
         entry_label = ttk.Label(self, text=label_text)
         entry_label.grid(row=row, column=0, sticky="w", pady=pady)
 
         variable = create_string_var(get_workbench().get_option(variable_name), self._on_change)
@@ -125,15 +124,14 @@
             if self._current_page is not None:
                 self._current_page.grid_forget()
             return
 
         page = self._get_conf_page(backend_desc)
 
         if page != self._current_page:
-
             if self._current_page is not None:
                 self._current_page.grid_forget()
 
             page.grid(sticky="nsew", padx=10, pady=5)
             self._current_page = page
 
     def _get_conf_page(self, backend_desc):
```

### Comparing `thonny-4.0.2/thonny/plugins/base_syntax_themes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/base_syntax_themes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/base_ui_themes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/base_ui_themes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/birdseye_frontend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/birdseye_frontend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/calltip.py` & `thonny-4.1.0b1.dev0/thonny/plugins/calltip.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/cells.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     def _patched_perform_return(self, event):
         text = event.widget
         ranges = text.tag_ranges("CURRENT_CELL")
 
         if len(ranges) == 2 and (
             ui_utils.shift_is_pressed(event) or ui_utils.control_is_pressed(event)
         ):
-
             if run_enabled():
                 code = text.get(ranges[0], ranges[1]).strip()
                 _submit_code(code)
 
                 if ui_utils.shift_is_pressed(event):
                     # advance to next cell
                     text.mark_set("insert", ranges[1])
```

### Comparing `thonny-4.0.2/thonny/plugins/circuitpython/cirpy_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_back.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import os.path
+import sys
 from logging import getLogger
 from typing import List, Optional
 
+# make sure thonny folder is in sys.path (relevant in dev)
+thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+if thonny_container not in sys.path:
+    sys.path.insert(0, thonny_container)
+
+
 from thonny.plugins.micropython.bare_metal_backend import (
     BareMetalMicroPythonBackend,
     launch_bare_metal_backend,
 )
 
 # Can't use __name__, because it will be "__main__"
 logger = getLogger("thonny.plugins.micropython.cirpy_backend")
```

### Comparing `thonny-4.0.2/thonny/plugins/circuitpython/cirpy_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/circuitpython/cirpy_front.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import sys
 from logging import getLogger
+from typing import List
 
+from thonny import ui_utils
 from thonny.languages import tr
+from thonny.plugins.microbit import MicrobitFlashingDialog
+from thonny.plugins.micropython.esptool_dialog import try_launch_esptool_dialog
 from thonny.plugins.micropython.mp_front import (
     BareMetalMicroPythonConfigPage,
     BareMetalMicroPythonProxy,
 )
 from thonny.plugins.micropython.uf2dialog import show_uf2_installer
 
 logger = getLogger(__name__)
@@ -84,15 +88,21 @@
             return super()._is_potential_port(p)
 
 
 class CircuitPythonConfigPage(BareMetalMicroPythonConfigPage):
     def _get_intro_url(self):
         return "https://learn.adafruit.com/welcome-to-circuitpython/installing-circuitpython"
 
-    def _has_flashing_dialog(self):
-        return True
+    def get_flashing_dialog_kinds(self) -> List[str]:
+        return ["UF2", "esptool", "BBC micro:bit"]
 
-    def _open_flashing_dialog(self):
-        show_uf2_installer(self, firmware_name="CircuitPython")
+    def _open_flashing_dialog(self, kind: str) -> None:
+        if kind == "UF2":
+            show_uf2_installer(self, firmware_name="CircuitPython")
+        elif kind == "esptool":
+            try_launch_esptool_dialog(self.winfo_toplevel(), "CircuitPython")
+        elif kind == "BBC micro:bit":
+            dlg = MicrobitFlashingDialog(self, "CircuitPython")
+            ui_utils.show_dialog(dlg)
 
     def _get_flasher_link_title(self) -> str:
         return tr("Install or update %s") % "CircuitPython"
```

### Comparing `thonny-4.0.2/thonny/plugins/clean_ui_themes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/clean_ui_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     normal_foreground: str,
     high_foreground: str,
     low_foreground: str,
     custom_menubar: Optional[
         int
     ] = None,  # NB! Should be 1 or 0, not True or False (Tk would convert False to "False")
 ) -> UiThemeSettings:
-
     # https://wiki.tcl.tk/37973 (Changing colors)
     # https://github.com/tcltk/tk/blob/master/library/ttk/clamTheme.tcl
     # https://github.com/tcltk/tk/blob/master/generic/ttk/ttkClamTheme.c
 
     return {
         ".": {
             "configure": {
```

### Comparing `thonny-4.0.2/thonny/plugins/coloring.py` & `thonny-4.1.0b1.dev0/thonny/plugins/coloring.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/commenting_indenting.py` & `thonny-4.1.0b1.dev0/thonny/plugins/commenting_indenting.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 
         text.delete("1.0", "end")
 
         text.insert("1.0", "".join(new_lines))
 
 
 def load_plugin() -> None:
-
     get_workbench().add_command(
         "indent",
         "edit",
         tr("Indent selected lines"),
         _cmd_indent_selection,
         tester=_writable_text_is_focused,
         accelerator="Tab",
```

### Comparing `thonny-4.0.2/thonny/plugins/common_editing_commands.py` & `thonny-4.1.0b1.dev0/thonny/plugins/common_editing_commands.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/cpython_backend/cp_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_back.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Frontend plugin is in cpython_frontend.py
 import ast
 import builtins
 import functools
-import importlib
+import importlib.util
 import inspect
 import io
 import os.path
 import queue
 import re
 import site
 import subprocess
@@ -57,24 +57,26 @@
 _CONFIG_FILENAME = os.path.join(thonny.THONNY_USER_DIR, "backend_configuration.ini")
 
 
 _backend = None
 
 
 class MainCPythonBackend(MainBackend):
-    def __init__(self, target_cwd):
+    def __init__(self, target_cwd, options):
         report_time("Before MainBackend")
         MainBackend.__init__(self)
         report_time("After MainBackend")
 
         global _backend
         _backend = self
 
         self._ini = None
+        self._options = options
         self._object_info_tweakers = []
+        self._warned_shadow_casters = set()
         self._import_handlers = {}
         self._input_queue = queue.Queue()
         self._source_preprocessors = []
         self._ast_postprocessors = []
         self._main_dir = os.path.dirname(sys.modules["thonny"].__file__)
         self._heap = {}  # WeakValueDictionary would be better, but can't store reference to None
         self._source_info_by_frame = {}
@@ -98,29 +100,33 @@
         __main__.__package__ = None
         __main__.__spec__ = None
 
         logger.info("Loading plugins")
         report_time("Before loading plugins")
         execute_with_frontend_sys_path(self._load_plugins)
         report_time("After loading plugins")
+        if self._options.get("run.warn_module_shadowing", False):
+            sys.addaudithook(self.import_audit_hook)
 
-        # preceding code was run in the directory containing thonny module, now switch to provided
+        # preceding code was run in an empty directory, now switch to provided
         try:
             os.chdir(os.path.expanduser(target_cwd))
         except OSError:
             try:
                 os.chdir(os.path.expanduser("~"))
             except OSError:
                 os.chdir("/")  # yes, this works also in Windows
 
         # ... and replace current-dir path item
         # start in shell mode (may be later switched to script mode)
         # required in shell mode and also required to overwrite thonny location dir
-        sys.path[0] = ""
+        assert "" not in sys.path  # for avoiding
+        sys.path.insert(0, "")
         sys.argv[:] = [""]  # empty "script name"
+        self._check_warn_avoided_sys_path_conflicts()
 
         if os.name == "nt":
             self._install_signal_handler()
 
     def _init_command_reader(self):
         # Can't use threaded reader
         # https://github.com/thonny/thonny/issues/1363
@@ -157,14 +163,81 @@
 
     def add_ast_postprocessor(self, func):
         self._ast_postprocessors.append(func)
 
     def get_main_module(self):
         return __main__
 
+    def import_audit_hook(self, event: str, args):
+        if event == "import":
+            logger.debug("detected Import event with args %r", args)
+            module_name = args[0]
+            self._check_warn_sys_path_conflict(module_name.split(".")[0])
+
+    def _check_warn_avoided_sys_path_conflicts(self):
+        if self._options.get("run.warn_module_shadowing", False):
+            return
+
+        for name in sys.modules.keys():
+            if name != "__main__":
+                self._check_warn_sys_path_conflict(name.split(".")[0])
+
+    def _check_warn_sys_path_conflict(self, root_module_name: str):
+        user_dir = sys.path[0]
+        if user_dir == "":
+            user_dir = os.getcwd()
+
+        # rough test to see if it's worth invoking the finder
+        for ext in ["", ".py", ".pyw"]:
+            pot_path = os.path.join(user_dir, root_module_name + ext)
+            if os.path.exists(pot_path):
+                logger.debug("Found import candidate: %r", pot_path)
+                break
+        else:
+            return
+
+        # It looks like a module is about to be imported from the script dir or current dir.
+        # Is it shadowing a library module?
+
+        current_spec = importlib.util.find_spec(root_module_name)
+
+        first_entry = sys.path[0]
+        del sys.path[0]
+        try:
+            shadowed_spec = importlib.util.find_spec(root_module_name)
+        finally:
+            sys.path.insert(0, first_entry)
+
+        if shadowed_spec is None:
+            logger.debug("No shadowed spec")
+            return
+
+        if shadowed_spec.origin == current_spec.origin:
+            logger.debug("Equal current and shadowed spec")
+            return
+
+        logger.debug("%r shadows %r", current_spec.origin, shadowed_spec.origin)
+
+        if current_spec.origin in self._warned_shadow_casters:
+            return
+
+        if root_module_name in sys.modules:
+            # i.e. the method is called for post-import warning
+            verb = "can shadow"
+        else:
+            verb = "is shadowing"
+
+        self._send_output(
+            # using backticks, because Shell would present file path in quotes as frame link
+            f"WARNING: Your `{current_spec.origin}` {verb} the library module '{root_module_name}'. Consider renaming or moving it!\n",
+            "stderr",
+        )
+
+        self._warned_shadow_casters.add(current_spec.origin)
+
     def _read_incoming_msg_line(self) -> str:
         return self._original_stdin.readline()
 
     def _handle_user_input(self, msg: InputSubmission) -> None:
         self._input_queue.put(msg)
 
     def _handle_eof_command(self, msg: EOFCommand) -> None:
@@ -256,14 +329,16 @@
 
         filename = cmd.args[0]
         if os.path.isfile(filename):
             abs_filename = os.path.abspath(filename)
             sys.path.insert(0, os.path.dirname(abs_filename))
             __main__.__dict__["__file__"] = abs_filename
 
+        self._check_warn_avoided_sys_path_conflicts()
+
     def _custom_import(self, *args, **kw):
         module = self._original_import(*args, **kw)
 
         if not hasattr(module, "__name__"):
             return module
 
         # module specific handlers
@@ -579,15 +654,14 @@
                     shutil.rmtree(path)
             except Exception as e:
                 print("Could not delete %s: %s" % (path, str(e)), file=sys.stderr)
 
     def _perform_pip_operation_and_list(
         self, cmd_line: List[str]
     ) -> Tuple[int, Dict[str, DistInfo]]:
-
         extra_switches = ["--disable-pip-version-check"]
         proxy = os.environ.get("https_proxy", os.environ.get("http_proxy", None))
         if proxy:
             extra_switches.append("--proxy=" + proxy)
 
         returncode = subprocess.call([sys.executable, "-m", "pip"] + extra_switches + cmd_line)
         return returncode, self._get_distributions_info()
@@ -630,15 +704,14 @@
 
     def _get_dir_children_info(
         self, path: str, include_hidden: bool = False
     ) -> Optional[Dict[str, Dict]]:
         return get_single_dir_child_data(path, include_hidden)
 
     def _get_path_info(self, path: str) -> Optional[Dict]:
-
         try:
             if not os.path.exists(path):
                 return None
         except OSError:
             pass
 
         try:
@@ -1031,14 +1104,16 @@
 
             if data != "":
                 self._backend._send_output(data=data, stream_name=self._stream_name)
                 self._processed_symbol_count += len(data)
         finally:
             self._backend._exit_io_function()
 
+        return len(data)
+
     def writelines(self, lines):
         try:
             self._backend._enter_io_function()
             self.write("".join(lines))
         finally:
             self._backend._exit_io_function()
```

### Comparing `thonny-4.0.2/thonny/plugins/cpython_backend/cp_launcher.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_launcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 
 (Why separate file for launching? I want to have clean global scope
 in toplevel __main__ module (because that's where user scripts run), but backend's global scope
 is far from clean.
 I could also do python -c "from backend import MainCPythonBackend: MainCPythonBackend().mainloop()",
 but looks like this gives relative __file__-s on imported modules.)
 """
+import ast
 
 # NB! This module can be also imported (when querying its path for uploading)
 if __name__ == "__main__":
-    import os
+    import ast
+    import os.path
     import sys
 
+    # make sure thonny folder is in sys.path (relevant in dev)
+    thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+    if thonny_container not in sys.path:
+        sys.path.insert(0, thonny_container)
+
     if sys.platform == "darwin":
         try:
             os.getcwd()
         except Exception:
             print(
                 "\nNB! Potential problems detected, see\nhttps://github.com/thonny/thonny/wiki/MacOSX#catalina\n",
                 file=sys.stderr,
@@ -31,15 +38,18 @@
             file=sys.stderr,
         )
         sys.exit(1)
     import thonny
     from thonny import report_time
 
     report_time("Before importing MainCPythonBackend")
+    from thonny.common import PROCESS_ACK
     from thonny.plugins.cpython_backend.cp_back import MainCPythonBackend
 
     thonny.prepare_thonny_user_dir()
     thonny.configure_backend_logging()
+    print(PROCESS_ACK)
 
     target_cwd = sys.argv[1]
+    options = ast.literal_eval(sys.argv[2])
     report_time("Before constructing backend")
-    MainCPythonBackend(target_cwd).mainloop()
+    MainCPythonBackend(target_cwd, options).mainloop()
```

### Comparing `thonny-4.0.2/thonny/plugins/cpython_backend/cp_tracers.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_backend/cp_tracers.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,14 @@
     def _cmd_step_out_completed(self, frame):
         return self._command_frame_returned or self._at_a_breakpoint(frame)
 
     def _cmd_resume_completed(self, frame):
         return self._at_a_breakpoint(frame)
 
     def _get_breakpoints_in_code(self, f_code):
-
         bps_in_file = self._get_breakpoints_in_file(f_code.co_filename)
 
         code_id = id(f_code)
         result = self._code_breakpoints_cache.get(code_id, None)
 
         if result is None:
             if not bps_in_file:
@@ -689,15 +688,14 @@
         if (
             prev_state is not None
             and id(prev_state_frame.system_frame) == id(frame)
             and prev_state["exception_value"] is self._get_current_exception()[1]
             and prev_state["fresh_exception_id"] == id(self._fresh_exception)
             and ("before" in event or "skipexport" in node.tags)
         ):
-
             exception_info = prev_state["exception_info"]
             # share the stack ...
             stack = prev_state["stack"]
             # ... but override certain things
             active_frame_overrides = {
                 "event": custom_frame.event,
                 "focus": custom_frame.focus,
@@ -846,15 +844,14 @@
             if (
                 "last_child" in original_node.tags
                 or "or_arg" in original_node.tags
                 and value
                 or "and_arg" in original_node.tags
                 and not value
             ):
-
                 # there may be explicit exceptions
                 if (
                     "skip_after_statement_again" in original_node.parent_node.tags
                     or "skip_after_expression_again" in original_node.parent_node.tags
                 ):
                     return
```

### Comparing `thonny-4.0.2/thonny/plugins/cpython_frontend/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/cpython_frontend/cp_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_front.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os.path
 import subprocess
 import sys
 import textwrap
 import tkinter as tk
+import traceback
 from logging import getLogger
 from tkinter import messagebox, ttk
 from typing import Any, Dict
 
 import thonny
-from thonny import get_runner, get_workbench, running, ui_utils
+from thonny import get_runner, get_shell, get_workbench, running, ui_utils
 from thonny.common import (
     InlineCommand,
     InlineResponse,
     ToplevelCommand,
     get_base_executable,
     is_private_python,
     is_virtual_executable,
@@ -30,25 +31,47 @@
 
 class LocalCPythonProxy(SubprocessProxy):
     def __init__(self, clean: bool) -> None:
         logger.info("Creating LocalCPythonProxy")
         executable = get_workbench().get_option("LocalCPython.executable")
         self._expecting_response_for_gui_update = False
         super().__init__(clean, executable)
-        self._send_msg(ToplevelCommand("get_environment_info"))
+        try:
+            self._send_msg(ToplevelCommand("get_environment_info"))
+        except Exception:
+            get_shell().report_exception()
 
     def _get_initial_cwd(self):
         return get_workbench().get_local_cwd()
 
     def _get_launch_cwd(self):
-        # launch in the directory containing thonny package, so that other interpreters can import it as well
-        return os.path.dirname(os.path.dirname(thonny.__file__))
+        # use a directory which doesn't contain misleading modules
+        empty_dir = os.path.join(thonny.THONNY_USER_DIR, "leave_this_empty")
+        os.makedirs(empty_dir, exist_ok=True)
+        return empty_dir
 
     def _get_launcher_with_args(self):
-        return ["-m", "thonny.plugins.cpython_backend.cp_launcher", self.get_cwd()]
+        launcher_file = os.path.join(
+            os.path.dirname(os.path.dirname(__file__)), "cpython_backend", "cp_launcher.py"
+        )
+        return [
+            launcher_file,
+            self.get_cwd(),
+            repr(
+                {
+                    "run.warn_module_shadowing": get_workbench().get_option(
+                        "run.warn_module_shadowing"
+                    )
+                }
+            ),
+        ]
+
+    def can_be_isolated(self) -> bool:
+        # Can't run in isolated mode as it would hide user site-packages
+        return False
 
     def _store_state_info(self, msg):
         super()._store_state_info(msg)
 
         if "gui_is_active" in msg:
             self._update_gui_updating(msg)
 
@@ -73,16 +96,18 @@
         and needs updating.
         """
         if "gui_is_active" not in msg:
             return
 
         if msg["gui_is_active"] and self._gui_update_loop_id is None:
             # Start updating
+            logger.info("Starting GUI update loop")
             self._loop_gui_update(True)
         elif not msg["gui_is_active"] and self._gui_update_loop_id is not None:
+            logger.info("Cancelling GUI update loop")
             self._cancel_gui_update_loop()
 
     def _loop_gui_update(self, force=False):
         if force or get_runner().is_waiting_toplevel_command():
             # Don't send command if response for the last one hasn't arrived yet
             if not self._expecting_response_for_gui_update:
                 try:
@@ -211,14 +236,15 @@
 
         self._entry = ttk.Combobox(
             self,
             exportselection=False,
             textvariable=self._configuration_variable,
             values=_get_interpreters(),
         )
+        self._entry.state(["!disabled", "readonly"])
 
         self._entry.grid(row=1, column=1, sticky=tk.NSEW)
 
         self._select_button = ttk.Button(
             self,
             text="...",
             width=3,
@@ -346,26 +372,26 @@
 def _get_interpreters():
     result = set()
 
     if running_on_windows():
         # registry
         result.update(_get_interpreters_from_windows_registry())
 
-        for minor in [7, 8, 9, 10, 11]:
+        for minor in [8, 9, 10, 11, 12]:
             for dir_ in [
                 "C:\\Python3%d" % minor,
                 "C:\\Python3%d-32" % minor,
                 "C:\\Python3%d-64" % minor,
                 "C:\\Program Files\\Python 3.%d" % minor,
                 "C:\\Program Files\\Python 3.%d-64" % minor,
                 "C:\\Program Files (x86)\\Python 3.%d" % minor,
                 "C:\\Program Files (x86)\\Python 3.%d-32" % minor,
                 "C:\\Program Files (x86)\\Python 3.%d-32" % minor,
-                os.path.expanduser("~\\AppData\Local\Programs\Python\Python3%d" % minor),
-                os.path.expanduser("~\\AppData\Local\Programs\Python\Python3%d-32" % minor),
+                os.path.expanduser(r"~\AppData\Local\Programs\Python\Python3%d" % minor),
+                os.path.expanduser(r"~\AppData\Local\Programs\Python\Python3%d-32" % minor),
             ]:
                 path = os.path.join(dir_, WINDOWS_EXE)
                 if os.path.exists(path):
                     result.add(normpath_with_actual_case(path))
 
         # other locations
         for dir_ in [
@@ -398,30 +424,31 @@
                 continue
             for name in [
                 "python3",
                 "python3.8",
                 "python3.9",
                 "python3.10",
                 "python3.11",
+                "python3.12",
             ]:
                 path = os.path.join(dir_, name)
                 if os.path.exists(path):
                     result.add(path)
 
     if running_on_mac_os():
-        for version in ["3.8", "3.9", "3.10", "3.11"]:
+        for version in ["3.8", "3.9", "3.10", "3.11", "3.12"]:
             dir_ = os.path.join("/Library/Frameworks/Python.framework/Versions", version, "bin")
             path = os.path.join(dir_, "python3")
 
             if os.path.exists(path):
                 result.add(path)
 
     from shutil import which
 
-    for command in ["python3", "python3.8", "python3.9", "python3.10", "python3.11"]:
+    for command in ["python3", "python3.8", "python3.9", "python3.10", "python3.11", "python3.12"]:
         path = which(command)
         if path is not None and os.path.isabs(path):
             result.add(path)
 
     for conf in get_workbench().get_option(f"LocalCPython.last_configurations"):
         path = conf["LocalCPython.executable"]
         if os.path.exists(path):
@@ -466,17 +493,14 @@
     # https://github.com/python/cpython/blob/master/Tools/msi/README.txt
     # https://www.python.org/dev/peps/pep-0514/#installpath
     import winreg
 
     result = set()
     for key in [winreg.HKEY_LOCAL_MACHINE, winreg.HKEY_CURRENT_USER]:
         for version in [
-            "3.6",
-            "3.6-32",
-            "3.6-64",
             "3.8",
             "3.8-32",
             "3.8-64",
             "3.9",
             "3.9-32",
             "3.9-64",
             "3.10",
```

### Comparing `thonny-4.0.2/thonny/plugins/cpython_frontend/cp_pip_gui.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_frontend/cp_pip_gui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/cpython_ssh/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/cpython_ssh/cps_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_back.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,38 +2,47 @@
 
 import ast
 import os.path
 import sys
 import threading
 from logging import getLogger
 from threading import Thread
+from typing import Any, Dict
+
+# make sure thonny folder is in sys.path (relevant in dev)
+thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+if thonny_container not in sys.path:
+    sys.path.insert(0, thonny_container)
+
 
 import thonny
 from thonny.backend import (
     BaseBackend,
     RemoteProcess,
     SshMixin,
     ensure_posix_directory,
     interrupt_local_process,
 )
 from thonny.common import (
+    PROCESS_ACK,
     CommandToBackend,
     EOFCommand,
     ImmediateCommand,
     InputSubmission,
     MessageFromBackend,
     serialize_message,
 )
 
 logger = getLogger("thonny.plugins.cpython_ssh.cps_back")
 
 
 class SshCPythonBackend(BaseBackend, SshMixin):
-    def __init__(self, host, user, interpreter, cwd):
+    def __init__(self, host, user, interpreter, cwd, main_backend_options: Dict[str, Any]):
         logger.info("Starting mediator for %s @ %s", user, host)
+        self._main_backend_options = main_backend_options
         password = sys.stdin.readline().strip("\r\n")
         SshMixin.__init__(self, host, user, password, interpreter, cwd)
         self._upload_main_backend()
         self._proc = self._start_main_backend()
         self._main_backend_is_fresh = True
 
         self._response_lock = threading.Lock()
@@ -125,19 +134,22 @@
         if self._proc is None or self._proc.poll() is not None:
             raise ConnectionAbortedError()
 
     def _start_main_backend(self) -> RemoteProcess:
         env = {"THONNY_USER_DIR": "~/.config/Thonny", "THONNY_FRONTEND_SYS_PATH": "[]"}
         self._main_backend_is_fresh = True
 
+        cp_launcher_file = os.path.join(
+            os.path.dirname(os.path.dirname(__file__)), "cpython_backend", "cp_launcher.py"
+        )
         args = [
             self._target_interpreter,
-            "-m",
-            "thonny.plugins.cpython_backend.cp_launcher",
+            cp_launcher_file,
             self._cwd,
+            repr(self._main_backend_options),
         ]
         logger.info("Starting remote process: %r", args)
         return self._create_remote_process(
             args,
             cwd=self._get_remote_program_directory(),
             env=env,
         )
@@ -190,10 +202,11 @@
             remote_path = launch_dir + local_suffix.replace("\\", "/")
             logger.info("Uploading %s => %s", local_path, remote_path)
             self._perform_sftp_operation_with_retry(lambda sftp: sftp.put(local_path, remote_path))
 
 
 if __name__ == "__main__":
     thonny.configure_backend_logging()
+    print(PROCESS_ACK)
     args = ast.literal_eval(sys.argv[1])
     backend = SshCPythonBackend(**args)
     backend.mainloop()
```

### Comparing `thonny-4.0.2/thonny/plugins/cpython_ssh/cps_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/cpython_ssh/cps_front.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 import shutil
 from tkinter import messagebox
 from typing import Any, Dict, Optional
 
 from thonny import get_runner, get_shell, get_workbench
 from thonny.common import ImmediateCommand, ToplevelCommand
 from thonny.plugins.backend_config_page import BaseSshProxyConfigPage, get_ssh_password
@@ -26,23 +27,28 @@
     def can_run_in_terminal(self) -> bool:
         return False
 
     def can_debug(self) -> bool:
         return True
 
     def _get_launcher_with_args(self):
+        launcher_file = os.path.join(os.path.dirname(__file__), "cps_back.py")
         return [
-            "-m",
-            "thonny.plugins.cpython_ssh.cps_back",
+            launcher_file,
             repr(
                 {
                     "host": self._host,
                     "user": self._user,
                     "interpreter": self._target_executable,
                     "cwd": self._get_initial_cwd(),
+                    "main_backend_options": {
+                        "run.warn_module_shadowing": get_workbench().get_option(
+                            "run.warn_module_shadowing"
+                        )
+                    },
                 }
             ),
         ]
 
     def _send_initial_input(self) -> None:
         assert self._proc is not None
         self._proc.stdin.write((get_ssh_password("SshCPython") or "") + "\n")
```

### Comparing `thonny-4.0.2/thonny/plugins/debugger.py` & `thonny-4.1.0b1.dev0/thonny/plugins/debugger.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,15 +641,14 @@
         return opts
 
     def update_expression(self, msg, frame_info):
         focus = frame_info.focus
         event = frame_info.event
 
         if frame_info.current_root_expression is not None:
-
             if self._last_root_expression != frame_info.current_root_expression:
                 # can happen, eg. when focus jumps from the last expr in while body
                 # to while test expression
                 self.clear_debug_view()
 
             with tokenize.open(frame_info.filename) as fp:
                 whole_source = fp.read()
@@ -1124,15 +1123,14 @@
 
         if exception_lines_with_frame_info is None:
             self._show_description()
             return
 
         self.text.configure(foreground=get_syntax_options_for_tag("stderr")["foreground"])
         for line, frame_id, filename, lineno in exception_lines_with_frame_info:
-
             if frame_id is not None:
                 frame_tag = "frame_%d" % frame_id
 
                 def handle_frame_click(event, frame_id=frame_id, filename=filename, lineno=lineno):
                     get_runner().send_command(InlineCommand("get_frame_info", frame_id=frame_id))
                     if os.path.exists(filename):
                         get_workbench().get_editor_notebook().show_file(
@@ -1278,15 +1276,14 @@
 
         return debug_with_birdseye()
     else:
         return _request_debug("Debug")
 
 
 def load_plugin() -> None:
-
     global RESUME_COMMAND_CAPTION
     RESUME_COMMAND_CAPTION = tr("Resume")
 
     if get_workbench().in_simple_mode():
         get_workbench().set_default("debugger.frames_in_separate_windows", False)
     else:
         get_workbench().set_default("debugger.frames_in_separate_windows", True)
```

### Comparing `thonny-4.0.2/thonny/plugins/dock_user_windows_frontend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/dock_user_windows_frontend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/editor_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/editor_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/esp/esp32_api_stubs/esp32.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/esp32.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/esp32_api_stubs/mp-1.18-esp32.txt`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/esp/esp_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/prime_inventor_back.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os.path
+import sys
 from logging import getLogger
 from typing import List, Optional
 
+import thonny
 from thonny.plugins.micropython.bare_metal_backend import (
     BareMetalMicroPythonBackend,
     launch_bare_metal_backend,
 )
 
-# Can't use __name__, because it will be "__main__"
-logger = getLogger("thonny.plugins.micropython.esp_backend")
+logger = getLogger("thonny.plugins.prime_inventor.prime_inventor_back")
 
 
-class EspMicroPythonBackend(BareMetalMicroPythonBackend):
+class PrimeInventorMicroPythonBackend(BareMetalMicroPythonBackend):
     def _get_sys_path_for_analysis(self) -> Optional[List[str]]:
         return [
-            os.path.join(os.path.dirname(__file__), "esp_32_api_stubs"),
-            os.path.join(os.path.dirname(__file__), "esp_common_api_stubs"),
+            os.path.join(os.path.dirname(__file__), "api_stubs"),
         ] + super()._get_sys_path_for_analysis()
 
 
 if __name__ == "__main__":
-    launch_bare_metal_backend(EspMicroPythonBackend)
+    launch_bare_metal_backend(PrimeInventorMicroPythonBackend)
```

### Comparing `thonny-4.0.2/thonny/plugins/ev3/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/ev3/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/ev3/ev3_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/ev3/ev3_back.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import os.path
 import sys
 from logging import getLogger
 from typing import List, Optional
 
+# make sure thonny folder is in sys.path (relevant in dev)
+thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+if thonny_container not in sys.path:
+    sys.path.insert(0, thonny_container)
+
 import thonny
+from thonny.common import PROCESS_ACK
 from thonny.plugins.micropython.os_mp_backend import SshUnixMicroPythonBackend
 
 logger = getLogger("thonny.plugins.ev3.ev3_back")
 
 
 class EV3MicroPythonBackend(SshUnixMicroPythonBackend):
     def _get_sys_path_for_analysis(self) -> Optional[List[str]]:
@@ -15,13 +21,14 @@
             os.path.join(os.path.dirname(__file__), "api_stubs"),
         ] + super()._get_sys_path_for_analysis()
 
 
 if __name__ == "__main__":
     THONNY_USER_DIR = os.environ["THONNY_USER_DIR"]
     thonny.configure_backend_logging()
+    print(PROCESS_ACK)
 
     import ast
 
     args = ast.literal_eval(sys.argv[1])
 
     EV3MicroPythonBackend(args)
```

### Comparing `thonny-4.0.2/thonny/plugins/event_logging.py` & `thonny-4.1.0b1.dev0/thonny/plugins/event_logging.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/event_view.py` & `thonny-4.1.0b1.dev0/thonny/plugins/event_view.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/files.py` & `thonny-4.1.0b1.dev0/thonny/plugins/files.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/find_replace.py` & `thonny-4.1.0b1.dev0/thonny/plugins/find_replace.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 _active_find_dialog = None
 
 logger = getLogger(__name__)
 
 
 class FindDialog(CommonDialog):
-
     last_searched_word = None
 
     def __init__(self, master):
         padx = 15
         pady = 15
 
         super().__init__(master, skip_tk_dialog_attributes=running_on_mac_os(), takefocus=1)
@@ -208,15 +207,14 @@
             tofind == FindDialog.last_searched_word
             and self.last_processed_indexes is not None
             and self.last_search_case == self._is_search_case_sensitive()
         )
 
     # performs the replace operation - replaces the currently active found word with what is entered in the replace field
     def _perform_replace(self):
-
         # nothing is currently in found status
         if self.active_found_tag == None:
             return
 
         # get the found word bounds
         del_start = self.active_found_tag[0]
         del_end = self.active_found_tag[1]
@@ -247,15 +245,14 @@
         if self.active_found_tag == None:
             return
         self._perform_replace()
         self._perform_find()
 
     # replaces all occurrences of the search string with the replace string
     def _perform_replace_all(self):
-
         tofind = self.find_entry.get()
         if len(tofind) == 0:
             self.infotext_label_var.set(tr("Enter string to be replaced."))
             return
 
         toreplace = self.replace_entry.get()
```

### Comparing `thonny-4.0.2/thonny/plugins/general_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/general_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/goto_definition.py` & `thonny-4.1.0b1.dev0/thonny/plugins/goto_definition.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/heap.py` & `thonny-4.1.0b1.dev0/thonny/plugins/heap.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/help/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/help/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/help/assistant.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/assistant.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 If your program ends with an error, it tries
 to explain it in simpler terms and offers some advice for finding and fixing the underlying problem.
 
 Sometimes your program may not work as you want even if you don't get any error messages. In this case
 sometimes it helps to investigate the code carefully in order to spot certain bad smells or
 peculiarities, which may lead to discovering the problem. There are two popular tools, which are used
-for such investigations: `Pylint <pylint.pycqa.or>`_ and `Mypy <http://mypy-lang.org/>`_.
+for such investigations: `Pylint <pylint.pycqa.org>`_ and `Mypy <http://mypy-lang.org/>`_.
 
 Mypy tries to detect certain contradictions in your code, for example when a function seems to
 expect an integer argument, but your code calls it with a string. Pylint is not as good with this
 kind of checks, but it can do many other checks. The number of Pylint checks is actually so large,
 that most users let it skip many checks they don't find relevant. Thonny has picked a bunch of
 Pylint checks, which are most likely releavant for beginners. If you want more checks, then you
 could run Pylint on your code via command line. If you want to omit certain checks picked by Thonny,
```

### Comparing `thonny-4.0.2/thonny/plugins/help/birdseye.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/birdseye.rst`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 of intermediate values. 
 
 NB! When using Birdseye in Thonny you don't need to import ``birdseye.eye`` or use it 
 for decorating your functions. Thonny executes Birdseye such that it records information about all
 functions.
 
 The local server uses port 7777 by default. If this is used by another application, then configure
-another port (Tools → Options → Debugger) and restart Thonny.
+another port in *Tools → Options → Run & Debug* and restart Thonny.
```

### Comparing `thonny-4.0.2/thonny/plugins/help/debuggers.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/debuggers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 and zoom into this piece of code. (How does it work? Even when you take a big step, Thonny
 saves all intermediate program states, which it can replay after you take the step back.) 
 
 If you want to reach a specific part of the code, then you can speed up the 
 process by placing your cursor on that line and selecting *Run → Run to cursor*. 
 This makes Thonny automatically step until this line. You can take the command from there.
 
-If you have editor line numbers enabled (Tools → Options → Editor), then you can 
+If you have editor line numbers enabled in *Tools → Options → Editor*, then you can 
 also use **breakpoints**. When you click next to a statement in the editor left margin, a dot
 appears. When you now start the debugger, it doesn't stop before first statement but runs to the 
 statement marked with the dot a.k.a breakpoint. You can place as many breakpoints to your programs as 
 required. Breakpoints can be removed by clicking on the margin again.
 
 
 "Faster" mode
@@ -51,14 +51,14 @@
 programmers are accustomed with.
 
 
 Different styles for showing the call stack
 -------------------------------------------
 By default Thonny uses stacked windows for presenting the call stack. This gives good intuition about 
 the concept, but it may become cumbersome to use. Therefore, since version 3.0 one can choose between 
-two different styles for presenting call stack. In “Tools → Options → Debugger” you can switch to more 
+two different styles for presenting call stack. In *Tools → Options → Run & Debug* you can switch to more 
 traditional style with a separate view for presenting and switching call frames. Note that both 
 styles can be used with both debugging modes.
 
 Birdseye
 --------
-Command *Debug current script (Birdseye)* is explained at a `separate page <birdseye.rst>`_
+Command *Debug current script (Birdseye)* is explained at a `separate page <birdseye.rst>`_.
```

### Comparing `thonny-4.0.2/thonny/plugins/help/debugging.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/debugging.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/help/dock.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/dock.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
  
 **Dock user windows** in the **Run menu** is meant to help you in this situation. If you 
 check it and run your Tkinter program, Thonny performs following magic tricks:
 
 * It remembers where you position your window. Next time it places the window at the same position.
 * It makes your window stay on top even if you click on Thonny window to start modifying the code. In fact, after your Tkinter window becomes visible, Thonny automatically focuses its own window so that you can continue editing the script without grabbing the mouse. When you're done, just press F5 again and old window gets replaced with the new one.
  
-*Staying on top currently does not work with turtle programs on macOS (https://github.com/thonny/thonny/issues/798)*
+Staying on top currently does not work with turtle programs on macOS (https://github.com/thonny/thonny/issues/798).
```

### Comparing `thonny-4.0.2/thonny/plugins/help/errors.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/errors.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/help/flask.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/flask.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 just like any other program (with simple F5). If it detects you are running a Flask program, then it executes
 it with some lines of code appended, which start the development server with suitable settings.
 
 Debugging
 ---------
 If you want to step through your Flask program, set a breakpoint inside some function and invoke 
 the debugger (both nicer and faster work, but faster is ... faster). Reload your page and start 
-stepping inside the function. You may want to turn off "Frames in separate windows" (Tools => Options
-=> Run & Debug) for more comfortable operation. 
+stepping inside the function. You may want to turn off "Frames in separate windows" in *Tools → Options
+→ Run & Debug* for more comfortable operation.
 
 Details
 -------
 Thonny will start the development server approximately like this:
 
 .. code::
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `thonny-4.0.2/thonny/plugins/help/index.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/index.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/help/modes.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/modes.rst`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 Regular mode
 ------------
 This is the default mode. Nothing much to say about this.
 
 Simple mode
 -----------
-In this mode the menus are hidden, toolbar buttons have captions and Variables view gets automatically opened. 
+In this mode the menus are hidden and toolbar buttons have captions.
 Use a small link in the upper-right corner of the main window to return to regular mode.
 
 Expert mode
 -----------
 This mode looks almost like regular mode, but has some extra features, which are
 useful for teachers.
 
 * View menu gets an extra item *Full screen* which puts Thonny to full screen.
-* Double clicking on the tab of an editor or view maximizes this editor or view. Unmaximize by double clicking the tab again.
+* Double clicking on the tab of an editor or view maximizes this editor or view. Unmaximize by typing ESC.
 * Tools menu gets an extra item *Open replayer...* which allows replaying user action logs.
```

### Comparing `thonny-4.0.2/thonny/plugins/help/packages.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/packages.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 -------------
 From "Tools" menu select "Manage packages..." and follow the instructions.
 
 With pip on command line
 ------------------------
 #. From "Tools" menu select "Open system shell...". You should get a new terminal window stating the correct name of *pip* command (usually ``pip`` or ``pip3``). In the following I've assumed the command name is ``pip``.
 #. Enter ``pip install <package name>`` (eg. ``pip install pygame``) and press ENTER. You should see *pip* downloading and installing the package and printing a success message.
-#. Close the terminal (optional)
-#. Return to Thonny
-#. Reset interpreter by selecting "Stop/Reset" from "Run menu" (this is required only first time you do pip install)
-#. Start using the package
+#. Close the terminal (optional).
+#. Return to Thonny.
+#. Reset interpreter by selecting "Stop/Restart backend" from "Run" menu (this is required only first time you do pip install).
+#. Start using the package.
 
 .. NOTE::
    The "Open system shell..." menu is not available when running from the Flatpak on Linux.
    Flatpak applications are sandboxed to protect the user's host system and data.
    Allowing Thonny to open a shell on the host system would circumvent these protections.
    To install Python packages from the command-line, please open your system's terminal application directly.
 
@@ -41,11 +41,11 @@
 your platform. Most likely you want graphical installer and 64-bit version (you may need 
 32-bit version if you have very old system).
 
 Install it and find out where it puts Python executable (*pythonw.exe* in Windows and 
 *python3* or *python* in Linux and Mac).
 
 In Thonny open "Tools" menu and select "Options...". In the options dialog open "Interpreter" 
-tab, click "Select executable" and show the location of Anaconda's Python executable.
+tab and show the location of Anaconda's Python executable.
 
 After you have done this, next time you run your program, it will be run through Anaconda's 
 Python and all the libraries installed there are available.
```

### Comparing `thonny-4.0.2/thonny/plugins/help/plotter.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/plotter.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/help/program_arguments.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/program_arguments.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,11 +15,10 @@
 
     import sys
     print(sys.argv)
 
 Fixing the command line arguments
 ---------------------------------
 If you need to use same set of arguments several times, it may become tedious to construct
-the ``%Run`` by hand. In this case check **Program arguments** in the **View menu**. This 
+the ``%Run`` by hand. In this case check **Program arguments** in the **View** menu. This
 opens a small entry box next to the toolbar buttons. From now on, everything you type in this
 box gets appended to ``%Run <script name>`` each time you press F5.
-
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_55m5swun_/tmp68un9zl5_TarContainer/0/305.rst", line 25, column 2: CDATA terminal not found*

 * *File "/tmp/diffoscope_55m5swun_/tmp68un9zl5_TarContainer/0/305.rst", line 25, column 2: CDATA terminal not found*

```diff
@@ -5,10 +5,10 @@
 that script. When you go to shell and take the ``%Run`` command back (with up-
 arrow), you can add *command line arguments* to it. For example change the
 command to ``%Run my_program.py first second`` and press ENTER. When you run
 your program like this, you can access the arguments from ``sys.argv``: ..
 code:: import sys print(sys.argv) Fixing the command line arguments -----------
 ---------------------- If you need to use same set of arguments several times,
 it may become tedious to construct the ``%Run`` by hand. In this case check
-**Program arguments** in the **View menu**. This opens a small entry box next
+**Program arguments** in the **View** menu. This opens a small entry box next
 to the toolbar buttons. From now on, everything you type in this box gets
 appended to ``%Run
```

### Comparing `thonny-4.0.2/thonny/plugins/help/shell.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/shell.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 single-line and multiline. If you press ENTER, then Thonny uses some heuristics to predict 
 whether you wanted to submit the command or continue typing the command on the next line. 
 If you want to submit the command but Thonny offers you a new line, then check whether you forgot
 to close some parentheses.   
 
 Magic commands
 --------------
-If you select "Run => Run current script" or press F5, then you'll see how Thonny inserts a command
+If you select *Run →  Run current script* or press F5, then you'll see how Thonny inserts a command
 starting with ``%Run`` into Shell. Commands starting with ``%`` are called *magic commands* (just 
-like in `IPython <https://ipython.org/>`_ and they perform certain actions, which can't be
+like in `IPython <https://ipython.org/>`_) and they perform certain actions, which can't be
 (easily) expressed as Python commands. Thonny's magic commands usually have
 corresponding menu commands so you don't need write them by hand.
 
 System commands
 ---------------
 If you need to quickly run a simple system command then you don't have to start a Terminal. Just
 prefix the command with ``!`` (eg. ``!pytest my-script.py``) and enter it into Thonny's shell.
@@ -29,15 +29,15 @@
 ---------------
 If you want to issue same or similar command several times, then you don't need to type it each time --
 use Up-key to fetch previous command from the command history. Another Up-press brings you the command
 before that and so on. Use Down-key to move in the opposite direction in history.  
 
 Colored output
 --------------
-If you have your Shell in Terminal emulation mode (see Tools => Options => Shell), then you can
+If you have your Shell in Terminal emulation mode (see *Tools → Options → Shell*), then you can
 use `ANSI codes <https://en.wikipedia.org/wiki/ANSI_escape_code>`_ to produce colored output. 
 
 Try the following example:
 
 .. code::
 
 	print("\033[31m" + "Red" + "\033[m")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `thonny-4.0.2/thonny/plugins/help/turtle.rst` & `thonny-4.1.0b1.dev0/thonny/plugins/help/turtle.rst`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/highlight_names.py` & `thonny-4.1.0b1.dev0/thonny/plugins/highlight_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     def get_positions(self):
         index = self.text.index("insert")
 
         # ignore if cursor in open string
         if self.text.tag_prevrange("open_string", index) or self.text.tag_prevrange(
             "open_string3", index
         ):
-
             return set()
 
         source = self.text.get("1.0", "end")
         index_parts = index.split(".")
         line, column = int(index_parts[0]), int(index_parts[1])
 
         return self.get_positions_for(source, line, column)
```

### Comparing `thonny-4.0.2/thonny/plugins/locals_marker.py` & `thonny-4.1.0b1.dev0/thonny/plugins/locals_marker.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import os.path
 import sys
 import time
 from time import sleep
-from typing import Optional
+from typing import Dict, List, Optional
 
 from thonny import ui_utils
 from thonny.languages import tr
 from thonny.plugins.micropython import (
     BareMetalMicroPythonConfigPage,
     BareMetalMicroPythonProxy,
     add_micropython_backend,
 )
 from thonny.plugins.micropython.mp_common import PASTE_SUBMIT_MODE
-from thonny.plugins.micropython.uf2dialog import TargetInfo, Uf2FlashingDialog
+from thonny.plugins.micropython.uf2dialog import (
+    TargetInfo,
+    Uf2FlashingDialog,
+    create_volume_description,
+)
 
 LATEST_RELEASE_URL = "https://api.github.com/repos/bbcmicrobit/micropython/releases/latest"
 
 
 class MicrobitProxy(BareMetalMicroPythonProxy):
     def _get_backend_launcher_path(self) -> str:
         import thonny.plugins.microbit.microbit_back
@@ -57,41 +61,48 @@
             + "\n\n"
             + tr("Make sure MicroPython has been installed to your micro:bit.")
             + "\n("
             + tr("Don't forget that main.py only works without embedded main script.")
             + ")"
         )
 
-    def _has_flashing_dialog(self):
-        return True
+    def get_flashing_dialog_kinds(self) -> List[str]:
+        return [""]
 
-    def _open_flashing_dialog(self):
+    def _open_flashing_dialog(self, kind: str) -> None:
+        assert kind == ""
         dlg = MicrobitFlashingDialog(self, "MicroPython")
         ui_utils.show_dialog(dlg)
 
 
 class MicrobitFlashingDialog(Uf2FlashingDialog):
     """
     Technically micro:bit doesn't use UF2, but Uf2FlashingDialog is similar enough to be used
     as baseclass here.
     """
 
     def get_variants_url(self) -> str:
         return f"https://raw.githubusercontent.com/thonny/thonny/master/data/{self.firmware_name.lower()}-variants-daplink.json"
 
+    def get_families_mapping(self) -> Dict[str, str]:
+        return {
+            "nRF51": "nrf51",
+            "nRF52": "nrf52",
+        }
+
     def get_instructions(self) -> Optional[str]:
         return (
-            "This dialog allows you to install or update MicroPython on your micro:bit.\n"
+            f"This dialog allows you to install or update {self.firmware_name} on your micro:bit.\n"
             "\n"
             "1. Plug in your micro:bit.\n"
             "2. Wait until device information appears.\n"
             "3. Click 'Install' and wait for some seconds until done.\n"
             "4. Close the dialog and start programming!\n"
             "\n"
-            "NB! Installing MicroPython will erase all files you may have on your\n"
+            f"NB! Installing {self.firmware_name} will erase all files you may have on your\n"
             "device. Make sure you have important files backed up!"
         )
 
     def get_info_file_name(self):
         return "DETAILS.TXT"
 
     def create_target_info(self, path: str) -> Optional[TargetInfo]:
@@ -114,40 +125,42 @@
             id_marker = "Unique ID:"
             for line in fp:
                 if line.startswith(id_marker):
                     board_id = line[len(id_marker) :].strip()[:4]
                     if board_id in models:
                         model, family = models[board_id]
                         return TargetInfo(
-                            title=self.describe_target_path(path),
+                            title=create_volume_description(path),
                             path=path,
                             family=family,
                             model=model,
                             board_id=board_id,
+                            port=None,
                         )
 
             # With older bootloaders, the file may be different
             fp.seek(0)
             for line in fp:
                 if "Version: 0234" in line:
                     board_id = "9900"
                     model, family = models[board_id]
                     return TargetInfo(
-                        title=self.describe_target_path(path),
+                        title=create_volume_description(path),
                         path=path,
                         family=family,
                         model=model,
                         board_id=board_id,
+                        port=None,
                     )
 
         # probably not micro:bit
         return None
 
     def get_title(self):
-        return f"Install {self.firmware_name} for BBC micro:bit"
+        return f"Install or update {self.firmware_name} for BBC micro:bit"
 
     def perform_post_installation_steps(self, ports_before):
         # can't check the ports as in the superclass, because the port is always there
         # simply wait for a couple of seconds, just in case
         self.append_text("\nWaiting for device to restart...\n")
         self.set_action_text("Waiting for device to restart...")
         time.sleep(5)
```

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/audio.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/audio.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/math.py` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/math.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/microbit.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/microbit.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/music.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/music.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/neopixel.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/neopixel.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/os.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/os.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/radio.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/radio.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/random.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/speech.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/speech.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/sys.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/sys.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/uarray.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/uarray.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/ustruct.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/ustruct.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/microbit/api_stubs/utime.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/microbit/api_stubs/utime.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/micropython/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     LocalMicroPythonConfigPage,
     LocalMicroPythonProxy,
     MicroPythonProxy,
     SshMicroPythonConfigPage,
     SshMicroPythonProxy,
     add_micropython_backend,
     list_serial_ports,
-    list_serial_ports_with_descriptions,
 )
 
 
 def load_plugin():
     add_micropython_backend(
         "GenericMicroPython",
         GenericBareMetalMicroPythonProxy,
@@ -52,7 +51,9 @@
     )
     get_workbench().set_default("SshMicroPython.executable", "micropython")
     get_workbench().set_default("SshMicroPython.cwd", None)
     get_workbench().set_default("SshMicroPython.host", "")
     get_workbench().set_default("SshMicroPython.user", "")
     get_workbench().set_default("SshMicroPython.auth_method", "password")
     get_workbench().set_default("SshMicroPython.make_uploaded_shebang_scripts_executable", True)
+
+    get_workbench().set_default("esptool.show_advanced_options", False)
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/bare_metal_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/bare_metal_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 import struct
 import sys
 import time
 from logging import getLogger
 from textwrap import dedent, indent
 from typing import BinaryIO, Callable, List, Optional, Union
 
+# make sure thonny folder is in sys.path (relevant in dev)
+thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+if thonny_container not in sys.path:
+    sys.path.insert(0, thonny_container)
+
 import thonny
 from thonny import report_time
 from thonny.backend import UploadDownloadMixin, convert_newlines_if_has_shebang
 from thonny.common import (
+    PROCESS_ACK,
     BackendEvent,
     EOFCommand,
     OscEvent,
     ToplevelResponse,
     execute_system_command,
     serialize_message,
 )
@@ -34,15 +40,19 @@
     MicroPythonBackend,
     ProtocolError,
     ReadOnlyFilesystemError,
     ends_overlap,
     is_continuation_byte,
     starts_with_continuation_byte,
 )
-from thonny.plugins.micropython.mp_common import PASTE_SUBMIT_MODE, RAW_PASTE_SUBMIT_MODE
+from thonny.plugins.micropython.mp_common import (
+    PASTE_SUBMIT_MODE,
+    RAW_PASTE_SUBMIT_MODE,
+    RAW_SUBMIT_MODE,
+)
 from thonny.plugins.micropython.webrepl_connection import WebReplConnection
 
 RAW_PASTE_COMMAND = b"\x05A\x01"
 RAW_PASTE_CONFIRMATION = b"R\x01"
 RAW_PASTE_CONTINUE = b"\x01"
 
 
@@ -464,15 +474,16 @@
         if self._last_prompt in [
             RAW_PROMPT,
             EOT + RAW_PROMPT,
             FIRST_RAW_PROMPT,
             W600_FIRST_RAW_PROMPT,
         ]:
             return
-        logger.debug("requesting raw mode at %r", self._last_prompt)
+
+        logger.info("Requesting raw mode at %r", self._last_prompt)
 
         # assuming we are currently on a normal prompt
         self._write(RAW_MODE_CMD)
         self._log_output_until_active_prompt()
         if self._last_prompt == NORMAL_PROMPT:
             # Don't know why this happens sometimes (eg. when interrupting a Ctrl+D or restarted
             # program, which is outputting text on ESP32)
@@ -483,33 +494,38 @@
 
         if self._last_prompt not in [FIRST_RAW_PROMPT, W600_FIRST_RAW_PROMPT]:
             logger.error(
                 "Could not enter raw prompt, got %r",
                 self._last_prompt,
             )
             raise ProtocolError("Could not enter raw prompt")
+        else:
+            logger.info("Entered raw prompt")
 
     def _ensure_normal_mode(self, force=False):
         if self._last_prompt == NORMAL_PROMPT and not force:
             return
 
-        logger.debug("requesting normal mode at %r", self._last_prompt)
+        logger.info("Requesting normal mode at %r", self._last_prompt)
         self._write(NORMAL_MODE_CMD)
         self._log_output_until_active_prompt()
         assert self._last_prompt == NORMAL_PROMPT, (
             "Could not get normal prompt, got %s" % self._last_prompt
         )
 
     def _clear_repl(self):
         """NB! assumes prompt and may be called without __thonny_helper"""
         logger.debug("_create_fresh_repl")
         self._ensure_raw_mode()
         self._write(SOFT_REBOOT_CMD)
+        assuming_ok = self._connection.soft_read(2, timeout=0.1)
+        if assuming_ok != OK:
+            logger.warning("Got %r after requesting soft reboot")
         self._check_reconnect()
-        self._log_output_until_active_prompt()
+        self._forward_output_until_active_prompt()
         logger.debug("Done _create_fresh_repl")
 
     def _soft_reboot_for_restarting_user_program(self):
         # Need to go to normal mode. MP doesn't run user code in raw mode
         # (CP does, but it doesn't hurt to do it there as well)
         logger.debug("_soft_reboot_for_restarting_user_program")
         self._ensure_normal_mode()
@@ -543,18 +559,27 @@
         with self._interrupt_lock:
             if self._submit_mode == PASTE_SUBMIT_MODE:
                 self._submit_code_via_paste_mode(to_be_sent)
             elif self._submit_mode == RAW_PASTE_SUBMIT_MODE:
                 try:
                     self._submit_code_via_raw_paste_mode(to_be_sent)
                 except RawPasteNotSupportedError:
-                    logger.info("WARNING: Could not use expected raw paste, falling back to raw")
-                    self._submit_code_via_raw_mode(
-                        to_be_sent, self._infer_write_block_size(), self._infer_write_block_delay()
+                    # raw is safest, as some M5 ESP32-s don't play nice with paste mode,
+                    # even with as small block size as 30 (echo is randomly missing characters)
+                    self._submit_mode = RAW_SUBMIT_MODE
+                    self._write_block_size = self._infer_write_block_size()
+                    self._write_block_delay = self._infer_write_block_delay()
+                    logger.warning(
+                        "Could not use raw_paste, falling back to %s"
+                        + " with write_block_size %s and write_block_delay %s",
+                        self._submit_mode,
+                        self._write_block_size,
+                        self._write_block_delay,
                     )
+                    self._submit_code_via_raw_mode(to_be_sent)
             else:
                 self._submit_code_via_raw_mode(to_be_sent)
 
     def _submit_code_via_paste_mode(self, script_bytes: bytes) -> None:
         # Go to paste mode
         self._ensure_normal_mode()
         self._write(PASTE_MODE_CMD)
@@ -592,23 +617,16 @@
             len(expected_confirmation), timeout=WAIT_OR_CRASH_TIMEOUT
         )
         assert actual_confirmation == expected_confirmation, "Expected %r, got %r" % (
             expected_confirmation,
             actual_confirmation,
         )
 
-    def _submit_code_via_raw_mode(
-        self,
-        script_bytes: bytes,
-        block_size: Optional[int] = None,
-        block_delay: Optional[float] = None,
-    ) -> None:
+    def _submit_code_via_raw_mode(self, script_bytes: bytes) -> None:
         self._ensure_raw_mode()
-        block_size = block_size or self._write_block_size
-        block_delay = block_delay or self._write_block_delay
         to_be_written = script_bytes + EOT
 
         while to_be_written:
             block = self._extract_block_without_splitting_chars(to_be_written)
             self._write(block)
             to_be_written = to_be_written[len(block) :]
             if to_be_written:
@@ -625,24 +643,26 @@
                 "Could not read command confirmation for script\n\n: %s\n\n" "Got: %r",
                 self._decode(script_bytes),
                 data,
             )
             raise ProtocolError("Could not read command confirmation")
 
     def _submit_code_via_raw_paste_mode(self, script_bytes: bytes) -> None:
+        # Occasionally, the device initially supports raw paste but later doesn't allow it (?)
+        # https://github.com/thonny/thonny/issues/1545
+
         self._ensure_raw_mode()
         self._connection.set_text_mode(False)
         self._write(RAW_PASTE_COMMAND)
         response = self._connection.soft_read(2, timeout=WAIT_OR_CRASH_TIMEOUT)
         if response != RAW_PASTE_CONFIRMATION:
-            # Occasionally, the device initially supports raw paste but later doesn't allow it
-            # https://github.com/thonny/thonny/issues/1545
-            time.sleep(0.01)
-            response += self._connection.read_all()
-            if response == FIRST_RAW_PROMPT:
+            # perhaps the device doesn't support raw paste ...
+            response += self._connection.soft_read_until(FIRST_RAW_PROMPT, timeout=0.5)
+            if response.endswith(FIRST_RAW_PROMPT):
+                # ... yup, it doesn't support it
                 self._last_prompt = FIRST_RAW_PROMPT
                 raise RawPasteNotSupportedError()
             else:
                 logger.error("Got %r instead of raw-paste confirmation", response)
                 raise ProtocolError("Could not get raw-paste confirmation")
 
         self._raw_paste_write(script_bytes)
@@ -900,14 +920,15 @@
                     follow_up += self._connection.soft_read_until(ST)
                     if follow_up.endswith(ST):
                         logger.debug("Found OSC sequence %r", follow_up)
                         self.send_message(OscEvent(follow_up.decode("utf-8", errors="replace")))
                     follow_up = b""
 
                 if follow_up:
+                    logger.info("Found inactive prompt followed by %r", follow_up)
                     # Nope, the prompt is not active.
                     # (Actually it may be that a background thread has produced this follow up,
                     # but this would be too hard to consider.)
                     # Don't output yet, because the follow up may turn into another prompt
                     # and they can be captured all together.
                     self._connection.unread(follow_up)
                     # read prompt must remain in pending
@@ -919,15 +940,15 @@
                         for potential_prompt in prompts:
                             if pending.endswith(potential_prompt):
                                 pending = pending[: -len(potential_prompt)]
                         else:
                             break
                     output_consumer(self._decode(pending), stream_name)
                     self._last_prompt = current_prompt
-                    # logger.debug("Found prompt %r", current_prompt)
+                    logger.debug("Found prompt %r", current_prompt)
                     return current_prompt
 
             if pending.endswith(LF):
                 # Maybe it's a penultimate char in a first raw repl?
                 if pending.endswith(FIRST_RAW_PROMPT[:-1]) or pending.endswith(
                     W600_FIRST_RAW_PROMPT[:-1]
                 ):
@@ -984,14 +1005,21 @@
         def collect_output(data, stream):
             logger.info("Discarding %s: %r", stream, data)
 
         self._process_output_until_active_prompt(
             collect_output, interrupt_times=interrupt_times, poke_after=poke_after
         )
 
+    def _forward_output_until_active_prompt(
+        self, interrupt_times: Optional[List[float]] = None, poke_after: Optional[float] = None
+    ) -> None:
+        self._process_output_until_active_prompt(
+            self._send_output, interrupt_times=interrupt_times, poke_after=poke_after
+        )
+
     def _forward_unexpected_output(self, stream_name="stdout"):
         "Invoked between commands"
         # TODO: This should be as careful as _forward_output_until_active_prompt
         data = self._connection.read_all(check_error=False)
         if data:
             met_prompt = False
             while data.endswith(NORMAL_PROMPT) or data.endswith(FIRST_RAW_PROMPT):
@@ -1158,15 +1186,14 @@
 
         logger.info("Read %s in %.1f seconds", source_path, time.time() - start_time)
         return size
 
     def _read_file_via_serial(
         self, source_path: str, target_fp: BinaryIO, callback: Callable[[int, int], None]
     ) -> None:
-
         hex_mode = self._should_hexlify(source_path)
 
         self._execute_without_output(
             "__thonny_fp = __thonny_helper.builtins.open(%r, 'rb')" % source_path
         )
         if hex_mode:
             self._execute_without_output("from binascii import hexlify as __temp_hexlify")
@@ -1691,14 +1718,15 @@
 
 class RawPasteNotSupportedError(RuntimeError):
     pass
 
 
 def launch_bare_metal_backend(backend_class: Callable[..., BareMetalMicroPythonBackend]) -> None:
     thonny.configure_backend_logging()
+    print(PROCESS_ACK)
 
     import ast
 
     args = ast.literal_eval(sys.argv[1])
     logger.info("Starting backend, args: %r", args)
 
     try:
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/micropython/mp_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_back.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 from thonny import BACKEND_LOG_MARKER, get_backend_log_file, report_time
 from thonny.backend import MainBackend
 from thonny.common import (
     OBJECT_LINK_END,
     OBJECT_LINK_START,
     BackendEvent,
     CommandToBackend,
+    CompletionInfo,
     DistInfo,
     EOFCommand,
     ImmediateCommand,
     InlineCommand,
     InlineResponse,
     InputSubmission,
     MessageFromBackend,
@@ -127,16 +128,14 @@
         self._progress_times = {}
         self._welcome_text = None
         self._sys_path = None
         self._epoch_year = None
         self._builtin_modules = []
         self._number_of_interrupts_sent = 0
 
-        self._builtins_info = self._fetch_builtins_info()
-
         MainBackend.__init__(self)
         try:
             report_time("before prepare")
             self._process_until_initial_prompt(
                 interrupt=args.get("interrupt_on_connect", False) or clean, clean=clean
             )
             if self._welcome_text is None:
@@ -341,14 +340,16 @@
 
     def _handle_normal_command(self, cmd: CommandToBackend) -> None:
         logger.debug("Handling normal command '%s' in micropython backend ", cmd.name)
         report_time("before " + cmd.name)
 
         if "local_cwd" in cmd:
             self._local_cwd = cmd["local_cwd"]
+            if os.path.isdir(self._local_cwd):
+                os.chdir(self._local_cwd)
 
         super()._handle_normal_command(cmd)
 
         self._check_perform_just_in_case_gc()
         report_time("after " + cmd.name)
 
     def _check_for_connection_error(self) -> None:
@@ -390,23 +391,14 @@
 
     def _fetch_sys_path(self):
         if not self._supports_directories():
             return []
         else:
             return self._evaluate("__thonny_helper.sys.path")
 
-    def _fetch_builtins_info(self):
-        for stubs_dir in self._get_sys_path_for_analysis():
-            for name in ["builtins.py", "builtins.pyi"]:
-                path = os.path.join(stubs_dir, name)
-                if os.path.exists(path):
-                    return parse_api_information(path)
-
-        return {}
-
     def _fetch_epoch_year(self):
         if self._using_microbit_micropython():
             return None
 
         if self._connected_to_circuitpython() and "rtc" not in self._builtin_modules:
             return self._resolve_unknown_epoch()
 
@@ -715,14 +707,81 @@
                     __thonny_helper.inspector_values[__thonny_helper.builtins.id(__thonny_helper.object_info)] = __thonny_helper.object_info
             """
             )
         )
 
         return {"id": cmd.object_id, "info": info}
 
+    def _cmd_shell_autocomplete(self, cmd):
+        source = cmd.source
+        response = dict(source=cmd.source, row=cmd.row, column=cmd.column, completions=[])
+
+        # First the dynamic completions
+        match = re.search(
+            r"(\w+\.)*(\w+)?$", source
+        )  # https://github.com/takluyver/ubit_kernel/blob/master/ubit_kernel/kernel.py
+        if match:
+            prefix = match.group()
+            if "." in prefix:
+                obj, prefix = prefix.rsplit(".", 1)
+                names = self._evaluate(
+                    "__thonny_helper.builtins.dir({obj}) if '{obj}' in __thonny_helper.builtins.locals() or '{obj}' in __thonny_helper.builtins.globals() else []".format(
+                        obj=obj
+                    )
+                )
+            else:
+                names = self._evaluate("__thonny_helper.builtins.dir()")
+        else:
+            names = []
+            prefix = ""
+
+        # prevent TypeError (iterating over None)
+        names = names if names else []
+
+        for name in names:
+            if name.startswith(prefix) and not name.startswith("__"):
+                response["completions"].append(self._create_shell_completion(name, prefix))
+
+        # add keywords, import modules etc. from jedi
+        try:
+            from thonny import jedi_utils
+
+            # at the moment I'm assuming source is the code before cursor, not whole input
+            lines = source.split("\n")
+            jedi_completions = jedi_utils.get_script_completions(
+                source,
+                len(lines),
+                len(lines[-1]),
+                "<shell>",
+                sys_path=self._get_sys_path_for_analysis(),
+            )
+            response["completions"] += [
+                comp
+                for comp in jedi_completions
+                if (comp.type in ["module", "keyword"] or comp.module_name == "builtins")
+                and self._should_present_completion(comp)
+            ]
+        except Exception as e:
+            logger.exception("Problem with jedi shell autocomplete")
+
+        return response
+
+    def _create_shell_completion(self, name: str, prefix: str) -> CompletionInfo:
+        return CompletionInfo(
+            name=name,
+            name_with_symbols=name,
+            full_name=name,
+            type="name",
+            prefix_length=len(prefix),
+            signatures=None,  # must be queried separately
+            docstring=None,  # must be queried separately
+            module_path=None,
+            module_name=None,
+        )
+
     def _find_basic_object_info(self, object_id, context_id):
         """If object is found then returns basic info and leaves object reference
         to __thonny_helper.object_info.
 
         Can't leave it in a global object, because when querying globals(),
         repr(globals()) would cause infinite recursion."""
 
@@ -1024,36 +1083,36 @@
 
     def _cmd_mkdir(self, cmd):
         assert self._supports_directories()
         assert cmd.path.startswith("/")
         assert not cmd.path.startswith("//")
         self._mkdir(cmd.path)
 
-    def _filter_completions(self, completions):
-        # filter out completions not applicable to MicroPython
-        result = []
-        for completion in completions:
-            if completion.name.startswith("__"):
-                continue
-
-            if completion.parent() and completion.full_name:
-                parent_name = completion.parent().name
-                name = completion.name
-                root = completion.full_name.split(".")[0]
-
-                # jedi proposes names from CPython builtins
-                if root in self._builtins_info and name not in self._builtins_info[root]:
-                    continue
+    def _should_present_completion(self, completion: CompletionInfo) -> bool:
+        if completion.name.startswith("__"):
+            return False
 
-                if parent_name == "builtins" and name not in self._builtins_info:
-                    continue
+        if completion.module_path is None and completion.type == "module":
+            # That's how jedi 0.18 (and maybe later) lists CPython stdlib modules
+            return False
 
-            result.append({"name": completion.name})
+        if completion.module_name == "builtins":
+            # Jedi's builtins.pyi is pretty good
+            return True
 
-        return result
+        if completion.module_path:
+            # if it's in our stubs folder, then it's good
+            for path in self._get_sys_path_for_analysis():
+                if os.path.normcase(completion.module_path).startswith(os.path.normcase(path)):
+                    return True
+
+            # somewhere else, not good
+            return False
+
+        return True
 
     def _get_sys_path_for_analysis(self) -> Optional[List[str]]:
         return [os.path.join(os.path.dirname(__file__), "base_api_stubs")]
 
     def _join_remote_path_parts(self, left, right):
         if left == "":  # micro:bit
             assert not self._supports_directories()
@@ -1347,42 +1406,14 @@
     def __init__(self, msg, script, out, err):
         RuntimeError.__init__(self, msg)
         self.script = script
         self.out = out
         self.err = err
 
 
-def parse_api_information(file_path):
-    import tokenize
-
-    with tokenize.open(file_path) as fp:
-        source = fp.read()
-
-    tree = ast.parse(source)
-
-    defs = {}
-
-    # TODO: read also docstrings ?
-
-    for toplevel_item in tree.body:
-        if isinstance(toplevel_item, ast.ClassDef):
-            class_name = toplevel_item.name
-            member_names = []
-            for item in toplevel_item.body:
-                if isinstance(item, ast.FunctionDef):
-                    member_names.append(item.name)
-                elif isinstance(item, ast.Assign):
-                    # TODO: check Python 3.4
-                    "TODO: item.targets[0].id"
-
-            defs[class_name] = member_names
-
-    return defs
-
-
 def unix_dirname_basename(path):
     if path == "/":
         return ("/", "")
 
     if "/" not in path:  # micro:bit
         return "", path
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/mp_front.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/mp_front.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self._lib_dirs = []
         super().__init__(clean, running.get_front_interpreter_for_subprocess())
 
     def get_pip_gui_class(self):
         return None
 
     def get_pip_target_dir(self) -> Optional[str]:
-
         lib_dirs = self.get_lib_dirs()
         if not lib_dirs:
             return None
 
         for path in lib_dirs:
             if path.startswith("/home/"):
                 return path
@@ -352,15 +351,24 @@
     @classmethod
     def get_switcher_configuration_label(cls, conf: Dict[str, Any]) -> str:
         port = conf[f"{cls.backend_name}.port"]
         if port == WEBREPL_PORT_VALUE:
             url = conf[f"{cls.backend_name}.webrepl_url"]
             return f"{cls.backend_description}  •  {url}"
         else:
-            return f"{cls.backend_description}  •  {port}"
+            try:
+                p = get_port_info(port)
+            except Exception:
+                p = None
+                logger.exception("Could not get port info for %r", port)
+
+            if p:
+                return f"{cls.backend_description}  •  {get_serial_port_label(p)}"
+            else:
+                return f"{cls.backend_description}  •  {port}"
 
     @classmethod
     def get_switcher_entries(cls):
         def should_show(conf):
             port = conf[f"{cls.backend_name}.port"]
             if port == WEBREPL_PORT_VALUE:
                 return True
@@ -442,20 +450,15 @@
             intro_url_label.grid(row=1, column=0, sticky="nw")
 
         port_label = ttk.Label(
             self, text=tr("Port or WebREPL") if self.allow_webrepl else tr("Port")
         )
         port_label.grid(row=3, column=0, sticky="nw", pady=(10, 0))
 
-        self._ports_by_desc = {
-            p.description
-            if p.device in p.description
-            else p.description + " (" + p.device + ")": p.device
-            for p in list_serial_ports()
-        }
+        self._ports_by_desc = {get_serial_port_label(p) for p in list_serial_ports()}
         self._ports_by_desc["< " + tr("Try to detect port automatically") + " >"] = "auto"
 
         self._WEBREPL_OPTION_DESC = "< WebREPL >"
         if self.allow_webrepl:
             self._ports_by_desc[self._WEBREPL_OPTION_DESC] = WEBREPL_PORT_VALUE
 
         def port_order(p):
@@ -514,39 +517,46 @@
         )
 
         last_row = ttk.Frame(self)
         last_row.grid(row=100, sticky="swe")
         self.rowconfigure(100, weight=1)
         last_row.columnconfigure(1, weight=1)
 
-        advanced_link = ui_utils.create_action_label(
-            last_row, tr("Advanced options"), lambda event: self._show_advanced_options()
-        )
-        # advanced_link.grid(row=0, column=1, sticky="e")
+        kinds = self.get_flashing_dialog_kinds()
+        for i, kind in enumerate(kinds):
+
+            def _click_flashing_link(event, kind=kind):
+                self._handle_python_installer_link(kind=kind)
+
+            if i == 0:
+                link_text = self._get_flasher_link_title()
+            else:
+                link_text = ""
+
+            if kind != "":
+                if link_text:
+                    link_text += " "
+                link_text += f"({kind})"
 
-        if self._has_flashing_dialog():
             python_link = ui_utils.create_action_label(
                 last_row,
-                self._get_flasher_link_title(),
-                self._on_click_python_installer_link,
+                link_text,
+                _click_flashing_link,
             )
-            python_link.grid(row=1, column=1, sticky="e")
+            python_link.grid(row=i, column=1, sticky="e")
 
         self._on_change_port()
 
     def _get_flasher_link_title(self) -> str:
         return tr("Install or update %s") % "MicroPython"
 
-    def _on_click_python_installer_link(self, event=None):
-        self._open_flashing_dialog()
+    def _handle_python_installer_link(self, kind: str):
+        self._open_flashing_dialog(kind)
         self._has_opened_python_flasher = True
 
-    def _show_advanced_options(self):
-        pass
-
     def _get_intro_text(self):
         result = (
             tr("Connect your device to the computer and select corresponding port below")
             + "\n"
             + "("
             + tr('look for your device name, "USB Serial" or "UART"')
             + ").\n"
@@ -566,15 +576,14 @@
                     + "< WebREPL > below"
                 )
             )
 
         return result
 
     def _get_webrepl_frame(self):
-
         if self._webrepl_frame is not None:
             return self._webrepl_frame
 
         self._webrepl_frame = ttk.Frame(self)
 
         self._webrepl_url_var = create_string_var(
             get_workbench().get_option(self.backend_name + ".webrepl_url")
@@ -647,18 +656,18 @@
 
     def may_have_rtc(self):
         return True
 
     def _get_intro_url(self) -> Optional[str]:
         return None
 
-    def _has_flashing_dialog(self):
-        return False
+    def get_flashing_dialog_kinds(self) -> List[str]:
+        return []
 
-    def _open_flashing_dialog(self):
+    def _open_flashing_dialog(self, kind: str) -> None:
         raise NotImplementedError()
 
     @property
     def allow_webrepl(self):
         return False
 
 
@@ -957,15 +966,50 @@
         return True
 
 
 class SshMicroPythonConfigPage(BaseSshProxyConfigPage):
     pass
 
 
-def list_serial_ports():
+_PORTS_CACHE = []
+_PORTS_CACHE_TIME = 0
+
+
+def get_serial_port_label(p) -> str:
+    # On Windows, port is given also in description
+    if p.product:
+        desc = p.product
+    elif p.interface:
+        desc = p.interface
+    else:
+        desc = p.description.replace(f" ({p.device})", "")
+
+    if desc == "USB Serial Device":
+        # Try finding something less generic
+        if p.product:
+            desc = p.product
+        elif p.interface:
+            desc = p.interface
+
+    return f"{desc} @ {p.device}"
+
+
+def list_serial_ports(max_cache_age: float = 0.5):
+    global _PORTS_CACHE, _PORTS_CACHE_TIME
+
+    cur_time = time.time()
+    if cur_time - _PORTS_CACHE_TIME > max_cache_age:
+        _PORTS_CACHE = _list_serial_ports_uncached()
+        _PORTS_CACHE_TIME = cur_time
+
+    return _PORTS_CACHE
+
+
+def _list_serial_ports_uncached():
+    logger.info("Listing serial ports")
     # serial.tools.list_ports.comports() can be too slow
     # because os.path.islink can be too slow (https://github.com/pyserial/pyserial/pull/303)
     # Workarond: temporally patch os.path.islink
     old_islink = os.path.islink
     try:
         if sys.platform == "win32":
             os.path.islink = lambda _: False
@@ -986,48 +1030,22 @@
             from serial.tools.list_ports import comports
 
         return comports()
     finally:
         os.path.islink = old_islink
 
 
-def list_serial_port_infos():
-    return [f"{p.device} ({p.hwid})" for p in list_serial_ports()]
-
-
 def port_exists(device):
     for port in list_serial_ports():
         if port.device == device:
             return True
 
     return False
 
 
-def list_serial_ports_with_descriptions():
-    def port_order(p):
-        name = p.device
-        if name is None:
-            return ""
-        elif name.startswith("COM") and len(name) == 4:
-            # Make one-digit COM ports go before COM10
-            return name.replace("COM", "COM0")
-        else:
-            return name
-
-    sorted_ports = sorted(list_serial_ports(), key=port_order)
-
-    return [
-        (
-            p.description if p.device in p.description else p.description + " (" + p.device + ")",
-            p.device,
-        )
-        for p in sorted_ports
-    ]
-
-
 def get_uart_adapter_vids_pids():
     # https://github.com/per1234/zzInoVIDPID
     # https://github.com/per1234/zzInoVIDPID/blob/master/zzInoVIDPID/boards.txt
     # http://esp32.net/usb-uart/
     # https://www.usb.org/developers
     return {
         (0x1A86, 0x7523),  # CH340 (HL-340?)
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/os_mp_backend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/os_mp_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,23 @@
 import sys
 import textwrap
 import time
 from abc import ABC
 from logging import getLogger
 from typing import Callable, Optional, Union
 
+# make sure thonny folder is in sys.path (relevant in dev)
+thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+if thonny_container not in sys.path:
+    sys.path.insert(0, thonny_container)
+
 import thonny
 from thonny import report_time
 from thonny.backend import SshMixin
-from thonny.common import BackendEvent, serialize_message
+from thonny.common import PROCESS_ACK, BackendEvent, serialize_message
 from thonny.plugins.micropython.bare_metal_backend import LF, NORMAL_PROMPT
 from thonny.plugins.micropython.connection import MicroPythonConnection
 from thonny.plugins.micropython.mp_back import (
     ENCODING,
     EOT,
     PASTE_MODE_CMD,
     PASTE_MODE_LINE_PREFIX,
@@ -144,15 +149,15 @@
         # (%Run script.py does not create a new instance of this class)
         output = []
 
         def collect_output(data, stream_name):
             output.append(data)
 
         report_time("befini")
-        self._forward_output_until_active_prompt(collect_output, "stdout")
+        self._process_output_until_active_prompt(collect_output, "stdout")
         self._original_welcome_text = "".join(output).replace("\r\n", "\n")
         self._welcome_text = self._tweak_welcome_text(self._original_welcome_text)
         report_time("afini")
 
     def _fetch_builtin_modules(self):
         return FALLBACK_BUILTIN_MODULES
 
@@ -171,17 +176,17 @@
         end_marker = "#uIuIu"
         self._write(PASTE_MODE_CMD)
         self._connection.read_until(PASTE_MODE_LINE_PREFIX)
         self._write((script + end_marker).encode(ENCODING))
         self._connection.read_until(end_marker.encode("ascii"))
         self._write(EOT)
         self._connection.read_until(b"\n")
-        self._forward_output_until_active_prompt(output_consumer)
+        self._process_output_until_active_prompt(output_consumer)
 
-    def _forward_output_until_active_prompt(
+    def _process_output_until_active_prompt(
         self, output_consumer: Callable[[str, str], None], stream_name="stdout"
     ):
         INCREMENTAL_OUTPUT_BLOCK_CLOSERS = re.compile(
             b"|".join(map(re.escape, [LF, NORMAL_PROMPT]))
         )
 
         pending = b""
@@ -244,15 +249,15 @@
                     "Warning: MicroPython doesn't allow program arguments (%s) together with '-c'"
                     % " ".join(map(shlex.quote, args[1:]))
                 )
             args = ["-c", cmd.source]
 
         self._connection = self._create_connection(args)
         report_time("afconn")
-        self._forward_output_until_active_prompt(self._send_output, "stdout")
+        self._process_output_until_active_prompt(self._send_output, "stdout")
         report_time("afforv")
         self.send_message(
             BackendEvent(event_type="HideTrailingOutput", text=self._original_welcome_text)
         )
         report_time("beffhelp")
         self._prepare_after_soft_reboot()
         report_time("affhelp")
@@ -379,14 +384,15 @@
     def _create_pipkin_adapter(self):
         raise NotImplementedError()
 
 
 if __name__ == "__main__":
     THONNY_USER_DIR = os.environ["THONNY_USER_DIR"]
     thonny.configure_backend_logging()
+    print(PROCESS_ACK)
 
     import ast
 
     args = ast.literal_eval(sys.argv[1])
 
     if "host" in args:
         backend = SshUnixMicroPythonBackend(args)
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/pip_gui.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/pip_gui.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/micropython/serial_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/serial_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 
 logger = getLogger(__name__)
 
 
 class SerialConnection(MicroPythonConnection):
     def __init__(self, port, baudrate=115200, dtr=None, rts=None, skip_reader=False):
-
         import serial
         from serial.serialutil import SerialException
 
         super().__init__()
 
         try:
             self._serial = serial.Serial(
@@ -155,15 +154,14 @@
                     logger.exception("Couldn't close serial")
 
 
 class DifficultSerialConnection(SerialConnection):
     """For hardening the communication protocol"""
 
     def _make_output_available(self, data, block=True):
-
         # output prompts in parts
         if FIRST_RAW_PROMPT in data or NORMAL_PROMPT in data:
             if FIRST_RAW_PROMPT in data:
                 start = data.find(FIRST_RAW_PROMPT)
                 end = start + len(FIRST_RAW_PROMPT)
             else:
                 start = data.find(NORMAL_PROMPT)
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/ssh_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/ssh_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/micropython/subprocess_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/subprocess_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/micropython/uf2dialog.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/base_flashing_dialog.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,215 @@
 import os.path
 import re
-import sys
+import shutil
+import tempfile
 import threading
 import time
 import traceback
 import urllib.request
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from logging import getLogger
 from tkinter import ttk
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Dict, List, Optional, Tuple
 
 from thonny import get_runner
+from thonny.common import UserError
 from thonny.languages import tr
-from thonny.misc_utils import get_win_volume_name, list_volumes
-from thonny.plugins.micropython.mp_front import list_serial_port_infos
 from thonny.ui_utils import AdvancedLabel, MappingCombobox, set_text_if_different
 from thonny.workdlg import WorkDialog
 
 logger = getLogger(__name__)
 
 FAKE_USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_9_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.1916.47 Safari/537.36"
 
+FAMILY_CODES_TO_NAMES = {
+    "rp2": "RP2",
+    "samd21": "SAMD21",
+    "samd51": "SAMD51",
+    "esp8266": "ESP8266",
+    "esp32": "ESP32",
+    "esp32s2": "ESP32-S2",
+    "esp32s3": "ESP32-S3",
+    "esp32c3": "ESP32-C3",
+    "nrf51": "nRF51",
+    "nrf52": "nRF52",
+}
+
 
 @dataclass()
 class TargetInfo:
     title: str
-    path: str
+    path: Optional[str]
     family: Optional[str]
     model: Optional[str]
     board_id: Optional[str]
+    port: Optional[Any]
 
 
-class Uf2FlashingDialog(WorkDialog):
+class BaseFlashingDialog(WorkDialog, ABC):
     def __init__(self, master, firmware_name: str):
         self._downloaded_variants: List[Dict[str, Any]] = []
 
         self._last_handled_target = None
+        self._last_handled_family = None
+        self._last_handled_family_target = None
         self._last_handled_variant = None
         self.firmware_name = firmware_name
 
         threading.Thread(target=self._download_variants, daemon=True).start()
 
         super().__init__(master, autostart=False)
 
+    @abstractmethod
     def get_variants_url(self) -> str:
-        return f"https://raw.githubusercontent.com/thonny/thonny/master/data/{self.firmware_name.lower()}-variants-uf2.json"
+        ...
+
+    @abstractmethod
+    def get_target_label(self) -> str:
+        ...
 
     def populate_main_frame(self):
         epadx = self.get_large_padding()
         ipadx = self.get_small_padding()
         epady = epadx
         ipady = ipadx
 
-        target_label = ttk.Label(self.main_frame, text="Target volume")
+        target_label = ttk.Label(self.main_frame, text=self.get_target_label())
         target_label.grid(row=1, column=1, sticky="e", padx=(epadx, 0), pady=(epady, 0))
         self._target_combo = MappingCombobox(self.main_frame, exportselection=False)
         self._target_combo.grid(
             row=1, column=2, sticky="nsew", padx=(ipadx, epadx), pady=(epady, 0)
         )
+        self._target_combo.bind("<<ComboboxSelected>>", self.register_settings_changed, True)
 
         self._target_info_label = ttk.Label(self.main_frame, text="model")
         self._target_info_label.grid(row=2, column=1, sticky="e", padx=(epadx, 0), pady=(ipady, 0))
         self._target_info_content_label = ttk.Label(self.main_frame)
         self._target_info_content_label.grid(
             row=2, column=2, sticky="w", padx=(ipadx, epadx), pady=(ipady, 0)
         )
 
-        variant_label = ttk.Label(self.main_frame, text=f"{self.firmware_name} variant")
-        variant_label.grid(row=5, column=1, sticky="e", padx=(epadx, 0), pady=(epady, 0))
+        family_label = ttk.Label(self.main_frame, text=f"{self.firmware_name} family")
+        family_label.grid(row=5, column=1, sticky="e", padx=(epadx, 0), pady=(epady, 0))
+        self._family_combo = MappingCombobox(
+            self.main_frame,
+            exportselection=False,
+            state="enabled",
+            mapping=self.get_families_mapping(),
+        )
+        self._family_combo.grid(
+            row=5, column=2, sticky="nsew", padx=(ipadx, epadx), pady=(epady, 0)
+        )
+        self._family_combo.bind("<<ComboboxSelected>>", self.register_settings_changed, True)
+
+        variant_label = ttk.Label(self.main_frame, text=f"variant")
+        variant_label.grid(row=6, column=1, sticky="e", padx=(epadx, 0), pady=(ipady, 0))
         self._variant_combo = MappingCombobox(
             self.main_frame, exportselection=False, state="disabled"
         )
         self._variant_combo.grid(
-            row=5, column=2, sticky="nsew", padx=(ipadx, epadx), pady=(epady, 0)
+            row=6, column=2, sticky="nsew", padx=(ipadx, epadx), pady=(ipady, 0)
         )
+        self._variant_combo.bind("<<ComboboxSelected>>", self.register_settings_changed, True)
 
         version_label = ttk.Label(self.main_frame, text="version")
-        version_label.grid(row=6, column=1, sticky="e", padx=(epadx, 0), pady=(ipady, 0))
+        version_label.grid(row=7, column=1, sticky="e", padx=(epadx, 0), pady=(ipady, 0))
         self._version_combo = MappingCombobox(
             self.main_frame, exportselection=False, state="disabled"
         )
         self._version_combo.grid(
-            row=6, column=2, sticky="nsew", padx=(ipadx, epadx), pady=(ipady, 0)
+            row=7, column=2, sticky="nsew", padx=(ipadx, epadx), pady=(ipady, 0)
         )
+        self._version_combo.bind("<<ComboboxSelected>>", self.register_settings_changed, True)
 
         variant_info_label = ttk.Label(self.main_frame, text="info")
-        variant_info_label.grid(row=7, column=1, sticky="e", padx=(epadx, 0), pady=(ipady, 0))
+        variant_info_label.grid(row=8, column=1, sticky="e", padx=(epadx, 0), pady=(ipady, 0))
         self._variant_info_content_label = AdvancedLabel(self.main_frame)
         self._variant_info_content_label.grid(
-            row=7, column=2, sticky="w", padx=(ipadx, epadx), pady=(ipady, 0)
+            row=8, column=2, sticky="w", padx=(ipadx, epadx), pady=(ipady, 0)
         )
 
         self.main_frame.columnconfigure(2, weight=1)
 
+    @abstractmethod
+    def get_families_mapping(self) -> Dict[str, str]:
+        ...
+
     def update_ui(self):
+        for widget in self.main_frame.winfo_children():
+            if isinstance(widget, (ttk.Combobox, ttk.Checkbutton)):
+                if self._state == "working" or not self._downloaded_variants:
+                    widget.state(["disabled", "readonly"])
+                else:
+                    widget.state(["!disabled", "readonly"])
+
         if self._state == "idle":
             targets = self.find_targets()
             if targets != self._target_combo.mapping:
                 self.show_new_targets(targets)
                 self._last_handled_target = None
+                self._last_handled_family_target = None
 
             current_target = self._target_combo.get_selected_value()
-            if not current_target:
-                self._variant_combo.set_mapping({})
-                self._variant_combo.select_none()
-            elif current_target != self._last_handled_target and self._downloaded_variants:
-                self._variant_combo.state(["!disabled", "readonly"])
-                self._version_combo.state(["!disabled", "readonly"])
-                self._present_variants_for_target(current_target)
+            if current_target != self._last_handled_target:
+                if current_target.family:
+                    self._family_combo.select_value(current_target.family)
+                self._update_target_info()
                 self._last_handled_target = current_target
-                self._last_handled_variant = None
-            self._update_target_info()
+                self._last_handled_family_target = None
+
+            current_family = self._family_combo.get_selected_value()
+            if self._last_handled_family != current_family:
+                logger.debug(
+                    "Changing family from %r to %r", self._last_handled_family, current_family
+                )
+                self.on_change_family(current_family)
+                if self._downloaded_variants:
+                    # not handled yet if still downloading
+                    self._last_handled_family = current_family
+
+            if self._last_handled_family_target != (current_family, current_target):
+                if current_family and current_target and self._downloaded_variants:
+                    self._try_preselect_a_variant(current_target)
+                    self._last_handled_family_target = (current_family, current_target)
 
             current_variant = self._variant_combo.get_selected_value()
-            if not current_variant:
-                self._version_combo.select_none()
-                self._version_combo.set_mapping({})
-            elif current_variant != self._last_handled_variant:
-                self._present_versions_for_variant(current_variant)
+            if current_variant != self._last_handled_variant:
+                if not current_variant:
+                    self._version_combo.select_none()
+                    self._version_combo.set_mapping({})
+                else:
+                    self._present_versions_for_variant(current_variant)
                 self._last_handled_variant = current_variant
+
+            # always updating the multipurpose label
             self._update_variant_info()
 
         super().update_ui()
 
+    @abstractmethod
     def find_targets(self) -> Dict[str, TargetInfo]:
-        paths = [
-            vol
-            for vol in list_volumes(skip_letters=["A"])
-            if os.path.isfile(os.path.join(vol, self.get_info_file_name()))
-        ]
-
-        result = {}
-        for path in paths:
-            try:
-                target_info = self.create_target_info(path)
-                if target_info:
-                    result[target_info.title] = target_info
-            except:
-                # the disk may have been ejected during read or smth like this
-                logger.exception("Could not create target info")
-
-        return result
+        ...
 
     def show_new_targets(self, targets: Dict[str, TargetInfo]) -> None:
         self._target_combo.set_mapping(targets)
         if len(targets) == 1:
             self._target_combo.select_value(list(targets.values())[0])
         else:
             self._target_combo.select_none()
 
+    @abstractmethod
+    def compute_target_info_text_and_label(self, target: TargetInfo) -> Tuple[str, str]:
+        ...
+
     def _update_target_info(self):
         current_target = self._target_combo.get_selected_value()
         if current_target is not None:
-            if current_target.model:
-                if current_target.model == "Raspberry Pi RP2":
-                    # too general to be called model
-                    text = "RP2"
-                    label = "family"
-                else:
-                    text = current_target.model
-                    label = "model"
-            elif current_target.board_id:
-                text = current_target.board_id
-                label = "board id"
-            elif current_target.family:
-                text = current_target.family
-                label = "family"
-            else:
-                text = "Unknown board"
-                label = "info"
+            text, label = self.compute_target_info_text_and_label(current_target)
 
         elif not self._target_combo.mapping:
             text = "[no suitable targets detected]"
             label = ""
         else:
             text = f"[found {len(self._target_combo.mapping)} targets, please select one]"
             label = ""
@@ -194,31 +231,26 @@
         else:
             url = None
             text = ""
 
         set_text_if_different(self._variant_info_content_label, text)
         self._variant_info_content_label.set_url(url)
 
-    def _present_variants_for_target(self, target: TargetInfo) -> None:
-        assert self._downloaded_variants
+    def on_change_family(self, family: Optional[str]) -> None:
+        self._variant_combo.select_none()
 
-        whole_mapping = {self._create_variant_description(v): v for v in self._downloaded_variants}
+        if not family or not self._downloaded_variants:
+            self._variant_combo.set_mapping({})
+            return
 
-        if target.family is not None:
-            filtered_mapping = {
-                item[0]: item[1]
-                for item in whole_mapping.items()
-                if item[1]["family"].startswith(target.family)
-            }
-            if not filtered_mapping:
-                filtered_mapping = whole_mapping
-        else:
-            filtered_mapping = whole_mapping
+        whole_mapping = {self._create_variant_description(v): v for v in self._downloaded_variants}
 
-        prev_variant = self._variant_combo.get_selected_value()
+        filtered_mapping = {
+            item[0]: item[1] for item in whole_mapping.items() if item[1]["family"] == family
+        }
 
         populars = {
             key: variant
             for key, variant in filtered_mapping.items()
             if variant.get("popular", False)
         }
         if populars and len(populars) < len(filtered_mapping):
@@ -232,103 +264,46 @@
 
             enhanced_mapping["--- ALL VARIANTS " + "-" * 100] = {}
             enhanced_mapping.update(filtered_mapping)
         else:
             enhanced_mapping = filtered_mapping
 
         self._variant_combo.set_mapping(enhanced_mapping)
-        matches = list(
-            filter(
-                lambda v: self._variant_is_meant_for_target(v, target), filtered_mapping.values()
-            )
-        )
+
+    def _try_preselect_a_variant(self, target: TargetInfo) -> None:
+        assert self._downloaded_variants
+        assert target
+
+        matches = []
+        for v in self._variant_combo.mapping.values():
+            if v and v not in matches and self._variant_can_be_recommended_for_target(v, target):
+                matches.append(v)
 
         if len(matches) == 1:
             self._variant_combo.select_value(matches[0])
-        elif prev_variant and prev_variant in filtered_mapping.values():
-            self._variant_combo.select_value(prev_variant)
 
     def _present_versions_for_variant(self, variant: Dict[str, Any]) -> None:
         versions_mapping = {d["version"]: d for d in variant["downloads"]}
         self._version_combo.set_mapping(versions_mapping)
         if len(versions_mapping) > 0:
             self._version_combo.select_value(list(versions_mapping.values())[0])
         else:
             self._version_combo.select_none()
 
     def _create_variant_description(self, variant: Dict[str, Any]) -> str:
-        return variant["vendor"] + " • " + variant.get("title", variant["model"])
-
-    def _variant_is_meant_for_target(self, variant: Dict[str, Any], target: TargetInfo):
-        if target.family is None:
-            # Don't assume anything about unknown targets
-            return False
-
-        if not variant["family"].startswith(target.family):
-            return False
-
-        if target.model is None:
-            return False
-
-        # Compare set of words both with and without considering the possibility that one of them
-        # may have vendor name added and other not.
-        return self._extract_normalized_words(target.model) == self._extract_normalized_words(
-            variant["model"]
-        ) or self._extract_normalized_words(
-            target.model + " " + variant["vendor"]
-        ) == self._extract_normalized_words(
-            variant["model"] + " " + variant["vendor"]
-        )
-
-    def _extract_normalized_words(self, text: str) -> Set[str]:
-        return set(text.replace("_", " ").replace("-", "").lower().split())
-
-    def describe_target_path(self, path: str) -> str:
-        if sys.platform == "win32":
-            try:
-                label = get_win_volume_name(path)
-                disk = path.strip("\\")
-                return f"{label} ({disk})"
-            except:
-                logger.error("Could not query volume name for %r", path)
-                return path
-        else:
-            return path
-
-    def create_target_info(self, path: str) -> Optional[TargetInfo]:
-        info_path = os.path.join(path, self.get_info_file_name())
-        assert os.path.isfile(info_path)
-        with open(info_path, encoding="utf-8") as fp:
-            info_content = fp.read()
-        info_lines = info_content.splitlines()
-        normalized_content = info_content.lower().replace(" ", "").replace("_", "").replace("-", "")
-
-        model = find_uf2_property(info_lines, "Model")
-        board_id = find_uf2_property(info_lines, "Board-ID")
+        result = variant.get("vendor", "")
+        if result:
+            result += " • "
 
-        if "boardid:rpirp2" in normalized_content:
-            family = "rp2"
-        else:
-            for keyword in ["samd21", "samd51", "nrf51", "nrf52", "esp32s3", "esp32s3"]:
-                if keyword in normalized_content:
-                    family = keyword
-                    break
-            else:
-                family = None
-
-        return TargetInfo(
-            title=self.describe_target_path(path),
-            path=path,
-            family=family,
-            model=model,
-            board_id=board_id,
-        )
+        result += variant.get("title", variant["model"])
+        return result
 
-    def get_info_file_name(self):
-        return "INFO_UF2.TXT"
+    @abstractmethod
+    def _variant_can_be_recommended_for_target(self, variant: Dict[str, Any], target: TargetInfo):
+        ...
 
     def _download_variants(self):
         logger.info("Downloading %r", self.get_variants_url())
         import json
         from urllib.request import urlopen
 
         try:
@@ -350,26 +325,32 @@
             msg = f"Could not download variants info from {self.get_variants_url()}"
             logger.exception(msg)
             self.append_text(msg + "\n")
             self.set_action_text("Error!")
             self.grid_progress_widgets()
             return
 
-        self._downloaded_variants = variants
+        if self._downloaded_variants:
+            # it looks like the user already got ahead of us by browsing a local file
+            logger.warning("Ignoring downloaded variants as variants already present")
+            return
+        else:
+            logger.debug("Assigning self._downloaded_variants")
+            self._downloaded_variants = variants
 
     def _tweak_variants(self, variants):
         """
         A hack for getting the latest pre-release for micropython.org downloads.
         The build that is loaded from the json may already be deleted.
         In order to avoid adding another async operation into the process (after selecting
         a variant and before presenting versions), I'm getting the latest build substring
         from the download page of the first board and downloading it together with the json.
         """
         latest_prerelease_substitute = None
-        latest_prerelease_regex: str
+        latest_prerelease_regex: Optional[str] = None
         for variant in variants:
             new_regex = variant.get("latest_prerelease_regex", None)
             if new_regex:
                 latest_prerelease_regex = new_regex
                 import json
                 import urllib.request
 
@@ -412,99 +393,95 @@
                         logger.debug("Replacing %r with %r", download["url"], patched_url)
                         download["url"] = patched_url
                         download["version"] = latest_prerelease_substitute
 
     def get_ok_text(self):
         return tr("Install")
 
-    def get_instructions(self) -> Optional[str]:
-        return (
-            f"Here you can install or update {self.firmware_name} for devices having an UF2 bootloader\n"
-            "(this includes most boards meant for beginners).\n"
-            "\n"
-            "1. Put your device into bootloader mode: \n"
-            "     - some devices have to be plugged in while holding the BOOTSEL button,\n"
-            "     - some require double-tapping the RESET button with proper rythm.\n"
-            "2. Wait for couple of seconds until the target volume appears.\n"
-            "3. Select desired variant and version.\n"
-            "4. Click 'Install' and wait for some seconds until done.\n"
-            "5. Close the dialog and start programming!"
-        )
-
-    def _on_variant_select(self, *args):
-        pass
-
-    def get_title(self):
-        return f"Install {self.firmware_name}"
-
     def is_ready_for_work(self):
         return self._target_combo.get_selected_value() and self._version_combo.get_selected_value()
 
     def start_work(self):
         from thonny.plugins.micropython import BareMetalMicroPythonProxy
 
+        variant_info: Dict[str, Any] = self._variant_combo.get_selected_value()
         download_info: Dict[str, Any] = self._version_combo.get_selected_value()
-        assert download_info
-        target: TargetInfo = self._target_combo.get_selected_value()
-        assert target
-
-        target_filename = download_info.get("filename", download_info["url"].split("/")[-1])
+        target_info: TargetInfo = self._target_combo.get_selected_value()
 
         self.report_progress(0, 100)
         proxy = get_runner().get_backend_proxy()
         if isinstance(proxy, BareMetalMicroPythonProxy):
             proxy.disconnect()
 
+        work_options = self.prepare_work_get_options()
+        self.clear_log()
         threading.Thread(
-            target=self._perform_work,
-            args=[
-                download_info["url"],
-                download_info.get("size", None),
-                target.path,
-                target_filename,
-            ],
+            target=self._perform_work_and_update_status,
+            args=[variant_info, download_info, target_info, work_options],
             daemon=True,
         ).start()
         return True
 
-    def _perform_work(
-        self, download_url: str, size: Optional[int], target_dir: str, target_filename: str
-    ) -> None:
-        from thonny.plugins.micropython import list_serial_ports
+    def prepare_work_get_options(self) -> Dict[str, Any]:
+        return {}
 
+    def _perform_work_and_update_status(
+        self,
+        variant_info: Dict[str, Any],
+        download_info: Dict[str, str],
+        target_info: TargetInfo,
+        work_options: Dict[str, Any],
+    ) -> None:
+        temp_file = None
         try:
-            ports_before = list_serial_port_infos()
-            logger.debug("Ports before: %s", ports_before)
-            self._download_to_the_device(download_url, size, target_dir, target_filename)
-            if self._state == "working":
-                self.perform_post_installation_steps(ports_before)
+            if download_info:
+                temp_file = self._download_to_temp(download_info)
+            else:
+                temp_file = None
+
+            core_result = self.perform_core_operation(
+                temp_file, variant_info, download_info, target_info, work_options
+            )
         except Exception as e:
-            self.append_text("\n" + "".join(traceback.format_exc()))
+            if isinstance(e, UserError):
+                self.append_text("\n" + str(e))
+            else:
+                self.append_text("\n" + "".join(traceback.format_exc()))
             self.set_action_text("Error...")
             self.report_done(False)
             return
+        finally:
+            if temp_file:
+                os.remove(temp_file)
 
-        if self._state == "working":
-            self.append_text("\nDone!\n")
+        if core_result:
             self.set_action_text("Done!")
-            self.report_done(True)
         else:
-            assert self._state == "cancelling"
-            self.append_text("\nCancelled\n")
-            self.set_action_text("Cancelled")
-            self.report_done(False)
+            self.set_action_text("Error...")
 
-    def _download_to_the_device(
-        self, download_url: str, size: Optional[int], target_dir: str, target_filename: str
-    ):
-        from urllib.request import urlopen
+        self.report_done(core_result)
 
+    def _download_to_temp(self, download_info: Dict[str, str]) -> Optional[str]:
         """Running in a bg thread"""
+        from urllib.request import urlopen
+
+        target_dir = tempfile.mkdtemp()
+        target_filename = download_info.get("filename", download_info["url"].split("/")[-1])
+        download_url = download_info["url"]
+        size = download_info.get("size", None)
+
         target_path = os.path.join(target_dir, target_filename)
-        logger.debug("Downloading from %s to %s", download_url, target_path)
+
+        url_protocol = download_url.split(":")[0].lower()
+        if url_protocol not in ["http", "https"]:
+            logger.debug("Copying local file %r", download_url)
+            shutil.copyfile(download_url, target_path)
+            return target_path
+
+        logger.debug("Downloading from %s", download_url)
 
         self.set_action_text("Starting...")
         self.append_text("Downloading from %s\n" % download_url)
 
         req = urllib.request.Request(
             download_url,
             data=None,
@@ -523,85 +500,53 @@
             if fsrc.length:
                 # override (possibly inaccurate) size
                 size = fsrc.length
 
             block_size = 8 * 1024
             with open(target_path, "wb") as fdst:
                 while True:
-
                     block = fsrc.read(block_size)
                     if not block:
                         break
 
                     if self._state == "cancelling":
-                        break
+                        raise UserError("Cancelled download per user request")
 
                     fdst.write(block)
                     bytes_copied += len(block)
-                    fdst.flush()
-                    try:
-                        # May fail after last block
-                        os.fsync(fdst.fileno())
-                    except Exception:
-                        if bytes_copied == size:
-                            logger.warning("Could not fsync last block")
-                        else:
-                            logger.exception("Could not fsync")
-                    percent_str = "%.0f%%" % (bytes_copied / size * 100)
-                    self.set_action_text("Copying... " + percent_str)
-                    self.report_progress(bytes_copied, size)
-                    self.replace_last_line(percent_str)
-
-    def _wait_for_new_ports(self, old_ports):
-        from thonny.plugins.micropython import list_serial_ports
+                    percent_done = bytes_copied / size * 100
+                    percent_str = "%.0f%%" % (percent_done)
+                    self.set_action_text("Downloading... " + percent_str)
 
-        self.append_text("\nWaiting for the port...\n")
-        self.set_action_text("Waiting for the port...")
+                    # leaving left half of the progressbar for downloading
+                    self.report_progress(percent_done, 200)
+                    self.replace_last_line(percent_str)
 
-        wait_time = 0
-        step = 0.2
-        while wait_time < 10:
-            new_ports = list_serial_port_infos()
-            added_ports = set(new_ports) - set(old_ports)
-            if added_ports:
-                for p in added_ports:
-                    self.append_text("Found port %s\n" % p)
-                    self.set_action_text("Found port")
-                return
-            if self._state == "cancelling":
-                return
-            time.sleep(step)
-            wait_time += step
-        else:
-            logger.debug("Ports after: %s", list_serial_port_infos())
-            self.set_action_text("Warning: Could not find port")
-            self.append_text("Warning: Could not find port in %s seconds\n" % int(wait_time))
-            # leave some time to see the warning
-            time.sleep(2)
+        return target_path
 
-    def perform_post_installation_steps(self, ports_before):
-        self._wait_for_new_ports(ports_before)
+    @abstractmethod
+    def perform_core_operation(
+        self,
+        source_path: Optional[str],
+        variant_info: Optional[Dict[str, Any]],
+        download_info: Optional[Dict[str, str]],
+        target_info: Optional[TargetInfo],
+        work_options: Dict[str, Any],
+    ) -> bool:
+        ...
+
+    def register_settings_changed(self, event=None):
+        if self._state == "done":
+            self.allow_new_work()
 
 
 def find_uf2_property(lines: List[str], prop_name: str) -> Optional[str]:
     marker = prop_name + ": "
     for line in lines:
         if line.startswith(marker):
             return line[len(marker) :]
 
     return None
 
 
-def show_uf2_installer(master, firmware_name: str) -> None:
-    dlg = Uf2FlashingDialog(master, firmware_name=firmware_name)
-    from thonny import ui_utils
-
-    ui_utils.show_dialog(dlg)
-
-
-def uf2_device_is_present_in_bootloader_mode() -> bool:
-    for vol in list_volumes(skip_letters=["A"]):
-        info_path = os.path.join(vol, "INFO_UF2.TXT")
-        if os.path.isfile(info_path):
-            return True
-
-    return False
+def family_code_to_name(code: str) -> str:
+    return FAMILY_CODES_TO_NAMES.get(code, code)
```

### Comparing `thonny-4.0.2/thonny/plugins/micropython/webrepl_connection.py` & `thonny-4.1.0b1.dev0/thonny/plugins/micropython/webrepl_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Problem with block size:
     https://github.com/micropython/micropython/issues/2497
     Start with conservative delay.
     Client may later reduce it for better efficiency
     """
 
     def __init__(self, url, password, num_bytes_received=0):
-
         self.num_bytes_received = num_bytes_received
         super().__init__()
 
         try:
             import websockets  # @UnusedImport
         except:
             print(
```

### Comparing `thonny-4.0.2/thonny/plugins/misc_analyzers.py` & `thonny-4.1.0b1.dev0/thonny/plugins/misc_analyzers.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,14 @@
             return
 
         library_modules = known_stdlib_modules | self._get_3rd_party_modules()
 
         for item in os.listdir(main_file_dir):
             full_path = os.path.join(main_file_dir, item)
             if item.endswith(".py") and item[:-3] in library_modules:
-
                 if is_same_path(full_path, main_file_path):
                     prelude = "Your program file is named '%s'." % item
                     rename_hint = " (*File → Rename…* )"
                 else:
                     prelude = (
                         "Your working directory `%s <%s>`__ contains a file named '%s'.\n\n"
                         % (rst_utils.escape(main_file_dir), rst_utils.escape(main_file_dir), item)
```

### Comparing `thonny-4.0.2/thonny/plugins/mypy/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/notes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/notes.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/object_inspector.py` & `thonny-4.1.0b1.dev0/thonny/plugins/object_inspector.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,14 @@
         self.text.configure(background="white")
         self.text.tag_configure("read", foreground="lightgray")
 
     def applies_to(self, object_info):
         return "file_content" in object_info or "file_error" in object_info
 
     def set_object_info(self, object_info):
-
         if "file_content" not in object_info:
             logger.exception("File error: " + object_info["file_error"])
             return
 
         assert "file_content" in object_info
         content = object_info["file_content"]
         line_count_sep = len(content.split("\n"))
```

### Comparing `thonny-4.0.2/thonny/plugins/outline.py` & `thonny-4.1.0b1.dev0/thonny/plugins/outline.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/paren_matcher.py` & `thonny-4.1.0b1.dev0/thonny/plugins/paren_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,14 @@
             self._tokens_cache[(start_index, end_index)] = result
 
         return result
 
 
 class ShellParenMatcher(ParenMatcher):
     def _update_highlighting_for_active_range(self):
-
         # TODO: check that cursor is in this range
         index_parts = self.text.tag_prevrange("command", "end")
 
         if index_parts:
             start_index, end_index = index_parts
             self._highlight(start_index, end_index)
```

### Comparing `thonny-4.0.2/thonny/plugins/pgzero_frontend.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pgzero_frontend.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,14 @@
 
     if options:
         for name in ["TkDefaultFont", "TkMenuFont", "TkTextFont", "TkHeadingFont"]:
             font.nametofont(name).configure(**options)
 
 
 def load_plugin():
-
     # set custom images
     if get_workbench().get_ui_mode() == "simple" and get_workbench().winfo_screenwidth() >= 1280:
         images = {
             "run-current-script": "media-playback-start48.png",
             "stop": "process-stop48.png",
             "new-file": "document-new48.png",
             "open-file": "document-open48.png",
```

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run-cursor.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run-cursor48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-run48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-run48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-into.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-into48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-into48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-out.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-out48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-out48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-over.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_debug-step-over48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_debug-step-over48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-new48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-new48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-open.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-open48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-open48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-save.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_document-save48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_document-save48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_media-playback-start.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_media-playback-start48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_media-playback-start48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_process-stop.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_process-stop48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_process-stop48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_quit.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_quit48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_quit48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_resume.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_resume48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_resume48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_window-close-act.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_window-close-act.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_zoom.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/_disabled_zoom48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/_disabled_zoom48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-run-cursor.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-run-cursor48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run-cursor48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-run.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-run48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-run48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-step-into.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-step-into48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-into48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-step-out.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-step-out48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-out48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-step-over.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/debug-step-over48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/debug-step-over48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/document-new48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-new48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/document-open.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/document-open48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-open48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/document-save.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/document-save48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/document-save48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/media-playback-start.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/media-playback-start48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/media-playback-start48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/process-stop.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/process-stop48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/process-stop48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/quit.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/quit48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/quit48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/resume.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/resume48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/resume48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-down-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-down.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-down.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-left-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-left.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-left.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-right-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-right.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-right.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-up-insens.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up-insens.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/scrollbar-button-up.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/scrollbar-button-up.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/window-close-act.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/window-close-act.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/zoom.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pi/res/zoom48.png` & `thonny-4.1.0b1.dev0/thonny/plugins/pi/res/zoom48.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pip_gui.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pip_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     def get_upgrade_button_text(self):
         return tr("Upgrade")
 
     def get_uninstall_button_text(self):
         return tr("Uninstall")
 
     def _create_widgets(self, parent):
-
         header_frame = ttk.Frame(parent)
         header_frame.grid(
             row=1,
             column=0,
             sticky="nsew",
             padx=self.get_medium_padding(),
             pady=(self.get_medium_padding(), 0),
@@ -866,15 +865,14 @@
             return None
         else:
             return dist.version
 
     def _get_active_dist(self, name):
         normname = self._normalize_name(name)
         for key in self._active_distributions:
-
             if self._normalize_name(key) == normname:
                 return self._active_distributions[key]
 
         return None
 
     def _run_pip_with_dialog(
         self, command: str, args: List[str], title: str
@@ -1424,15 +1422,14 @@
     import urllib.parse
 
     url = "https://pypi.org/search/?q={}".format(urllib.parse.quote(query))
 
     url_future = _fetch_url_future(url)
 
     def poll_fetch_complete():
-
         if url_future.done():
             try:
                 _, bin_data = url_future.result()
                 raw_data = bin_data.decode("UTF-8")
                 completion_handler(query, _extract_search_results(raw_data))
             except Exception as e:
                 completion_handler(query, str(e))
```

### Comparing `thonny-4.0.2/thonny/plugins/prime_inventor/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,14 @@
     def _get_backend_launcher_path(self) -> str:
         import thonny.plugins.prime_inventor.prime_inventor_back
 
         return thonny.plugins.prime_inventor.prime_inventor_back.__file__
 
 
 class PrimeInventorMicroPythonConfigPage(BareMetalMicroPythonConfigPage):
-    def _has_flashing_dialog(self):
-        return False
-
     def _get_intro_text(self):
         return "Instructions:"
 
     def _get_intro_url(self):
         return "https://github.com/thonny/thonny/wiki/InventorPrime"
 
     def may_have_rtc(self):
```

### Comparing `thonny-4.0.2/thonny/plugins/prime_inventor/api_stubs/hub.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/prime_inventor/api_stubs/hub.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/prime_inventor/prime_inventor_back.py` & `thonny-4.1.0b1.dev0/thonny/plugins/esp/esp_back.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import os.path
 import sys
 from logging import getLogger
 from typing import List, Optional
 
-import thonny
+# make sure thonny folder is in sys.path (relevant in dev)
+thonny_container = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(__file__))))
+if thonny_container not in sys.path:
+    sys.path.insert(0, thonny_container)
+
 from thonny.plugins.micropython.bare_metal_backend import (
     BareMetalMicroPythonBackend,
     launch_bare_metal_backend,
 )
 
-logger = getLogger("thonny.plugins.prime_inventor.prime_inventor_back")
+# Can't use __name__, because it will be "__main__"
+logger = getLogger("thonny.plugins.micropython.esp_backend")
 
 
-class PrimeInventorMicroPythonBackend(BareMetalMicroPythonBackend):
+class EspMicroPythonBackend(BareMetalMicroPythonBackend):
     def _get_sys_path_for_analysis(self) -> Optional[List[str]]:
         return [
-            os.path.join(os.path.dirname(__file__), "api_stubs"),
+            os.path.join(os.path.dirname(__file__), "esp_32_api_stubs"),
+            os.path.join(os.path.dirname(__file__), "esp_common_api_stubs"),
         ] + super()._get_sys_path_for_analysis()
 
 
 if __name__ == "__main__":
-    launch_bare_metal_backend(PrimeInventorMicroPythonBackend)
+    launch_bare_metal_backend(EspMicroPythonBackend)
```

### Comparing `thonny-4.0.2/thonny/plugins/printing/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/printing/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/printing/template.html` & `thonny-4.1.0b1.dev0/thonny/plugins/printing/template.html`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pylint/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pylint/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pylint/messages.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pylint/messages.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/pythontutor.py` & `thonny-4.1.0b1.dev0/thonny/plugins/pythontutor.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/remove_old_data_dir.py` & `thonny-4.1.0b1.dev0/thonny/plugins/remove_old_data_dir.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/replayer.py` & `thonny-4.1.0b1.dev0/thonny/plugins/replayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
 
 class ReplayerEditorNotebook(ttk.Notebook):
     def __init__(self, master):
         ttk.Notebook.__init__(self, master, padding=0)
         self._editors_by_text_widget_id = {}
 
     def clear(self):
-
         for child in self.winfo_children():
             child.destroy()
 
         self._editors_by_text_widget_id = {}
 
     def get_editor_by_text_widget_id(self, text_widget_id):
         if text_widget_id not in self._editors_by_text_widget_id:
```

### Comparing `thonny-4.0.2/thonny/plugins/rp2040/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/rp2040/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from logging import getLogger
+from typing import List
 
 from thonny.plugins.micropython import add_micropython_backend
 from thonny.plugins.micropython.mp_common import RAW_PASTE_SUBMIT_MODE
 from thonny.plugins.micropython.mp_front import (
     BareMetalMicroPythonConfigPage,
     BareMetalMicroPythonProxy,
     get_uart_adapter_vids_pids,
@@ -34,18 +35,19 @@
 
     @classmethod
     def get_vids_pids_to_avoid(self):
         return get_uart_adapter_vids_pids() | VIDS_PIDS_TO_AVOID_IN_RP2040
 
 
 class RP2040BackendConfigPage(BareMetalMicroPythonConfigPage):
-    def _has_flashing_dialog(self):
-        return True
+    def get_flashing_dialog_kinds(self) -> List[str]:
+        return [""]
 
-    def _open_flashing_dialog(self):
+    def _open_flashing_dialog(self, kind: str) -> None:
+        assert kind == ""
         show_uf2_installer(self, firmware_name="MicroPython")
 
 
 def load_plugin():
     add_micropython_backend(
         "RP2040",
         RP2040BackendProxy,
```

### Comparing `thonny-4.0.2/thonny/plugins/rp2040/api_stubs/rp2.pyi` & `thonny-4.1.0b1.dev0/thonny/plugins/rp2040/api_stubs/rp2.pyi`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/rpi_pico/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/rpi_pico/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/run_debug_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/run_debug_config_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,31 @@
 
 
 class RunDebugConfigurationPage(ConfigurationPage):
     def __init__(self, master):
         super().__init__(master)
 
         self.add_checkbox(
+            "run.allow_running_unnamed_programs",
+            tr("Allow running unnamed programs"),
+            row=3,
+            columnspan=3,
+        )
+
+        self.add_checkbox(
             "run.auto_cd",
             tr("Change working directory to script directory on Run / Debug"),
             row=5,
             columnspan=3,
+        )
+        self.add_checkbox(
+            "run.warn_module_shadowing",
+            tr("Warn if a user module shadows a library module"),
+            row=6,
+            columnspan=3,
             pady=(0, 20),
         )
 
         self.add_checkbox(
             "debugger.frames_in_separate_windows",
             tr("Show function calls (frames) in separate windows"),
             tooltip=tr("Uncheck if you want more traditional experience."),
```

### Comparing `thonny-4.0.2/thonny/plugins/shell_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/shell_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/shell_macro.py` & `thonny-4.1.0b1.dev0/thonny/plugins/shell_macro.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         self._create_widgets()
 
         self.bind("<Escape>", self._on_close, True)
         self.protocol("WM_DELETE_WINDOW", self._on_close)
         self.main_command_text.focus_set()
 
     def _create_widgets(self):
-
         bg = "#ffff99"
         banner_frame = tk.Frame(self, background=bg)
         banner_frame.grid(row=0, column=0, sticky="nsew")
         banner_frame.rowconfigure(0, weight=1)
         banner_frame.columnconfigure(0, weight=1)
         banner_text = tk.Label(
             banner_frame,
```

### Comparing `thonny-4.0.2/thonny/plugins/statement_boxes.py` & `thonny-4.1.0b1.dev0/thonny/plugins/statement_boxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import thonny
 from thonny import get_workbench
 from thonny.codeview import get_syntax_options_for_tag
 
 
 def create_bitmap_file(width, height, predicate, name):
-
     cache_dir = os.path.join(thonny.THONNY_USER_DIR, "image_cache")
     name = "%s_%d_%d.xbm" % (name, width, height)
     filename = os.path.join(cache_dir, name)
 
     # if os.path.exists(filename):
     #    return filename
 
@@ -154,15 +153,14 @@
     last_col = 0
 
     def tag_tree(node):
         nonlocal last_line, last_col
         from parso.python import tree as python_tree
 
         if node.type == "simple_stmt" or isinstance(node, (python_tree.Flow, python_tree.Scope)):
-
             start_line, start_col = node.start_pos
             end_line, end_col = node.end_pos
 
             # Before dealing with this node,
             # handle the case, where last vertical tag was meant for
             # same column, but there were empty or comment lines between
             if start_col == last_col:
@@ -176,15 +174,14 @@
 
             print(node)
 
             # usually end_col is 0
             # exceptions: several statements on the same line (semicoloned statements)
             # also unclosed parens in if-header
             for lineno in range(start_line, end_line if end_col == 0 else end_line + 1):
-
                 top = lineno == start_line and lineno > 1
                 bottom = False  # start_line == end_line-1
 
                 # horizontal line (only for first or last line)
                 if top or bottom:
                     text.tag_add(
                         "hor_%s_%s" % (top, bottom),
```

### Comparing `thonny-4.0.2/thonny/plugins/stdlib_error_helpers.py` & `thonny-4.1.0b1.dev0/thonny/plugins/stdlib_error_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
                         token.NEWLINE,
                         token.ENDMARKER,
                         token.COLON,  # colon may be OP
                         token.RBRACE,
                     ]
                     and self.tokens[i].string != ":"
                 ):
-
                     old_i = i
                     if self.tokens[i].string in "([{":
                         i = self._skip_braced_part(i)
                         assert i > old_i
                         if i == len(self.tokens):
                             return None
                     else:
@@ -159,15 +158,14 @@
         pass
 
     def _skip_braced_part(self, token_index):
         assert self.tokens[token_index].string in ["(", "[", "{"]
         level = 1
         token_index += 1
         while token_index < len(self.tokens):
-
             if self.tokens[token_index].string in ["(", "[", "{"]:
                 level += 1
             elif self.tokens[token_index].string in [")", "]", "}"]:
                 level -= 1
 
             token_index += 1
 
@@ -267,15 +265,14 @@
             "Did you actually mean string (text)?",
             'If you didn\'t mean a variable but literal text "%s", then surround it with quotes.'
             % self.name,
             relevance,
         )
 
     def _sug_bad_spelling(self):
-
         # Yes, it would be more proper to consult builtins from the backend,
         # but it's easier this way...
         all_names = {name for name in dir(builtins) if not name.startswith("_")}
         all_names |= {"pass", "break", "continue", "return", "yield"}
 
         if self.last_frame.globals is not None:
             all_names |= set(self.last_frame.globals.keys())
@@ -492,15 +489,14 @@
         self.suggestions = [
             self._sug_wrong_attribute_instead_of_len(),
             self._sug_bad_spelling(),
             self._sug_bad_type(),
         ]
 
     def _sug_wrong_attribute_instead_of_len(self):
-
         if self.type_name == "str":
             goal = "length"
         elif self.type_name == "bytes":
             goal = "number of bytes"
         elif self.type_name == "list":
             goal = "number of elements"
         elif self.type_name == "tuple":
```

### Comparing `thonny-4.0.2/thonny/plugins/system_shell/__init__.py` & `thonny-4.1.0b1.dev0/thonny/plugins/system_shell/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/system_shell/explain_environment.py` & `thonny-4.1.0b1.dev0/thonny/plugins/system_shell/explain_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 def is_private_exe(p):
     pdir = os.path.dirname(p)
     return os.path.exists(os.path.join(pdir, "thonny_python.ini"))
 
 
 def list_commands(prefix, highlighted_reals, highlighted_dirs):
-    for suffix in ["", "3", "3.8", "3.9", "3.10", "3.11"]:
+    for suffix in ["", "3", "3.8", "3.9", "3.10", "3.11", "3.12"]:
         cmd = prefix + suffix
         import shutil
 
         target = shutil.which(cmd)
         if target is not None:
             target = os.path.abspath(target)
             target = normpath_with_actual_case(target)
```

### Comparing `thonny-4.0.2/thonny/plugins/terminal_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/terminal_config_page.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/theme_and_font_config_page.py` & `thonny-4.1.0b1.dev0/thonny/plugins/theme_and_font_config_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from thonny.languages import tr
 from thonny.shell import BaseShellText
 from thonny.ui_utils import create_string_var, scrollbar_style
 
 
 class ThemeAndFontConfigurationPage(ConfigurationPage):
     def __init__(self, master):
-
         ConfigurationPage.__init__(self, master)
 
         self._init_themes()
         self._init_fonts()
         self._init_previews()
 
         self.columnconfigure(2, weight=1)
```

### Comparing `thonny-4.0.2/thonny/plugins/thonny_folders.py` & `thonny-4.1.0b1.dev0/thonny/plugins/thonny_folders.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/todo_view.py` & `thonny-4.1.0b1.dev0/thonny/plugins/todo_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 logger = getLogger(__name__)
 
 INFO_TEXT = "---"
 
 
 class TodoView(ui_utils.TreeFrame):
     def __init__(self, master):
-
         ui_utils.TreeFrame.__init__(
             self,
             master,
             columns=("line_no", "todo_text"),
             displaycolumns=(0, 1),
         )
 
@@ -77,15 +76,14 @@
 
             self._current_code_view.text.after_idle(delay_update)
 
         else:
             self._update(event)
 
     def _update(self, event):
-
         if not self.winfo_ismapped():
             return
 
         editor = get_workbench().get_editor_notebook().get_current_editor()
 
         if editor is None:
             self._current_code_view = None
@@ -101,15 +99,15 @@
         self.clear()
 
         self._current_code_view = new_codeview
         self._current_source = new_source
 
         # todo support of other file types and introducing comment tags
 
-        r_ex = r"^.*((#[\t ]*(TODO|BUG|FIXME|ERROR|NOTE|REMARK)([:\t ]*))(.*))$"
+        r_ex = r"^.*((#.*[\t ]*(TODO|BUG|FIXME|ERROR|NOTE|REMARK)([:\t ]*))(.*))$"
         r_match = re.compile(r_ex, re.IGNORECASE | re.MULTILINE)
 
         line_no = 0
         for line in new_source.splitlines():
             line_no += 1
             matches = r_match.finditer(line)
             if matches:
```

### Comparing `thonny-4.0.2/thonny/plugins/tomorrow_syntax_theme.py` & `thonny-4.1.0b1.dev0/thonny/plugins/tomorrow_syntax_theme.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/plugins/variables.py` & `thonny-4.1.0b1.dev0/thonny/plugins/variables.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/16x16-blank.gif` & `thonny-4.1.0b1.dev0/thonny/res/16x16-blank.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/1x1-white.gif` & `thonny-4.1.0b1.dev0/thonny/res/1x1-white.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/Ukraine_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/Ukraine_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_create_disabled_variants.py` & `thonny-4.1.0b1.dev0/thonny/res/_create_disabled_variants.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_16x16-blank.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_16x16-blank.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_1x1-white.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_1x1-white.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_arrow-down.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_arrow-down.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_birdseye.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_birdseye.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_broken.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_broken.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_closed-folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_closed-folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_debug-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_debug-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_debug-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_delete.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_delete.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_generic-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_generic-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_hard-drive.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_hard-drive.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_harddisk.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_harddisk_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_harddisk_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_help.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_help.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_help_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_help_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_information.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_information.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_information_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_information_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_nav-backward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-backward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_nav-forward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_nav-forward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_new-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_new-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_open-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_open-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_open_folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_open_folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_outline-class.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_outline-class_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-class_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_outline-method.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_outline-method.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_python-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_python-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_python-icon.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_python-icon.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_quit_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_quit_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_resume_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_resume_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_run-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_run-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_run-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_run-to-cursor_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_run-to-cursor_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_save-file_2x_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_2x_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_save-file_Linux.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_save-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_save-file_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_save-file_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_star.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_star.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_star_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_star_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_step-into_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-into_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_step-out_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-out_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_step-over.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_step-over_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_step-over_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_stop.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_stop_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_stop_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_tab-close-active-clam-dark.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam-dark.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_tab-close-active-clam.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active-clam.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_tab-close-active.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-active.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_tab-close-clam.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close-clam.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_tab-close.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_tab-close.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_terminal_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_terminal_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_text-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_text-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/_disabled_thonny.png` & `thonny-4.1.0b1.dev0/thonny/res/_disabled_thonny.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/arrow-down.gif` & `thonny-4.1.0b1.dev0/thonny/res/arrow-down.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/birdseye.png` & `thonny-4.1.0b1.dev0/thonny/res/birdseye.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/boxminus_light.png` & `thonny-4.1.0b1.dev0/thonny/res/boxminus_light.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/boxplus_light.png` & `thonny-4.1.0b1.dev0/thonny/res/boxplus_light.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/broken.png` & `thonny-4.1.0b1.dev0/thonny/res/broken.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/closed-folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/closed-folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/debug-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/debug-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/debug-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/debug-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/delete.gif` & `thonny-4.1.0b1.dev0/thonny/res/delete.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/hard-drive.gif` & `thonny-4.1.0b1.dev0/thonny/res/hard-drive.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/harddisk.png` & `thonny-4.1.0b1.dev0/thonny/res/harddisk.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/harddisk_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/harddisk_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/help.png` & `thonny-4.1.0b1.dev0/thonny/res/help.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/help_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/help_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/information.png` & `thonny-4.1.0b1.dev0/thonny/res/information.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/information_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/information_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/nav-backward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/nav-backward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/nav-forward_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/nav-forward_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/new-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/new-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/open-file.png` & `thonny-4.1.0b1.dev0/thonny/res/open-file.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/open-file_Linux.png` & `thonny-4.1.0b1.dev0/thonny/res/open-file_Linux.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/open-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/open-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/open_folder.gif` & `thonny-4.1.0b1.dev0/thonny/res/open_folder.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/outline-class.png` & `thonny-4.1.0b1.dev0/thonny/res/outline-class.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/outline-class_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/outline-class_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/outline-method.gif` & `thonny-4.1.0b1.dev0/thonny/res/outline-method.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/python-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/python-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/python-icon.gif` & `thonny-4.1.0b1.dev0/thonny/res/python-icon.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/python-icon_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/python-icon_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/quit.png` & `thonny-4.1.0b1.dev0/thonny/res/quit.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/quit_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/quit_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/resume.png` & `thonny-4.1.0b1.dev0/thonny/res/resume.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/resume_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/resume_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/run-current-script.png` & `thonny-4.1.0b1.dev0/thonny/res/run-current-script.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/run-current-script_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/run-current-script_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/save-file.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/save-file_2x_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_2x_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/save-file_Linux.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_Linux.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/save-file_Linux_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_Linux_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/save-file_alt.png` & `thonny-4.1.0b1.dev0/thonny/res/save-file_alt.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/star.png` & `thonny-4.1.0b1.dev0/thonny/res/star.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/star_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/star_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/step-into_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/step-into_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/step-out_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/step-out_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/step-over_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/step-over_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/stop.png` & `thonny-4.1.0b1.dev0/thonny/res/stop.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/stop_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/stop_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/tab-close-clam.gif` & `thonny-4.1.0b1.dev0/thonny/res/tab-close-clam.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/tab-close.gif` & `thonny-4.1.0b1.dev0/thonny/res/tab-close.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/terminal.png` & `thonny-4.1.0b1.dev0/thonny/res/terminal.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/terminal_2x.png` & `thonny-4.1.0b1.dev0/thonny/res/terminal_2x.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/text-file.gif` & `thonny-4.1.0b1.dev0/thonny/res/text-file.gif`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/thonny.ico` & `thonny-4.1.0b1.dev0/thonny/res/thonny.ico`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/thonny.png` & `thonny-4.1.0b1.dev0/thonny/res/thonny.png`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/res/thonny_small.ico` & `thonny-4.1.0b1.dev0/thonny/res/thonny_small.ico`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/roughparse.py` & `thonny-4.1.0b1.dev0/thonny/roughparse.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/rst_utils.py` & `thonny-4.1.0b1.dev0/thonny/rst_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from thonny.ui_utils import get_hyperlink_cursor
 
 logger = getLogger(__name__)
 
 
 class RstText(TweakableText):
     def __init__(self, master=None, cnf={}, read_only=False, **kw):
-
         super().__init__(
             master=master,
             cnf=cnf,
             read_only=read_only,
             **{
                 "font": "TkDefaultFont",
                 # "cursor" : "",
```

### Comparing `thonny-4.0.2/thonny/running.py` & `thonny-4.1.0b1.dev0/thonny/running.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     get_runner,
     get_shell,
     get_version,
     get_workbench,
     report_time,
 )
 from thonny.common import (
+    PROCESS_ACK,
     BackendEvent,
     CommandToBackend,
     DebuggerCommand,
     DebuggerResponse,
     EOFCommand,
     InlineCommand,
     InlineResponse,
@@ -89,18 +90,54 @@
 OSC_TERMINATOR = re.compile(r"\a|\x1B\\")
 
 # other components may turn it on in order to avoid grouping output lines into one event
 io_animation_required = False
 
 _console_allocated = False
 
+BASE_MODULES = [
+    "_abc",
+    "_codecs",
+    "_collections_abc",
+    "_distutils_hack",
+    "_frozen_importlib",
+    "_frozen_importlib_external",
+    "_imp",
+    "_io",
+    "_signal",
+    "_sitebuiltins",
+    "_stat",
+    "_thread",
+    "_warnings",
+    "_weakref",
+    "_winapi",
+    "abc",
+    "builtins",
+    "codecs",
+    "encodings",
+    "genericpath",
+    "io",
+    "marshal",
+    "nt",
+    "ntpath",
+    "os",
+    "site",
+    "stat",
+    "sys",
+    "time",
+    "winreg",
+    "zipimport",
+]
+
 
 class Runner:
     def __init__(self) -> None:
+        get_workbench().set_default("run.allow_running_unnamed_programs", True)
         get_workbench().set_default("run.auto_cd", True)
+        get_workbench().set_default("run.warn_module_shadowing", True)
 
         self._init_commands()
         self._state = "starting"
         self._proxy: Optional[BackendProxy] = None
         self._publishing_events = False
         self._polling_after_id = None
         self._postponed_commands = []  # type: List[CommandToBackend]
@@ -318,15 +355,14 @@
         self._proxy.send_program_input(data)
 
     def execute_via_shell(
         self,
         cmd_line: Union[str, List[str]],
         working_directory: Optional[str] = None,
     ) -> None:
-
         if working_directory and self._proxy.get_cwd() != working_directory:
             # create compound command
             # start with %cd
             cd_cmd_line = construct_cd_command(working_directory) + "\n"
         else:
             # create simple command
             cd_cmd_line = ""
@@ -347,15 +383,15 @@
         rel_filename = universal_relpath(script_path, working_directory)
         cmd_parts = ["%" + command_name, rel_filename] + args
         cmd_line = construct_cmd_line(cmd_parts, [EDITOR_CONTENT_TOKEN])
 
         self.execute_via_shell(cmd_line, working_directory)
 
     def execute_editor_content(self, command_name, args):
-        if command_name.lower() == "debug":
+        if command_name.lower() in ["debug", "fastdebug"]:
             messagebox.showinfo(
                 tr("Information"),
                 tr("For debugging the program must be saved first."),
                 master=get_workbench(),
             )
             return
 
@@ -407,15 +443,17 @@
                     return
 
         editor = get_workbench().get_editor_notebook().get_current_editor()
         if not editor:
             return
 
         UNTITLED = "<untitled>"
-        if editor.get_filename():
+        if editor.get_filename() or not get_workbench().get_option(
+            "run.allow_running_unnamed_programs"
+        ):
             filename = editor.save_file()
             if not filename:
                 # user has cancelled file saving
                 return
         else:
             filename = UNTITLED
 
@@ -1016,30 +1054,29 @@
         self._response_queue = collections.deque()
 
         if not os.path.exists(self._mgmt_executable):
             get_shell().print_error(
                 f"Interpreter {self._mgmt_executable!r} not found.\nPlease select another!"
             )
             return
-            # raise UserError(
-            #    "Interpreter (%s) not found. Please recheck corresponding option!"
-            #    % self._mgmt_executable
-            # )
 
         cmd_line = (
             [
                 self._mgmt_executable,
                 "-u",  # unbuffered IO
                 "-B",  # don't write pyo/pyc files
                 # (to avoid problems when using different Python versions without write permissions)
             ]
             + self._get_launcher_with_args()
             + extra_args
         )
 
+        if self.can_be_isolated():
+            cmd_line.insert(1, "-I")
+
         creationflags = 0
         if running_on_windows():
             creationflags = subprocess.CREATE_NEW_PROCESS_GROUP
 
         logger.info("Starting the backend: %s %s", cmd_line, get_workbench().get_local_cwd())
 
         self._proc = subprocess.Popen(
@@ -1052,25 +1089,38 @@
             cwd=self._get_launch_cwd(),
             env=self._get_environment(),
             universal_newlines=True,
             creationflags=creationflags,
             encoding="utf-8",
         )
 
-        self._send_initial_input()
+        # read success acknowledgement
+        ack = self._proc.stdout.readline()
 
         # setup asynchronous output listeners
         Thread(target=self._listen_stdout, args=(self._proc.stdout,), daemon=True).start()
         Thread(target=self._listen_stderr, args=(self._proc.stderr,), daemon=True).start()
 
+        # only attempt initial input if process started nicely,
+        # otherwise can't read the error from stderr
+        if ack.strip() == PROCESS_ACK:
+            self._send_initial_input()
+        else:
+            get_shell().print_error(
+                f"INTERNAL ERROR, got {ack!r} instead of {PROCESS_ACK!r}\n---\n"
+            )
+
     def _send_initial_input(self) -> None:
+        # Used for sending data sending for startup, which can't be send by other means
+        # (e.g. don't want the password to end up in logs)
+
         pass
 
     def _get_launch_cwd(self):
-        return self.get_cwd() if self.uses_local_filesystem() else None
+        return get_workbench().get_local_cwd()
 
     def _get_launcher_with_args(self):
         raise NotImplementedError()
 
     def send_command(self, cmd: CommandToBackend) -> Optional[str]:
         """Send the command to backend. Return None, 'discard' or 'postpone'"""
         if isinstance(cmd, ToplevelCommand) and cmd.name[0].isupper():
@@ -1238,14 +1288,18 @@
 
     def get_cwd(self):
         return self._cwd
 
     def get_exe_dirs(self):
         return self._exe_dirs
 
+    def can_be_isolated(self) -> bool:
+        """Says whether the backend may be launched with -I switch"""
+        return True
+
     def fetch_next_message(self):
         if not self._response_queue or len(self._response_queue) == 0:
             if self.is_terminated():
                 raise BackendTerminatedError(self._proc.returncode if self._proc else None)
             else:
                 return None
 
@@ -1335,15 +1389,14 @@
     stdin=None,
     stdout=subprocess.PIPE,
     stderr=subprocess.STDOUT,
     shell=False,
     env=None,
     universal_newlines=True,
 ):
-
     cmd = [python_exe] + args
 
     if running_on_windows():
         creationflags = subprocess.CREATE_NEW_PROCESS_GROUP
         startupinfo = subprocess.STARTUPINFO()
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
     else:
```

### Comparing `thonny-4.0.2/thonny/shell.py` & `thonny-4.1.0b1.dev0/thonny/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,15 +1177,14 @@
 
             self._submit_input(submittable_text)
 
     def _editing_allowed(self):
         return get_runner() is not None
 
     def _extract_submittable_input(self, input_text, tail):
-
         if get_runner().is_waiting_toplevel_command():
             if input_text.endswith("\n"):
                 if input_text.strip().startswith("%") or input_text.strip().startswith("!"):
                     # if several magic command are submitted, then take only first
                     return input_text[: input_text.index("\n") + 1]
                 elif self._code_is_ready_for_submission(input_text, tail):
                     return input_text
@@ -1499,15 +1498,14 @@
                         webbrowser.open(url)
 
         except Exception as e:
             logger.exception("Could not handle hyperlink click", exc_info=e)
 
     def _show_user_exception(self, user_exception):
         for line, frame_id, *_ in user_exception["items"]:
-
             tags = ("io", "stderr")
             if frame_id is not None:
                 frame_tag = "frame_%d" % frame_id
 
                 def handle_frame_click(event, frame_id=frame_id):
                     get_runner().send_command(InlineCommand("get_frame_info", frame_id=frame_id))
                     return "break"
@@ -1969,15 +1967,14 @@
 
         # raise certain elements above segments
         self.tag_raise("tick")
         self.tag_raise("close")
         return count
 
     def draw_segment(self, color, pos, nums):
-
         x = self.x_padding_left + pos * self.x_scale
 
         args = []
         for num in nums:
             y = self.y_padding + (self.range_end - num) * self.y_scale
             args.extend([x, y])
             x += self.x_scale
```

### Comparing `thonny-4.0.2/thonny/terminal.py` & `thonny-4.1.0b1.dev0/thonny/terminal.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/test/plugins/test_locals_marker.py` & `thonny-4.1.0b1.dev0/thonny/test/plugins/test_locals_marker.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 def joo():
     global num_cars
     num_cars = 2
 """
 
 
 def test_regular_closed():
-
     expected_local = {("5.4", "5.12"), ("6.10", "6.18"), ("6.21", "6.29")}
 
     text_widget = tkinter.Text()
     text_widget.insert("end", TEST_STR1)
 
     highlighter = LocalsHighlighter(text_widget)
```

### Comparing `thonny-4.0.2/thonny/test/plugins/test_name_highlighter.py` & `thonny-4.1.0b1.dev0/thonny/test/plugins/test_name_highlighter.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/test/test_common.py` & `thonny-4.1.0b1.dev0/thonny/test/test_common.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/tktextext.py` & `thonny-4.1.0b1.dev0/thonny/tktextext.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,14 @@
     def on_secondary_click(self, event=None):
         "Use this for invoking context menu"
         self.focus_set()
         if event:
             self.mark_set("insert", "@%d,%d" % (event.x, event.y))
 
     def _reload_theme_options(self, event=None):
-
         style = ttk.Style()
 
         states = []
         if self.is_read_only():
             states.append("readonly")
 
         # Following crashes when a combobox is focused
@@ -1170,15 +1169,14 @@
 
     def _reload_theme_options(self, event=None):
         super()._reload_theme_options(event)
         if self._gutter is not None:
             self._reload_gutter_theme_options(event)
 
     def _reload_gutter_theme_options(self, event=None):
-
         style = ttk.Style()
         background = style.lookup("GUTTER", "background")
         if background:
             self._gutter.configure(background=background, selectbackground=background)
             self._margin_line.configure(background=background)
 
         foreground = style.lookup("GUTTER", "foreground")
```

### Comparing `thonny-4.0.2/thonny/token_utils.py` & `thonny-4.1.0b1.dev0/thonny/token_utils.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/ui_utils.py` & `thonny-4.1.0b1.dev0/thonny/ui_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2821,2369 +2821,2389 @@
 0000b040: 2020 2020 7365 6c66 2e74 6578 742e 6469      self.text.di
 0000b050: 7265 6374 5f69 6e73 6572 7428 2265 6e64  rect_insert("end
 0000b060: 222c 2063 6861 7273 2c20 7461 6773 290a  ", chars, tags).
 0000b070: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
 0000b080: 7272 656e 745f 6368 6172 7320 2b3d 2063  rrent_chars += c
 0000b090: 6861 7273 0a0a 2020 2020 6465 6620 706c  hars..    def pl
 0000b0a0: 6163 6528 7365 6c66 2c20 7461 7267 6574  ace(self, target
-0000b0b0: 2c20 666f 6375 733d 4e6f 6e65 293a 0a0a  , focus=None):..
-0000b0c0: 2020 2020 2020 2020 2320 436f 6d70 7574          # Comput
-0000b0d0: 6520 7468 6520 6172 6561 2074 6861 7420  e the area that 
-0000b0e0: 7769 6c6c 2062 6520 6465 7363 7269 6265  will be describe
-0000b0f0: 6420 6279 2074 6869 7320 4e6f 7465 0a20  d by this Note. 
-0000b100: 2020 2020 2020 2066 6f63 7573 5f78 203d         focus_x =
-0000b110: 2074 6172 6765 742e 7769 6e66 6f5f 726f   target.winfo_ro
-0000b120: 6f74 7828 290a 2020 2020 2020 2020 666f  otx().        fo
-0000b130: 6375 735f 7920 3d20 7461 7267 6574 2e77  cus_y = target.w
-0000b140: 696e 666f 5f72 6f6f 7479 2829 0a20 2020  info_rooty().   
-0000b150: 2020 2020 2066 6f63 7573 5f68 6569 6768       focus_heigh
-0000b160: 7420 3d20 7461 7267 6574 2e77 696e 666f  t = target.winfo
-0000b170: 5f68 6569 6768 7428 290a 0a20 2020 2020  _height()..     
-0000b180: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000b190: 2866 6f63 7573 2c20 5465 7874 5261 6e67  (focus, TextRang
-0000b1a0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000b1b0: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
-0000b1c0: 6528 7461 7267 6574 2c20 746b 2e54 6578  e(target, tk.Tex
-0000b1d0: 7429 0a20 2020 2020 2020 2020 2020 2074  t).            t
-0000b1e0: 6f70 6c65 6674 203d 2074 6172 6765 742e  opleft = target.
-0000b1f0: 6262 6f78 2822 2564 2e25 6422 2025 2028  bbox("%d.%d" % (
-0000b200: 666f 6375 732e 6c69 6e65 6e6f 2c20 666f  focus.lineno, fo
-0000b210: 6375 732e 636f 6c5f 6f66 6673 6574 2929  cus.col_offset))
-0000b220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000b230: 666f 6375 732e 656e 645f 636f 6c5f 6f66  focus.end_col_of
-0000b240: 6673 6574 203d 3d20 303a 0a20 2020 2020  fset == 0:.     
-0000b250: 2020 2020 2020 2020 2020 2062 6f74 7269             botri
-0000b260: 6768 7420 3d20 7461 7267 6574 2e62 626f  ght = target.bbo
-0000b270: 7828 0a20 2020 2020 2020 2020 2020 2020  x(.             
-0000b280: 2020 2020 2020 2022 2564 2e25 6420 6c69         "%d.%d li
-0000b290: 6e65 656e 6422 2025 2028 666f 6375 732e  neend" % (focus.
-0000b2a0: 656e 645f 6c69 6e65 6e6f 202d 2031 2c20  end_lineno - 1, 
-0000b2b0: 666f 6375 732e 656e 645f 6c69 6e65 6e6f  focus.end_lineno
-0000b2c0: 202d 2031 290a 2020 2020 2020 2020 2020   - 1).          
-0000b2d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000b2e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000b2f0: 2020 2020 2020 2020 2020 626f 7472 6967            botrig
-0000b300: 6874 203d 2074 6172 6765 742e 6262 6f78  ht = target.bbox
-0000b310: 2822 2564 2e25 6422 2025 2028 666f 6375  ("%d.%d" % (focu
-0000b320: 732e 656e 645f 6c69 6e65 6e6f 2c20 666f  s.end_lineno, fo
-0000b330: 6375 732e 656e 645f 636f 6c5f 6f66 6673  cus.end_col_offs
-0000b340: 6574 2929 0a0a 2020 2020 2020 2020 2020  et))..          
-0000b350: 2020 6966 2074 6f70 6c65 6674 2061 6e64    if topleft and
-0000b360: 2062 6f74 7269 6768 743a 0a20 2020 2020   botright:.     
-0000b370: 2020 2020 2020 2020 2020 2066 6f63 7573             focus
-0000b380: 5f78 202b 3d20 746f 706c 6566 745b 305d  _x += topleft[0]
-0000b390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3a0: 2066 6f63 7573 5f79 202b 3d20 746f 706c   focus_y += topl
-0000b3b0: 6566 745b 315d 0a20 2020 2020 2020 2020  eft[1].         
-0000b3c0: 2020 2020 2020 2066 6f63 7573 5f68 6569         focus_hei
-0000b3d0: 6768 7420 3d20 626f 7472 6967 6874 5b31  ght = botright[1
-0000b3e0: 5d20 2d20 746f 706c 6566 745b 315d 202b  ] - topleft[1] +
-0000b3f0: 2062 6f74 7269 6768 745b 335d 0a0a 2020   botright[3]..  
-0000b400: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-0000b410: 7461 6e63 6528 666f 6375 732c 2028 6c69  tance(focus, (li
-0000b420: 7374 2c20 7475 706c 6529 293a 0a20 2020  st, tuple)):.   
-0000b430: 2020 2020 2020 2020 2066 6f63 7573 5f78           focus_x
-0000b440: 202b 3d20 666f 6375 735b 305d 0a20 2020   += focus[0].   
-0000b450: 2020 2020 2020 2020 2066 6f63 7573 5f79           focus_y
-0000b460: 202b 3d20 666f 6375 735b 315d 0a20 2020   += focus[1].   
-0000b470: 2020 2020 2020 2020 2066 6f63 7573 5f68           focus_h
-0000b480: 6569 6768 7420 3d20 666f 6375 735b 335d  eight = focus[3]
-0000b490: 0a0a 2020 2020 2020 2020 656c 6966 2066  ..        elif f
-0000b4a0: 6f63 7573 2069 7320 4e6f 6e65 3a0a 2020  ocus is None:.  
-0000b4b0: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
-0000b4c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b4d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000b4e0: 5479 7065 4572 726f 7228 2255 6e73 7570  TypeError("Unsup
-0000b4f0: 706f 7274 6564 2066 6f63 7573 2229 0a0a  ported focus")..
-0000b500: 2020 2020 2020 2020 2320 436f 6d70 7574          # Comput
-0000b510: 6520 6469 6d65 6e73 696f 6e73 206f 6620  e dimensions of 
-0000b520: 7468 6520 6e6f 7465 0a20 2020 2020 2020  the note.       
-0000b530: 2066 6f6e 7420 3d20 7365 6c66 2e74 6578   font = self.tex
-0000b540: 745b 2266 6f6e 7422 5d0a 2020 2020 2020  t["font"].      
-0000b550: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000b560: 666f 6e74 2c20 7374 7229 3a0a 2020 2020  font, str):.    
-0000b570: 2020 2020 2020 2020 666f 6e74 203d 2074          font = t
-0000b580: 6b2e 666f 6e74 2e6e 616d 6574 6f66 6f6e  k.font.nametofon
-0000b590: 7428 666f 6e74 290a 0a20 2020 2020 2020  t(font)..       
-0000b5a0: 206c 696e 6573 203d 2073 656c 662e 5f63   lines = self._c
-0000b5b0: 7572 7265 6e74 5f63 6861 7273 2e73 706c  urrent_chars.spl
-0000b5c0: 6974 6c69 6e65 7328 290a 2020 2020 2020  itlines().      
-0000b5d0: 2020 6d61 785f 6c69 6e65 5f77 6964 7468    max_line_width
-0000b5e0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
-0000b5f0: 206c 696e 6520 696e 206c 696e 6573 3a0a   line in lines:.
-0000b600: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-0000b610: 6c69 6e65 5f77 6964 7468 203d 206d 6178  line_width = max
-0000b620: 286d 6178 5f6c 696e 655f 7769 6474 682c  (max_line_width,
-0000b630: 2066 6f6e 742e 6d65 6173 7572 6528 6c69   font.measure(li
-0000b640: 6e65 2929 0a0a 2020 2020 2020 2020 7769  ne))..        wi
-0000b650: 6474 6820 3d20 6d69 6e28 6d61 785f 6c69  dth = min(max_li
-0000b660: 6e65 5f77 6964 7468 2c20 7365 6c66 2e5f  ne_width, self._
-0000b670: 6d61 785f 6465 6661 756c 745f 7769 6474  max_default_widt
-0000b680: 6829 202b 2073 656c 662e 7061 6478 202a  h) + self.padx *
-0000b690: 2032 202b 2032 0a20 2020 2020 2020 2073   2 + 2.        s
-0000b6a0: 656c 662e 776d 5f67 656f 6d65 7472 7928  elf.wm_geometry(
-0000b6b0: 2225 6478 2564 2b25 642b 2564 2220 2520  "%dx%d+%d+%d" % 
-0000b6c0: 2877 6964 7468 2c20 3130 302c 2066 6f63  (width, 100, foc
-0000b6d0: 7573 5f78 2c20 666f 6375 735f 7920 2b20  us_x, focus_y + 
-0000b6e0: 666f 6375 735f 6865 6967 6874 2929 0a0a  focus_height))..
-0000b6f0: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
-0000b700: 6174 655f 6964 6c65 7461 736b 7328 290a  ate_idletasks().
-0000b710: 2020 2020 2020 2020 6c69 6e65 5f63 6f75          line_cou
-0000b720: 6e74 203d 2069 6e74 2866 6c6f 6174 2873  nt = int(float(s
-0000b730: 656c 662e 7465 7874 2e69 6e64 6578 2822  elf.text.index("
-0000b740: 656e 6422 2929 290a 2020 2020 2020 2020  end"))).        
-0000b750: 6c69 6e65 5f68 6569 6768 7420 3d20 666f  line_height = fo
-0000b760: 6e74 2e6d 6574 7269 6373 2829 5b22 6c69  nt.metrics()["li
-0000b770: 6e65 7370 6163 6522 5d0a 0a20 2020 2020  nespace"]..     
-0000b780: 2020 2073 656c 662e 776d 5f67 656f 6d65     self.wm_geome
-0000b790: 7472 7928 0a20 2020 2020 2020 2020 2020  try(.           
-0000b7a0: 2022 2564 7825 642b 2564 2b25 6422 2025   "%dx%d+%d+%d" %
-0000b7b0: 2028 7769 6474 682c 206c 696e 655f 636f   (width, line_co
-0000b7c0: 756e 7420 2a20 6c69 6e65 5f68 6569 6768  unt * line_heigh
-0000b7d0: 742c 2066 6f63 7573 5f78 2c20 666f 6375  t, focus_x, focu
-0000b7e0: 735f 7920 2b20 666f 6375 735f 6865 6967  s_y + focus_heig
-0000b7f0: 6874 290a 2020 2020 2020 2020 290a 0a20  ht).        ).. 
-0000b800: 2020 2020 2020 2023 2054 4f44 4f3a 2064         # TODO: d
-0000b810: 6574 6563 7420 7468 6520 7369 7475 6174  etect the situat
-0000b820: 696f 6e20 7768 656e 206e 6f74 6520 646f  ion when note do
-0000b830: 6573 6e27 7420 6669 7420 756e 6465 720a  esn't fit under.
-0000b840: 2020 2020 2020 2020 2320 7468 6520 666f          # the fo
-0000b850: 6375 7320 626f 7820 616e 6420 7368 6f75  cus box and shou
-0000b860: 6c64 2062 6520 706c 6163 6564 2061 626f  ld be placed abo
-0000b870: 7665 0a0a 2020 2020 2020 2020 7365 6c66  ve..        self
-0000b880: 2e64 6569 636f 6e69 6679 2829 0a0a 2020  .deiconify()..  
-0000b890: 2020 6465 6620 7368 6f77 5f6e 6f74 6528    def show_note(
-0000b8a0: 7365 6c66 2c20 2a63 6f6e 7465 6e74 5f69  self, *content_i
-0000b8b0: 7465 6d73 3a20 556e 696f 6e5b 7374 722c  tems: Union[str,
-0000b8c0: 204c 6973 745d 2c20 7461 7267 6574 3d4e   List], target=N
-0000b8d0: 6f6e 652c 2066 6f63 7573 3d4e 6f6e 6529  one, focus=None)
-0000b8e0: 202d 3e20 4e6f 6e65 3a0a 0a20 2020 2020   -> None:..     
-0000b8f0: 2020 2073 656c 662e 7365 745f 636f 6e74     self.set_cont
-0000b900: 656e 7428 2a63 6f6e 7465 6e74 5f69 7465  ent(*content_ite
-0000b910: 6d73 290a 2020 2020 2020 2020 7365 6c66  ms).        self
-0000b920: 2e70 6c61 6365 2874 6172 6765 742c 2066  .place(target, f
-0000b930: 6f63 7573 290a 0a20 2020 2064 6566 205f  ocus)..    def _
-0000b940: 636c 6f73 655f 6d61 7962 6528 7365 6c66  close_maybe(self
-0000b950: 2c20 6576 656e 7429 3a0a 2020 2020 2020  , event):.      
-0000b960: 2020 6966 2065 7665 6e74 2e77 6964 6765    if event.widge
-0000b970: 7420 6e6f 7420 696e 205b 7365 6c66 2c20  t not in [self, 
-0000b980: 7365 6c66 2e74 6578 745d 3a0a 2020 2020  self.text]:.    
-0000b990: 2020 2020 2020 2020 7365 6c66 2e63 6c6f          self.clo
-0000b9a0: 7365 2865 7665 6e74 290a 0a20 2020 2064  se(event)..    d
-0000b9b0: 6566 2063 6c6f 7365 2873 656c 662c 2065  ef close(self, e
-0000b9c0: 7665 6e74 3d4e 6f6e 6529 3a0a 2020 2020  vent=None):.    
-0000b9d0: 2020 2020 7365 6c66 2e77 6974 6864 7261      self.withdra
-0000b9e0: 7728 290a 0a0a 6465 6620 6765 745f 7769  w()...def get_wi
-0000b9f0: 6467 6574 5f6f 6666 7365 745f 6672 6f6d  dget_offset_from
-0000ba00: 5f74 6f70 6c65 7665 6c28 7769 6467 6574  _toplevel(widget
-0000ba10: 293a 0a20 2020 2078 203d 2030 0a20 2020  ):.    x = 0.   
-0000ba20: 2079 203d 2030 0a20 2020 2074 6f70 6c65   y = 0.    tople
-0000ba30: 7665 6c20 3d20 7769 6467 6574 2e77 696e  vel = widget.win
-0000ba40: 666f 5f74 6f70 6c65 7665 6c28 290a 2020  fo_toplevel().  
-0000ba50: 2020 7768 696c 6520 7769 6467 6574 2021    while widget !
-0000ba60: 3d20 746f 706c 6576 656c 3a0a 2020 2020  = toplevel:.    
-0000ba70: 2020 2020 7820 2b3d 2077 6964 6765 742e      x += widget.
-0000ba80: 7769 6e66 6f5f 7828 290a 2020 2020 2020  winfo_x().      
-0000ba90: 2020 7920 2b3d 2077 6964 6765 742e 7769    y += widget.wi
-0000baa0: 6e66 6f5f 7928 290a 2020 2020 2020 2020  nfo_y().        
-0000bab0: 7769 6467 6574 203d 2077 6964 6765 742e  widget = widget.
-0000bac0: 6d61 7374 6572 0a20 2020 2072 6574 7572  master.    retur
-0000bad0: 6e20 782c 2079 0a0a 0a63 6c61 7373 2045  n x, y...class E
-0000bae0: 6e68 616e 6365 6456 6172 2874 6b2e 5661  nhancedVar(tk.Va
-0000baf0: 7269 6162 6c65 293a 0a20 2020 2064 6566  riable):.    def
-0000bb00: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0000bb10: 6d61 7374 6572 3d4e 6f6e 652c 2076 616c  master=None, val
-0000bb20: 7565 3d4e 6f6e 652c 206e 616d 653d 4e6f  ue=None, name=No
-0000bb30: 6e65 2c20 6d6f 6469 6669 6361 7469 6f6e  ne, modification
-0000bb40: 5f6c 6973 7465 6e65 723d 4e6f 6e65 293a  _listener=None):
-0000bb50: 0a20 2020 2020 2020 2069 6620 6d61 7374  .        if mast
-0000bb60: 6572 2069 7320 6e6f 7420 4e6f 6e65 2061  er is not None a
-0000bb70: 6e64 206e 6f74 2069 7369 6e73 7461 6e63  nd not isinstanc
-0000bb80: 6528 6d61 7374 6572 2c20 2874 6b2e 5769  e(master, (tk.Wi
-0000bb90: 6467 6574 2c20 746b 2e57 6d29 293a 0a20  dget, tk.Wm)):. 
-0000bba0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000bbb0: 2054 7970 6545 7272 6f72 2822 4669 7273   TypeError("Firs
-0000bbc0: 7420 706f 7369 7469 6f6e 616c 2061 7267  t positional arg
-0000bbd0: 756d 656e 7420 276d 6173 7465 7227 206d  ument 'master' m
-0000bbe0: 7573 7420 6265 204e 6f6e 652c 2057 6964  ust be None, Wid
-0000bbf0: 6765 7420 6f72 2057 6d22 290a 0a20 2020  get or Wm")..   
-0000bc00: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-0000bc10: 6e69 745f 5f28 6d61 7374 6572 3d6d 6173  nit__(master=mas
-0000bc20: 7465 722c 2076 616c 7565 3d76 616c 7565  ter, value=value
-0000bc30: 2c20 6e61 6d65 3d6e 616d 6529 0a20 2020  , name=name).   
-0000bc40: 2020 2020 2073 656c 662e 6d6f 6469 6669       self.modifi
-0000bc50: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
-0000bc60: 2020 2073 656c 662e 6d6f 6469 6669 6361     self.modifica
-0000bc70: 7469 6f6e 5f6c 6973 7465 6e65 7220 3d20  tion_listener = 
-0000bc80: 6d6f 6469 6669 6361 7469 6f6e 5f6c 6973  modification_lis
-0000bc90: 7465 6e65 720a 2020 2020 2020 2020 6966  tener.        if
-0000bca0: 2073 7973 2e76 6572 7369 6f6e 5f69 6e66   sys.version_inf
-0000bcb0: 6f20 3c20 2833 2c20 3629 3a0a 2020 2020  o < (3, 6):.    
-0000bcc0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000bcd0: 6365 2822 7722 2c20 7365 6c66 2e5f 6f6e  ce("w", self._on
-0000bce0: 5f77 7269 7465 290a 2020 2020 2020 2020  _write).        
-0000bcf0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000bd00: 2020 7365 6c66 2e74 7261 6365 5f61 6464    self.trace_add
-0000bd10: 2822 7772 6974 6522 2c20 7365 6c66 2e5f  ("write", self._
-0000bd20: 6f6e 5f77 7269 7465 290a 0a20 2020 2064  on_write)..    d
-0000bd30: 6566 205f 6f6e 5f77 7269 7465 2873 656c  ef _on_write(sel
-0000bd40: 662c 202a 6172 6773 293a 0a20 2020 2020  f, *args):.     
-0000bd50: 2020 2073 656c 662e 6d6f 6469 6669 6564     self.modified
-0000bd60: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-0000bd70: 6966 2073 656c 662e 6d6f 6469 6669 6361  if self.modifica
-0000bd80: 7469 6f6e 5f6c 6973 7465 6e65 723a 0a20  tion_listener:. 
-0000bd90: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 7365 6c66 2e6d 6f64 6966 6963 6174 696f  self.modificatio
-0000bdc0: 6e5f 6c69 7374 656e 6572 2829 0a20 2020  n_listener().   
-0000bdd0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-0000bde0: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
-0000bdf0: 2020 2020 2020 2020 2020 2023 204f 7468             # Oth
-0000be00: 6572 7769 7365 2077 686f 6c65 2070 726f  erwise whole pro
-0000be10: 6365 7373 2077 696c 6c20 6265 2062 726f  cess will be bro
-0000be20: 7567 6874 2064 6f77 6e0a 2020 2020 2020  ught down.      
-0000be30: 2020 2020 2020 2020 2020 2320 6265 6361            # beca
-0000be40: 7573 6520 666f 7220 736f 6d65 2072 6561  use for some rea
-0000be50: 736f 6e20 546b 2074 7269 6573 2074 6f20  son Tk tries to 
-0000be60: 6361 6c6c 206e 6f6e 2d65 7869 7374 696e  call non-existin
-0000be70: 6720 6d65 7468 6f64 0a20 2020 2020 2020  g method.       
-0000be80: 2020 2020 2020 2020 2023 206f 6e20 7661           # on va
-0000be90: 7269 6162 6c65 0a20 2020 2020 2020 2020  riable.         
-0000bea0: 2020 2020 2020 2067 6574 5f77 6f72 6b62         get_workb
-0000beb0: 656e 6368 2829 2e72 6570 6f72 745f 6578  ench().report_ex
-0000bec0: 6365 7074 696f 6e28 290a 0a0a 636c 6173  ception()...clas
-0000bed0: 7320 456e 6861 6e63 6564 5374 7269 6e67  s EnhancedString
-0000bee0: 5661 7228 456e 6861 6e63 6564 5661 722c  Var(EnhancedVar,
-0000bef0: 2074 6b2e 5374 7269 6e67 5661 7229 3a0a   tk.StringVar):.
-0000bf00: 2020 2020 7061 7373 0a0a 0a63 6c61 7373      pass...class
-0000bf10: 2045 6e68 616e 6365 6449 6e74 5661 7228   EnhancedIntVar(
-0000bf20: 456e 6861 6e63 6564 5661 722c 2074 6b2e  EnhancedVar, tk.
-0000bf30: 496e 7456 6172 293a 0a20 2020 2070 6173  IntVar):.    pas
-0000bf40: 730a 0a0a 636c 6173 7320 456e 6861 6e63  s...class Enhanc
-0000bf50: 6564 426f 6f6c 6561 6e56 6172 2845 6e68  edBooleanVar(Enh
-0000bf60: 616e 6365 6456 6172 2c20 746b 2e42 6f6f  ancedVar, tk.Boo
-0000bf70: 6c65 616e 5661 7229 3a0a 2020 2020 7061  leanVar):.    pa
-0000bf80: 7373 0a0a 0a63 6c61 7373 2045 6e68 616e  ss...class Enhan
-0000bf90: 6365 6444 6f75 626c 6556 6172 2845 6e68  cedDoubleVar(Enh
-0000bfa0: 616e 6365 6456 6172 2c20 746b 2e44 6f75  ancedVar, tk.Dou
-0000bfb0: 626c 6556 6172 293a 0a20 2020 2070 6173  bleVar):.    pas
-0000bfc0: 730a 0a0a 6465 6620 6372 6561 7465 5f73  s...def create_s
-0000bfd0: 7472 696e 675f 7661 7228 7661 6c75 652c  tring_var(value,
-0000bfe0: 206d 6f64 6966 6963 6174 696f 6e5f 6c69   modification_li
-0000bff0: 7374 656e 6572 3d4e 6f6e 6529 202d 3e20  stener=None) -> 
-0000c000: 456e 6861 6e63 6564 5374 7269 6e67 5661  EnhancedStringVa
-0000c010: 723a 0a20 2020 2022 2222 4372 6561 7465  r:.    """Create
-0000c020: 7320 6120 746b 2e53 7472 696e 6756 6172  s a tk.StringVar
-0000c030: 2077 6974 6820 226d 6f64 6966 6965 6422   with "modified"
-0000c040: 2061 7474 7269 6275 7465 0a20 2020 2073   attribute.    s
-0000c050: 686f 7769 6e67 2077 6865 7468 6572 2074  howing whether t
-0000c060: 6865 2076 6172 6961 626c 6520 6861 7320  he variable has 
-0000c070: 6265 656e 206d 6f64 6966 6965 6420 6166  been modified af
-0000c080: 7465 7220 6372 6561 7469 6f6e 2222 220a  ter creation""".
-0000c090: 2020 2020 7265 7475 726e 2045 6e68 616e      return Enhan
-0000c0a0: 6365 6453 7472 696e 6756 6172 284e 6f6e  cedStringVar(Non
-0000c0b0: 652c 2076 616c 7565 2c20 4e6f 6e65 2c20  e, value, None, 
-0000c0c0: 6d6f 6469 6669 6361 7469 6f6e 5f6c 6973  modification_lis
-0000c0d0: 7465 6e65 7229 0a0a 0a64 6566 2063 7265  tener)...def cre
-0000c0e0: 6174 655f 696e 745f 7661 7228 7661 6c75  ate_int_var(valu
-0000c0f0: 652c 206d 6f64 6966 6963 6174 696f 6e5f  e, modification_
-0000c100: 6c69 7374 656e 6572 3d4e 6f6e 6529 202d  listener=None) -
-0000c110: 3e20 456e 6861 6e63 6564 496e 7456 6172  > EnhancedIntVar
-0000c120: 3a0a 2020 2020 2222 2253 6565 2063 7265  :.    """See cre
-0000c130: 6174 655f 7374 7269 6e67 5f76 6172 2222  ate_string_var""
-0000c140: 220a 2020 2020 7265 7475 726e 2045 6e68  ".    return Enh
-0000c150: 616e 6365 6449 6e74 5661 7228 4e6f 6e65  ancedIntVar(None
-0000c160: 2c20 7661 6c75 652c 204e 6f6e 652c 206d  , value, None, m
-0000c170: 6f64 6966 6963 6174 696f 6e5f 6c69 7374  odification_list
-0000c180: 656e 6572 290a 0a0a 6465 6620 6372 6561  ener)...def crea
-0000c190: 7465 5f64 6f75 626c 655f 7661 7228 7661  te_double_var(va
-0000c1a0: 6c75 652c 206d 6f64 6966 6963 6174 696f  lue, modificatio
-0000c1b0: 6e5f 6c69 7374 656e 6572 3d4e 6f6e 6529  n_listener=None)
-0000c1c0: 202d 3e20 456e 6861 6e63 6564 446f 7562   -> EnhancedDoub
-0000c1d0: 6c65 5661 723a 0a20 2020 2022 2222 5365  leVar:.    """Se
-0000c1e0: 6520 6372 6561 7465 5f73 7472 696e 675f  e create_string_
-0000c1f0: 7661 7222 2222 0a20 2020 2072 6574 7572  var""".    retur
-0000c200: 6e20 456e 6861 6e63 6564 446f 7562 6c65  n EnhancedDouble
-0000c210: 5661 7228 4e6f 6e65 2c20 7661 6c75 652c  Var(None, value,
-0000c220: 204e 6f6e 652c 206d 6f64 6966 6963 6174   None, modificat
-0000c230: 696f 6e5f 6c69 7374 656e 6572 290a 0a0a  ion_listener)...
-0000c240: 6465 6620 6372 6561 7465 5f62 6f6f 6c65  def create_boole
-0000c250: 616e 5f76 6172 2876 616c 7565 2c20 6d6f  an_var(value, mo
-0000c260: 6469 6669 6361 7469 6f6e 5f6c 6973 7465  dification_liste
-0000c270: 6e65 723d 4e6f 6e65 2920 2d3e 2045 6e68  ner=None) -> Enh
-0000c280: 616e 6365 6442 6f6f 6c65 616e 5661 723a  ancedBooleanVar:
-0000c290: 0a20 2020 2022 2222 5365 6520 6372 6561  .    """See crea
-0000c2a0: 7465 5f73 7472 696e 675f 7661 7222 2222  te_string_var"""
-0000c2b0: 0a20 2020 2072 6574 7572 6e20 456e 6861  .    return Enha
-0000c2c0: 6e63 6564 426f 6f6c 6561 6e56 6172 284e  ncedBooleanVar(N
-0000c2d0: 6f6e 652c 2076 616c 7565 2c20 4e6f 6e65  one, value, None
-0000c2e0: 2c20 6d6f 6469 6669 6361 7469 6f6e 5f6c  , modification_l
-0000c2f0: 6973 7465 6e65 7229 0a0a 0a64 6566 2073  istener)...def s
-0000c300: 6869 6674 5f69 735f 7072 6573 7365 6428  hift_is_pressed(
-0000c310: 6576 656e 743a 2074 6b2e 4576 656e 7429  event: tk.Event)
-0000c320: 202d 3e20 626f 6f6c 3a0a 2020 2020 2320   -> bool:.    # 
-0000c330: 6874 7470 733a 2f2f 746b 646f 6373 2e63  https://tkdocs.c
-0000c340: 6f6d 2f73 6869 706d 616e 2f65 7665 6e74  om/shipman/event
-0000c350: 2d68 616e 646c 6572 732e 6874 6d6c 0a20  -handlers.html. 
-0000c360: 2020 2023 2068 7474 703a 2f2f 7374 6163     # http://stac
-0000c370: 6b6f 7665 7266 6c6f 772e 636f 6d2f 712f  koverflow.com/q/
-0000c380: 3332 3432 3632 3530 2f32 3631 3138 310a  32426250/261181.
-0000c390: 2020 2020 7265 7475 726e 2065 7665 6e74      return event
-0000c3a0: 2e73 7461 7465 2026 2030 7830 3030 310a  .state & 0x0001.
-0000c3b0: 0a0a 6465 6620 6361 7073 5f6c 6f63 6b5f  ..def caps_lock_
-0000c3c0: 6973 5f6f 6e28 6576 656e 743a 2074 6b2e  is_on(event: tk.
-0000c3d0: 4576 656e 7429 202d 3e20 626f 6f6c 3a0a  Event) -> bool:.
-0000c3e0: 2020 2020 2320 6874 7470 733a 2f2f 746b      # https://tk
-0000c3f0: 646f 6373 2e63 6f6d 2f73 6869 706d 616e  docs.com/shipman
-0000c400: 2f65 7665 6e74 2d68 616e 646c 6572 732e  /event-handlers.
-0000c410: 6874 6d6c 0a20 2020 2023 2068 7474 703a  html.    # http:
-0000c420: 2f2f 7374 6163 6b6f 7665 7266 6c6f 772e  //stackoverflow.
-0000c430: 636f 6d2f 712f 3332 3432 3632 3530 2f32  com/q/32426250/2
-0000c440: 3631 3138 310a 2020 2020 7265 7475 726e  61181.    return
-0000c450: 2065 7665 6e74 2e73 7461 7465 2026 2030   event.state & 0
-0000c460: 7830 3030 320a 0a0a 6465 6620 636f 6e74  x0002...def cont
-0000c470: 726f 6c5f 6973 5f70 7265 7373 6564 2865  rol_is_pressed(e
-0000c480: 7665 6e74 3a20 746b 2e45 7665 6e74 2920  vent: tk.Event) 
-0000c490: 2d3e 2062 6f6f 6c3a 0a20 2020 2023 2068  -> bool:.    # h
-0000c4a0: 7474 7073 3a2f 2f74 6b64 6f63 732e 636f  ttps://tkdocs.co
-0000c4b0: 6d2f 7368 6970 6d61 6e2f 6576 656e 742d  m/shipman/event-
-0000c4c0: 6861 6e64 6c65 7273 2e68 746d 6c0a 2020  handlers.html.  
-0000c4d0: 2020 2320 6874 7470 3a2f 2f73 7461 636b    # http://stack
-0000c4e0: 6f76 6572 666c 6f77 2e63 6f6d 2f71 2f33  overflow.com/q/3
-0000c4f0: 3234 3236 3235 302f 3236 3131 3831 0a20  2426250/261181. 
-0000c500: 2020 2072 6574 7572 6e20 6576 656e 742e     return event.
-0000c510: 7374 6174 6520 2620 3078 3030 3034 0a0a  state & 0x0004..
-0000c520: 0a64 6566 2061 6c74 5f69 735f 7072 6573  .def alt_is_pres
-0000c530: 7365 645f 7769 7468 6f75 745f 6368 6172  sed_without_char
-0000c540: 2865 7665 6e74 3a20 746b 2e45 7665 6e74  (event: tk.Event
-0000c550: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2023  ) -> bool:.    #
-0000c560: 2068 7474 7073 3a2f 2f74 6b64 6f63 732e   https://tkdocs.
-0000c570: 636f 6d2f 7368 6970 6d61 6e2f 6576 656e  com/shipman/even
-0000c580: 742d 6861 6e64 6c65 7273 2e68 746d 6c0a  t-handlers.html.
-0000c590: 2020 2020 2320 6874 7470 3a2f 2f73 7461      # http://sta
-0000c5a0: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
-0000c5b0: 2f33 3234 3236 3235 302f 3236 3131 3831  /32426250/261181
-0000c5c0: 0a20 2020 2023 2068 7474 7073 3a2f 2f62  .    # https://b
-0000c5d0: 7567 732e 7079 7468 6f6e 2e6f 7267 2f6d  ugs.python.org/m
-0000c5e0: 7367 3236 3834 3239 0a20 2020 2069 6620  sg268429.    if 
-0000c5f0: 6576 656e 742e 6368 6172 3a0a 2020 2020  event.char:.    
-0000c600: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000c610: 0a0a 2020 2020 6966 2072 756e 6e69 6e67  ..    if running
-0000c620: 5f6f 6e5f 7769 6e64 6f77 7328 293a 0a20  _on_windows():. 
-0000c630: 2020 2020 2020 2072 6574 7572 6e20 6576         return ev
-0000c640: 656e 742e 7374 6174 6520 2620 3078 3230  ent.state & 0x20
-0000c650: 3030 300a 2020 2020 656c 6966 2072 756e  000.    elif run
-0000c660: 6e69 6e67 5f6f 6e5f 6d61 635f 6f73 2829  ning_on_mac_os()
-0000c670: 3a0a 2020 2020 2020 2020 2320 636f 6d62  :.        # comb
-0000c680: 696e 6174 696f 6e73 2061 6c77 6179 7320  inations always 
-0000c690: 7072 6f64 7563 6520 6120 6368 6172 206f  produce a char o
-0000c6a0: 7220 6172 6520 636f 6e73 756d 6564 2062  r are consumed b
-0000c6b0: 7920 7468 6520 4f53 0a20 2020 2020 2020  y the OS.       
-0000c6c0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0000c6d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000c6e0: 7265 7475 726e 2065 7665 6e74 2e73 7461  return event.sta
-0000c6f0: 7465 2026 2030 7830 3031 300a 0a0a 6465  te & 0x0010...de
-0000c700: 6620 636f 6d6d 616e 645f 6973 5f70 7265  f command_is_pre
-0000c710: 7373 6564 2865 7665 6e74 3a20 746b 2e45  ssed(event: tk.E
-0000c720: 7665 6e74 2920 2d3e 2062 6f6f 6c3a 0a20  vent) -> bool:. 
-0000c730: 2020 2023 2068 7474 7073 3a2f 2f74 6b64     # https://tkd
-0000c740: 6f63 732e 636f 6d2f 7368 6970 6d61 6e2f  ocs.com/shipman/
-0000c750: 6576 656e 742d 6861 6e64 6c65 7273 2e68  event-handlers.h
-0000c760: 746d 6c0a 2020 2020 2320 6874 7470 3a2f  tml.    # http:/
-0000c770: 2f73 7461 636b 6f76 6572 666c 6f77 2e63  /stackoverflow.c
-0000c780: 6f6d 2f71 2f33 3234 3236 3235 302f 3236  om/q/32426250/26
-0000c790: 3131 3831 0a20 2020 2069 6620 6e6f 7420  1181.    if not 
-0000c7a0: 7275 6e6e 696e 675f 6f6e 5f6d 6163 5f6f  running_on_mac_o
-0000c7b0: 7328 293a 0a20 2020 2020 2020 2072 6574  s():.        ret
-0000c7c0: 7572 6e20 4661 6c73 650a 2020 2020 7265  urn False.    re
-0000c7d0: 7475 726e 2065 7665 6e74 2e73 7461 7465  turn event.state
-0000c7e0: 2026 2030 7830 3030 380a 0a0a 6465 6620   & 0x0008...def 
-0000c7f0: 6765 745f 6879 7065 726c 696e 6b5f 6375  get_hyperlink_cu
-0000c800: 7273 6f72 2829 202d 3e20 7374 723a 0a20  rsor() -> str:. 
-0000c810: 2020 2069 6620 7275 6e6e 696e 675f 6f6e     if running_on
-0000c820: 5f6d 6163 5f6f 7328 293a 0a20 2020 2020  _mac_os():.     
-0000c830: 2020 2072 6574 7572 6e20 2270 6f69 6e74     return "point
-0000c840: 696e 6768 616e 6422 0a20 2020 2065 6c73  inghand".    els
-0000c850: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-0000c860: 6e20 2268 616e 6432 220a 0a0a 6465 6620  n "hand2"...def 
-0000c870: 6765 745f 6265 616d 5f63 7572 736f 7228  get_beam_cursor(
-0000c880: 2920 2d3e 2073 7472 3a0a 2020 2020 6966  ) -> str:.    if
-0000c890: 2072 756e 6e69 6e67 5f6f 6e5f 6d61 635f   running_on_mac_
-0000c8a0: 6f73 2829 206f 7220 7275 6e6e 696e 675f  os() or running_
-0000c8b0: 6f6e 5f77 696e 646f 7773 2829 3a0a 2020  on_windows():.  
-0000c8c0: 2020 2020 2020 7265 7475 726e 2022 6962        return "ib
-0000c8d0: 6561 6d22 0a20 2020 2065 6c73 653a 0a20  eam".    else:. 
-0000c8e0: 2020 2020 2020 2072 6574 7572 6e20 2278         return "x
-0000c8f0: 7465 726d 220a 0a0a 6465 6620 7365 7175  term"...def sequ
-0000c900: 656e 6365 5f74 6f5f 6576 656e 745f 7374  ence_to_event_st
-0000c910: 6174 655f 616e 645f 6b65 7963 6f64 6528  ate_and_keycode(
-0000c920: 7365 7175 656e 6365 3a20 7374 7229 202d  sequence: str) -
-0000c930: 3e20 4f70 7469 6f6e 616c 5b54 7570 6c65  > Optional[Tuple
-0000c940: 5b69 6e74 2c20 696e 745d 5d3a 0a20 2020  [int, int]]:.   
-0000c950: 2023 2072 656d 656d 6265 7220 6861 6e64   # remember hand
-0000c960: 6c65 7273 2066 6f72 2063 6572 7461 696e  lers for certain
-0000c970: 2073 686f 7274 6375 7473 2077 6869 6368   shortcuts which
-0000c980: 2072 6571 7569 7265 0a20 2020 2023 2064   require.    # d
-0000c990: 6966 6665 7265 6e74 2074 7265 6174 6d65  ifferent treatme
-0000c9a0: 6e74 206f 6e20 6e6f 6e2d 6c61 7469 6e20  nt on non-latin 
-0000c9b0: 6b65 7962 6f61 7264 730a 2020 2020 6966  keyboards.    if
-0000c9c0: 2073 6571 7565 6e63 655b 305d 2021 3d20   sequence[0] != 
-0000c9d0: 223c 223a 0a20 2020 2020 2020 2072 6574  "<":.        ret
-0000c9e0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 7061  urn None..    pa
-0000c9f0: 7274 7320 3d20 7365 7175 656e 6365 2e73  rts = sequence.s
-0000ca00: 7472 6970 2822 3c22 292e 7374 7269 7028  trip("<").strip(
-0000ca10: 223e 2229 2e73 706c 6974 2822 2d22 290a  ">").split("-").
-0000ca20: 2020 2020 2320 7375 7070 6f72 7420 6f6e      # support on
-0000ca30: 6c79 206c 6174 696e 206c 6574 7465 7273  ly latin letters
-0000ca40: 2066 6f72 206e 6f77 0a20 2020 2069 6620   for now.    if 
-0000ca50: 7061 7274 735b 2d31 5d2e 6c6f 7765 7228  parts[-1].lower(
-0000ca60: 2920 6e6f 7420 696e 206c 6973 7428 2261  ) not in list("a
-0000ca70: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
-0000ca80: 7273 7475 7677 7879 7a22 293a 0a20 2020  rstuvwxyz"):.   
-0000ca90: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-0000caa0: 0a0a 2020 2020 6c65 7474 6572 203d 2070  ..    letter = p
-0000cab0: 6172 7473 2e70 6f70 282d 3129 0a20 2020  arts.pop(-1).   
-0000cac0: 2069 6620 224b 6579 2220 696e 2070 6172   if "Key" in par
-0000cad0: 7473 3a0a 2020 2020 2020 2020 7061 7274  ts:.        part
-0000cae0: 732e 7265 6d6f 7665 2822 4b65 7922 290a  s.remove("Key").
-0000caf0: 2020 2020 6966 2022 6b65 7922 2069 6e20      if "key" in 
-0000cb00: 7061 7274 733a 0a20 2020 2020 2020 2070  parts:.        p
-0000cb10: 6172 7473 2e72 656d 6f76 6528 226b 6579  arts.remove("key
-0000cb20: 2229 0a0a 2020 2020 6d6f 6469 6669 6572  ")..    modifier
-0000cb30: 7320 3d20 7b70 6172 742e 6c6f 7765 7228  s = {part.lower(
-0000cb40: 2920 666f 7220 7061 7274 2069 6e20 7061  ) for part in pa
-0000cb50: 7274 737d 0a0a 2020 2020 6966 206c 6574  rts}..    if let
-0000cb60: 7465 722e 6973 7570 7065 7228 293a 0a20  ter.isupper():. 
-0000cb70: 2020 2020 2020 206d 6f64 6966 6965 7273         modifiers
-0000cb80: 2e61 6464 2822 7368 6966 7422 290a 0a20  .add("shift").. 
-0000cb90: 2020 2069 6620 6d6f 6469 6669 6572 7320     if modifiers 
-0000cba0: 6e6f 7420 696e 205b 7b22 636f 6e74 726f  not in [{"contro
-0000cbb0: 6c22 7d2c 207b 2263 6f6e 7472 6f6c 222c  l"}, {"control",
-0000cbc0: 2022 7368 6966 7422 7d5d 3a0a 2020 2020   "shift"}]:.    
-0000cbd0: 2020 2020 2320 646f 6e27 7420 7375 7070      # don't supp
-0000cbe0: 6f72 7420 6f74 6865 7273 2066 6f72 206e  ort others for n
-0000cbf0: 6f77 0a20 2020 2020 2020 2072 6574 7572  ow.        retur
-0000cc00: 6e20 4e6f 6e65 0a0a 2020 2020 6576 656e  n None..    even
-0000cc10: 745f 7374 6174 6520 3d20 300a 2020 2020  t_state = 0.    
-0000cc20: 2320 6874 7470 733a 2f2f 746b 646f 6373  # https://tkdocs
-0000cc30: 2e63 6f6d 2f73 6869 706d 616e 2f65 7665  .com/shipman/eve
-0000cc40: 6e74 2d68 616e 646c 6572 732e 6874 6d6c  nt-handlers.html
-0000cc50: 0a20 2020 2023 2068 7474 7073 3a2f 2f73  .    # https://s
-0000cc60: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
-0000cc70: 2f71 7565 7374 696f 6e73 2f33 3234 3236  /questions/32426
-0000cc80: 3235 302f 7079 7468 6f6e 2d64 6f63 756d  250/python-docum
-0000cc90: 656e 7461 7469 6f6e 2d61 6e64 2d6f 722d  entation-and-or-
-0000cca0: 6c61 636b 2d74 6865 7265 6f66 2d65 2d67  lack-thereof-e-g
-0000ccb0: 2d6b 6579 626f 6172 642d 6576 656e 742d  -keyboard-event-
-0000ccc0: 7374 6174 650a 2020 2020 666f 7220 6d6f  state.    for mo
-0000ccd0: 6469 6669 6572 2069 6e20 6d6f 6469 6669  difier in modifi
-0000cce0: 6572 733a 0a20 2020 2020 2020 2069 6620  ers:.        if 
-0000ccf0: 6d6f 6469 6669 6572 203d 3d20 2273 6869  modifier == "shi
-0000cd00: 6674 223a 0a20 2020 2020 2020 2020 2020  ft":.           
-0000cd10: 2065 7665 6e74 5f73 7461 7465 207c 3d20   event_state |= 
-0000cd20: 3078 3030 3031 0a20 2020 2020 2020 2065  0x0001.        e
-0000cd30: 6c69 6620 6d6f 6469 6669 6572 203d 3d20  lif modifier == 
-0000cd40: 2263 6f6e 7472 6f6c 223a 0a20 2020 2020  "control":.     
-0000cd50: 2020 2020 2020 2065 7665 6e74 5f73 7461         event_sta
-0000cd60: 7465 207c 3d20 3078 3030 3034 0a20 2020  te |= 0x0004.   
-0000cd70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000cd80: 2020 2020 2020 2023 2075 6e73 7570 706f         # unsuppo
-0000cd90: 7274 6564 206d 6f64 6966 6965 720a 2020  rted modifier.  
-0000cda0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000cdb0: 204e 6f6e 650a 0a20 2020 2023 2066 6f72   None..    # for
-0000cdc0: 206c 6174 696e 206c 6574 7465 7273 206b   latin letters k
-0000cdd0: 6579 636f 6465 2069 7320 7361 6d65 2061  eycode is same a
-0000cde0: 7320 6974 7320 6173 6369 6920 636f 6465  s its ascii code
-0000cdf0: 0a20 2020 2072 6574 7572 6e20 2865 7665  .    return (eve
-0000ce00: 6e74 5f73 7461 7465 2c20 6f72 6428 6c65  nt_state, ord(le
-0000ce10: 7474 6572 2e75 7070 6572 2829 2929 0a0a  tter.upper()))..
-0000ce20: 0a64 6566 2073 656c 6563 745f 7365 7175  .def select_sequ
-0000ce30: 656e 6365 2877 696e 5f76 6572 7369 6f6e  ence(win_version
-0000ce40: 2c20 6d61 635f 7665 7273 696f 6e2c 206c  , mac_version, l
-0000ce50: 696e 7578 5f76 6572 7369 6f6e 3d4e 6f6e  inux_version=Non
-0000ce60: 6529 3a0a 2020 2020 6966 2072 756e 6e69  e):.    if runni
-0000ce70: 6e67 5f6f 6e5f 7769 6e64 6f77 7328 293a  ng_on_windows():
-0000ce80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000ce90: 7769 6e5f 7665 7273 696f 6e0a 2020 2020  win_version.    
-0000cea0: 656c 6966 2072 756e 6e69 6e67 5f6f 6e5f  elif running_on_
-0000ceb0: 6d61 635f 6f73 2829 3a0a 2020 2020 2020  mac_os():.      
-0000cec0: 2020 7265 7475 726e 206d 6163 5f76 6572    return mac_ver
-0000ced0: 7369 6f6e 0a20 2020 2065 6c69 6620 7275  sion.    elif ru
-0000cee0: 6e6e 696e 675f 6f6e 5f6c 696e 7578 2829  nning_on_linux()
-0000cef0: 2061 6e64 206c 696e 7578 5f76 6572 7369   and linux_versi
-0000cf00: 6f6e 3a0a 2020 2020 2020 2020 7265 7475  on:.        retu
-0000cf10: 726e 206c 696e 7578 5f76 6572 7369 6f6e  rn linux_version
-0000cf20: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000cf30: 2020 2072 6574 7572 6e20 7769 6e5f 7665     return win_ve
-0000cf40: 7273 696f 6e0a 0a0a 6465 6620 7472 795f  rsion...def try_
-0000cf50: 7265 6d6f 7665 5f6c 696e 656e 756d 6265  remove_linenumbe
-0000cf60: 7273 2874 6578 742c 206d 6173 7465 7229  rs(text, master)
-0000cf70: 3a0a 2020 2020 7472 793a 0a20 2020 2020  :.    try:.     
-0000cf80: 2020 2069 6620 6861 735f 6c69 6e65 5f6e     if has_line_n
-0000cf90: 756d 6265 7273 2874 6578 7429 2061 6e64  umbers(text) and
-0000cfa0: 206d 6573 7361 6765 626f 782e 6173 6b79   messagebox.asky
-0000cfb0: 6573 6e6f 280a 2020 2020 2020 2020 2020  esno(.          
-0000cfc0: 2020 7469 746c 653d 2252 656d 6f76 6520    title="Remove 
-0000cfd0: 6c69 6e65 6e75 6d62 6572 7322 2c0a 2020  linenumbers",.  
-0000cfe0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-0000cff0: 653d 2244 6f20 796f 7520 7761 6e74 2074  e="Do you want t
-0000d000: 6f20 7265 6d6f 7665 206c 696e 656e 756d  o remove linenum
-0000d010: 6265 7273 2066 726f 6d20 7061 7374 6564  bers from pasted
-0000d020: 2074 6578 743f 222c 0a20 2020 2020 2020   text?",.       
-0000d030: 2020 2020 2064 6566 6175 6c74 3d6d 6573       default=mes
-0000d040: 7361 6765 626f 782e 5945 532c 0a20 2020  sagebox.YES,.   
-0000d050: 2020 2020 2020 2020 206d 6173 7465 723d           master=
-0000d060: 6d61 7374 6572 2c0a 2020 2020 2020 2020  master,.        
-0000d070: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000d080: 6574 7572 6e20 7265 6d6f 7665 5f6c 696e  eturn remove_lin
-0000d090: 655f 6e75 6d62 6572 7328 7465 7874 290a  e_numbers(text).
-0000d0a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000d0b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d0c0: 2074 6578 740a 2020 2020 6578 6365 7074   text.    except
-0000d0d0: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
-0000d0e0: 2020 2020 7472 6163 6562 6163 6b2e 7072      traceback.pr
-0000d0f0: 696e 745f 6578 6328 290a 2020 2020 2020  int_exc().      
-0000d100: 2020 7265 7475 726e 2074 6578 740a 0a0a    return text...
-0000d110: 6465 6620 6861 735f 6c69 6e65 5f6e 756d  def has_line_num
-0000d120: 6265 7273 2874 6578 7429 3a0a 2020 2020  bers(text):.    
-0000d130: 6c69 6e65 7320 3d20 7465 7874 2e73 706c  lines = text.spl
-0000d140: 6974 6c69 6e65 7328 290a 2020 2020 7265  itlines().    re
-0000d150: 7475 726e 206c 656e 286c 696e 6573 2920  turn len(lines) 
-0000d160: 3e20 3220 616e 6420 616c 6c28 5b6c 656e  > 2 and all([len
-0000d170: 2873 706c 6974 5f61 6674 6572 5f6c 696e  (split_after_lin
-0000d180: 655f 6e75 6d62 6572 286c 696e 6529 2920  e_number(line)) 
-0000d190: 3d3d 2032 2066 6f72 206c 696e 6520 696e  == 2 for line in
-0000d1a0: 206c 696e 6573 5d29 0a0a 0a64 6566 2073   lines])...def s
-0000d1b0: 706c 6974 5f61 6674 6572 5f6c 696e 655f  plit_after_line_
-0000d1c0: 6e75 6d62 6572 2873 293a 0a20 2020 2070  number(s):.    p
-0000d1d0: 6172 7473 203d 2072 652e 7370 6c69 7428  arts = re.split(
-0000d1e0: 7222 285e 5c73 2a5c 642b 5c2e 3f29 222c  r"(^\s*\d+\.?)",
-0000d1f0: 2073 290a 2020 2020 6966 206c 656e 2870   s).    if len(p
-0000d200: 6172 7473 2920 3d3d 2031 3a0a 2020 2020  arts) == 1:.    
-0000d210: 2020 2020 7265 7475 726e 2070 6172 7473      return parts
-0000d220: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000d230: 2020 2061 7373 6572 7420 6c65 6e28 7061     assert len(pa
-0000d240: 7274 7329 203d 3d20 3320 616e 6420 7061  rts) == 3 and pa
-0000d250: 7274 735b 305d 203d 3d20 2222 0a20 2020  rts[0] == "".   
-0000d260: 2020 2020 2072 6574 7572 6e20 7061 7274       return part
-0000d270: 735b 313a 5d0a 0a0a 6465 6620 7265 6d6f  s[1:]...def remo
-0000d280: 7665 5f6c 696e 655f 6e75 6d62 6572 7328  ve_line_numbers(
-0000d290: 7329 3a0a 2020 2020 636c 6561 6e65 645f  s):.    cleaned_
-0000d2a0: 6c69 6e65 7320 3d20 5b5d 0a20 2020 2066  lines = [].    f
-0000d2b0: 6f72 206c 696e 6520 696e 2073 2e73 706c  or line in s.spl
-0000d2c0: 6974 6c69 6e65 7328 293a 0a20 2020 2020  itlines():.     
-0000d2d0: 2020 2070 6172 7473 203d 2073 706c 6974     parts = split
-0000d2e0: 5f61 6674 6572 5f6c 696e 655f 6e75 6d62  _after_line_numb
-0000d2f0: 6572 286c 696e 6529 0a20 2020 2020 2020  er(line).       
-0000d300: 2069 6620 6c65 6e28 7061 7274 7329 2021   if len(parts) !
-0000d310: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-0000d320: 2072 6574 7572 6e20 730a 2020 2020 2020   return s.      
-0000d330: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000d340: 2020 2020 636c 6561 6e65 645f 6c69 6e65      cleaned_line
-0000d350: 732e 6170 7065 6e64 2870 6172 7473 5b31  s.append(parts[1
-0000d360: 5d29 0a0a 2020 2020 7265 7475 726e 2074  ])..    return t
-0000d370: 6578 7477 7261 702e 6465 6465 6e74 2828  extwrap.dedent((
-0000d380: 225c 6e22 2e6a 6f69 6e28 636c 6561 6e65  "\n".join(cleane
-0000d390: 645f 6c69 6e65 7329 2920 2b20 225c 6e22  d_lines)) + "\n"
-0000d3a0: 290a 0a0a 2320 506c 6163 6520 6120 746f  )...# Place a to
-0000d3b0: 706c 6576 656c 2077 696e 646f 7720 6174  plevel window at
-0000d3c0: 2074 6865 2063 656e 7465 7220 6f66 2070   the center of p
-0000d3d0: 6172 656e 7420 6f72 2073 6372 6565 6e0a  arent or screen.
-0000d3e0: 2320 4974 2069 7320 6120 5079 7468 6f6e  # It is a Python
-0000d3f0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-0000d400: 6f66 203a 3a74 6b3a 3a50 6c61 6365 5769  of ::tk::PlaceWi
-0000d410: 6e64 6f77 2e0a 2320 436f 7069 6564 2061  ndow..# Copied a
-0000d420: 6e64 2061 6461 7074 6564 2066 726f 6d20  nd adapted from 
-0000d430: 746b 696e 7465 722e 7369 6d70 6c65 6469  tkinter.simpledi
-0000d440: 616c 6f67 206f 6620 5079 7468 6f6e 2033  alog of Python 3
-0000d450: 2e31 302e 320a 6465 6620 5f70 6c61 6365  .10.2.def _place
-0000d460: 5f77 696e 646f 7728 772c 2070 6172 656e  _window(w, paren
-0000d470: 743d 4e6f 6e65 2c20 7769 6474 683d 4e6f  t=None, width=No
-0000d480: 6e65 2c20 6865 6967 6874 3d4e 6f6e 6529  ne, height=None)
-0000d490: 3a0a 2020 2020 772e 776d 5f77 6974 6864  :.    w.wm_withd
-0000d4a0: 7261 7728 2920 2023 2052 656d 6169 6e20  raw()  # Remain 
-0000d4b0: 696e 7669 7369 626c 6520 7768 696c 6520  invisible while 
-0000d4c0: 7765 2066 6967 7572 6520 6f75 7420 7468  we figure out th
-0000d4d0: 6520 6765 6f6d 6574 7279 0a20 2020 2077  e geometry.    w
-0000d4e0: 2e75 7064 6174 655f 6964 6c65 7461 736b  .update_idletask
-0000d4f0: 7328 2920 2023 2041 6374 7561 6c69 7a65  s()  # Actualize
-0000d500: 2067 656f 6d65 7472 7920 696e 666f 726d   geometry inform
-0000d510: 6174 696f 6e0a 0a20 2020 206d 696e 7769  ation..    minwi
-0000d520: 6474 6820 3d20 7769 6474 6820 6f72 2077  dth = width or w
-0000d530: 2e77 696e 666f 5f72 6571 7769 6474 6828  .winfo_reqwidth(
-0000d540: 290a 2020 2020 6d69 6e68 6569 6768 7420  ).    minheight 
-0000d550: 3d20 6865 6967 6874 206f 7220 772e 7769  = height or w.wi
-0000d560: 6e66 6f5f 7265 7168 6569 6768 7428 290a  nfo_reqheight().
-0000d570: 2020 2020 6d61 7877 6964 7468 203d 2077      maxwidth = w
-0000d580: 2e77 696e 666f 5f76 726f 6f74 7769 6474  .winfo_vrootwidt
-0000d590: 6828 290a 2020 2020 6d61 7868 6569 6768  h().    maxheigh
-0000d5a0: 7420 3d20 772e 7769 6e66 6f5f 7672 6f6f  t = w.winfo_vroo
-0000d5b0: 7468 6569 6768 7428 290a 2020 2020 6966  theight().    if
-0000d5c0: 2070 6172 656e 7420 6973 206e 6f74 204e   parent is not N
-0000d5d0: 6f6e 6520 616e 6420 7061 7265 6e74 2e77  one and parent.w
-0000d5e0: 696e 666f 5f69 736d 6170 7065 6428 293a  info_ismapped():
-0000d5f0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000d600: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
-0000d610: 2020 6622 5061 7265 6e74 2079 3a20 7b70    f"Parent y: {p
-0000d620: 6172 656e 742e 7769 6e66 6f5f 7928 297d  arent.winfo_y()}
-0000d630: 2c20 726f 6f74 793a 207b 7061 7265 6e74  , rooty: {parent
-0000d640: 2e77 696e 666f 5f72 6f6f 7479 2829 7d2c  .winfo_rooty()},
-0000d650: 2076 726f 6f74 793a 207b 7061 7265 6e74   vrooty: {parent
-0000d660: 2e77 696e 666f 5f76 726f 6f74 7928 297d  .winfo_vrooty()}
-0000d670: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-0000d680: 2020 2020 7820 3d20 7061 7265 6e74 2e77      x = parent.w
-0000d690: 696e 666f 5f72 6f6f 7478 2829 202b 2028  info_rootx() + (
-0000d6a0: 7061 7265 6e74 2e77 696e 666f 5f77 6964  parent.winfo_wid
-0000d6b0: 7468 2829 202d 206d 696e 7769 6474 6829  th() - minwidth)
-0000d6c0: 202f 2f20 320a 2020 2020 2020 2020 7920   // 2.        y 
-0000d6d0: 3d20 7061 7265 6e74 2e77 696e 666f 5f79  = parent.winfo_y
-0000d6e0: 2829 202b 2028 7061 7265 6e74 2e77 696e  () + (parent.win
-0000d6f0: 666f 5f68 6569 6768 7428 2920 2d20 6d69  fo_height() - mi
-0000d700: 6e68 6569 6768 7429 202f 2f20 320a 2020  nheight) // 2.  
-0000d710: 2020 2020 2020 7672 6f6f 7478 203d 2077        vrootx = w
-0000d720: 2e77 696e 666f 5f76 726f 6f74 7828 290a  .winfo_vrootx().
-0000d730: 2020 2020 2020 2020 7672 6f6f 7479 203d          vrooty =
-0000d740: 2077 2e77 696e 666f 5f76 726f 6f74 7928   w.winfo_vrooty(
-0000d750: 290a 2020 2020 2020 2020 7820 3d20 6d69  ).        x = mi
-0000d760: 6e28 782c 2076 726f 6f74 7820 2b20 6d61  n(x, vrootx + ma
-0000d770: 7877 6964 7468 202d 206d 696e 7769 6474  xwidth - minwidt
-0000d780: 6829 0a20 2020 2020 2020 2078 203d 206d  h).        x = m
-0000d790: 6178 2878 2c20 7672 6f6f 7478 290a 2020  ax(x, vrootx).  
-0000d7a0: 2020 2020 2020 7920 3d20 6d69 6e28 792c        y = min(y,
-0000d7b0: 2076 726f 6f74 7920 2b20 6d61 7868 6569   vrooty + maxhei
-0000d7c0: 6768 7420 2d20 6d69 6e68 6569 6768 7429  ght - minheight)
-0000d7d0: 0a20 2020 2020 2020 2023 2064 6f6e 2774  .        # don't
-0000d7e0: 2061 6c6c 6f77 2074 6865 2064 6961 6c6f   allow the dialo
-0000d7f0: 6720 676f 2068 6967 6865 7220 7468 616e  g go higher than
-0000d800: 2070 6172 656e 742e 2054 6869 7320 7761   parent. This wa
-0000d810: 7920 7468 6520 7469 746c 6520 6261 7220  y the title bar 
-0000d820: 7265 6d61 696e 7320 7669 7369 626c 652e  remains visible.
-0000d830: 0a20 2020 2020 2020 2079 203d 206d 6178  .        y = max
-0000d840: 2879 2c20 7672 6f6f 7479 2c20 7061 7265  (y, vrooty, pare
-0000d850: 6e74 2e77 696e 666f 5f79 2829 290a 2020  nt.winfo_y()).  
-0000d860: 2020 2020 2020 6966 2077 2e5f 7769 6e64        if w._wind
-0000d870: 6f77 696e 6773 7973 7465 6d20 3d3d 2022  owingsystem == "
-0000d880: 6171 7561 223a 0a20 2020 2020 2020 2020  aqua":.         
-0000d890: 2020 2023 2041 766f 6964 2074 6865 206e     # Avoid the n
-0000d8a0: 6174 6976 6520 6d65 6e75 2062 6172 2077  ative menu bar w
-0000d8b0: 6869 6368 2073 6974 7320 6f6e 2074 6f70  hich sits on top
-0000d8c0: 206f 6620 6576 6572 7974 6869 6e67 2e0a   of everything..
-0000d8d0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
-0000d8e0: 6d61 7828 792c 2065 6d73 5f74 6f5f 7069  max(y, ems_to_pi
-0000d8f0: 7865 6c73 2832 2929 0a0a 2020 2020 2020  xels(2))..      
-0000d900: 2020 6966 2079 202b 206d 696e 6865 6967    if y + minheig
-0000d910: 6874 203e 206d 6178 6865 6967 6874 3a0a  ht > maxheight:.
-0000d920: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d930: 6572 2e64 6562 7567 2822 416c 6967 6e69  er.debug("Aligni
-0000d940: 6e67 2074 6f70 2077 6974 6820 7061 7265  ng top with pare
-0000d950: 6e74 2028 2573 2076 7320 2573 2922 2c20  nt (%s vs %s)", 
-0000d960: 7920 2b20 6d69 6e68 6569 6768 742c 206d  y + minheight, m
-0000d970: 6178 6865 6967 6874 290a 2020 2020 2020  axheight).      
-0000d980: 2020 2020 2020 7920 3d20 7061 7265 6e74        y = parent
-0000d990: 2e77 696e 666f 5f79 2829 0a20 2020 2065  .winfo_y().    e
-0000d9a0: 6c73 653a 0a20 2020 2020 2020 2078 203d  lse:.        x =
-0000d9b0: 2028 772e 7769 6e66 6f5f 7363 7265 656e   (w.winfo_screen
-0000d9c0: 7769 6474 6828 2920 2d20 6d69 6e77 6964  width() - minwid
-0000d9d0: 7468 2920 2f2f 2032 0a20 2020 2020 2020  th) // 2.       
-0000d9e0: 2079 203d 2028 772e 7769 6e66 6f5f 7363   y = (w.winfo_sc
-0000d9f0: 7265 656e 6865 6967 6874 2829 202d 206d  reenheight() - m
-0000da00: 696e 6865 6967 6874 2920 2f2f 2032 0a0a  inheight) // 2..
-0000da10: 2020 2020 772e 776d 5f6d 6178 7369 7a65      w.wm_maxsize
-0000da20: 286d 6178 7769 6474 682c 206d 6178 6865  (maxwidth, maxhe
-0000da30: 6967 6874 290a 2020 2020 6966 2077 6964  ight).    if wid
-0000da40: 7468 2061 6e64 2068 6569 6768 743a 0a20  th and height:. 
-0000da50: 2020 2020 2020 2067 656f 6d65 7472 7920         geometry 
-0000da60: 3d20 2225 6478 2564 2b25 642b 2564 2220  = "%dx%d+%d+%d" 
-0000da70: 2520 2877 6964 7468 2c20 6865 6967 6874  % (width, height
-0000da80: 2c20 782c 2079 290a 2020 2020 656c 7365  , x, y).    else
-0000da90: 3a0a 2020 2020 2020 2020 6765 6f6d 6574  :.        geomet
-0000daa0: 7279 203d 2022 2b25 642b 2564 2220 2520  ry = "+%d+%d" % 
-0000dab0: 2878 2c20 7929 0a0a 2020 2020 6c6f 6767  (x, y)..    logg
-0000dac0: 6572 2e69 6e66 6f28 6622 506c 6163 696e  er.info(f"Placin
-0000dad0: 6720 7b77 7d20 7769 7468 2067 656f 6d65  g {w} with geome
-0000dae0: 7472 7920 7b67 656f 6d65 7472 797d 2229  try {geometry}")
-0000daf0: 0a20 2020 2077 2e77 6d5f 6765 6f6d 6574  .    w.wm_geomet
-0000db00: 7279 2867 656f 6d65 7472 7929 0a20 2020  ry(geometry).   
-0000db10: 2077 2e77 6d5f 6465 6963 6f6e 6966 7928   w.wm_deiconify(
-0000db20: 2920 2023 2042 6563 6f6d 6520 7669 7369  )  # Become visi
-0000db30: 626c 6520 6174 2074 6865 2064 6573 6972  ble at the desir
-0000db40: 6564 206c 6f63 6174 696f 6e0a 0a0a 636c  ed location...cl
-0000db50: 6173 7320 5761 6974 696e 6744 6961 6c6f  ass WaitingDialo
-0000db60: 6728 436f 6d6d 6f6e 4469 616c 6f67 293a  g(CommonDialog):
-0000db70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000db80: 5f28 7365 6c66 2c20 6d61 7374 6572 2c20  _(self, master, 
-0000db90: 6173 796e 635f 7265 7375 6c74 2c20 6465  async_result, de
-0000dba0: 7363 7269 7074 696f 6e2c 2074 6974 6c65  scription, title
-0000dbb0: 3d22 506c 6561 7365 2077 6169 7421 222c  ="Please wait!",
-0000dbc0: 2074 696d 656f 7574 3d4e 6f6e 6529 3a0a   timeout=None):.
-0000dbd0: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-0000dbe0: 796e 635f 7265 7375 6c74 203d 2061 7379  ync_result = asy
-0000dbf0: 6e63 5f72 6573 756c 740a 2020 2020 2020  nc_result.      
-0000dc00: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-0000dc10: 5f5f 286d 6173 7465 7229 0a20 2020 2020  __(master).     
-0000dc20: 2020 2069 6620 6d69 7363 5f75 7469 6c73     if misc_utils
-0000dc30: 2e72 756e 6e69 6e67 5f6f 6e5f 6d61 635f  .running_on_mac_
-0000dc40: 6f73 2829 3a0a 2020 2020 2020 2020 2020  os():.          
-0000dc50: 2020 7365 6c66 2e63 6f6e 6669 6775 7265    self.configure
-0000dc60: 2862 6163 6b67 726f 756e 643d 2273 7973  (background="sys
-0000dc70: 7465 6d53 6865 6574 4261 636b 6772 6f75  temSheetBackgrou
-0000dc80: 6e64 2229 0a20 2020 2020 2020 2073 656c  nd").        sel
-0000dc90: 662e 7469 746c 6528 7469 746c 6529 0a20  f.title(title). 
-0000dca0: 2020 2020 2020 2073 656c 662e 7265 7369         self.resi
-0000dcb0: 7a61 626c 6528 6865 6967 6874 3d74 6b2e  zable(height=tk.
-0000dcc0: 4641 4c53 452c 2077 6964 7468 3d74 6b2e  FALSE, width=tk.
-0000dcd0: 4641 4c53 4529 0a20 2020 2020 2020 2023  FALSE).        #
-0000dce0: 2073 656c 662e 7072 6f74 6f63 6f6c 2822   self.protocol("
-0000dcf0: 574d 5f44 454c 4554 455f 5749 4e44 4f57  WM_DELETE_WINDOW
-0000dd00: 222c 2073 656c 662e 5f63 6c6f 7365 290a  ", self._close).
-0000dd10: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
-0000dd20: 635f 6c61 6265 6c20 3d20 7474 6b2e 4c61  c_label = ttk.La
-0000dd30: 6265 6c28 7365 6c66 2c20 7465 7874 3d64  bel(self, text=d
-0000dd40: 6573 6372 6970 7469 6f6e 2c20 7772 6170  escription, wrap
-0000dd50: 6c65 6e67 7468 3d33 3030 290a 2020 2020  length=300).    
-0000dd60: 2020 2020 7365 6c66 2e64 6573 635f 6c61      self.desc_la
-0000dd70: 6265 6c2e 6772 6964 2870 6164 783d 3230  bel.grid(padx=20
-0000dd80: 2c20 7061 6479 3d32 3029 0a0a 2020 2020  , pady=20)..    
-0000dd90: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
-0000dda0: 6964 6c65 7461 736b 7328 290a 0a20 2020  idletasks()..   
-0000ddb0: 2020 2020 2073 656c 662e 7469 6d65 6f75       self.timeou
-0000ddc0: 7420 3d20 7469 6d65 6f75 740a 2020 2020  t = timeout.    
-0000ddd0: 2020 2020 7365 6c66 2e73 7461 7274 5f74      self.start_t
-0000dde0: 696d 6520 3d20 7469 6d65 2e74 696d 6528  ime = time.time(
-0000ddf0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000de00: 6674 6572 2835 3030 2c20 7365 6c66 2e5f  fter(500, self._
-0000de10: 706f 6c6c 290a 0a20 2020 2064 6566 205f  poll)..    def _
-0000de20: 706f 6c6c 2873 656c 6629 3a0a 2020 2020  poll(self):.    
-0000de30: 2020 2020 6966 2073 656c 662e 5f61 7379      if self._asy
-0000de40: 6e63 5f72 6573 756c 742e 7265 6164 7928  nc_result.ready(
-0000de50: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000de60: 656c 662e 5f63 6c6f 7365 2829 0a20 2020  elf._close().   
-0000de70: 2020 2020 2065 6c69 6620 7365 6c66 2e74       elif self.t
-0000de80: 696d 656f 7574 2061 6e64 2074 696d 652e  imeout and time.
-0000de90: 7469 6d65 2829 202d 2073 656c 662e 7374  time() - self.st
-0000dea0: 6172 745f 7469 6d65 203e 2073 656c 662e  art_time > self.
-0000deb0: 7469 6d65 6f75 743a 0a20 2020 2020 2020  timeout:.       
-0000dec0: 2020 2020 2072 6169 7365 2054 696d 656f       raise Timeo
-0000ded0: 7574 4572 726f 7228 290a 2020 2020 2020  utError().      
-0000dee0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000def0: 2020 2020 7365 6c66 2e61 6674 6572 2835      self.after(5
-0000df00: 3030 2c20 7365 6c66 2e5f 706f 6c6c 290a  00, self._poll).
-0000df10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000df20: 2e64 6573 635f 6c61 6265 6c5b 2274 6578  .desc_label["tex
-0000df30: 7422 5d20 3d20 7365 6c66 2e64 6573 635f  t"] = self.desc_
-0000df40: 6c61 6265 6c5b 2274 6578 7422 5d20 2b20  label["text"] + 
-0000df50: 222e 220a 0a20 2020 2064 6566 205f 636c  "."..    def _cl
-0000df60: 6f73 6528 7365 6c66 293a 0a20 2020 2020  ose(self):.     
-0000df70: 2020 2073 656c 662e 6465 7374 726f 7928     self.destroy(
-0000df80: 290a 0a0a 6465 6620 7275 6e5f 7769 7468  )...def run_with
-0000df90: 5f77 6169 7469 6e67 5f64 6961 6c6f 6728  _waiting_dialog(
-0000dfa0: 6d61 7374 6572 2c20 6163 7469 6f6e 2c20  master, action, 
-0000dfb0: 6172 6773 3d28 292c 2064 6573 6372 6970  args=(), descrip
-0000dfc0: 7469 6f6e 3d22 576f 726b 696e 6722 293a  tion="Working"):
-0000dfd0: 0a20 2020 2023 2068 7474 703a 2f2f 7374  .    # http://st
-0000dfe0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-0000dff0: 612f 3134 3239 3930 3034 2f32 3631 3138  a/14299004/26118
-0000e000: 310a 2020 2020 6672 6f6d 206d 756c 7469  1.    from multi
-0000e010: 7072 6f63 6573 7369 6e67 2e70 6f6f 6c20  processing.pool 
-0000e020: 696d 706f 7274 2054 6872 6561 6450 6f6f  import ThreadPoo
-0000e030: 6c0a 0a20 2020 2070 6f6f 6c20 3d20 5468  l..    pool = Th
-0000e040: 7265 6164 506f 6f6c 2870 726f 6365 7373  readPool(process
-0000e050: 6573 3d31 290a 0a20 2020 2061 7379 6e63  es=1)..    async
-0000e060: 5f72 6573 756c 7420 3d20 706f 6f6c 2e61  _result = pool.a
-0000e070: 7070 6c79 5f61 7379 6e63 2861 6374 696f  pply_async(actio
-0000e080: 6e2c 2061 7267 7329 0a20 2020 2064 6c67  n, args).    dlg
-0000e090: 203d 2057 6169 7469 6e67 4469 616c 6f67   = WaitingDialog
-0000e0a0: 286d 6173 7465 722c 2061 7379 6e63 5f72  (master, async_r
-0000e0b0: 6573 756c 742c 2064 6573 6372 6970 7469  esult, descripti
-0000e0c0: 6f6e 3d64 6573 6372 6970 7469 6f6e 290a  on=description).
-0000e0d0: 2020 2020 7368 6f77 5f64 6961 6c6f 6728      show_dialog(
-0000e0e0: 646c 672c 206d 6173 7465 7229 0a0a 2020  dlg, master)..  
-0000e0f0: 2020 7265 7475 726e 2061 7379 6e63 5f72    return async_r
-0000e100: 6573 756c 742e 6765 7428 290a 0a0a 636c  esult.get()...cl
-0000e110: 6173 7320 4669 6c65 436f 7079 4469 616c  ass FileCopyDial
-0000e120: 6f67 2843 6f6d 6d6f 6e44 6961 6c6f 6729  og(CommonDialog)
-0000e130: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0000e140: 5f5f 2873 656c 662c 206d 6173 7465 722c  __(self, master,
-0000e150: 2073 6f75 7263 652c 2064 6573 7469 6e61   source, destina
-0000e160: 7469 6f6e 2c20 6465 7363 7269 7074 696f  tion, descriptio
-0000e170: 6e3d 4e6f 6e65 2c20 6673 796e 633d 5472  n=None, fsync=Tr
-0000e180: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-0000e190: 662e 5f73 6f75 7263 6520 3d20 736f 7572  f._source = sour
-0000e1a0: 6365 0a20 2020 2020 2020 2073 656c 662e  ce.        self.
-0000e1b0: 5f64 6573 7469 6e61 7469 6f6e 203d 2064  _destination = d
-0000e1c0: 6573 7469 6e61 7469 6f6e 0a20 2020 2020  estination.     
-0000e1d0: 2020 2073 656c 662e 5f6f 6c64 5f62 7974     self._old_byt
-0000e1e0: 6573 5f63 6f70 6965 6420 3d20 300a 2020  es_copied = 0.  
-0000e1f0: 2020 2020 2020 7365 6c66 2e5f 6279 7465        self._byte
-0000e200: 735f 636f 7069 6564 203d 2030 0a20 2020  s_copied = 0.   
-0000e210: 2020 2020 2073 656c 662e 5f66 7379 6e63       self._fsync
-0000e220: 203d 2066 7379 6e63 0a20 2020 2020 2020   = fsync.       
-0000e230: 2073 656c 662e 5f64 6f6e 6520 3d20 4661   self._done = Fa
-0000e240: 6c73 650a 2020 2020 2020 2020 7365 6c66  lse.        self
-0000e250: 2e5f 6361 6e63 656c 6c65 6420 3d20 4661  ._cancelled = Fa
-0000e260: 6c73 650a 2020 2020 2020 2020 7365 6c66  lse.        self
-0000e270: 2e5f 636c 6f73 6564 203d 2046 616c 7365  ._closed = False
-0000e280: 0a0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-0000e290: 292e 5f5f 696e 6974 5f5f 286d 6173 7465  ).__init__(maste
-0000e2a0: 7229 0a0a 2020 2020 2020 2020 6d61 696e  r)..        main
-0000e2b0: 5f66 7261 6d65 203d 2074 746b 2e46 7261  _frame = ttk.Fra
-0000e2c0: 6d65 2873 656c 6629 2020 2320 546f 2067  me(self)  # To g
-0000e2d0: 6574 2073 7479 6c65 6420 6261 636b 6772  et styled backgr
-0000e2e0: 6f75 6e64 0a20 2020 2020 2020 206d 6169  ound.        mai
-0000e2f0: 6e5f 6672 616d 652e 6772 6964 2872 6f77  n_frame.grid(row
-0000e300: 3d30 2c20 636f 6c75 6d6e 3d30 2c20 7374  =0, column=0, st
-0000e310: 6963 6b79 3d22 6e73 6577 2229 0a20 2020  icky="nsew").   
-0000e320: 2020 2020 2073 656c 662e 726f 7763 6f6e       self.rowcon
-0000e330: 6669 6775 7265 2830 2c20 7765 6967 6874  figure(0, weight
-0000e340: 3d31 290a 2020 2020 2020 2020 7365 6c66  =1).        self
-0000e350: 2e63 6f6c 756d 6e63 6f6e 6669 6775 7265  .columnconfigure
-0000e360: 2830 2c20 7765 6967 6874 3d31 290a 0a20  (0, weight=1).. 
-0000e370: 2020 2020 2020 2073 656c 662e 7469 746c         self.titl
-0000e380: 6528 7472 2822 436f 7079 696e 6722 2929  e(tr("Copying"))
-0000e390: 0a0a 2020 2020 2020 2020 6966 2064 6573  ..        if des
-0000e3a0: 6372 6970 7469 6f6e 2069 7320 4e6f 6e65  cription is None
-0000e3b0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-0000e3c0: 7363 7269 7074 696f 6e20 3d20 7472 2822  scription = tr("
-0000e3d0: 436f 7079 696e 675c 6e20 2025 735c 6e74  Copying\n  %s\nt
-0000e3e0: 6f5c 6e20 2025 7322 2920 2520 2873 6f75  o\n  %s") % (sou
-0000e3f0: 7263 652c 2064 6573 7469 6e61 7469 6f6e  rce, destination
-0000e400: 290a 0a20 2020 2020 2020 206c 6162 656c  )..        label
-0000e410: 203d 2074 746b 2e4c 6162 656c 286d 6169   = ttk.Label(mai
-0000e420: 6e5f 6672 616d 652c 2074 6578 743d 6465  n_frame, text=de
-0000e430: 7363 7269 7074 696f 6e29 0a20 2020 2020  scription).     
-0000e440: 2020 206c 6162 656c 2e67 7269 6428 726f     label.grid(ro
-0000e450: 773d 302c 2063 6f6c 756d 6e3d 302c 2063  w=0, column=0, c
-0000e460: 6f6c 756d 6e73 7061 6e3d 322c 2073 7469  olumnspan=2, sti
-0000e470: 636b 793d 226e 7722 2c20 7061 6478 3d31  cky="nw", padx=1
-0000e480: 352c 2070 6164 793d 3135 290a 0a20 2020  5, pady=15)..   
-0000e490: 2020 2020 2073 656c 662e 5f62 6172 203d       self._bar =
-0000e4a0: 2074 746b 2e50 726f 6772 6573 7362 6172   ttk.Progressbar
-0000e4b0: 286d 6169 6e5f 6672 616d 652c 206d 6178  (main_frame, max
-0000e4c0: 696d 756d 3d6f 732e 7061 7468 2e67 6574  imum=os.path.get
-0000e4d0: 7369 7a65 2873 6f75 7263 6529 2c20 6c65  size(source), le
-0000e4e0: 6e67 7468 3d32 3030 290a 2020 2020 2020  ngth=200).      
-0000e4f0: 2020 7365 6c66 2e5f 6261 722e 6772 6964    self._bar.grid
-0000e500: 2872 6f77 3d31 2c20 636f 6c75 6d6e 3d30  (row=1, column=0
-0000e510: 2c20 636f 6c75 6d6e 7370 616e 3d32 2c20  , columnspan=2, 
-0000e520: 7374 6963 6b79 3d22 6e73 6577 222c 2070  sticky="nsew", p
-0000e530: 6164 783d 3135 2c20 7061 6479 3d30 290a  adx=15, pady=0).
-0000e540: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-0000e550: 616e 6365 6c5f 6275 7474 6f6e 203d 2074  ancel_button = t
-0000e560: 746b 2e42 7574 746f 6e28 6d61 696e 5f66  tk.Button(main_f
-0000e570: 7261 6d65 2c20 7465 7874 3d74 7228 2243  rame, text=tr("C
-0000e580: 616e 6365 6c22 292c 2063 6f6d 6d61 6e64  ancel"), command
-0000e590: 3d73 656c 662e 5f63 616e 6365 6c29 0a20  =self._cancel). 
-0000e5a0: 2020 2020 2020 2073 656c 662e 5f63 616e         self._can
-0000e5b0: 6365 6c5f 6275 7474 6f6e 2e67 7269 6428  cel_button.grid(
-0000e5c0: 726f 773d 322c 2063 6f6c 756d 6e3d 312c  row=2, column=1,
-0000e5d0: 2073 7469 636b 793d 226e 6522 2c20 7061   sticky="ne", pa
-0000e5e0: 6478 3d31 352c 2070 6164 793d 3135 290a  dx=15, pady=15).
-0000e5f0: 2020 2020 2020 2020 7365 6c66 2e5f 6261          self._ba
-0000e600: 722e 666f 6375 735f 7365 7428 290a 0a20  r.focus_set().. 
-0000e610: 2020 2020 2020 206d 6169 6e5f 6672 616d         main_fram
-0000e620: 652e 636f 6c75 6d6e 636f 6e66 6967 7572  e.columnconfigur
-0000e630: 6528 302c 2077 6569 6768 743d 3129 0a0a  e(0, weight=1)..
-0000e640: 2020 2020 2020 2020 7365 6c66 2e5f 7570          self._up
-0000e650: 6461 7465 5f70 726f 6772 6573 7328 290a  date_progress().
-0000e660: 0a20 2020 2020 2020 2073 656c 662e 6269  .        self.bi
-0000e670: 6e64 2822 3c45 7363 6170 653e 222c 2073  nd("<Escape>", s
-0000e680: 656c 662e 5f63 616e 6365 6c2c 2054 7275  elf._cancel, Tru
-0000e690: 6529 2020 2320 6573 6361 7065 2d63 6c6f  e)  # escape-clo
-0000e6a0: 7365 206f 6e6c 7920 6966 2070 726f 6365  se only if proce
-0000e6b0: 7373 2068 6173 2063 6f6d 706c 6574 6564  ss has completed
-0000e6c0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-0000e6d0: 6f74 6f63 6f6c 2822 574d 5f44 454c 4554  otocol("WM_DELET
-0000e6e0: 455f 5749 4e44 4f57 222c 2073 656c 662e  E_WINDOW", self.
-0000e6f0: 5f63 616e 6365 6c29 0a20 2020 2020 2020  _cancel).       
-0000e700: 2073 656c 662e 5f73 7461 7274 2829 0a0a   self._start()..
-0000e710: 2020 2020 6465 6620 5f73 7461 7274 2873      def _start(s
-0000e720: 656c 6629 3a0a 2020 2020 2020 2020 6465  elf):.        de
-0000e730: 6620 776f 726b 2829 3a0a 2020 2020 2020  f work():.      
-0000e740: 2020 2020 2020 7365 6c66 2e5f 636f 7079        self._copy
-0000e750: 5f70 726f 6765 7373 203d 2030 0a0a 2020  _progess = 0..  
-0000e760: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-0000e770: 7065 6e28 7365 6c66 2e5f 736f 7572 6365  pen(self._source
-0000e780: 2c20 2272 6222 2920 6173 2066 7372 633a  , "rb") as fsrc:
-0000e790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e7a0: 2077 6974 6820 6f70 656e 2873 656c 662e   with open(self.
-0000e7b0: 5f64 6573 7469 6e61 7469 6f6e 2c20 2277  _destination, "w
-0000e7c0: 6222 2920 6173 2066 6473 743a 0a20 2020  b") as fdst:.   
-0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7e0: 2077 6869 6c65 2054 7275 653a 0a20 2020   while True:.   
+0000b0b0: 2c20 666f 6375 733d 4e6f 6e65 293a 0a20  , focus=None):. 
+0000b0c0: 2020 2020 2020 2023 2043 6f6d 7075 7465         # Compute
+0000b0d0: 2074 6865 2061 7265 6120 7468 6174 2077   the area that w
+0000b0e0: 696c 6c20 6265 2064 6573 6372 6962 6564  ill be described
+0000b0f0: 2062 7920 7468 6973 204e 6f74 650a 2020   by this Note.  
+0000b100: 2020 2020 2020 666f 6375 735f 7820 3d20        focus_x = 
+0000b110: 7461 7267 6574 2e77 696e 666f 5f72 6f6f  target.winfo_roo
+0000b120: 7478 2829 0a20 2020 2020 2020 2066 6f63  tx().        foc
+0000b130: 7573 5f79 203d 2074 6172 6765 742e 7769  us_y = target.wi
+0000b140: 6e66 6f5f 726f 6f74 7928 290a 2020 2020  nfo_rooty().    
+0000b150: 2020 2020 666f 6375 735f 6865 6967 6874      focus_height
+0000b160: 203d 2074 6172 6765 742e 7769 6e66 6f5f   = target.winfo_
+0000b170: 6865 6967 6874 2829 0a0a 2020 2020 2020  height()..      
+0000b180: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000b190: 666f 6375 732c 2054 6578 7452 616e 6765  focus, TextRange
+0000b1a0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+0000b1b0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
+0000b1c0: 2874 6172 6765 742c 2074 6b2e 5465 7874  (target, tk.Text
+0000b1d0: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
+0000b1e0: 706c 6566 7420 3d20 7461 7267 6574 2e62  pleft = target.b
+0000b1f0: 626f 7828 2225 642e 2564 2220 2520 2866  box("%d.%d" % (f
+0000b200: 6f63 7573 2e6c 696e 656e 6f2c 2066 6f63  ocus.lineno, foc
+0000b210: 7573 2e63 6f6c 5f6f 6666 7365 7429 290a  us.col_offset)).
+0000b220: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+0000b230: 6f63 7573 2e65 6e64 5f63 6f6c 5f6f 6666  ocus.end_col_off
+0000b240: 7365 7420 3d3d 2030 3a0a 2020 2020 2020  set == 0:.      
+0000b250: 2020 2020 2020 2020 2020 626f 7472 6967            botrig
+0000b260: 6874 203d 2074 6172 6765 742e 6262 6f78  ht = target.bbox
+0000b270: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000b280: 2020 2020 2020 2225 642e 2564 206c 696e        "%d.%d lin
+0000b290: 6565 6e64 2220 2520 2866 6f63 7573 2e65  eend" % (focus.e
+0000b2a0: 6e64 5f6c 696e 656e 6f20 2d20 312c 2066  nd_lineno - 1, f
+0000b2b0: 6f63 7573 2e65 6e64 5f6c 696e 656e 6f20  ocus.end_lineno 
+0000b2c0: 2d20 3129 0a20 2020 2020 2020 2020 2020  - 1).           
+0000b2d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000b2e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b2f0: 2020 2020 2020 2020 2062 6f74 7269 6768           botrigh
+0000b300: 7420 3d20 7461 7267 6574 2e62 626f 7828  t = target.bbox(
+0000b310: 2225 642e 2564 2220 2520 2866 6f63 7573  "%d.%d" % (focus
+0000b320: 2e65 6e64 5f6c 696e 656e 6f2c 2066 6f63  .end_lineno, foc
+0000b330: 7573 2e65 6e64 5f63 6f6c 5f6f 6666 7365  us.end_col_offse
+0000b340: 7429 290a 0a20 2020 2020 2020 2020 2020  t))..           
+0000b350: 2069 6620 746f 706c 6566 7420 616e 6420   if topleft and 
+0000b360: 626f 7472 6967 6874 3a0a 2020 2020 2020  botright:.      
+0000b370: 2020 2020 2020 2020 2020 666f 6375 735f            focus_
+0000b380: 7820 2b3d 2074 6f70 6c65 6674 5b30 5d0a  x += topleft[0].
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 666f 6375 735f 7920 2b3d 2074 6f70 6c65  focus_y += tople
+0000b3b0: 6674 5b31 5d0a 2020 2020 2020 2020 2020  ft[1].          
+0000b3c0: 2020 2020 2020 666f 6375 735f 6865 6967        focus_heig
+0000b3d0: 6874 203d 2062 6f74 7269 6768 745b 315d  ht = botright[1]
+0000b3e0: 202d 2074 6f70 6c65 6674 5b31 5d20 2b20   - topleft[1] + 
+0000b3f0: 626f 7472 6967 6874 5b33 5d0a 0a20 2020  botright[3]..   
+0000b400: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+0000b410: 616e 6365 2866 6f63 7573 2c20 286c 6973  ance(focus, (lis
+0000b420: 742c 2074 7570 6c65 2929 3a0a 2020 2020  t, tuple)):.    
+0000b430: 2020 2020 2020 2020 666f 6375 735f 7820          focus_x 
+0000b440: 2b3d 2066 6f63 7573 5b30 5d0a 2020 2020  += focus[0].    
+0000b450: 2020 2020 2020 2020 666f 6375 735f 7920          focus_y 
+0000b460: 2b3d 2066 6f63 7573 5b31 5d0a 2020 2020  += focus[1].    
+0000b470: 2020 2020 2020 2020 666f 6375 735f 6865          focus_he
+0000b480: 6967 6874 203d 2066 6f63 7573 5b33 5d0a  ight = focus[3].
+0000b490: 0a20 2020 2020 2020 2065 6c69 6620 666f  .        elif fo
+0000b4a0: 6375 7320 6973 204e 6f6e 653a 0a20 2020  cus is None:.   
+0000b4b0: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
+0000b4c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000b4d0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0000b4e0: 7970 6545 7272 6f72 2822 556e 7375 7070  ypeError("Unsupp
+0000b4f0: 6f72 7465 6420 666f 6375 7322 290a 0a20  orted focus").. 
+0000b500: 2020 2020 2020 2023 2043 6f6d 7075 7465         # Compute
+0000b510: 2064 696d 656e 7369 6f6e 7320 6f66 2074   dimensions of t
+0000b520: 6865 206e 6f74 650a 2020 2020 2020 2020  he note.        
+0000b530: 666f 6e74 203d 2073 656c 662e 7465 7874  font = self.text
+0000b540: 5b22 666f 6e74 225d 0a20 2020 2020 2020  ["font"].       
+0000b550: 2069 6620 6973 696e 7374 616e 6365 2866   if isinstance(f
+0000b560: 6f6e 742c 2073 7472 293a 0a20 2020 2020  ont, str):.     
+0000b570: 2020 2020 2020 2066 6f6e 7420 3d20 746b         font = tk
+0000b580: 2e66 6f6e 742e 6e61 6d65 746f 666f 6e74  .font.nametofont
+0000b590: 2866 6f6e 7429 0a0a 2020 2020 2020 2020  (font)..        
+0000b5a0: 6c69 6e65 7320 3d20 7365 6c66 2e5f 6375  lines = self._cu
+0000b5b0: 7272 656e 745f 6368 6172 732e 7370 6c69  rrent_chars.spli
+0000b5c0: 746c 696e 6573 2829 0a20 2020 2020 2020  tlines().       
+0000b5d0: 206d 6178 5f6c 696e 655f 7769 6474 6820   max_line_width 
+0000b5e0: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
+0000b5f0: 6c69 6e65 2069 6e20 6c69 6e65 733a 0a20  line in lines:. 
+0000b600: 2020 2020 2020 2020 2020 206d 6178 5f6c             max_l
+0000b610: 696e 655f 7769 6474 6820 3d20 6d61 7828  ine_width = max(
+0000b620: 6d61 785f 6c69 6e65 5f77 6964 7468 2c20  max_line_width, 
+0000b630: 666f 6e74 2e6d 6561 7375 7265 286c 696e  font.measure(lin
+0000b640: 6529 290a 0a20 2020 2020 2020 2077 6964  e))..        wid
+0000b650: 7468 203d 206d 696e 286d 6178 5f6c 696e  th = min(max_lin
+0000b660: 655f 7769 6474 682c 2073 656c 662e 5f6d  e_width, self._m
+0000b670: 6178 5f64 6566 6175 6c74 5f77 6964 7468  ax_default_width
+0000b680: 2920 2b20 7365 6c66 2e70 6164 7820 2a20  ) + self.padx * 
+0000b690: 3220 2b20 320a 2020 2020 2020 2020 7365  2 + 2.        se
+0000b6a0: 6c66 2e77 6d5f 6765 6f6d 6574 7279 2822  lf.wm_geometry("
+0000b6b0: 2564 7825 642b 2564 2b25 6422 2025 2028  %dx%d+%d+%d" % (
+0000b6c0: 7769 6474 682c 2031 3030 2c20 666f 6375  width, 100, focu
+0000b6d0: 735f 782c 2066 6f63 7573 5f79 202b 2066  s_x, focus_y + f
+0000b6e0: 6f63 7573 5f68 6569 6768 7429 290a 0a20  ocus_height)).. 
+0000b6f0: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+0000b700: 7465 5f69 646c 6574 6173 6b73 2829 0a20  te_idletasks(). 
+0000b710: 2020 2020 2020 206c 696e 655f 636f 756e         line_coun
+0000b720: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
+0000b730: 6c66 2e74 6578 742e 696e 6465 7828 2265  lf.text.index("e
+0000b740: 6e64 2229 2929 0a20 2020 2020 2020 206c  nd"))).        l
+0000b750: 696e 655f 6865 6967 6874 203d 2066 6f6e  ine_height = fon
+0000b760: 742e 6d65 7472 6963 7328 295b 226c 696e  t.metrics()["lin
+0000b770: 6573 7061 6365 225d 0a0a 2020 2020 2020  espace"]..      
+0000b780: 2020 7365 6c66 2e77 6d5f 6765 6f6d 6574    self.wm_geomet
+0000b790: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
+0000b7a0: 2225 6478 2564 2b25 642b 2564 2220 2520  "%dx%d+%d+%d" % 
+0000b7b0: 2877 6964 7468 2c20 6c69 6e65 5f63 6f75  (width, line_cou
+0000b7c0: 6e74 202a 206c 696e 655f 6865 6967 6874  nt * line_height
+0000b7d0: 2c20 666f 6375 735f 782c 2066 6f63 7573  , focus_x, focus
+0000b7e0: 5f79 202b 2066 6f63 7573 5f68 6569 6768  _y + focus_heigh
+0000b7f0: 7429 0a20 2020 2020 2020 2029 0a0a 2020  t).        )..  
+0000b800: 2020 2020 2020 2320 544f 444f 3a20 6465        # TODO: de
+0000b810: 7465 6374 2074 6865 2073 6974 7561 7469  tect the situati
+0000b820: 6f6e 2077 6865 6e20 6e6f 7465 2064 6f65  on when note doe
+0000b830: 736e 2774 2066 6974 2075 6e64 6572 0a20  sn't fit under. 
+0000b840: 2020 2020 2020 2023 2074 6865 2066 6f63         # the foc
+0000b850: 7573 2062 6f78 2061 6e64 2073 686f 756c  us box and shoul
+0000b860: 6420 6265 2070 6c61 6365 6420 6162 6f76  d be placed abov
+0000b870: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0000b880: 6465 6963 6f6e 6966 7928 290a 0a20 2020  deiconify()..   
+0000b890: 2064 6566 2073 686f 775f 6e6f 7465 2873   def show_note(s
+0000b8a0: 656c 662c 202a 636f 6e74 656e 745f 6974  elf, *content_it
+0000b8b0: 656d 733a 2055 6e69 6f6e 5b73 7472 2c20  ems: Union[str, 
+0000b8c0: 4c69 7374 5d2c 2074 6172 6765 743d 4e6f  List], target=No
+0000b8d0: 6e65 2c20 666f 6375 733d 4e6f 6e65 2920  ne, focus=None) 
+0000b8e0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+0000b8f0: 2073 656c 662e 7365 745f 636f 6e74 656e   self.set_conten
+0000b900: 7428 2a63 6f6e 7465 6e74 5f69 7465 6d73  t(*content_items
+0000b910: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+0000b920: 6c61 6365 2874 6172 6765 742c 2066 6f63  lace(target, foc
+0000b930: 7573 290a 0a20 2020 2064 6566 205f 636c  us)..    def _cl
+0000b940: 6f73 655f 6d61 7962 6528 7365 6c66 2c20  ose_maybe(self, 
+0000b950: 6576 656e 7429 3a0a 2020 2020 2020 2020  event):.        
+0000b960: 6966 2065 7665 6e74 2e77 6964 6765 7420  if event.widget 
+0000b970: 6e6f 7420 696e 205b 7365 6c66 2c20 7365  not in [self, se
+0000b980: 6c66 2e74 6578 745d 3a0a 2020 2020 2020  lf.text]:.      
+0000b990: 2020 2020 2020 7365 6c66 2e63 6c6f 7365        self.close
+0000b9a0: 2865 7665 6e74 290a 0a20 2020 2064 6566  (event)..    def
+0000b9b0: 2063 6c6f 7365 2873 656c 662c 2065 7665   close(self, eve
+0000b9c0: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
+0000b9d0: 2020 7365 6c66 2e77 6974 6864 7261 7728    self.withdraw(
+0000b9e0: 290a 0a0a 6465 6620 6765 745f 7769 6467  )...def get_widg
+0000b9f0: 6574 5f6f 6666 7365 745f 6672 6f6d 5f74  et_offset_from_t
+0000ba00: 6f70 6c65 7665 6c28 7769 6467 6574 293a  oplevel(widget):
+0000ba10: 0a20 2020 2078 203d 2030 0a20 2020 2079  .    x = 0.    y
+0000ba20: 203d 2030 0a20 2020 2074 6f70 6c65 7665   = 0.    topleve
+0000ba30: 6c20 3d20 7769 6467 6574 2e77 696e 666f  l = widget.winfo
+0000ba40: 5f74 6f70 6c65 7665 6c28 290a 2020 2020  _toplevel().    
+0000ba50: 7768 696c 6520 7769 6467 6574 2021 3d20  while widget != 
+0000ba60: 746f 706c 6576 656c 3a0a 2020 2020 2020  toplevel:.      
+0000ba70: 2020 7820 2b3d 2077 6964 6765 742e 7769    x += widget.wi
+0000ba80: 6e66 6f5f 7828 290a 2020 2020 2020 2020  nfo_x().        
+0000ba90: 7920 2b3d 2077 6964 6765 742e 7769 6e66  y += widget.winf
+0000baa0: 6f5f 7928 290a 2020 2020 2020 2020 7769  o_y().        wi
+0000bab0: 6467 6574 203d 2077 6964 6765 742e 6d61  dget = widget.ma
+0000bac0: 7374 6572 0a20 2020 2072 6574 7572 6e20  ster.    return 
+0000bad0: 782c 2079 0a0a 0a63 6c61 7373 2045 6e68  x, y...class Enh
+0000bae0: 616e 6365 6456 6172 2874 6b2e 5661 7269  ancedVar(tk.Vari
+0000baf0: 6162 6c65 293a 0a20 2020 2064 6566 205f  able):.    def _
+0000bb00: 5f69 6e69 745f 5f28 7365 6c66 2c20 6d61  _init__(self, ma
+0000bb10: 7374 6572 3d4e 6f6e 652c 2076 616c 7565  ster=None, value
+0000bb20: 3d4e 6f6e 652c 206e 616d 653d 4e6f 6e65  =None, name=None
+0000bb30: 2c20 6d6f 6469 6669 6361 7469 6f6e 5f6c  , modification_l
+0000bb40: 6973 7465 6e65 723d 4e6f 6e65 293a 0a20  istener=None):. 
+0000bb50: 2020 2020 2020 2069 6620 6d61 7374 6572         if master
+0000bb60: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000bb70: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0000bb80: 6d61 7374 6572 2c20 2874 6b2e 5769 6467  master, (tk.Widg
+0000bb90: 6574 2c20 746b 2e57 6d29 293a 0a20 2020  et, tk.Wm)):.   
+0000bba0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0000bbb0: 7970 6545 7272 6f72 2822 4669 7273 7420  ypeError("First 
+0000bbc0: 706f 7369 7469 6f6e 616c 2061 7267 756d  positional argum
+0000bbd0: 656e 7420 276d 6173 7465 7227 206d 7573  ent 'master' mus
+0000bbe0: 7420 6265 204e 6f6e 652c 2057 6964 6765  t be None, Widge
+0000bbf0: 7420 6f72 2057 6d22 290a 0a20 2020 2020  t or Wm")..     
+0000bc00: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+0000bc10: 745f 5f28 6d61 7374 6572 3d6d 6173 7465  t__(master=maste
+0000bc20: 722c 2076 616c 7565 3d76 616c 7565 2c20  r, value=value, 
+0000bc30: 6e61 6d65 3d6e 616d 6529 0a20 2020 2020  name=name).     
+0000bc40: 2020 2073 656c 662e 6d6f 6469 6669 6564     self.modified
+0000bc50: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+0000bc60: 2073 656c 662e 6d6f 6469 6669 6361 7469   self.modificati
+0000bc70: 6f6e 5f6c 6973 7465 6e65 7220 3d20 6d6f  on_listener = mo
+0000bc80: 6469 6669 6361 7469 6f6e 5f6c 6973 7465  dification_liste
+0000bc90: 6e65 720a 2020 2020 2020 2020 6966 2073  ner.        if s
+0000bca0: 7973 2e76 6572 7369 6f6e 5f69 6e66 6f20  ys.version_info 
+0000bcb0: 3c20 2833 2c20 3629 3a0a 2020 2020 2020  < (3, 6):.      
+0000bcc0: 2020 2020 2020 7365 6c66 2e74 7261 6365        self.trace
+0000bcd0: 2822 7722 2c20 7365 6c66 2e5f 6f6e 5f77  ("w", self._on_w
+0000bce0: 7269 7465 290a 2020 2020 2020 2020 656c  rite).        el
+0000bcf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000bd00: 7365 6c66 2e74 7261 6365 5f61 6464 2822  self.trace_add("
+0000bd10: 7772 6974 6522 2c20 7365 6c66 2e5f 6f6e  write", self._on
+0000bd20: 5f77 7269 7465 290a 0a20 2020 2064 6566  _write)..    def
+0000bd30: 205f 6f6e 5f77 7269 7465 2873 656c 662c   _on_write(self,
+0000bd40: 202a 6172 6773 293a 0a20 2020 2020 2020   *args):.       
+0000bd50: 2073 656c 662e 6d6f 6469 6669 6564 203d   self.modified =
+0000bd60: 2054 7275 650a 2020 2020 2020 2020 6966   True.        if
+0000bd70: 2073 656c 662e 6d6f 6469 6669 6361 7469   self.modificati
+0000bd80: 6f6e 5f6c 6973 7465 6e65 723a 0a20 2020  on_listener:.   
+0000bd90: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000bdb0: 6c66 2e6d 6f64 6966 6963 6174 696f 6e5f  lf.modification_
+0000bdc0: 6c69 7374 656e 6572 2829 0a20 2020 2020  listener().     
+0000bdd0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+0000bde0: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
+0000bdf0: 2020 2020 2020 2020 2023 204f 7468 6572           # Other
+0000be00: 7769 7365 2077 686f 6c65 2070 726f 6365  wise whole proce
+0000be10: 7373 2077 696c 6c20 6265 2062 726f 7567  ss will be broug
+0000be20: 6874 2064 6f77 6e0a 2020 2020 2020 2020  ht down.        
+0000be30: 2020 2020 2020 2020 2320 6265 6361 7573          # becaus
+0000be40: 6520 666f 7220 736f 6d65 2072 6561 736f  e for some reaso
+0000be50: 6e20 546b 2074 7269 6573 2074 6f20 6361  n Tk tries to ca
+0000be60: 6c6c 206e 6f6e 2d65 7869 7374 696e 6720  ll non-existing 
+0000be70: 6d65 7468 6f64 0a20 2020 2020 2020 2020  method.         
+0000be80: 2020 2020 2020 2023 206f 6e20 7661 7269         # on vari
+0000be90: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+0000bea0: 2020 2020 2067 6574 5f77 6f72 6b62 656e       get_workben
+0000beb0: 6368 2829 2e72 6570 6f72 745f 6578 6365  ch().report_exce
+0000bec0: 7074 696f 6e28 290a 0a0a 636c 6173 7320  ption()...class 
+0000bed0: 456e 6861 6e63 6564 5374 7269 6e67 5661  EnhancedStringVa
+0000bee0: 7228 456e 6861 6e63 6564 5661 722c 2074  r(EnhancedVar, t
+0000bef0: 6b2e 5374 7269 6e67 5661 7229 3a0a 2020  k.StringVar):.  
+0000bf00: 2020 7061 7373 0a0a 0a63 6c61 7373 2045    pass...class E
+0000bf10: 6e68 616e 6365 6449 6e74 5661 7228 456e  nhancedIntVar(En
+0000bf20: 6861 6e63 6564 5661 722c 2074 6b2e 496e  hancedVar, tk.In
+0000bf30: 7456 6172 293a 0a20 2020 2070 6173 730a  tVar):.    pass.
+0000bf40: 0a0a 636c 6173 7320 456e 6861 6e63 6564  ..class Enhanced
+0000bf50: 426f 6f6c 6561 6e56 6172 2845 6e68 616e  BooleanVar(Enhan
+0000bf60: 6365 6456 6172 2c20 746b 2e42 6f6f 6c65  cedVar, tk.Boole
+0000bf70: 616e 5661 7229 3a0a 2020 2020 7061 7373  anVar):.    pass
+0000bf80: 0a0a 0a63 6c61 7373 2045 6e68 616e 6365  ...class Enhance
+0000bf90: 6444 6f75 626c 6556 6172 2845 6e68 616e  dDoubleVar(Enhan
+0000bfa0: 6365 6456 6172 2c20 746b 2e44 6f75 626c  cedVar, tk.Doubl
+0000bfb0: 6556 6172 293a 0a20 2020 2070 6173 730a  eVar):.    pass.
+0000bfc0: 0a0a 6465 6620 6372 6561 7465 5f73 7472  ..def create_str
+0000bfd0: 696e 675f 7661 7228 7661 6c75 652c 206d  ing_var(value, m
+0000bfe0: 6f64 6966 6963 6174 696f 6e5f 6c69 7374  odification_list
+0000bff0: 656e 6572 3d4e 6f6e 6529 202d 3e20 456e  ener=None) -> En
+0000c000: 6861 6e63 6564 5374 7269 6e67 5661 723a  hancedStringVar:
+0000c010: 0a20 2020 2022 2222 4372 6561 7465 7320  .    """Creates 
+0000c020: 6120 746b 2e53 7472 696e 6756 6172 2077  a tk.StringVar w
+0000c030: 6974 6820 226d 6f64 6966 6965 6422 2061  ith "modified" a
+0000c040: 7474 7269 6275 7465 0a20 2020 2073 686f  ttribute.    sho
+0000c050: 7769 6e67 2077 6865 7468 6572 2074 6865  wing whether the
+0000c060: 2076 6172 6961 626c 6520 6861 7320 6265   variable has be
+0000c070: 656e 206d 6f64 6966 6965 6420 6166 7465  en modified afte
+0000c080: 7220 6372 6561 7469 6f6e 2222 220a 2020  r creation""".  
+0000c090: 2020 7265 7475 726e 2045 6e68 616e 6365    return Enhance
+0000c0a0: 6453 7472 696e 6756 6172 284e 6f6e 652c  dStringVar(None,
+0000c0b0: 2076 616c 7565 2c20 4e6f 6e65 2c20 6d6f   value, None, mo
+0000c0c0: 6469 6669 6361 7469 6f6e 5f6c 6973 7465  dification_liste
+0000c0d0: 6e65 7229 0a0a 0a64 6566 2063 7265 6174  ner)...def creat
+0000c0e0: 655f 696e 745f 7661 7228 7661 6c75 652c  e_int_var(value,
+0000c0f0: 206d 6f64 6966 6963 6174 696f 6e5f 6c69   modification_li
+0000c100: 7374 656e 6572 3d4e 6f6e 6529 202d 3e20  stener=None) -> 
+0000c110: 456e 6861 6e63 6564 496e 7456 6172 3a0a  EnhancedIntVar:.
+0000c120: 2020 2020 2222 2253 6565 2063 7265 6174      """See creat
+0000c130: 655f 7374 7269 6e67 5f76 6172 2222 220a  e_string_var""".
+0000c140: 2020 2020 7265 7475 726e 2045 6e68 616e      return Enhan
+0000c150: 6365 6449 6e74 5661 7228 4e6f 6e65 2c20  cedIntVar(None, 
+0000c160: 7661 6c75 652c 204e 6f6e 652c 206d 6f64  value, None, mod
+0000c170: 6966 6963 6174 696f 6e5f 6c69 7374 656e  ification_listen
+0000c180: 6572 290a 0a0a 6465 6620 6372 6561 7465  er)...def create
+0000c190: 5f64 6f75 626c 655f 7661 7228 7661 6c75  _double_var(valu
+0000c1a0: 652c 206d 6f64 6966 6963 6174 696f 6e5f  e, modification_
+0000c1b0: 6c69 7374 656e 6572 3d4e 6f6e 6529 202d  listener=None) -
+0000c1c0: 3e20 456e 6861 6e63 6564 446f 7562 6c65  > EnhancedDouble
+0000c1d0: 5661 723a 0a20 2020 2022 2222 5365 6520  Var:.    """See 
+0000c1e0: 6372 6561 7465 5f73 7472 696e 675f 7661  create_string_va
+0000c1f0: 7222 2222 0a20 2020 2072 6574 7572 6e20  r""".    return 
+0000c200: 456e 6861 6e63 6564 446f 7562 6c65 5661  EnhancedDoubleVa
+0000c210: 7228 4e6f 6e65 2c20 7661 6c75 652c 204e  r(None, value, N
+0000c220: 6f6e 652c 206d 6f64 6966 6963 6174 696f  one, modificatio
+0000c230: 6e5f 6c69 7374 656e 6572 290a 0a0a 6465  n_listener)...de
+0000c240: 6620 6372 6561 7465 5f62 6f6f 6c65 616e  f create_boolean
+0000c250: 5f76 6172 2876 616c 7565 2c20 6d6f 6469  _var(value, modi
+0000c260: 6669 6361 7469 6f6e 5f6c 6973 7465 6e65  fication_listene
+0000c270: 723d 4e6f 6e65 2920 2d3e 2045 6e68 616e  r=None) -> Enhan
+0000c280: 6365 6442 6f6f 6c65 616e 5661 723a 0a20  cedBooleanVar:. 
+0000c290: 2020 2022 2222 5365 6520 6372 6561 7465     """See create
+0000c2a0: 5f73 7472 696e 675f 7661 7222 2222 0a20  _string_var""". 
+0000c2b0: 2020 2072 6574 7572 6e20 456e 6861 6e63     return Enhanc
+0000c2c0: 6564 426f 6f6c 6561 6e56 6172 284e 6f6e  edBooleanVar(Non
+0000c2d0: 652c 2076 616c 7565 2c20 4e6f 6e65 2c20  e, value, None, 
+0000c2e0: 6d6f 6469 6669 6361 7469 6f6e 5f6c 6973  modification_lis
+0000c2f0: 7465 6e65 7229 0a0a 0a64 6566 2073 6869  tener)...def shi
+0000c300: 6674 5f69 735f 7072 6573 7365 6428 6576  ft_is_pressed(ev
+0000c310: 656e 743a 2074 6b2e 4576 656e 7429 202d  ent: tk.Event) -
+0000c320: 3e20 626f 6f6c 3a0a 2020 2020 2320 6874  > bool:.    # ht
+0000c330: 7470 733a 2f2f 746b 646f 6373 2e63 6f6d  tps://tkdocs.com
+0000c340: 2f73 6869 706d 616e 2f65 7665 6e74 2d68  /shipman/event-h
+0000c350: 616e 646c 6572 732e 6874 6d6c 0a20 2020  andlers.html.   
+0000c360: 2023 2068 7474 703a 2f2f 7374 6163 6b6f   # http://stacko
+0000c370: 7665 7266 6c6f 772e 636f 6d2f 712f 3332  verflow.com/q/32
+0000c380: 3432 3632 3530 2f32 3631 3138 310a 2020  426250/261181.  
+0000c390: 2020 7265 7475 726e 2065 7665 6e74 2e73    return event.s
+0000c3a0: 7461 7465 2026 2030 7830 3030 310a 0a0a  tate & 0x0001...
+0000c3b0: 6465 6620 6361 7073 5f6c 6f63 6b5f 6973  def caps_lock_is
+0000c3c0: 5f6f 6e28 6576 656e 743a 2074 6b2e 4576  _on(event: tk.Ev
+0000c3d0: 656e 7429 202d 3e20 626f 6f6c 3a0a 2020  ent) -> bool:.  
+0000c3e0: 2020 2320 6874 7470 733a 2f2f 746b 646f    # https://tkdo
+0000c3f0: 6373 2e63 6f6d 2f73 6869 706d 616e 2f65  cs.com/shipman/e
+0000c400: 7665 6e74 2d68 616e 646c 6572 732e 6874  vent-handlers.ht
+0000c410: 6d6c 0a20 2020 2023 2068 7474 703a 2f2f  ml.    # http://
+0000c420: 7374 6163 6b6f 7665 7266 6c6f 772e 636f  stackoverflow.co
+0000c430: 6d2f 712f 3332 3432 3632 3530 2f32 3631  m/q/32426250/261
+0000c440: 3138 310a 2020 2020 7265 7475 726e 2065  181.    return e
+0000c450: 7665 6e74 2e73 7461 7465 2026 2030 7830  vent.state & 0x0
+0000c460: 3030 320a 0a0a 6465 6620 636f 6e74 726f  002...def contro
+0000c470: 6c5f 6973 5f70 7265 7373 6564 2865 7665  l_is_pressed(eve
+0000c480: 6e74 3a20 746b 2e45 7665 6e74 2920 2d3e  nt: tk.Event) ->
+0000c490: 2062 6f6f 6c3a 0a20 2020 2023 2068 7474   bool:.    # htt
+0000c4a0: 7073 3a2f 2f74 6b64 6f63 732e 636f 6d2f  ps://tkdocs.com/
+0000c4b0: 7368 6970 6d61 6e2f 6576 656e 742d 6861  shipman/event-ha
+0000c4c0: 6e64 6c65 7273 2e68 746d 6c0a 2020 2020  ndlers.html.    
+0000c4d0: 2320 6874 7470 3a2f 2f73 7461 636b 6f76  # http://stackov
+0000c4e0: 6572 666c 6f77 2e63 6f6d 2f71 2f33 3234  erflow.com/q/324
+0000c4f0: 3236 3235 302f 3236 3131 3831 0a20 2020  26250/261181.   
+0000c500: 2072 6574 7572 6e20 6576 656e 742e 7374   return event.st
+0000c510: 6174 6520 2620 3078 3030 3034 0a0a 0a64  ate & 0x0004...d
+0000c520: 6566 2061 6c74 5f69 735f 7072 6573 7365  ef alt_is_presse
+0000c530: 645f 7769 7468 6f75 745f 6368 6172 2865  d_without_char(e
+0000c540: 7665 6e74 3a20 746b 2e45 7665 6e74 2920  vent: tk.Event) 
+0000c550: 2d3e 2062 6f6f 6c3a 0a20 2020 2023 2068  -> bool:.    # h
+0000c560: 7474 7073 3a2f 2f74 6b64 6f63 732e 636f  ttps://tkdocs.co
+0000c570: 6d2f 7368 6970 6d61 6e2f 6576 656e 742d  m/shipman/event-
+0000c580: 6861 6e64 6c65 7273 2e68 746d 6c0a 2020  handlers.html.  
+0000c590: 2020 2320 6874 7470 3a2f 2f73 7461 636b    # http://stack
+0000c5a0: 6f76 6572 666c 6f77 2e63 6f6d 2f71 2f33  overflow.com/q/3
+0000c5b0: 3234 3236 3235 302f 3236 3131 3831 0a20  2426250/261181. 
+0000c5c0: 2020 2023 2068 7474 7073 3a2f 2f62 7567     # https://bug
+0000c5d0: 732e 7079 7468 6f6e 2e6f 7267 2f6d 7367  s.python.org/msg
+0000c5e0: 3236 3834 3239 0a20 2020 2069 6620 6576  268429.    if ev
+0000c5f0: 656e 742e 6368 6172 3a0a 2020 2020 2020  ent.char:.      
+0000c600: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+0000c610: 2020 2020 6966 2072 756e 6e69 6e67 5f6f      if running_o
+0000c620: 6e5f 7769 6e64 6f77 7328 293a 0a20 2020  n_windows():.   
+0000c630: 2020 2020 2072 6574 7572 6e20 6576 656e       return even
+0000c640: 742e 7374 6174 6520 2620 3078 3230 3030  t.state & 0x2000
+0000c650: 300a 2020 2020 656c 6966 2072 756e 6e69  0.    elif runni
+0000c660: 6e67 5f6f 6e5f 6d61 635f 6f73 2829 3a0a  ng_on_mac_os():.
+0000c670: 2020 2020 2020 2020 2320 636f 6d62 696e          # combin
+0000c680: 6174 696f 6e73 2061 6c77 6179 7320 7072  ations always pr
+0000c690: 6f64 7563 6520 6120 6368 6172 206f 7220  oduce a char or 
+0000c6a0: 6172 6520 636f 6e73 756d 6564 2062 7920  are consumed by 
+0000c6b0: 7468 6520 4f53 0a20 2020 2020 2020 2072  the OS.        r
+0000c6c0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0000c6d0: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+0000c6e0: 7475 726e 2065 7665 6e74 2e73 7461 7465  turn event.state
+0000c6f0: 2026 2030 7830 3031 300a 0a0a 6465 6620   & 0x0010...def 
+0000c700: 636f 6d6d 616e 645f 6973 5f70 7265 7373  command_is_press
+0000c710: 6564 2865 7665 6e74 3a20 746b 2e45 7665  ed(event: tk.Eve
+0000c720: 6e74 2920 2d3e 2062 6f6f 6c3a 0a20 2020  nt) -> bool:.   
+0000c730: 2023 2068 7474 7073 3a2f 2f74 6b64 6f63   # https://tkdoc
+0000c740: 732e 636f 6d2f 7368 6970 6d61 6e2f 6576  s.com/shipman/ev
+0000c750: 656e 742d 6861 6e64 6c65 7273 2e68 746d  ent-handlers.htm
+0000c760: 6c0a 2020 2020 2320 6874 7470 3a2f 2f73  l.    # http://s
+0000c770: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
+0000c780: 2f71 2f33 3234 3236 3235 302f 3236 3131  /q/32426250/2611
+0000c790: 3831 0a20 2020 2069 6620 6e6f 7420 7275  81.    if not ru
+0000c7a0: 6e6e 696e 675f 6f6e 5f6d 6163 5f6f 7328  nning_on_mac_os(
+0000c7b0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0000c7c0: 6e20 4661 6c73 650a 2020 2020 7265 7475  n False.    retu
+0000c7d0: 726e 2065 7665 6e74 2e73 7461 7465 2026  rn event.state &
+0000c7e0: 2030 7830 3030 380a 0a0a 6465 6620 6765   0x0008...def ge
+0000c7f0: 745f 6879 7065 726c 696e 6b5f 6375 7273  t_hyperlink_curs
+0000c800: 6f72 2829 202d 3e20 7374 723a 0a20 2020  or() -> str:.   
+0000c810: 2069 6620 7275 6e6e 696e 675f 6f6e 5f6d   if running_on_m
+0000c820: 6163 5f6f 7328 293a 0a20 2020 2020 2020  ac_os():.       
+0000c830: 2072 6574 7572 6e20 2270 6f69 6e74 696e   return "pointin
+0000c840: 6768 616e 6422 0a20 2020 2065 6c73 653a  ghand".    else:
+0000c850: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c860: 2268 616e 6432 220a 0a0a 6465 6620 6765  "hand2"...def ge
+0000c870: 745f 6265 616d 5f63 7572 736f 7228 2920  t_beam_cursor() 
+0000c880: 2d3e 2073 7472 3a0a 2020 2020 6966 2072  -> str:.    if r
+0000c890: 756e 6e69 6e67 5f6f 6e5f 6d61 635f 6f73  unning_on_mac_os
+0000c8a0: 2829 206f 7220 7275 6e6e 696e 675f 6f6e  () or running_on
+0000c8b0: 5f77 696e 646f 7773 2829 3a0a 2020 2020  _windows():.    
+0000c8c0: 2020 2020 7265 7475 726e 2022 6962 6561      return "ibea
+0000c8d0: 6d22 0a20 2020 2065 6c73 653a 0a20 2020  m".    else:.   
+0000c8e0: 2020 2020 2072 6574 7572 6e20 2278 7465       return "xte
+0000c8f0: 726d 220a 0a0a 6465 6620 7365 7175 656e  rm"...def sequen
+0000c900: 6365 5f74 6f5f 6576 656e 745f 7374 6174  ce_to_event_stat
+0000c910: 655f 616e 645f 6b65 7963 6f64 6528 7365  e_and_keycode(se
+0000c920: 7175 656e 6365 3a20 7374 7229 202d 3e20  quence: str) -> 
+0000c930: 4f70 7469 6f6e 616c 5b54 7570 6c65 5b69  Optional[Tuple[i
+0000c940: 6e74 2c20 696e 745d 5d3a 0a20 2020 2023  nt, int]]:.    #
+0000c950: 2072 656d 656d 6265 7220 6861 6e64 6c65   remember handle
+0000c960: 7273 2066 6f72 2063 6572 7461 696e 2073  rs for certain s
+0000c970: 686f 7274 6375 7473 2077 6869 6368 2072  hortcuts which r
+0000c980: 6571 7569 7265 0a20 2020 2023 2064 6966  equire.    # dif
+0000c990: 6665 7265 6e74 2074 7265 6174 6d65 6e74  ferent treatment
+0000c9a0: 206f 6e20 6e6f 6e2d 6c61 7469 6e20 6b65   on non-latin ke
+0000c9b0: 7962 6f61 7264 730a 2020 2020 6966 2073  yboards.    if s
+0000c9c0: 6571 7565 6e63 655b 305d 2021 3d20 223c  equence[0] != "<
+0000c9d0: 223a 0a20 2020 2020 2020 2072 6574 7572  ":.        retur
+0000c9e0: 6e20 4e6f 6e65 0a0a 2020 2020 7061 7274  n None..    part
+0000c9f0: 7320 3d20 7365 7175 656e 6365 2e73 7472  s = sequence.str
+0000ca00: 6970 2822 3c22 292e 7374 7269 7028 223e  ip("<").strip(">
+0000ca10: 2229 2e73 706c 6974 2822 2d22 290a 2020  ").split("-").  
+0000ca20: 2020 2320 7375 7070 6f72 7420 6f6e 6c79    # support only
+0000ca30: 206c 6174 696e 206c 6574 7465 7273 2066   latin letters f
+0000ca40: 6f72 206e 6f77 0a20 2020 2069 6620 7061  or now.    if pa
+0000ca50: 7274 735b 2d31 5d2e 6c6f 7765 7228 2920  rts[-1].lower() 
+0000ca60: 6e6f 7420 696e 206c 6973 7428 2261 6263  not in list("abc
+0000ca70: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+0000ca80: 7475 7677 7879 7a22 293a 0a20 2020 2020  tuvwxyz"):.     
+0000ca90: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+0000caa0: 2020 2020 6c65 7474 6572 203d 2070 6172      letter = par
+0000cab0: 7473 2e70 6f70 282d 3129 0a20 2020 2069  ts.pop(-1).    i
+0000cac0: 6620 224b 6579 2220 696e 2070 6172 7473  f "Key" in parts
+0000cad0: 3a0a 2020 2020 2020 2020 7061 7274 732e  :.        parts.
+0000cae0: 7265 6d6f 7665 2822 4b65 7922 290a 2020  remove("Key").  
+0000caf0: 2020 6966 2022 6b65 7922 2069 6e20 7061    if "key" in pa
+0000cb00: 7274 733a 0a20 2020 2020 2020 2070 6172  rts:.        par
+0000cb10: 7473 2e72 656d 6f76 6528 226b 6579 2229  ts.remove("key")
+0000cb20: 0a0a 2020 2020 6d6f 6469 6669 6572 7320  ..    modifiers 
+0000cb30: 3d20 7b70 6172 742e 6c6f 7765 7228 2920  = {part.lower() 
+0000cb40: 666f 7220 7061 7274 2069 6e20 7061 7274  for part in part
+0000cb50: 737d 0a0a 2020 2020 6966 206c 6574 7465  s}..    if lette
+0000cb60: 722e 6973 7570 7065 7228 293a 0a20 2020  r.isupper():.   
+0000cb70: 2020 2020 206d 6f64 6966 6965 7273 2e61       modifiers.a
+0000cb80: 6464 2822 7368 6966 7422 290a 0a20 2020  dd("shift")..   
+0000cb90: 2069 6620 6d6f 6469 6669 6572 7320 6e6f   if modifiers no
+0000cba0: 7420 696e 205b 7b22 636f 6e74 726f 6c22  t in [{"control"
+0000cbb0: 7d2c 207b 2263 6f6e 7472 6f6c 222c 2022  }, {"control", "
+0000cbc0: 7368 6966 7422 7d5d 3a0a 2020 2020 2020  shift"}]:.      
+0000cbd0: 2020 2320 646f 6e27 7420 7375 7070 6f72    # don't suppor
+0000cbe0: 7420 6f74 6865 7273 2066 6f72 206e 6f77  t others for now
+0000cbf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cc00: 4e6f 6e65 0a0a 2020 2020 6576 656e 745f  None..    event_
+0000cc10: 7374 6174 6520 3d20 300a 2020 2020 2320  state = 0.    # 
+0000cc20: 6874 7470 733a 2f2f 746b 646f 6373 2e63  https://tkdocs.c
+0000cc30: 6f6d 2f73 6869 706d 616e 2f65 7665 6e74  om/shipman/event
+0000cc40: 2d68 616e 646c 6572 732e 6874 6d6c 0a20  -handlers.html. 
+0000cc50: 2020 2023 2068 7474 7073 3a2f 2f73 7461     # https://sta
+0000cc60: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f71  ckoverflow.com/q
+0000cc70: 7565 7374 696f 6e73 2f33 3234 3236 3235  uestions/3242625
+0000cc80: 302f 7079 7468 6f6e 2d64 6f63 756d 656e  0/python-documen
+0000cc90: 7461 7469 6f6e 2d61 6e64 2d6f 722d 6c61  tation-and-or-la
+0000cca0: 636b 2d74 6865 7265 6f66 2d65 2d67 2d6b  ck-thereof-e-g-k
+0000ccb0: 6579 626f 6172 642d 6576 656e 742d 7374  eyboard-event-st
+0000ccc0: 6174 650a 2020 2020 666f 7220 6d6f 6469  ate.    for modi
+0000ccd0: 6669 6572 2069 6e20 6d6f 6469 6669 6572  fier in modifier
+0000cce0: 733a 0a20 2020 2020 2020 2069 6620 6d6f  s:.        if mo
+0000ccf0: 6469 6669 6572 203d 3d20 2273 6869 6674  difier == "shift
+0000cd00: 223a 0a20 2020 2020 2020 2020 2020 2065  ":.            e
+0000cd10: 7665 6e74 5f73 7461 7465 207c 3d20 3078  vent_state |= 0x
+0000cd20: 3030 3031 0a20 2020 2020 2020 2065 6c69  0001.        eli
+0000cd30: 6620 6d6f 6469 6669 6572 203d 3d20 2263  f modifier == "c
+0000cd40: 6f6e 7472 6f6c 223a 0a20 2020 2020 2020  ontrol":.       
+0000cd50: 2020 2020 2065 7665 6e74 5f73 7461 7465       event_state
+0000cd60: 207c 3d20 3078 3030 3034 0a20 2020 2020   |= 0x0004.     
+0000cd70: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000cd80: 2020 2020 2023 2075 6e73 7570 706f 7274       # unsupport
+0000cd90: 6564 206d 6f64 6966 6965 720a 2020 2020  ed modifier.    
+0000cda0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+0000cdb0: 6f6e 650a 0a20 2020 2023 2066 6f72 206c  one..    # for l
+0000cdc0: 6174 696e 206c 6574 7465 7273 206b 6579  atin letters key
+0000cdd0: 636f 6465 2069 7320 7361 6d65 2061 7320  code is same as 
+0000cde0: 6974 7320 6173 6369 6920 636f 6465 0a20  its ascii code. 
+0000cdf0: 2020 2072 6574 7572 6e20 2865 7665 6e74     return (event
+0000ce00: 5f73 7461 7465 2c20 6f72 6428 6c65 7474  _state, ord(lett
+0000ce10: 6572 2e75 7070 6572 2829 2929 0a0a 0a64  er.upper()))...d
+0000ce20: 6566 2073 656c 6563 745f 7365 7175 656e  ef select_sequen
+0000ce30: 6365 2877 696e 5f76 6572 7369 6f6e 2c20  ce(win_version, 
+0000ce40: 6d61 635f 7665 7273 696f 6e2c 206c 696e  mac_version, lin
+0000ce50: 7578 5f76 6572 7369 6f6e 3d4e 6f6e 6529  ux_version=None)
+0000ce60: 3a0a 2020 2020 6966 2072 756e 6e69 6e67  :.    if running
+0000ce70: 5f6f 6e5f 7769 6e64 6f77 7328 293a 0a20  _on_windows():. 
+0000ce80: 2020 2020 2020 2072 6574 7572 6e20 7769         return wi
+0000ce90: 6e5f 7665 7273 696f 6e0a 2020 2020 656c  n_version.    el
+0000cea0: 6966 2072 756e 6e69 6e67 5f6f 6e5f 6d61  if running_on_ma
+0000ceb0: 635f 6f73 2829 3a0a 2020 2020 2020 2020  c_os():.        
+0000cec0: 7265 7475 726e 206d 6163 5f76 6572 7369  return mac_versi
+0000ced0: 6f6e 0a20 2020 2065 6c69 6620 7275 6e6e  on.    elif runn
+0000cee0: 696e 675f 6f6e 5f6c 696e 7578 2829 2061  ing_on_linux() a
+0000cef0: 6e64 206c 696e 7578 5f76 6572 7369 6f6e  nd linux_version
+0000cf00: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000cf10: 206c 696e 7578 5f76 6572 7369 6f6e 0a20   linux_version. 
+0000cf20: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000cf30: 2072 6574 7572 6e20 7769 6e5f 7665 7273   return win_vers
+0000cf40: 696f 6e0a 0a0a 6465 6620 7472 795f 7265  ion...def try_re
+0000cf50: 6d6f 7665 5f6c 696e 656e 756d 6265 7273  move_linenumbers
+0000cf60: 2874 6578 742c 206d 6173 7465 7229 3a0a  (text, master):.
+0000cf70: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000cf80: 2069 6620 6861 735f 6c69 6e65 5f6e 756d   if has_line_num
+0000cf90: 6265 7273 2874 6578 7429 2061 6e64 206d  bers(text) and m
+0000cfa0: 6573 7361 6765 626f 782e 6173 6b79 6573  essagebox.askyes
+0000cfb0: 6e6f 280a 2020 2020 2020 2020 2020 2020  no(.            
+0000cfc0: 7469 746c 653d 2252 656d 6f76 6520 6c69  title="Remove li
+0000cfd0: 6e65 6e75 6d62 6572 7322 2c0a 2020 2020  nenumbers",.    
+0000cfe0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+0000cff0: 2244 6f20 796f 7520 7761 6e74 2074 6f20  "Do you want to 
+0000d000: 7265 6d6f 7665 206c 696e 656e 756d 6265  remove linenumbe
+0000d010: 7273 2066 726f 6d20 7061 7374 6564 2074  rs from pasted t
+0000d020: 6578 743f 222c 0a20 2020 2020 2020 2020  ext?",.         
+0000d030: 2020 2064 6566 6175 6c74 3d6d 6573 7361     default=messa
+0000d040: 6765 626f 782e 5945 532c 0a20 2020 2020  gebox.YES,.     
+0000d050: 2020 2020 2020 206d 6173 7465 723d 6d61         master=ma
+0000d060: 7374 6572 2c0a 2020 2020 2020 2020 293a  ster,.        ):
+0000d070: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d080: 7572 6e20 7265 6d6f 7665 5f6c 696e 655f  urn remove_line_
+0000d090: 6e75 6d62 6572 7328 7465 7874 290a 2020  numbers(text).  
+0000d0a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000d0b0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+0000d0c0: 6578 740a 2020 2020 6578 6365 7074 2045  ext.    except E
+0000d0d0: 7863 6570 7469 6f6e 3a0a 2020 2020 2020  xception:.      
+0000d0e0: 2020 7472 6163 6562 6163 6b2e 7072 696e    traceback.prin
+0000d0f0: 745f 6578 6328 290a 2020 2020 2020 2020  t_exc().        
+0000d100: 7265 7475 726e 2074 6578 740a 0a0a 6465  return text...de
+0000d110: 6620 6861 735f 6c69 6e65 5f6e 756d 6265  f has_line_numbe
+0000d120: 7273 2874 6578 7429 3a0a 2020 2020 6c69  rs(text):.    li
+0000d130: 6e65 7320 3d20 7465 7874 2e73 706c 6974  nes = text.split
+0000d140: 6c69 6e65 7328 290a 2020 2020 7265 7475  lines().    retu
+0000d150: 726e 206c 656e 286c 696e 6573 2920 3e20  rn len(lines) > 
+0000d160: 3220 616e 6420 616c 6c28 5b6c 656e 2873  2 and all([len(s
+0000d170: 706c 6974 5f61 6674 6572 5f6c 696e 655f  plit_after_line_
+0000d180: 6e75 6d62 6572 286c 696e 6529 2920 3d3d  number(line)) ==
+0000d190: 2032 2066 6f72 206c 696e 6520 696e 206c   2 for line in l
+0000d1a0: 696e 6573 5d29 0a0a 0a64 6566 2073 706c  ines])...def spl
+0000d1b0: 6974 5f61 6674 6572 5f6c 696e 655f 6e75  it_after_line_nu
+0000d1c0: 6d62 6572 2873 293a 0a20 2020 2070 6172  mber(s):.    par
+0000d1d0: 7473 203d 2072 652e 7370 6c69 7428 7222  ts = re.split(r"
+0000d1e0: 285e 5c73 2a5c 642b 5c2e 3f29 222c 2073  (^\s*\d+\.?)", s
+0000d1f0: 290a 2020 2020 6966 206c 656e 2870 6172  ).    if len(par
+0000d200: 7473 2920 3d3d 2031 3a0a 2020 2020 2020  ts) == 1:.      
+0000d210: 2020 7265 7475 726e 2070 6172 7473 0a20    return parts. 
+0000d220: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000d230: 2061 7373 6572 7420 6c65 6e28 7061 7274   assert len(part
+0000d240: 7329 203d 3d20 3320 616e 6420 7061 7274  s) == 3 and part
+0000d250: 735b 305d 203d 3d20 2222 0a20 2020 2020  s[0] == "".     
+0000d260: 2020 2072 6574 7572 6e20 7061 7274 735b     return parts[
+0000d270: 313a 5d0a 0a0a 6465 6620 7265 6d6f 7665  1:]...def remove
+0000d280: 5f6c 696e 655f 6e75 6d62 6572 7328 7329  _line_numbers(s)
+0000d290: 3a0a 2020 2020 636c 6561 6e65 645f 6c69  :.    cleaned_li
+0000d2a0: 6e65 7320 3d20 5b5d 0a20 2020 2066 6f72  nes = [].    for
+0000d2b0: 206c 696e 6520 696e 2073 2e73 706c 6974   line in s.split
+0000d2c0: 6c69 6e65 7328 293a 0a20 2020 2020 2020  lines():.       
+0000d2d0: 2070 6172 7473 203d 2073 706c 6974 5f61   parts = split_a
+0000d2e0: 6674 6572 5f6c 696e 655f 6e75 6d62 6572  fter_line_number
+0000d2f0: 286c 696e 6529 0a20 2020 2020 2020 2069  (line).        i
+0000d300: 6620 6c65 6e28 7061 7274 7329 2021 3d20  f len(parts) != 
+0000d310: 323a 0a20 2020 2020 2020 2020 2020 2072  2:.            r
+0000d320: 6574 7572 6e20 730a 2020 2020 2020 2020  eturn s.        
+0000d330: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000d340: 2020 636c 6561 6e65 645f 6c69 6e65 732e    cleaned_lines.
+0000d350: 6170 7065 6e64 2870 6172 7473 5b31 5d29  append(parts[1])
+0000d360: 0a0a 2020 2020 7265 7475 726e 2074 6578  ..    return tex
+0000d370: 7477 7261 702e 6465 6465 6e74 2828 225c  twrap.dedent(("\
+0000d380: 6e22 2e6a 6f69 6e28 636c 6561 6e65 645f  n".join(cleaned_
+0000d390: 6c69 6e65 7329 2920 2b20 225c 6e22 290a  lines)) + "\n").
+0000d3a0: 0a0a 2320 506c 6163 6520 6120 746f 706c  ..# Place a topl
+0000d3b0: 6576 656c 2077 696e 646f 7720 6174 2074  evel window at t
+0000d3c0: 6865 2063 656e 7465 7220 6f66 2070 6172  he center of par
+0000d3d0: 656e 7420 6f72 2073 6372 6565 6e0a 2320  ent or screen.# 
+0000d3e0: 4974 2069 7320 6120 5079 7468 6f6e 2069  It is a Python i
+0000d3f0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+0000d400: 203a 3a74 6b3a 3a50 6c61 6365 5769 6e64   ::tk::PlaceWind
+0000d410: 6f77 2e0a 2320 436f 7069 6564 2061 6e64  ow..# Copied and
+0000d420: 2061 6461 7074 6564 2066 726f 6d20 746b   adapted from tk
+0000d430: 696e 7465 722e 7369 6d70 6c65 6469 616c  inter.simpledial
+0000d440: 6f67 206f 6620 5079 7468 6f6e 2033 2e31  og of Python 3.1
+0000d450: 302e 320a 6465 6620 5f70 6c61 6365 5f77  0.2.def _place_w
+0000d460: 696e 646f 7728 772c 2070 6172 656e 743d  indow(w, parent=
+0000d470: 4e6f 6e65 2c20 7769 6474 683d 4e6f 6e65  None, width=None
+0000d480: 2c20 6865 6967 6874 3d4e 6f6e 6529 3a0a  , height=None):.
+0000d490: 2020 2020 772e 776d 5f77 6974 6864 7261      w.wm_withdra
+0000d4a0: 7728 2920 2023 2052 656d 6169 6e20 696e  w()  # Remain in
+0000d4b0: 7669 7369 626c 6520 7768 696c 6520 7765  visible while we
+0000d4c0: 2066 6967 7572 6520 6f75 7420 7468 6520   figure out the 
+0000d4d0: 6765 6f6d 6574 7279 0a20 2020 2077 2e75  geometry.    w.u
+0000d4e0: 7064 6174 655f 6964 6c65 7461 736b 7328  pdate_idletasks(
+0000d4f0: 2920 2023 2041 6374 7561 6c69 7a65 2067  )  # Actualize g
+0000d500: 656f 6d65 7472 7920 696e 666f 726d 6174  eometry informat
+0000d510: 696f 6e0a 0a20 2020 206d 696e 7769 6474  ion..    minwidt
+0000d520: 6820 3d20 7769 6474 6820 6f72 2077 2e77  h = width or w.w
+0000d530: 696e 666f 5f72 6571 7769 6474 6828 290a  info_reqwidth().
+0000d540: 2020 2020 6d69 6e68 6569 6768 7420 3d20      minheight = 
+0000d550: 6865 6967 6874 206f 7220 772e 7769 6e66  height or w.winf
+0000d560: 6f5f 7265 7168 6569 6768 7428 290a 2020  o_reqheight().  
+0000d570: 2020 6d61 7877 6964 7468 203d 2077 2e77    maxwidth = w.w
+0000d580: 696e 666f 5f76 726f 6f74 7769 6474 6828  info_vrootwidth(
+0000d590: 290a 2020 2020 6d61 7868 6569 6768 7420  ).    maxheight 
+0000d5a0: 3d20 772e 7769 6e66 6f5f 7672 6f6f 7468  = w.winfo_vrooth
+0000d5b0: 6569 6768 7428 290a 2020 2020 6966 2070  eight().    if p
+0000d5c0: 6172 656e 7420 6973 206e 6f74 204e 6f6e  arent is not Non
+0000d5d0: 6520 616e 6420 7061 7265 6e74 2e77 696e  e and parent.win
+0000d5e0: 666f 5f69 736d 6170 7065 6428 293a 0a20  fo_ismapped():. 
+0000d5f0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000d600: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
+0000d610: 6622 5061 7265 6e74 2079 3a20 7b70 6172  f"Parent y: {par
+0000d620: 656e 742e 7769 6e66 6f5f 7928 297d 2c20  ent.winfo_y()}, 
+0000d630: 726f 6f74 793a 207b 7061 7265 6e74 2e77  rooty: {parent.w
+0000d640: 696e 666f 5f72 6f6f 7479 2829 7d2c 2076  info_rooty()}, v
+0000d650: 726f 6f74 793a 207b 7061 7265 6e74 2e77  rooty: {parent.w
+0000d660: 696e 666f 5f76 726f 6f74 7928 297d 220a  info_vrooty()}".
+0000d670: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d680: 2020 7820 3d20 7061 7265 6e74 2e77 696e    x = parent.win
+0000d690: 666f 5f72 6f6f 7478 2829 202b 2028 7061  fo_rootx() + (pa
+0000d6a0: 7265 6e74 2e77 696e 666f 5f77 6964 7468  rent.winfo_width
+0000d6b0: 2829 202d 206d 696e 7769 6474 6829 202f  () - minwidth) /
+0000d6c0: 2f20 320a 2020 2020 2020 2020 7920 3d20  / 2.        y = 
+0000d6d0: 7061 7265 6e74 2e77 696e 666f 5f79 2829  parent.winfo_y()
+0000d6e0: 202b 2028 7061 7265 6e74 2e77 696e 666f   + (parent.winfo
+0000d6f0: 5f68 6569 6768 7428 2920 2d20 6d69 6e68  _height() - minh
+0000d700: 6569 6768 7429 202f 2f20 320a 2020 2020  eight) // 2.    
+0000d710: 2020 2020 7672 6f6f 7478 203d 2077 2e77      vrootx = w.w
+0000d720: 696e 666f 5f76 726f 6f74 7828 290a 2020  info_vrootx().  
+0000d730: 2020 2020 2020 7672 6f6f 7479 203d 2077        vrooty = w
+0000d740: 2e77 696e 666f 5f76 726f 6f74 7928 290a  .winfo_vrooty().
+0000d750: 2020 2020 2020 2020 7820 3d20 6d69 6e28          x = min(
+0000d760: 782c 2076 726f 6f74 7820 2b20 6d61 7877  x, vrootx + maxw
+0000d770: 6964 7468 202d 206d 696e 7769 6474 6829  idth - minwidth)
+0000d780: 0a20 2020 2020 2020 2078 203d 206d 6178  .        x = max
+0000d790: 2878 2c20 7672 6f6f 7478 290a 2020 2020  (x, vrootx).    
+0000d7a0: 2020 2020 7920 3d20 6d69 6e28 792c 2076      y = min(y, v
+0000d7b0: 726f 6f74 7920 2b20 6d61 7868 6569 6768  rooty + maxheigh
+0000d7c0: 7420 2d20 6d69 6e68 6569 6768 7429 0a20  t - minheight). 
+0000d7d0: 2020 2020 2020 2023 2064 6f6e 2774 2061         # don't a
+0000d7e0: 6c6c 6f77 2074 6865 2064 6961 6c6f 6720  llow the dialog 
+0000d7f0: 676f 2068 6967 6865 7220 7468 616e 2070  go higher than p
+0000d800: 6172 656e 742e 2054 6869 7320 7761 7920  arent. This way 
+0000d810: 7468 6520 7469 746c 6520 6261 7220 7265  the title bar re
+0000d820: 6d61 696e 7320 7669 7369 626c 652e 0a20  mains visible.. 
+0000d830: 2020 2020 2020 2079 203d 206d 6178 2879         y = max(y
+0000d840: 2c20 7672 6f6f 7479 2c20 7061 7265 6e74  , vrooty, parent
+0000d850: 2e77 696e 666f 5f79 2829 290a 2020 2020  .winfo_y()).    
+0000d860: 2020 2020 6966 2077 2e5f 7769 6e64 6f77      if w._window
+0000d870: 696e 6773 7973 7465 6d20 3d3d 2022 6171  ingsystem == "aq
+0000d880: 7561 223a 0a20 2020 2020 2020 2020 2020  ua":.           
+0000d890: 2023 2041 766f 6964 2074 6865 206e 6174   # Avoid the nat
+0000d8a0: 6976 6520 6d65 6e75 2062 6172 2077 6869  ive menu bar whi
+0000d8b0: 6368 2073 6974 7320 6f6e 2074 6f70 206f  ch sits on top o
+0000d8c0: 6620 6576 6572 7974 6869 6e67 2e0a 2020  f everything..  
+0000d8d0: 2020 2020 2020 2020 2020 7920 3d20 6d61            y = ma
+0000d8e0: 7828 792c 2065 6d73 5f74 6f5f 7069 7865  x(y, ems_to_pixe
+0000d8f0: 6c73 2832 2929 0a0a 2020 2020 2020 2020  ls(2))..        
+0000d900: 6966 2079 202b 206d 696e 6865 6967 6874  if y + minheight
+0000d910: 203e 206d 6178 6865 6967 6874 3a0a 2020   > maxheight:.  
+0000d920: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000d930: 2e64 6562 7567 2822 416c 6967 6e69 6e67  .debug("Aligning
+0000d940: 2074 6f70 2077 6974 6820 7061 7265 6e74   top with parent
+0000d950: 2028 2573 2076 7320 2573 2922 2c20 7920   (%s vs %s)", y 
+0000d960: 2b20 6d69 6e68 6569 6768 742c 206d 6178  + minheight, max
+0000d970: 6865 6967 6874 290a 2020 2020 2020 2020  height).        
+0000d980: 2020 2020 7920 3d20 7061 7265 6e74 2e77      y = parent.w
+0000d990: 696e 666f 5f79 2829 0a20 2020 2065 6c73  info_y().    els
+0000d9a0: 653a 0a20 2020 2020 2020 2078 203d 2028  e:.        x = (
+0000d9b0: 772e 7769 6e66 6f5f 7363 7265 656e 7769  w.winfo_screenwi
+0000d9c0: 6474 6828 2920 2d20 6d69 6e77 6964 7468  dth() - minwidth
+0000d9d0: 2920 2f2f 2032 0a20 2020 2020 2020 2079  ) // 2.        y
+0000d9e0: 203d 2028 772e 7769 6e66 6f5f 7363 7265   = (w.winfo_scre
+0000d9f0: 656e 6865 6967 6874 2829 202d 206d 696e  enheight() - min
+0000da00: 6865 6967 6874 2920 2f2f 2032 0a0a 2020  height) // 2..  
+0000da10: 2020 772e 776d 5f6d 6178 7369 7a65 286d    w.wm_maxsize(m
+0000da20: 6178 7769 6474 682c 206d 6178 6865 6967  axwidth, maxheig
+0000da30: 6874 290a 2020 2020 6966 2077 6964 7468  ht).    if width
+0000da40: 2061 6e64 2068 6569 6768 743a 0a20 2020   and height:.   
+0000da50: 2020 2020 2067 656f 6d65 7472 7920 3d20       geometry = 
+0000da60: 2225 6478 2564 2b25 642b 2564 2220 2520  "%dx%d+%d+%d" % 
+0000da70: 2877 6964 7468 2c20 6865 6967 6874 2c20  (width, height, 
+0000da80: 782c 2079 290a 2020 2020 656c 7365 3a0a  x, y).    else:.
+0000da90: 2020 2020 2020 2020 6765 6f6d 6574 7279          geometry
+0000daa0: 203d 2022 2b25 642b 2564 2220 2520 2878   = "+%d+%d" % (x
+0000dab0: 2c20 7929 0a0a 2020 2020 6c6f 6767 6572  , y)..    logger
+0000dac0: 2e69 6e66 6f28 6622 506c 6163 696e 6720  .info(f"Placing 
+0000dad0: 7b77 7d20 7769 7468 2067 656f 6d65 7472  {w} with geometr
+0000dae0: 7920 7b67 656f 6d65 7472 797d 2229 0a20  y {geometry}"). 
+0000daf0: 2020 2077 2e77 6d5f 6765 6f6d 6574 7279     w.wm_geometry
+0000db00: 2867 656f 6d65 7472 7929 0a20 2020 2077  (geometry).    w
+0000db10: 2e77 6d5f 6465 6963 6f6e 6966 7928 2920  .wm_deiconify() 
+0000db20: 2023 2042 6563 6f6d 6520 7669 7369 626c   # Become visibl
+0000db30: 6520 6174 2074 6865 2064 6573 6972 6564  e at the desired
+0000db40: 206c 6f63 6174 696f 6e0a 0a0a 636c 6173   location...clas
+0000db50: 7320 5761 6974 696e 6744 6961 6c6f 6728  s WaitingDialog(
+0000db60: 436f 6d6d 6f6e 4469 616c 6f67 293a 0a20  CommonDialog):. 
+0000db70: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000db80: 7365 6c66 2c20 6d61 7374 6572 2c20 6173  self, master, as
+0000db90: 796e 635f 7265 7375 6c74 2c20 6465 7363  ync_result, desc
+0000dba0: 7269 7074 696f 6e2c 2074 6974 6c65 3d22  ription, title="
+0000dbb0: 506c 6561 7365 2077 6169 7421 222c 2074  Please wait!", t
+0000dbc0: 696d 656f 7574 3d4e 6f6e 6529 3a0a 2020  imeout=None):.  
+0000dbd0: 2020 2020 2020 7365 6c66 2e5f 6173 796e        self._asyn
+0000dbe0: 635f 7265 7375 6c74 203d 2061 7379 6e63  c_result = async
+0000dbf0: 5f72 6573 756c 740a 2020 2020 2020 2020  _result.        
+0000dc00: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+0000dc10: 286d 6173 7465 7229 0a20 2020 2020 2020  (master).       
+0000dc20: 2069 6620 6d69 7363 5f75 7469 6c73 2e72   if misc_utils.r
+0000dc30: 756e 6e69 6e67 5f6f 6e5f 6d61 635f 6f73  unning_on_mac_os
+0000dc40: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0000dc50: 7365 6c66 2e63 6f6e 6669 6775 7265 2862  self.configure(b
+0000dc60: 6163 6b67 726f 756e 643d 2273 7973 7465  ackground="syste
+0000dc70: 6d53 6865 6574 4261 636b 6772 6f75 6e64  mSheetBackground
+0000dc80: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000dc90: 7469 746c 6528 7469 746c 6529 0a20 2020  title(title).   
+0000dca0: 2020 2020 2073 656c 662e 7265 7369 7a61       self.resiza
+0000dcb0: 626c 6528 6865 6967 6874 3d74 6b2e 4641  ble(height=tk.FA
+0000dcc0: 4c53 452c 2077 6964 7468 3d74 6b2e 4641  LSE, width=tk.FA
+0000dcd0: 4c53 4529 0a20 2020 2020 2020 2023 2073  LSE).        # s
+0000dce0: 656c 662e 7072 6f74 6f63 6f6c 2822 574d  elf.protocol("WM
+0000dcf0: 5f44 454c 4554 455f 5749 4e44 4f57 222c  _DELETE_WINDOW",
+0000dd00: 2073 656c 662e 5f63 6c6f 7365 290a 2020   self._close).  
+0000dd10: 2020 2020 2020 7365 6c66 2e64 6573 635f        self.desc_
+0000dd20: 6c61 6265 6c20 3d20 7474 6b2e 4c61 6265  label = ttk.Labe
+0000dd30: 6c28 7365 6c66 2c20 7465 7874 3d64 6573  l(self, text=des
+0000dd40: 6372 6970 7469 6f6e 2c20 7772 6170 6c65  cription, wraple
+0000dd50: 6e67 7468 3d33 3030 290a 2020 2020 2020  ngth=300).      
+0000dd60: 2020 7365 6c66 2e64 6573 635f 6c61 6265    self.desc_labe
+0000dd70: 6c2e 6772 6964 2870 6164 783d 3230 2c20  l.grid(padx=20, 
+0000dd80: 7061 6479 3d32 3029 0a0a 2020 2020 2020  pady=20)..      
+0000dd90: 2020 7365 6c66 2e75 7064 6174 655f 6964    self.update_id
+0000dda0: 6c65 7461 736b 7328 290a 0a20 2020 2020  letasks()..     
+0000ddb0: 2020 2073 656c 662e 7469 6d65 6f75 7420     self.timeout 
+0000ddc0: 3d20 7469 6d65 6f75 740a 2020 2020 2020  = timeout.      
+0000ddd0: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
+0000dde0: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
+0000ddf0: 2020 2020 2020 2020 7365 6c66 2e61 6674          self.aft
+0000de00: 6572 2835 3030 2c20 7365 6c66 2e5f 706f  er(500, self._po
+0000de10: 6c6c 290a 0a20 2020 2064 6566 205f 706f  ll)..    def _po
+0000de20: 6c6c 2873 656c 6629 3a0a 2020 2020 2020  ll(self):.      
+0000de30: 2020 6966 2073 656c 662e 5f61 7379 6e63    if self._async
+0000de40: 5f72 6573 756c 742e 7265 6164 7928 293a  _result.ready():
+0000de50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000de60: 662e 5f63 6c6f 7365 2829 0a20 2020 2020  f._close().     
+0000de70: 2020 2065 6c69 6620 7365 6c66 2e74 696d     elif self.tim
+0000de80: 656f 7574 2061 6e64 2074 696d 652e 7469  eout and time.ti
+0000de90: 6d65 2829 202d 2073 656c 662e 7374 6172  me() - self.star
+0000dea0: 745f 7469 6d65 203e 2073 656c 662e 7469  t_time > self.ti
+0000deb0: 6d65 6f75 743a 0a20 2020 2020 2020 2020  meout:.         
+0000dec0: 2020 2072 6169 7365 2054 696d 656f 7574     raise Timeout
+0000ded0: 4572 726f 7228 290a 2020 2020 2020 2020  Error().        
+0000dee0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000def0: 2020 7365 6c66 2e61 6674 6572 2835 3030    self.after(500
+0000df00: 2c20 7365 6c66 2e5f 706f 6c6c 290a 2020  , self._poll).  
+0000df10: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000df20: 6573 635f 6c61 6265 6c5b 2274 6578 7422  esc_label["text"
+0000df30: 5d20 3d20 7365 6c66 2e64 6573 635f 6c61  ] = self.desc_la
+0000df40: 6265 6c5b 2274 6578 7422 5d20 2b20 222e  bel["text"] + ".
+0000df50: 220a 0a20 2020 2064 6566 205f 636c 6f73  "..    def _clos
+0000df60: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0000df70: 2073 656c 662e 6465 7374 726f 7928 290a   self.destroy().
+0000df80: 0a0a 6465 6620 7275 6e5f 7769 7468 5f77  ..def run_with_w
+0000df90: 6169 7469 6e67 5f64 6961 6c6f 6728 6d61  aiting_dialog(ma
+0000dfa0: 7374 6572 2c20 6163 7469 6f6e 2c20 6172  ster, action, ar
+0000dfb0: 6773 3d28 292c 2064 6573 6372 6970 7469  gs=(), descripti
+0000dfc0: 6f6e 3d22 576f 726b 696e 6722 293a 0a20  on="Working"):. 
+0000dfd0: 2020 2023 2068 7474 703a 2f2f 7374 6163     # http://stac
+0000dfe0: 6b6f 7665 7266 6c6f 772e 636f 6d2f 612f  koverflow.com/a/
+0000dff0: 3134 3239 3930 3034 2f32 3631 3138 310a  14299004/261181.
+0000e000: 2020 2020 6672 6f6d 206d 756c 7469 7072      from multipr
+0000e010: 6f63 6573 7369 6e67 2e70 6f6f 6c20 696d  ocessing.pool im
+0000e020: 706f 7274 2054 6872 6561 6450 6f6f 6c0a  port ThreadPool.
+0000e030: 0a20 2020 2070 6f6f 6c20 3d20 5468 7265  .    pool = Thre
+0000e040: 6164 506f 6f6c 2870 726f 6365 7373 6573  adPool(processes
+0000e050: 3d31 290a 0a20 2020 2061 7379 6e63 5f72  =1)..    async_r
+0000e060: 6573 756c 7420 3d20 706f 6f6c 2e61 7070  esult = pool.app
+0000e070: 6c79 5f61 7379 6e63 2861 6374 696f 6e2c  ly_async(action,
+0000e080: 2061 7267 7329 0a20 2020 2064 6c67 203d   args).    dlg =
+0000e090: 2057 6169 7469 6e67 4469 616c 6f67 286d   WaitingDialog(m
+0000e0a0: 6173 7465 722c 2061 7379 6e63 5f72 6573  aster, async_res
+0000e0b0: 756c 742c 2064 6573 6372 6970 7469 6f6e  ult, description
+0000e0c0: 3d64 6573 6372 6970 7469 6f6e 290a 2020  =description).  
+0000e0d0: 2020 7368 6f77 5f64 6961 6c6f 6728 646c    show_dialog(dl
+0000e0e0: 672c 206d 6173 7465 7229 0a0a 2020 2020  g, master)..    
+0000e0f0: 7265 7475 726e 2061 7379 6e63 5f72 6573  return async_res
+0000e100: 756c 742e 6765 7428 290a 0a0a 636c 6173  ult.get()...clas
+0000e110: 7320 4669 6c65 436f 7079 4469 616c 6f67  s FileCopyDialog
+0000e120: 2843 6f6d 6d6f 6e44 6961 6c6f 6729 3a0a  (CommonDialog):.
+0000e130: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000e140: 2873 656c 662c 206d 6173 7465 722c 2073  (self, master, s
+0000e150: 6f75 7263 652c 2064 6573 7469 6e61 7469  ource, destinati
+0000e160: 6f6e 2c20 6465 7363 7269 7074 696f 6e3d  on, description=
+0000e170: 4e6f 6e65 2c20 6673 796e 633d 5472 7565  None, fsync=True
+0000e180: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000e190: 5f73 6f75 7263 6520 3d20 736f 7572 6365  _source = source
+0000e1a0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+0000e1b0: 6573 7469 6e61 7469 6f6e 203d 2064 6573  estination = des
+0000e1c0: 7469 6e61 7469 6f6e 0a20 2020 2020 2020  tination.       
+0000e1d0: 2073 656c 662e 5f6f 6c64 5f62 7974 6573   self._old_bytes
+0000e1e0: 5f63 6f70 6965 6420 3d20 300a 2020 2020  _copied = 0.    
+0000e1f0: 2020 2020 7365 6c66 2e5f 6279 7465 735f      self._bytes_
+0000e200: 636f 7069 6564 203d 2030 0a20 2020 2020  copied = 0.     
+0000e210: 2020 2073 656c 662e 5f66 7379 6e63 203d     self._fsync =
+0000e220: 2066 7379 6e63 0a20 2020 2020 2020 2073   fsync.        s
+0000e230: 656c 662e 5f64 6f6e 6520 3d20 4661 6c73  elf._done = Fals
+0000e240: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000e250: 6361 6e63 656c 6c65 6420 3d20 4661 6c73  cancelled = Fals
+0000e260: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+0000e270: 636c 6f73 6564 203d 2046 616c 7365 0a0a  closed = False..
+0000e280: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+0000e290: 5f5f 696e 6974 5f5f 286d 6173 7465 7229  __init__(master)
+0000e2a0: 0a0a 2020 2020 2020 2020 6d61 696e 5f66  ..        main_f
+0000e2b0: 7261 6d65 203d 2074 746b 2e46 7261 6d65  rame = ttk.Frame
+0000e2c0: 2873 656c 6629 2020 2320 546f 2067 6574  (self)  # To get
+0000e2d0: 2073 7479 6c65 6420 6261 636b 6772 6f75   styled backgrou
+0000e2e0: 6e64 0a20 2020 2020 2020 206d 6169 6e5f  nd.        main_
+0000e2f0: 6672 616d 652e 6772 6964 2872 6f77 3d30  frame.grid(row=0
+0000e300: 2c20 636f 6c75 6d6e 3d30 2c20 7374 6963  , column=0, stic
+0000e310: 6b79 3d22 6e73 6577 2229 0a20 2020 2020  ky="nsew").     
+0000e320: 2020 2073 656c 662e 726f 7763 6f6e 6669     self.rowconfi
+0000e330: 6775 7265 2830 2c20 7765 6967 6874 3d31  gure(0, weight=1
+0000e340: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000e350: 6f6c 756d 6e63 6f6e 6669 6775 7265 2830  olumnconfigure(0
+0000e360: 2c20 7765 6967 6874 3d31 290a 0a20 2020  , weight=1)..   
+0000e370: 2020 2020 2073 656c 662e 7469 746c 6528       self.title(
+0000e380: 7472 2822 436f 7079 696e 6722 2929 0a0a  tr("Copying"))..
+0000e390: 2020 2020 2020 2020 6966 2064 6573 6372          if descr
+0000e3a0: 6970 7469 6f6e 2069 7320 4e6f 6e65 3a0a  iption is None:.
+0000e3b0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+0000e3c0: 7269 7074 696f 6e20 3d20 7472 2822 436f  ription = tr("Co
+0000e3d0: 7079 696e 675c 6e20 2025 735c 6e74 6f5c  pying\n  %s\nto\
+0000e3e0: 6e20 2025 7322 2920 2520 2873 6f75 7263  n  %s") % (sourc
+0000e3f0: 652c 2064 6573 7469 6e61 7469 6f6e 290a  e, destination).
+0000e400: 0a20 2020 2020 2020 206c 6162 656c 203d  .        label =
+0000e410: 2074 746b 2e4c 6162 656c 286d 6169 6e5f   ttk.Label(main_
+0000e420: 6672 616d 652c 2074 6578 743d 6465 7363  frame, text=desc
+0000e430: 7269 7074 696f 6e29 0a20 2020 2020 2020  ription).       
+0000e440: 206c 6162 656c 2e67 7269 6428 726f 773d   label.grid(row=
+0000e450: 302c 2063 6f6c 756d 6e3d 302c 2063 6f6c  0, column=0, col
+0000e460: 756d 6e73 7061 6e3d 322c 2073 7469 636b  umnspan=2, stick
+0000e470: 793d 226e 7722 2c20 7061 6478 3d31 352c  y="nw", padx=15,
+0000e480: 2070 6164 793d 3135 290a 0a20 2020 2020   pady=15)..     
+0000e490: 2020 2073 656c 662e 5f62 6172 203d 2074     self._bar = t
+0000e4a0: 746b 2e50 726f 6772 6573 7362 6172 286d  tk.Progressbar(m
+0000e4b0: 6169 6e5f 6672 616d 652c 206d 6178 696d  ain_frame, maxim
+0000e4c0: 756d 3d6f 732e 7061 7468 2e67 6574 7369  um=os.path.getsi
+0000e4d0: 7a65 2873 6f75 7263 6529 2c20 6c65 6e67  ze(source), leng
+0000e4e0: 7468 3d32 3030 290a 2020 2020 2020 2020  th=200).        
+0000e4f0: 7365 6c66 2e5f 6261 722e 6772 6964 2872  self._bar.grid(r
+0000e500: 6f77 3d31 2c20 636f 6c75 6d6e 3d30 2c20  ow=1, column=0, 
+0000e510: 636f 6c75 6d6e 7370 616e 3d32 2c20 7374  columnspan=2, st
+0000e520: 6963 6b79 3d22 6e73 6577 222c 2070 6164  icky="nsew", pad
+0000e530: 783d 3135 2c20 7061 6479 3d30 290a 0a20  x=15, pady=0).. 
+0000e540: 2020 2020 2020 2073 656c 662e 5f63 616e         self._can
+0000e550: 6365 6c5f 6275 7474 6f6e 203d 2074 746b  cel_button = ttk
+0000e560: 2e42 7574 746f 6e28 6d61 696e 5f66 7261  .Button(main_fra
+0000e570: 6d65 2c20 7465 7874 3d74 7228 2243 616e  me, text=tr("Can
+0000e580: 6365 6c22 292c 2063 6f6d 6d61 6e64 3d73  cel"), command=s
+0000e590: 656c 662e 5f63 616e 6365 6c29 0a20 2020  elf._cancel).   
+0000e5a0: 2020 2020 2073 656c 662e 5f63 616e 6365       self._cance
+0000e5b0: 6c5f 6275 7474 6f6e 2e67 7269 6428 726f  l_button.grid(ro
+0000e5c0: 773d 322c 2063 6f6c 756d 6e3d 312c 2073  w=2, column=1, s
+0000e5d0: 7469 636b 793d 226e 6522 2c20 7061 6478  ticky="ne", padx
+0000e5e0: 3d31 352c 2070 6164 793d 3135 290a 2020  =15, pady=15).  
+0000e5f0: 2020 2020 2020 7365 6c66 2e5f 6261 722e        self._bar.
+0000e600: 666f 6375 735f 7365 7428 290a 0a20 2020  focus_set()..   
+0000e610: 2020 2020 206d 6169 6e5f 6672 616d 652e       main_frame.
+0000e620: 636f 6c75 6d6e 636f 6e66 6967 7572 6528  columnconfigure(
+0000e630: 302c 2077 6569 6768 743d 3129 0a0a 2020  0, weight=1)..  
+0000e640: 2020 2020 2020 7365 6c66 2e5f 7570 6461        self._upda
+0000e650: 7465 5f70 726f 6772 6573 7328 290a 0a20  te_progress().. 
+0000e660: 2020 2020 2020 2073 656c 662e 6269 6e64         self.bind
+0000e670: 2822 3c45 7363 6170 653e 222c 2073 656c  ("<Escape>", sel
+0000e680: 662e 5f63 616e 6365 6c2c 2054 7275 6529  f._cancel, True)
+0000e690: 2020 2320 6573 6361 7065 2d63 6c6f 7365    # escape-close
+0000e6a0: 206f 6e6c 7920 6966 2070 726f 6365 7373   only if process
+0000e6b0: 2068 6173 2063 6f6d 706c 6574 6564 0a20   has completed. 
+0000e6c0: 2020 2020 2020 2073 656c 662e 7072 6f74         self.prot
+0000e6d0: 6f63 6f6c 2822 574d 5f44 454c 4554 455f  ocol("WM_DELETE_
+0000e6e0: 5749 4e44 4f57 222c 2073 656c 662e 5f63  WINDOW", self._c
+0000e6f0: 616e 6365 6c29 0a20 2020 2020 2020 2073  ancel).        s
+0000e700: 656c 662e 5f73 7461 7274 2829 0a0a 2020  elf._start()..  
+0000e710: 2020 6465 6620 5f73 7461 7274 2873 656c    def _start(sel
+0000e720: 6629 3a0a 2020 2020 2020 2020 6465 6620  f):.        def 
+0000e730: 776f 726b 2829 3a0a 2020 2020 2020 2020  work():.        
+0000e740: 2020 2020 7365 6c66 2e5f 636f 7079 5f70      self._copy_p
+0000e750: 726f 6765 7373 203d 2030 0a0a 2020 2020  rogess = 0..    
+0000e760: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0000e770: 6e28 7365 6c66 2e5f 736f 7572 6365 2c20  n(self._source, 
+0000e780: 2272 6222 2920 6173 2066 7372 633a 0a20  "rb") as fsrc:. 
+0000e790: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000e7a0: 6974 6820 6f70 656e 2873 656c 662e 5f64  ith open(self._d
+0000e7b0: 6573 7469 6e61 7469 6f6e 2c20 2277 6222  estination, "wb"
+0000e7c0: 2920 6173 2066 6473 743a 0a20 2020 2020  ) as fdst:.     
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000e7e0: 6869 6c65 2054 7275 653a 0a20 2020 2020  hile True:.     
 0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 2020 2062 7566 203d 2066 7372 632e       buf = fsrc.
-0000e810: 7265 6164 2831 3620 2a20 3130 3234 290a  read(16 * 1024).
+0000e800: 2020 2062 7566 203d 2066 7372 632e 7265     buf = fsrc.re
+0000e810: 6164 2831 3620 2a20 3130 3234 290a 2020  ad(16 * 1024).  
 0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e830: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
-0000e840: 7566 3a0a 2020 2020 2020 2020 2020 2020  uf:.            
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 6272 6561 6b0a 0a20 2020 2020 2020 2020  break..         
-0000e870: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e880: 6473 742e 7772 6974 6528 6275 6629 0a20  dst.write(buf). 
+0000e830: 2020 2020 2020 6966 206e 6f74 2062 7566        if not buf
+0000e840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e850: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0000e860: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
+0000e870: 2020 2020 2020 2020 2020 2020 2066 6473               fds
+0000e880: 742e 7772 6974 6528 6275 6629 0a20 2020  t.write(buf).   
 0000e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8a0: 2020 2020 2020 2066 6473 742e 666c 7573         fdst.flus
-0000e8b0: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
-0000e8c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000e8d0: 656c 662e 5f66 7379 6e63 3a0a 2020 2020  elf._fsync:.    
+0000e8a0: 2020 2020 2066 6473 742e 666c 7573 6828       fdst.flush(
+0000e8b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e8c0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000e8d0: 662e 5f66 7379 6e63 3a0a 2020 2020 2020  f._fsync:.      
 0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2020 2020 2020 2020 6f73 2e66 7379 6e63          os.fsync
-0000e900: 2866 6473 7429 0a20 2020 2020 2020 2020  (fdst).         
-0000e910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e920: 656c 662e 5f62 7974 6573 5f63 6f70 6965  elf._bytes_copie
-0000e930: 6420 2b3d 206c 656e 2862 7566 290a 0a20  d += len(buf).. 
-0000e940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e950: 5f64 6f6e 6520 3d20 5472 7565 0a0a 2020  _done = True..  
-0000e960: 2020 2020 2020 7468 7265 6164 696e 672e        threading.
-0000e970: 5468 7265 6164 2874 6172 6765 743d 776f  Thread(target=wo
-0000e980: 726b 2c20 6461 656d 6f6e 3d54 7275 6529  rk, daemon=True)
-0000e990: 2e73 7461 7274 2829 0a0a 2020 2020 6465  .start()..    de
-0000e9a0: 6620 5f75 7064 6174 655f 7072 6f67 7265  f _update_progre
-0000e9b0: 7373 2873 656c 6629 3a0a 2020 2020 2020  ss(self):.      
-0000e9c0: 2020 6966 2073 656c 662e 5f64 6f6e 653a    if self._done:
-0000e9d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000e9e0: 6e6f 7420 7365 6c66 2e5f 636c 6f73 6564  not self._closed
-0000e9f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ea00: 2020 7365 6c66 2e5f 636c 6f73 6528 290a    self._close().
-0000ea10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000ea20: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
-0000ea30: 2e5f 6261 722e 7374 6570 2873 656c 662e  ._bar.step(self.
-0000ea40: 5f62 7974 6573 5f63 6f70 6965 6420 2d20  _bytes_copied - 
-0000ea50: 7365 6c66 2e5f 6f6c 645f 6279 7465 735f  self._old_bytes_
-0000ea60: 636f 7069 6564 290a 2020 2020 2020 2020  copied).        
-0000ea70: 7365 6c66 2e5f 6f6c 645f 6279 7465 735f  self._old_bytes_
-0000ea80: 636f 7069 6564 203d 2073 656c 662e 5f62  copied = self._b
-0000ea90: 7974 6573 5f63 6f70 6965 640a 0a20 2020  ytes_copied..   
-0000eaa0: 2020 2020 2073 656c 662e 6166 7465 7228       self.after(
-0000eab0: 3130 302c 2073 656c 662e 5f75 7064 6174  100, self._updat
-0000eac0: 655f 7072 6f67 7265 7373 290a 0a20 2020  e_progress)..   
-0000ead0: 2064 6566 205f 636c 6f73 6528 7365 6c66   def _close(self
-0000eae0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000eaf0: 6465 7374 726f 7928 290a 2020 2020 2020  destroy().      
-0000eb00: 2020 7365 6c66 2e5f 636c 6f73 6564 203d    self._closed =
-0000eb10: 2054 7275 650a 0a20 2020 2064 6566 205f   True..    def _
-0000eb20: 6361 6e63 656c 2873 656c 662c 2065 7665  cancel(self, eve
-0000eb30: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
-0000eb40: 2020 7365 6c66 2e5f 6361 6e63 656c 6c65    self._cancelle
-0000eb50: 6420 3d20 5472 7565 0a20 2020 2020 2020  d = True.       
-0000eb60: 2073 656c 662e 5f63 6c6f 7365 2829 0a0a   self._close()..
-0000eb70: 0a63 6c61 7373 2043 686f 6963 6544 6961  .class ChoiceDia
-0000eb80: 6c6f 6728 436f 6d6d 6f6e 4469 616c 6f67  log(CommonDialog
-0000eb90: 4578 293a 0a20 2020 2064 6566 205f 5f69  Ex):.    def __i
-0000eba0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0000ebb0: 656c 662c 0a20 2020 2020 2020 206d 6173  elf,.        mas
-0000ebc0: 7465 723d 4e6f 6e65 2c0a 2020 2020 2020  ter=None,.      
-0000ebd0: 2020 7469 746c 653d 2243 686f 6f73 6520    title="Choose 
-0000ebe0: 6f6e 6522 2c0a 2020 2020 2020 2020 7175  one",.        qu
-0000ebf0: 6573 7469 6f6e 3a20 7374 7220 3d20 2243  estion: str = "C
-0000ec00: 686f 6f73 6520 6f6e 653a 222c 0a20 2020  hoose one:",.   
-0000ec10: 2020 2020 2063 686f 6963 6573 3d5b 5d2c       choices=[],
-0000ec20: 0a20 2020 2020 2020 2069 6e69 7469 616c  .        initial
-0000ec30: 5f63 686f 6963 655f 696e 6465 783d 4e6f  _choice_index=No
-0000ec40: 6e65 2c0a 2020 2020 2920 2d3e 204e 6f6e  ne,.    ) -> Non
-0000ec50: 653a 0a20 2020 2020 2020 2073 656c 662e  e:.        self.
-0000ec60: 7265 7375 6c74 203d 204e 6f6e 650a 2020  result = None.  
-0000ec70: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
-0000ec80: 696e 6974 5f5f 286d 6173 7465 723d 6d61  init__(master=ma
-0000ec90: 7374 6572 290a 0a20 2020 2020 2020 2073  ster)..        s
-0000eca0: 656c 662e 7469 746c 6528 7469 746c 6529  elf.title(title)
-0000ecb0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000ecc0: 7369 7a61 626c 6528 4661 6c73 652c 2046  sizable(False, F
-0000ecd0: 616c 7365 290a 0a20 2020 2020 2020 2073  alse)..        s
-0000ece0: 656c 662e 6d61 696e 5f66 7261 6d65 2e63  elf.main_frame.c
-0000ecf0: 6f6c 756d 6e63 6f6e 6669 6775 7265 2830  olumnconfigure(0
-0000ed00: 2c20 7765 6967 6874 3d31 290a 0a20 2020  , weight=1)..   
-0000ed10: 2020 2020 2072 6f77 203d 2030 0a20 2020       row = 0.   
-0000ed20: 2020 2020 2071 7565 7374 696f 6e5f 6c61       question_la
-0000ed30: 6265 6c20 3d20 7474 6b2e 4c61 6265 6c28  bel = ttk.Label(
-0000ed40: 7365 6c66 2e6d 6169 6e5f 6672 616d 652c  self.main_frame,
-0000ed50: 2074 6578 743d 7175 6573 7469 6f6e 290a   text=question).
-0000ed60: 2020 2020 2020 2020 7175 6573 7469 6f6e          question
-0000ed70: 5f6c 6162 656c 2e67 7269 6428 726f 773d  _label.grid(row=
-0000ed80: 726f 772c 2063 6f6c 756d 6e3d 302c 2063  row, column=0, c
-0000ed90: 6f6c 756d 6e73 7061 6e3d 322c 2073 7469  olumnspan=2, sti
-0000eda0: 636b 793d 2277 222c 2070 6164 783d 3230  cky="w", padx=20
-0000edb0: 2c20 7061 6479 3d32 3029 0a20 2020 2020  , pady=20).     
-0000edc0: 2020 2072 6f77 202b 3d20 310a 0a20 2020     row += 1..   
-0000edd0: 2020 2020 2073 656c 662e 7661 7220 3d20       self.var = 
-0000ede0: 746b 2e53 7472 696e 6756 6172 2876 616c  tk.StringVar(val
-0000edf0: 7565 3d22 2229 0a20 2020 2020 2020 2069  ue="").        i
-0000ee00: 6620 696e 6974 6961 6c5f 6368 6f69 6365  f initial_choice
-0000ee10: 5f69 6e64 6578 2069 7320 6e6f 7420 4e6f  _index is not No
-0000ee20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000ee30: 7365 6c66 2e76 6172 2e73 6574 2863 686f  self.var.set(cho
-0000ee40: 6963 6573 5b69 6e69 7469 616c 5f63 686f  ices[initial_cho
-0000ee50: 6963 655f 696e 6465 785d 290a 2020 2020  ice_index]).    
-0000ee60: 2020 2020 666f 7220 6368 6f69 6365 2069      for choice i
-0000ee70: 6e20 6368 6f69 6365 733a 0a20 2020 2020  n choices:.     
-0000ee80: 2020 2020 2020 2072 6220 3d20 7474 6b2e         rb = ttk.
-0000ee90: 5261 6469 6f62 7574 746f 6e28 7365 6c66  Radiobutton(self
-0000eea0: 2e6d 6169 6e5f 6672 616d 652c 2074 6578  .main_frame, tex
-0000eeb0: 743d 6368 6f69 6365 2c20 7661 7269 6162  t=choice, variab
-0000eec0: 6c65 3d73 656c 662e 7661 722c 2076 616c  le=self.var, val
-0000eed0: 7565 3d63 686f 6963 6529 0a20 2020 2020  ue=choice).     
-0000eee0: 2020 2020 2020 2072 622e 6772 6964 2872         rb.grid(r
-0000eef0: 6f77 3d72 6f77 2c20 636f 6c75 6d6e 3d30  ow=row, column=0
-0000ef00: 2c20 636f 6c75 6d6e 7370 616e 3d32 2c20  , columnspan=2, 
-0000ef10: 7374 6963 6b79 3d22 7722 2c20 7061 6478  sticky="w", padx
-0000ef20: 3d32 3029 0a20 2020 2020 2020 2020 2020  =20).           
-0000ef30: 2072 6f77 202b 3d20 310a 0a20 2020 2020   row += 1..     
-0000ef40: 2020 206f 6b5f 6275 7474 6f6e 203d 2074     ok_button = t
-0000ef50: 746b 2e42 7574 746f 6e28 7365 6c66 2e6d  tk.Button(self.m
-0000ef60: 6169 6e5f 6672 616d 652c 2074 6578 743d  ain_frame, text=
-0000ef70: 7472 2822 4f4b 2229 2c20 636f 6d6d 616e  tr("OK"), comman
-0000ef80: 643d 7365 6c66 2e5f 6f6b 2c20 6465 6661  d=self._ok, defa
-0000ef90: 756c 743d 2261 6374 6976 6522 290a 2020  ult="active").  
-0000efa0: 2020 2020 2020 6f6b 5f62 7574 746f 6e2e        ok_button.
-0000efb0: 6772 6964 2872 6f77 3d72 6f77 2c20 636f  grid(row=row, co
-0000efc0: 6c75 6d6e 3d30 2c20 7374 6963 6b79 3d22  lumn=0, sticky="
-0000efd0: 6522 2c20 7061 6479 3d32 3029 0a0a 2020  e", pady=20)..  
-0000efe0: 2020 2020 2020 6361 6e63 656c 5f62 7574        cancel_but
-0000eff0: 746f 6e20 3d20 7474 6b2e 4275 7474 6f6e  ton = ttk.Button
-0000f000: 2873 656c 662e 6d61 696e 5f66 7261 6d65  (self.main_frame
-0000f010: 2c20 7465 7874 3d74 7228 2243 616e 6365  , text=tr("Cance
-0000f020: 6c22 292c 2063 6f6d 6d61 6e64 3d73 656c  l"), command=sel
-0000f030: 662e 5f63 616e 6365 6c29 0a20 2020 2020  f._cancel).     
-0000f040: 2020 2063 616e 6365 6c5f 6275 7474 6f6e     cancel_button
-0000f050: 2e67 7269 6428 726f 773d 726f 772c 2063  .grid(row=row, c
-0000f060: 6f6c 756d 6e3d 312c 2073 7469 636b 793d  olumn=1, sticky=
-0000f070: 2265 222c 2070 6164 783d 3230 2c20 7061  "e", padx=20, pa
-0000f080: 6479 3d32 3029 0a0a 2020 2020 2020 2020  dy=20)..        
-0000f090: 7365 6c66 2e62 696e 6428 223c 4573 6361  self.bind("<Esca
-0000f0a0: 7065 3e22 2c20 7365 6c66 2e5f 6361 6e63  pe>", self._canc
-0000f0b0: 656c 2c20 5472 7565 290a 2020 2020 2020  el, True).      
-0000f0c0: 2020 7365 6c66 2e62 696e 6428 223c 5265    self.bind("<Re
-0000f0d0: 7475 726e 3e22 2c20 7365 6c66 2e5f 6f6b  turn>", self._ok
-0000f0e0: 2c20 5472 7565 290a 2020 2020 2020 2020  , True).        
-0000f0f0: 7365 6c66 2e70 726f 746f 636f 6c28 2257  self.protocol("W
-0000f100: 4d5f 4445 4c45 5445 5f57 494e 444f 5722  M_DELETE_WINDOW"
-0000f110: 2c20 7365 6c66 2e5f 6361 6e63 656c 290a  , self._cancel).
-0000f120: 0a20 2020 2064 6566 205f 6f6b 2873 656c  .    def _ok(sel
-0000f130: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0000f140: 2e72 6573 756c 7420 3d20 7365 6c66 2e76  .result = self.v
-0000f150: 6172 2e67 6574 2829 0a20 2020 2020 2020  ar.get().       
-0000f160: 2069 6620 6e6f 7420 7365 6c66 2e72 6573   if not self.res
-0000f170: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
-0000f180: 2073 656c 662e 7265 7375 6c74 203d 204e   self.result = N
-0000f190: 6f6e 650a 0a20 2020 2020 2020 2073 656c  one..        sel
-0000f1a0: 662e 6465 7374 726f 7928 290a 0a20 2020  f.destroy()..   
-0000f1b0: 2064 6566 205f 6361 6e63 656c 2873 656c   def _cancel(sel
-0000f1c0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0000f1d0: 2e72 6573 756c 7420 3d20 4e6f 6e65 0a20  .result = None. 
-0000f1e0: 2020 2020 2020 2073 656c 662e 6465 7374         self.dest
-0000f1f0: 726f 7928 290a 0a0a 636c 6173 7320 4c6f  roy()...class Lo
-0000f200: 6e67 5465 7874 4469 616c 6f67 2843 6f6d  ngTextDialog(Com
-0000f210: 6d6f 6e44 6961 6c6f 6729 3a0a 2020 2020  monDialog):.    
-0000f220: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0000f230: 662c 2074 6974 6c65 2c20 7465 7874 5f63  f, title, text_c
-0000f240: 6f6e 7465 6e74 2c20 7061 7265 6e74 3d4e  ontent, parent=N
-0000f250: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-0000f260: 2070 6172 656e 7420 6973 204e 6f6e 653a   parent is None:
-0000f270: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-0000f280: 656e 7420 3d20 746b 2e5f 6465 6661 756c  ent = tk._defaul
-0000f290: 745f 726f 6f74 0a0a 2020 2020 2020 2020  t_root..        
-0000f2a0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-0000f2b0: 286d 6173 7465 723d 7061 7265 6e74 290a  (master=parent).
-0000f2c0: 2020 2020 2020 2020 7365 6c66 2e74 6974          self.tit
-0000f2d0: 6c65 2874 6974 6c65 290a 0a20 2020 2020  le(title)..     
-0000f2e0: 2020 206d 6169 6e5f 6672 616d 6520 3d20     main_frame = 
-0000f2f0: 7474 6b2e 4672 616d 6528 7365 6c66 290a  ttk.Frame(self).
-0000f300: 2020 2020 2020 2020 6d61 696e 5f66 7261          main_fra
-0000f310: 6d65 2e67 7269 6428 726f 773d 302c 2063  me.grid(row=0, c
-0000f320: 6f6c 756d 6e3d 302c 2073 7469 636b 793d  olumn=0, sticky=
-0000f330: 226e 7365 7722 290a 2020 2020 2020 2020  "nsew").        
-0000f340: 7365 6c66 2e63 6f6c 756d 6e63 6f6e 6669  self.columnconfi
-0000f350: 6775 7265 2830 2c20 7765 6967 6874 3d31  gure(0, weight=1
-0000f360: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-0000f370: 6f77 636f 6e66 6967 7572 6528 302c 2077  owconfigure(0, w
-0000f380: 6569 6768 743d 3129 0a0a 2020 2020 2020  eight=1)..      
-0000f390: 2020 6465 6661 756c 745f 666f 6e74 203d    default_font =
-0000f3a0: 2074 6b2e 666f 6e74 2e6e 616d 6574 6f66   tk.font.nametof
-0000f3b0: 6f6e 7428 2254 6b44 6566 6175 6c74 466f  ont("TkDefaultFo
-0000f3c0: 6e74 2229 0a20 2020 2020 2020 2073 656c  nt").        sel
-0000f3d0: 662e 5f74 6578 7420 3d20 746b 7465 7874  f._text = tktext
-0000f3e0: 6578 742e 5465 7874 4672 616d 6528 0a20  ext.TextFrame(. 
-0000f3f0: 2020 2020 2020 2020 2020 206d 6169 6e5f             main_
-0000f400: 6672 616d 652c 0a20 2020 2020 2020 2020  frame,.         
-0000f410: 2020 2072 6561 645f 6f6e 6c79 3d54 7275     read_only=Tru
-0000f420: 652c 0a20 2020 2020 2020 2020 2020 2077  e,.            w
-0000f430: 7261 703d 226e 6f6e 6522 2c0a 2020 2020  rap="none",.    
-0000f440: 2020 2020 2020 2020 666f 6e74 3d64 6566          font=def
-0000f450: 6175 6c74 5f66 6f6e 742c 0a20 2020 2020  ault_font,.     
-0000f460: 2020 2020 2020 2077 6964 7468 3d38 302c         width=80,
-0000f470: 0a20 2020 2020 2020 2020 2020 2068 6569  .            hei
-0000f480: 6768 743d 3130 2c0a 2020 2020 2020 2020  ght=10,.        
-0000f490: 2020 2020 7265 6c69 6566 3d22 7375 6e6b      relief="sunk
-0000f4a0: 656e 222c 0a20 2020 2020 2020 2020 2020  en",.           
-0000f4b0: 2062 6f72 6465 7277 6964 7468 3d31 2c0a   borderwidth=1,.
-0000f4c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000f4d0: 2020 7365 6c66 2e5f 7465 7874 2e67 7269    self._text.gri
-0000f4e0: 6428 726f 773d 312c 2063 6f6c 756d 6e3d  d(row=1, column=
-0000f4f0: 302c 2063 6f6c 756d 6e73 7061 6e3d 322c  0, columnspan=2,
-0000f500: 2073 7469 636b 793d 226e 7365 7722 2c20   sticky="nsew", 
-0000f510: 7061 6478 3d32 302c 2070 6164 793d 3230  padx=20, pady=20
-0000f520: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-0000f530: 7465 7874 2e74 6578 742e 6469 7265 6374  text.text.direct
-0000f540: 5f69 6e73 6572 7428 2231 2e30 222c 2074  _insert("1.0", t
-0000f550: 6578 745f 636f 6e74 656e 7429 0a20 2020  ext_content).   
-0000f560: 2020 2020 2073 656c 662e 5f74 6578 742e       self._text.
-0000f570: 7465 7874 2e73 6565 2822 312e 3022 290a  text.see("1.0").
-0000f580: 0a20 2020 2020 2020 2063 6f70 795f 6275  .        copy_bu
-0000f590: 7474 6f6e 203d 2074 746b 2e42 7574 746f  tton = ttk.Butto
-0000f5a0: 6e28 0a20 2020 2020 2020 2020 2020 206d  n(.            m
-0000f5b0: 6169 6e5f 6672 616d 652c 2063 6f6d 6d61  ain_frame, comma
-0000f5c0: 6e64 3d73 656c 662e 5f63 6f70 792c 2074  nd=self._copy, t
-0000f5d0: 6578 743d 7472 2822 436f 7079 2074 6f20  ext=tr("Copy to 
-0000f5e0: 636c 6970 626f 6172 6422 292c 2077 6964  clipboard"), wid
-0000f5f0: 7468 3d32 300a 2020 2020 2020 2020 290a  th=20.        ).
-0000f600: 2020 2020 2020 2020 636f 7079 5f62 7574          copy_but
-0000f610: 746f 6e2e 6772 6964 2872 6f77 3d32 2c20  ton.grid(row=2, 
-0000f620: 636f 6c75 6d6e 3d30 2c20 7374 6963 6b79  column=0, sticky
-0000f630: 3d22 7722 2c20 7061 6478 3d32 302c 2070  ="w", padx=20, p
-0000f640: 6164 793d 2830 2c20 3230 2929 0a0a 2020  ady=(0, 20))..  
-0000f650: 2020 2020 2020 636c 6f73 655f 6275 7474        close_butt
-0000f660: 6f6e 203d 2074 746b 2e42 7574 746f 6e28  on = ttk.Button(
-0000f670: 0a20 2020 2020 2020 2020 2020 206d 6169  .            mai
-0000f680: 6e5f 6672 616d 652c 2063 6f6d 6d61 6e64  n_frame, command
-0000f690: 3d73 656c 662e 5f63 6c6f 7365 2c20 7465  =self._close, te
-0000f6a0: 7874 3d74 7228 2243 6c6f 7365 2229 2c20  xt=tr("Close"), 
-0000f6b0: 6465 6661 756c 743d 2261 6374 6976 6522  default="active"
-0000f6c0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000f6d0: 2020 2063 6c6f 7365 5f62 7574 746f 6e2e     close_button.
-0000f6e0: 6772 6964 2872 6f77 3d32 2c20 636f 6c75  grid(row=2, colu
-0000f6f0: 6d6e 3d31 2c20 7374 6963 6b79 3d22 7722  mn=1, sticky="w"
-0000f700: 2c20 7061 6478 3d32 302c 2070 6164 793d  , padx=20, pady=
-0000f710: 2830 2c20 3230 2929 0a20 2020 2020 2020  (0, 20)).       
-0000f720: 2063 6c6f 7365 5f62 7574 746f 6e2e 666f   close_button.fo
-0000f730: 6375 735f 7365 7428 290a 0a20 2020 2020  cus_set()..     
-0000f740: 2020 206d 6169 6e5f 6672 616d 652e 636f     main_frame.co
-0000f750: 6c75 6d6e 636f 6e66 6967 7572 6528 302c  lumnconfigure(0,
-0000f760: 2077 6569 6768 743d 3129 0a20 2020 2020   weight=1).     
-0000f770: 2020 206d 6169 6e5f 6672 616d 652e 726f     main_frame.ro
-0000f780: 7763 6f6e 6669 6775 7265 2831 2c20 7765  wconfigure(1, we
-0000f790: 6967 6874 3d31 290a 0a20 2020 2020 2020  ight=1)..       
-0000f7a0: 2073 656c 662e 7072 6f74 6f63 6f6c 2822   self.protocol("
-0000f7b0: 574d 5f44 454c 4554 455f 5749 4e44 4f57  WM_DELETE_WINDOW
-0000f7c0: 222c 2073 656c 662e 5f63 6c6f 7365 290a  ", self._close).
-0000f7d0: 2020 2020 2020 2020 7365 6c66 2e62 696e          self.bin
-0000f7e0: 6428 223c 4573 6361 7065 3e22 2c20 7365  d("<Escape>", se
-0000f7f0: 6c66 2e5f 636c 6f73 652c 2054 7275 6529  lf._close, True)
-0000f800: 0a0a 2020 2020 6465 6620 5f63 6f70 7928  ..    def _copy(
-0000f810: 7365 6c66 2c20 6576 656e 743d 4e6f 6e65  self, event=None
-0000f820: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000f830: 636c 6970 626f 6172 645f 636c 6561 7228  clipboard_clear(
-0000f840: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000f850: 6c69 7062 6f61 7264 5f61 7070 656e 6428  lipboard_append(
-0000f860: 7365 6c66 2e5f 7465 7874 2e74 6578 742e  self._text.text.
-0000f870: 6765 7428 2231 2e30 222c 2022 656e 6422  get("1.0", "end"
-0000f880: 2929 0a0a 2020 2020 6465 6620 5f63 6c6f  ))..    def _clo
-0000f890: 7365 2873 656c 662c 2065 7665 6e74 3d4e  se(self, event=N
-0000f8a0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-0000f8b0: 6c66 2e64 6573 7472 6f79 2829 0a0a 0a64  lf.destroy()...d
-0000f8c0: 6566 2061 736b 5f6f 6e65 5f66 726f 6d5f  ef ask_one_from_
-0000f8d0: 6368 6f69 6365 7328 0a20 2020 206d 6173  choices(.    mas
-0000f8e0: 7465 723d 4e6f 6e65 2c0a 2020 2020 7469  ter=None,.    ti
-0000f8f0: 746c 653d 2243 686f 6f73 6520 6f6e 6522  tle="Choose one"
-0000f900: 2c0a 2020 2020 7175 6573 7469 6f6e 3a20  ,.    question: 
-0000f910: 7374 7220 3d20 2243 686f 6f73 6520 6f6e  str = "Choose on
-0000f920: 653a 222c 0a20 2020 2063 686f 6963 6573  e:",.    choices
-0000f930: 3d5b 5d2c 0a20 2020 2069 6e69 7469 616c  =[],.    initial
-0000f940: 5f63 686f 6963 655f 696e 6465 783d 4e6f  _choice_index=No
-0000f950: 6e65 2c0a 293a 0a20 2020 2064 6c67 203d  ne,.):.    dlg =
-0000f960: 2043 686f 6963 6544 6961 6c6f 6728 6d61   ChoiceDialog(ma
-0000f970: 7374 6572 2c20 7469 746c 652c 2071 7565  ster, title, que
-0000f980: 7374 696f 6e2c 2063 686f 6963 6573 2c20  stion, choices, 
-0000f990: 696e 6974 6961 6c5f 6368 6f69 6365 5f69  initial_choice_i
-0000f9a0: 6e64 6578 290a 2020 2020 7368 6f77 5f64  ndex).    show_d
-0000f9b0: 6961 6c6f 6728 646c 672c 206d 6173 7465  ialog(dlg, maste
-0000f9c0: 7229 0a20 2020 2072 6574 7572 6e20 646c  r).    return dl
-0000f9d0: 672e 7265 7375 6c74 0a0a 0a64 6566 2067  g.result...def g
-0000f9e0: 6574 5f62 7573 795f 6375 7273 6f72 2829  et_busy_cursor()
-0000f9f0: 3a0a 2020 2020 6966 2072 756e 6e69 6e67  :.    if running
-0000fa00: 5f6f 6e5f 7769 6e64 6f77 7328 293a 0a20  _on_windows():. 
-0000fa10: 2020 2020 2020 2072 6574 7572 6e20 2277         return "w
-0000fa20: 6169 7422 0a20 2020 2065 6c69 6620 7275  ait".    elif ru
-0000fa30: 6e6e 696e 675f 6f6e 5f6d 6163 5f6f 7328  nning_on_mac_os(
-0000fa40: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000fa50: 6e20 2273 7069 6e6e 696e 6722 0a20 2020  n "spinning".   
-0000fa60: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-0000fa70: 6574 7572 6e20 2277 6174 6368 220a 0a0a  eturn "watch"...
-0000fa80: 6465 6620 6765 745f 746b 5f76 6572 7369  def get_tk_versi
-0000fa90: 6f6e 5f73 7472 2829 3a0a 2020 2020 7265  on_str():.    re
-0000faa0: 7475 726e 2074 6b2e 5f64 6566 6175 6c74  turn tk._default
-0000fab0: 5f72 6f6f 742e 746b 2e63 616c 6c28 2269  _root.tk.call("i
-0000fac0: 6e66 6f22 2c20 2270 6174 6368 6c65 7665  nfo", "patchleve
-0000fad0: 6c22 290a 0a0a 6465 6620 6765 745f 746b  l")...def get_tk
-0000fae0: 5f76 6572 7369 6f6e 5f69 6e66 6f28 293a  _version_info():
-0000faf0: 0a20 2020 2072 6573 756c 7420 3d20 5b5d  .    result = []
-0000fb00: 0a20 2020 2066 6f72 2070 6172 7420 696e  .    for part in
-0000fb10: 2067 6574 5f74 6b5f 7665 7273 696f 6e5f   get_tk_version_
-0000fb20: 7374 7228 292e 7370 6c69 7428 222e 2229  str().split(".")
-0000fb30: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-0000fb40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000fb50: 742e 6170 7065 6e64 2869 6e74 2870 6172  t.append(int(par
-0000fb60: 7429 290a 2020 2020 2020 2020 6578 6365  t)).        exce
-0000fb70: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
-0000fb80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000fb90: 2e61 7070 656e 6428 3029 0a20 2020 2072  .append(0).    r
-0000fba0: 6574 7572 6e20 7475 706c 6528 7265 7375  eturn tuple(resu
-0000fbb0: 6c74 290a 0a0a 6465 6620 6765 745f 7374  lt)...def get_st
-0000fbc0: 796c 655f 636f 6e66 6967 7572 6174 696f  yle_configuratio
-0000fbd0: 6e28 7374 796c 655f 6e61 6d65 2c20 6465  n(style_name, de
-0000fbe0: 6661 756c 743d 7b7d 293a 0a20 2020 2073  fault={}):.    s
-0000fbf0: 7479 6c65 203d 2074 746b 2e53 7479 6c65  tyle = ttk.Style
-0000fc00: 2829 0a20 2020 2023 204e 4221 2073 7479  ().    # NB! sty
-0000fc10: 6c65 2e63 6f6e 6669 6775 7265 2073 6565  le.configure see
-0000fc20: 6d73 2074 6f20 7265 7573 6520 7468 6520  ms to reuse the 
-0000fc30: 7265 7475 726e 6564 2064 6963 740a 2020  returned dict.  
-0000fc40: 2020 2320 446f 6e27 7420 6368 616e 6765    # Don't change
-0000fc50: 2069 7420 7769 7468 6f75 7420 636f 7079   it without copy
-0000fc60: 696e 6720 6669 7273 740a 2020 2020 7265  ing first.    re
-0000fc70: 7375 6c74 203d 2073 7479 6c65 2e63 6f6e  sult = style.con
-0000fc80: 6669 6775 7265 2873 7479 6c65 5f6e 616d  figure(style_nam
-0000fc90: 6529 0a20 2020 2069 6620 7265 7375 6c74  e).    if result
-0000fca0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000fcb0: 2020 7265 7475 726e 2064 6566 6175 6c74    return default
-0000fcc0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000fcd0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0000fce0: 0a0a 0a64 6566 206c 6f6f 6b75 705f 7374  ...def lookup_st
-0000fcf0: 796c 655f 6f70 7469 6f6e 2873 7479 6c65  yle_option(style
-0000fd00: 5f6e 616d 652c 206f 7074 696f 6e5f 6e61  _name, option_na
-0000fd10: 6d65 2c20 6465 6661 756c 743d 4e6f 6e65  me, default=None
-0000fd20: 293a 0a20 2020 2073 7479 6c65 203d 2074  ):.    style = t
-0000fd30: 746b 2e53 7479 6c65 2829 0a20 2020 2073  tk.Style().    s
-0000fd40: 6574 7469 6e67 203d 2073 7479 6c65 2e6c  etting = style.l
-0000fd50: 6f6f 6b75 7028 7374 796c 655f 6e61 6d65  ookup(style_name
-0000fd60: 2c20 6f70 7469 6f6e 5f6e 616d 6529 0a20  , option_name). 
-0000fd70: 2020 2069 6620 7365 7474 696e 6720 696e     if setting in
-0000fd80: 205b 4e6f 6e65 2c20 2222 5d3a 0a20 2020   [None, ""]:.   
-0000fd90: 2020 2020 2072 6574 7572 6e20 6465 6661       return defa
-0000fda0: 756c 740a 2020 2020 656c 6966 2073 6574  ult.    elif set
-0000fdb0: 7469 6e67 203d 3d20 2254 7275 6522 3a0a  ting == "True":.
-0000fdc0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000fdd0: 7275 650a 2020 2020 656c 6966 2073 6574  rue.    elif set
-0000fde0: 7469 6e67 203d 3d20 2246 616c 7365 223a  ting == "False":
-0000fdf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000fe00: 4661 6c73 650a 2020 2020 656c 7365 3a0a  False.    else:.
-0000fe10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000fe20: 6574 7469 6e67 0a0a 0a64 6566 2073 6361  etting...def sca
-0000fe30: 6c65 2876 616c 7565 293a 0a20 2020 2072  le(value):.    r
-0000fe40: 6574 7572 6e20 6765 745f 776f 726b 6265  eturn get_workbe
-0000fe50: 6e63 6828 292e 7363 616c 6528 7661 6c75  nch().scale(valu
-0000fe60: 6529 0a0a 0a64 6566 206f 7065 6e5f 7061  e)...def open_pa
-0000fe70: 7468 5f69 6e5f 7379 7374 656d 5f66 696c  th_in_system_fil
-0000fe80: 655f 6d61 6e61 6765 7228 7061 7468 293a  e_manager(path):
-0000fe90: 0a20 2020 2069 6620 7275 6e6e 696e 675f  .    if running_
-0000fea0: 6f6e 5f6d 6163 5f6f 7328 293a 0a20 2020  on_mac_os():.   
-0000feb0: 2020 2020 2023 2068 7474 703a 2f2f 7374       # http://st
-0000fec0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-0000fed0: 612f 3335 3230 3639 332f 3236 3131 3831  a/3520693/261181
-0000fee0: 0a20 2020 2020 2020 2023 202d 5220 646f  .        # -R do
-0000fef0: 6573 6e27 7420 616c 6c6f 7720 7368 6f77  esn't allow show
-0000ff00: 696e 6720 6869 6464 656e 2066 6f6c 6465  ing hidden folde
-0000ff10: 7273 0a20 2020 2020 2020 2073 7562 7072  rs.        subpr
-0000ff20: 6f63 6573 732e 506f 7065 6e28 5b22 6f70  ocess.Popen(["op
-0000ff30: 656e 222c 2070 6174 685d 290a 2020 2020  en", path]).    
-0000ff40: 656c 6966 2072 756e 6e69 6e67 5f6f 6e5f  elif running_on_
-0000ff50: 6c69 6e75 7828 293a 0a20 2020 2020 2020  linux():.       
-0000ff60: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
-0000ff70: 6e28 5b22 7864 672d 6f70 656e 222c 2070  n(["xdg-open", p
-0000ff80: 6174 685d 290a 2020 2020 656c 7365 3a0a  ath]).    else:.
-0000ff90: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-0000ffa0: 756e 6e69 6e67 5f6f 6e5f 7769 6e64 6f77  unning_on_window
-0000ffb0: 7328 290a 2020 2020 2020 2020 7375 6270  s().        subp
-0000ffc0: 726f 6365 7373 2e50 6f70 656e 285b 2265  rocess.Popen(["e
-0000ffd0: 7870 6c6f 7265 7222 2c20 7061 7468 5d29  xplorer", path])
-0000ffe0: 0a0a 0a64 6566 205f 6765 745f 6469 616c  ...def _get_dial
-0000fff0: 6f67 5f70 726f 7669 6465 7228 293a 0a20  og_provider():. 
-00010000: 2020 2069 6620 706c 6174 666f 726d 2e73     if platform.s
-00010010: 7973 7465 6d28 2920 213d 2022 4c69 6e75  ystem() != "Linu
-00010020: 7822 206f 7220 6765 745f 776f 726b 6265  x" or get_workbe
-00010030: 6e63 6828 292e 6765 745f 6f70 7469 6f6e  nch().get_option
-00010040: 2822 6669 6c65 2e61 766f 6964 5f7a 656e  ("file.avoid_zen
-00010050: 6974 7922 293a 0a20 2020 2020 2020 2072  ity"):.        r
-00010060: 6574 7572 6e20 6669 6c65 6469 616c 6f67  eturn filedialog
-00010070: 0a0a 2020 2020 696d 706f 7274 2073 6875  ..    import shu
-00010080: 7469 6c0a 0a20 2020 2069 6620 7368 7574  til..    if shut
-00010090: 696c 2e77 6869 6368 2822 7a65 6e69 7479  il.which("zenity
-000100a0: 2229 3a0a 2020 2020 2020 2020 7265 7475  "):.        retu
-000100b0: 726e 205f 5a65 6e69 7479 4469 616c 6f67  rn _ZenityDialog
-000100c0: 5072 6f76 6964 6572 0a0a 2020 2020 2320  Provider..    # 
-000100d0: 6661 6c6c 6261 636b 0a20 2020 2072 6574  fallback.    ret
-000100e0: 7572 6e20 6669 6c65 6469 616c 6f67 0a0a  urn filedialog..
-000100f0: 0a64 6566 2074 7279 5f72 6573 746f 7265  .def try_restore
-00010100: 5f66 6f63 7573 5f61 6674 6572 5f66 696c  _focus_after_fil
-00010110: 655f 6469 616c 6f67 2864 6961 6c6f 675f  e_dialog(dialog_
-00010120: 7061 7265 6e74 293a 0a20 2020 2069 6620  parent):.    if 
-00010130: 6469 616c 6f67 5f70 6172 656e 7420 6973  dialog_parent is
-00010140: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
-00010150: 6574 7572 6e0a 0a20 2020 206c 6f67 6765  eturn..    logge
-00010160: 722e 696e 666f 2822 5265 7374 6f72 696e  r.info("Restorin
-00010170: 6720 666f 6375 7320 746f 2025 7322 2c20  g focus to %s", 
-00010180: 6469 616c 6f67 5f70 6172 656e 7429 0a20  dialog_parent). 
-00010190: 2020 206f 6c64 5f66 6f63 7573 6564 5f77     old_focused_w
-000101a0: 6964 6765 7420 3d20 6469 616c 6f67 5f70  idget = dialog_p
-000101b0: 6172 656e 742e 7769 6e66 6f5f 746f 706c  arent.winfo_topl
-000101c0: 6576 656c 2829 2e66 6f63 7573 5f67 6574  evel().focus_get
-000101d0: 2829 0a0a 2020 2020 6469 616c 6f67 5f70  ()..    dialog_p
-000101e0: 6172 656e 742e 7769 6e66 6f5f 746f 706c  arent.winfo_topl
-000101f0: 6576 656c 2829 2e6c 6966 7428 290a 2020  evel().lift().  
-00010200: 2020 6469 616c 6f67 5f70 6172 656e 742e    dialog_parent.
-00010210: 7769 6e66 6f5f 746f 706c 6576 656c 2829  winfo_toplevel()
-00010220: 2e66 6f63 7573 5f66 6f72 6365 2829 0a20  .focus_force(). 
-00010230: 2020 2064 6961 6c6f 675f 7061 7265 6e74     dialog_parent
-00010240: 2e77 696e 666f 5f74 6f70 6c65 7665 6c28  .winfo_toplevel(
-00010250: 292e 6772 6162 5f73 6574 2829 0a20 2020  ).grab_set().   
-00010260: 2069 6620 7275 6e6e 696e 675f 6f6e 5f6d   if running_on_m
-00010270: 6163 5f6f 7328 293a 0a20 2020 2020 2020  ac_os():.       
-00010280: 2064 6961 6c6f 675f 7061 7265 6e74 2e77   dialog_parent.w
-00010290: 696e 666f 5f74 6f70 6c65 7665 6c28 292e  info_toplevel().
-000102a0: 6772 6162 5f72 656c 6561 7365 2829 0a0a  grab_release()..
-000102b0: 2020 2020 6966 206f 6c64 5f66 6f63 7573      if old_focus
-000102c0: 6564 5f77 6964 6765 7420 6973 206e 6f74  ed_widget is not
-000102d0: 204e 6f6e 653a 0a20 2020 2020 2020 2074   None:.        t
-000102e0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000102f0: 6f6c 645f 666f 6375 7365 645f 7769 6467  old_focused_widg
-00010300: 6574 2e66 6f63 7573 5f66 6f72 6365 2829  et.focus_force()
-00010310: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00010320: 5463 6c45 7272 6f72 3a0a 2020 2020 2020  TclError:.      
-00010330: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-00010340: 6e69 6e67 2822 436f 756c 6420 6e6f 7420  ning("Could not 
-00010350: 7265 7374 6f72 6520 666f 6375 7320 746f  restore focus to
-00010360: 2025 7222 2c20 6f6c 645f 666f 6375 7365   %r", old_focuse
-00010370: 645f 7769 6467 6574 290a 0a0a 6465 6620  d_widget)...def 
-00010380: 6173 6b73 6176 6561 7366 696c 656e 616d  asksaveasfilenam
-00010390: 6528 2a2a 6f70 7469 6f6e 7329 3a0a 2020  e(**options):.  
-000103a0: 2020 2320 6874 7470 733a 2f2f 7463 6c2e    # https://tcl.
-000103b0: 746b 2f6d 616e 2f74 636c 382e 362f 546b  tk/man/tcl8.6/Tk
-000103c0: 436d 642f 6765 744f 7065 6e46 696c 652e  Cmd/getOpenFile.
-000103d0: 6874 6d0a 2020 2020 7061 7265 6e74 203d  htm.    parent =
-000103e0: 205f 6368 6563 6b5f 6469 616c 6f67 5f70   _check_dialog_p
-000103f0: 6172 656e 7428 6f70 7469 6f6e 7329 0a20  arent(options). 
-00010400: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00010410: 7265 7475 726e 205f 6765 745f 6469 616c  return _get_dial
-00010420: 6f67 5f70 726f 7669 6465 7228 292e 6173  og_provider().as
-00010430: 6b73 6176 6561 7366 696c 656e 616d 6528  ksaveasfilename(
-00010440: 2a2a 6f70 7469 6f6e 7329 0a20 2020 2066  **options).    f
-00010450: 696e 616c 6c79 3a0a 2020 2020 2020 2020  inally:.        
-00010460: 7472 795f 7265 7374 6f72 655f 666f 6375  try_restore_focu
-00010470: 735f 6166 7465 725f 6669 6c65 5f64 6961  s_after_file_dia
-00010480: 6c6f 6728 7061 7265 6e74 290a 0a0a 6465  log(parent)...de
-00010490: 6620 6173 6b6f 7065 6e66 696c 656e 616d  f askopenfilenam
-000104a0: 6528 2a2a 6f70 7469 6f6e 7329 3a0a 2020  e(**options):.  
-000104b0: 2020 2320 6874 7470 733a 2f2f 7463 6c2e    # https://tcl.
-000104c0: 746b 2f6d 616e 2f74 636c 382e 362f 546b  tk/man/tcl8.6/Tk
-000104d0: 436d 642f 6765 744f 7065 6e46 696c 652e  Cmd/getOpenFile.
-000104e0: 6874 6d0a 2020 2020 7061 7265 6e74 203d  htm.    parent =
-000104f0: 205f 6368 6563 6b5f 6469 616c 6f67 5f70   _check_dialog_p
-00010500: 6172 656e 7428 6f70 7469 6f6e 7329 0a20  arent(options). 
-00010510: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00010520: 7265 7475 726e 205f 6765 745f 6469 616c  return _get_dial
-00010530: 6f67 5f70 726f 7669 6465 7228 292e 6173  og_provider().as
-00010540: 6b6f 7065 6e66 696c 656e 616d 6528 2a2a  kopenfilename(**
-00010550: 6f70 7469 6f6e 7329 0a20 2020 2066 696e  options).    fin
-00010560: 616c 6c79 3a0a 2020 2020 2020 2020 7472  ally:.        tr
-00010570: 795f 7265 7374 6f72 655f 666f 6375 735f  y_restore_focus_
-00010580: 6166 7465 725f 6669 6c65 5f64 6961 6c6f  after_file_dialo
-00010590: 6728 7061 7265 6e74 290a 0a0a 6465 6620  g(parent)...def 
-000105a0: 6173 6b6f 7065 6e66 696c 656e 616d 6573  askopenfilenames
-000105b0: 282a 2a6f 7074 696f 6e73 293a 0a20 2020  (**options):.   
-000105c0: 2023 2068 7474 7073 3a2f 2f74 636c 2e74   # https://tcl.t
-000105d0: 6b2f 6d61 6e2f 7463 6c38 2e36 2f54 6b43  k/man/tcl8.6/TkC
-000105e0: 6d64 2f67 6574 4f70 656e 4669 6c65 2e68  md/getOpenFile.h
-000105f0: 746d 0a20 2020 2070 6172 656e 7420 3d20  tm.    parent = 
-00010600: 5f63 6865 636b 5f64 6961 6c6f 675f 7061  _check_dialog_pa
-00010610: 7265 6e74 286f 7074 696f 6e73 290a 2020  rent(options).  
-00010620: 2020 7472 793a 0a20 2020 2020 2020 2072    try:.        r
-00010630: 6574 7572 6e20 5f67 6574 5f64 6961 6c6f  eturn _get_dialo
-00010640: 675f 7072 6f76 6964 6572 2829 2e61 736b  g_provider().ask
-00010650: 6f70 656e 6669 6c65 6e61 6d65 7328 2a2a  openfilenames(**
-00010660: 6f70 7469 6f6e 7329 0a20 2020 2066 696e  options).    fin
-00010670: 616c 6c79 3a0a 2020 2020 2020 2020 7472  ally:.        tr
-00010680: 795f 7265 7374 6f72 655f 666f 6375 735f  y_restore_focus_
-00010690: 6166 7465 725f 6669 6c65 5f64 6961 6c6f  after_file_dialo
-000106a0: 6728 7061 7265 6e74 290a 0a0a 6465 6620  g(parent)...def 
-000106b0: 6173 6b64 6972 6563 746f 7279 282a 2a6f  askdirectory(**o
-000106c0: 7074 696f 6e73 293a 0a20 2020 2023 2068  ptions):.    # h
-000106d0: 7474 7073 3a2f 2f74 636c 2e74 6b2f 6d61  ttps://tcl.tk/ma
-000106e0: 6e2f 7463 6c38 2e36 2f54 6b43 6d64 2f63  n/tcl8.6/TkCmd/c
-000106f0: 686f 6f73 6544 6972 6563 746f 7279 2e68  hooseDirectory.h
-00010700: 746d 0a20 2020 2070 6172 656e 7420 3d20  tm.    parent = 
-00010710: 5f63 6865 636b 5f64 6961 6c6f 675f 7061  _check_dialog_pa
-00010720: 7265 6e74 286f 7074 696f 6e73 290a 2020  rent(options).  
-00010730: 2020 7472 793a 0a20 2020 2020 2020 2072    try:.        r
-00010740: 6574 7572 6e20 5f67 6574 5f64 6961 6c6f  eturn _get_dialo
-00010750: 675f 7072 6f76 6964 6572 2829 2e61 736b  g_provider().ask
-00010760: 6469 7265 6374 6f72 7928 2a2a 6f70 7469  directory(**opti
-00010770: 6f6e 7329 0a20 2020 2066 696e 616c 6c79  ons).    finally
-00010780: 3a0a 2020 2020 2020 2020 7472 795f 7265  :.        try_re
-00010790: 7374 6f72 655f 666f 6375 735f 6166 7465  store_focus_afte
-000107a0: 725f 6669 6c65 5f64 6961 6c6f 6728 7061  r_file_dialog(pa
-000107b0: 7265 6e74 290a 0a0a 6465 6620 5f63 6865  rent)...def _che
-000107c0: 636b 5f64 6961 6c6f 675f 7061 7265 6e74  ck_dialog_parent
-000107d0: 286f 7074 696f 6e73 293a 0a20 2020 2069  (options):.    i
-000107e0: 6620 6f70 7469 6f6e 732e 6765 7428 2270  f options.get("p
-000107f0: 6172 656e 7422 2920 616e 6420 6f70 7469  arent") and opti
-00010800: 6f6e 732e 6765 7428 226d 6173 7465 7222  ons.get("master"
-00010810: 293a 0a20 2020 2020 2020 2070 6172 656e  ):.        paren
-00010820: 7420 3d20 6f70 7469 6f6e 735b 2270 6172  t = options["par
-00010830: 656e 7422 5d2e 7769 6e66 6f5f 746f 706c  ent"].winfo_topl
-00010840: 6576 656c 2829 0a20 2020 2020 2020 206d  evel().        m
-00010850: 6173 7465 7220 3d20 6f70 7469 6f6e 735b  aster = options[
-00010860: 226d 6173 7465 7222 5d2e 7769 6e66 6f5f  "master"].winfo_
-00010870: 746f 706c 6576 656c 2829 0a20 2020 2020  toplevel().     
-00010880: 2020 2069 6620 7061 7265 6e74 2069 7320     if parent is 
-00010890: 6e6f 7420 6d61 7374 6572 3a0a 2020 2020  not master:.    
-000108a0: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-000108b0: 6172 6e69 6e67 280a 2020 2020 2020 2020  arning(.        
-000108c0: 2020 2020 2020 2020 2244 6961 6c6f 6720          "Dialog 
-000108d0: 7769 7468 2064 6966 6665 7265 6e74 2070  with different p
-000108e0: 6172 656e 742f 6d61 7374 6572 2074 6f70  arent/master top
-000108f0: 6c65 7665 6c73 3a5c 6e25 7322 2c0a 2020  levels:\n%s",.  
-00010900: 2020 2020 2020 2020 2020 2020 2020 2222                ""
-00010910: 2e6a 6f69 6e28 7472 6163 6562 6163 6b2e  .join(traceback.
-00010920: 666f 726d 6174 5f73 7461 636b 2829 292c  format_stack()),
-00010930: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00010940: 2020 2065 6c69 6620 6f70 7469 6f6e 732e     elif options.
-00010950: 6765 7428 2270 6172 656e 7422 293a 0a20  get("parent"):. 
-00010960: 2020 2020 2020 2070 6172 656e 7420 3d20         parent = 
-00010970: 6f70 7469 6f6e 735b 2270 6172 656e 7422  options["parent"
-00010980: 5d2e 7769 6e66 6f5f 746f 706c 6576 656c  ].winfo_toplevel
-00010990: 2829 0a20 2020 2020 2020 206d 6173 7465  ().        maste
-000109a0: 7220 3d20 6f70 7469 6f6e 735b 2270 6172  r = options["par
-000109b0: 656e 7422 5d2e 7769 6e66 6f5f 746f 706c  ent"].winfo_topl
-000109c0: 6576 656c 2829 0a20 2020 2065 6c69 6620  evel().    elif 
-000109d0: 6f70 7469 6f6e 732e 6765 7428 226d 6173  options.get("mas
-000109e0: 7465 7222 293a 0a20 2020 2020 2020 2070  ter"):.        p
-000109f0: 6172 656e 7420 3d20 6f70 7469 6f6e 735b  arent = options[
-00010a00: 226d 6173 7465 7222 5d2e 7769 6e66 6f5f  "master"].winfo_
-00010a10: 746f 706c 6576 656c 2829 0a20 2020 2020  toplevel().     
-00010a20: 2020 206d 6173 7465 7220 3d20 6f70 7469     master = opti
-00010a30: 6f6e 735b 226d 6173 7465 7222 5d2e 7769  ons["master"].wi
-00010a40: 6e66 6f5f 746f 706c 6576 656c 2829 0a20  nfo_toplevel(). 
-00010a50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00010a60: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-00010a70: 2244 6961 6c6f 6720 7769 7468 6f75 7420  "Dialog without 
-00010a80: 7061 7265 6e74 3a5c 6e25 7322 2c20 2222  parent:\n%s", ""
-00010a90: 2e6a 6f69 6e28 7472 6163 6562 6163 6b2e  .join(traceback.
-00010aa0: 666f 726d 6174 5f73 7461 636b 2829 2929  format_stack()))
-00010ab0: 0a20 2020 2020 2020 2070 6172 656e 7420  .        parent 
-00010ac0: 3d20 746b 2e5f 6465 6661 756c 745f 726f  = tk._default_ro
-00010ad0: 6f74 0a20 2020 2020 2020 206d 6173 7465  ot.        maste
-00010ae0: 7220 3d20 746b 2e5f 6465 6661 756c 745f  r = tk._default_
-00010af0: 726f 6f74 0a0a 2020 2020 6f70 7469 6f6e  root..    option
-00010b00: 735b 2270 6172 656e 7422 5d20 3d20 7061  s["parent"] = pa
-00010b10: 7265 6e74 0a20 2020 206f 7074 696f 6e73  rent.    options
-00010b20: 5b22 6d61 7374 6572 225d 203d 206d 6173  ["master"] = mas
-00010b30: 7465 720a 0a20 2020 2069 6620 7275 6e6e  ter..    if runn
-00010b40: 696e 675f 6f6e 5f6d 6163 5f6f 7328 293a  ing_on_mac_os():
-00010b50: 0a20 2020 2020 2020 2023 2075 7365 6420  .        # used 
-00010b60: 746f 2072 6571 7569 7265 206d 6173 7465  to require maste
-00010b70: 722f 7061 7265 6e74 2028 6874 7470 733a  r/parent (https:
-00010b80: 2f2f 6275 6773 2e70 7974 686f 6e2e 6f72  //bugs.python.or
-00010b90: 672f 6973 7375 6533 3439 3237 290a 2020  g/issue34927).  
-00010ba0: 2020 2020 2020 2320 6275 7420 7468 6973        # but this
-00010bb0: 2069 7320 6465 7072 6563 6174 6564 2069   is deprecated i
-00010bc0: 6e20 4361 7461 6c69 6e61 2028 6874 7470  n Catalina (http
-00010bd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00010be0: 686f 6e6e 792f 7468 6f6e 6e79 2f69 7373  honny/thonny/iss
-00010bf0: 7565 732f 3834 3029 0a20 2020 2020 2020  ues/840).       
-00010c00: 2023 2054 4f44 4f3a 2043 6f6e 7369 6465   # TODO: Conside
-00010c10: 7220 7265 6d6f 7669 6e67 2074 6869 7320  r removing this 
-00010c20: 7768 656e 2075 7067 7261 6469 6e67 2066  when upgrading f
-00010c30: 726f 6d20 546b 2038 2e36 2e38 0a20 2020  rom Tk 8.6.8.   
-00010c40: 2020 2020 2064 656c 206f 7074 696f 6e73       del options
-00010c50: 5b22 6d61 7374 6572 225d 0a20 2020 2020  ["master"].     
-00010c60: 2020 2064 656c 206f 7074 696f 6e73 5b22     del options["
-00010c70: 7061 7265 6e74 225d 0a0a 2020 2020 7265  parent"]..    re
-00010c80: 7475 726e 2070 6172 656e 740a 0a0a 636c  turn parent...cl
-00010c90: 6173 7320 5f5a 656e 6974 7944 6961 6c6f  ass _ZenityDialo
-00010ca0: 6750 726f 7669 6465 723a 0a20 2020 2023  gProvider:.    #
-00010cb0: 2068 7474 7073 3a2f 2f77 7777 2e77 7269   https://www.wri
-00010cc0: 7465 6261 7368 2e63 6f6d 2f62 6173 682d  tebash.com/bash-
-00010cd0: 6775 692f 7a65 6e69 7479 2d63 7265 6174  gui/zenity-creat
-00010ce0: 652d 6669 6c65 2d73 656c 6563 7469 6f6e  e-file-selection
-00010cf0: 2d64 6961 6c6f 672d 3232 342e 6874 6d6c  -dialog-224.html
-00010d00: 0a20 2020 2023 2068 7474 703a 2f2f 6c69  .    # http://li
-00010d10: 6e75 782e 6279 6578 616d 706c 6573 2e63  nux.byexamples.c
-00010d20: 6f6d 2f61 7263 6869 7665 732f 3235 392f  om/archives/259/
-00010d30: 612d 636f 6d70 6c65 7465 2d7a 656e 6974  a-complete-zenit
-00010d40: 792d 6469 616c 6f67 2d65 7861 6d70 6c65  y-dialog-example
-00010d50: 732d 312f 0a20 2020 2023 2068 7474 703a  s-1/.    # http:
-00010d60: 2f2f 6c69 6e75 782e 6279 6578 616d 706c  //linux.byexampl
-00010d70: 6573 2e63 6f6d 2f61 7263 6869 7665 732f  es.com/archives/
-00010d80: 3236 352f 612d 636f 6d70 6c65 7465 2d7a  265/a-complete-z
-00010d90: 656e 6974 792d 6469 616c 6f67 2d65 7861  enity-dialog-exa
-00010da0: 6d70 6c65 732d 322f 0a0a 2020 2020 2320  mples-2/..    # 
-00010db0: 616e 6f74 6865 7220 706f 7373 6962 696c  another possibil
-00010dc0: 6974 7920 6973 2074 6f20 7573 6520 5079  ity is to use Py
-00010dd0: 476f 626a 6563 743a 2068 7474 7073 3a2f  Gobject: https:/
-00010de0: 2f67 6974 6875 622e 636f 6d2f 706f 756c  /github.com/poul
-00010df0: 702f 7a65 6e69 7079 0a0a 2020 2020 4063  p/zenipy..    @c
-00010e00: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00010e10: 6566 2061 736b 6f70 656e 6669 6c65 6e61  ef askopenfilena
-00010e20: 6d65 2863 6c73 2c20 2a2a 6f70 7469 6f6e  me(cls, **option
-00010e30: 7329 3a0a 2020 2020 2020 2020 6172 6773  s):.        args
-00010e40: 203d 2063 6c73 2e5f 636f 6e76 6572 745f   = cls._convert_
-00010e50: 636f 6d6d 6f6e 5f6f 7074 696f 6e73 2822  common_options("
-00010e60: 4f70 656e 2066 696c 6522 2c20 2a2a 6f70  Open file", **op
-00010e70: 7469 6f6e 7329 0a20 2020 2020 2020 2072  tions).        r
-00010e80: 6574 7572 6e20 636c 732e 5f63 616c 6c28  eturn cls._call(
-00010e90: 6172 6773 290a 0a20 2020 2040 636c 6173  args)..    @clas
-00010ea0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00010eb0: 6173 6b6f 7065 6e66 696c 656e 616d 6573  askopenfilenames
-00010ec0: 2863 6c73 2c20 2a2a 6f70 7469 6f6e 7329  (cls, **options)
-00010ed0: 3a0a 2020 2020 2020 2020 6172 6773 203d  :.        args =
-00010ee0: 2063 6c73 2e5f 636f 6e76 6572 745f 636f   cls._convert_co
-00010ef0: 6d6d 6f6e 5f6f 7074 696f 6e73 2822 4f70  mmon_options("Op
-00010f00: 656e 2066 696c 6573 222c 202a 2a6f 7074  en files", **opt
-00010f10: 696f 6e73 290a 2020 2020 2020 2020 7265  ions).        re
-00010f20: 7475 726e 2063 6c73 2e5f 6361 6c6c 2861  turn cls._call(a
-00010f30: 7267 7320 2b20 5b22 2d2d 6d75 6c74 6970  rgs + ["--multip
-00010f40: 6c65 225d 292e 7370 6c69 7428 227c 2229  le"]).split("|")
-00010f50: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00010f60: 6f64 0a20 2020 2064 6566 2061 736b 7361  od.    def asksa
-00010f70: 7665 6173 6669 6c65 6e61 6d65 2863 6c73  veasfilename(cls
-00010f80: 2c20 2a2a 6f70 7469 6f6e 7329 3a0a 2020  , **options):.  
-00010f90: 2020 2020 2020 6172 6773 203d 2063 6c73        args = cls
-00010fa0: 2e5f 636f 6e76 6572 745f 636f 6d6d 6f6e  ._convert_common
-00010fb0: 5f6f 7074 696f 6e73 2822 5361 7665 2061  _options("Save a
-00010fc0: 7322 2c20 2a2a 6f70 7469 6f6e 7329 0a20  s", **options). 
-00010fd0: 2020 2020 2020 2061 7267 732e 6170 7065         args.appe
-00010fe0: 6e64 2822 2d2d 7361 7665 2229 0a20 2020  nd("--save").   
-00010ff0: 2020 2020 2069 6620 6f70 7469 6f6e 732e       if options.
-00011000: 6765 7428 2263 6f6e 6669 726d 6f76 6572  get("confirmover
-00011010: 7772 6974 6522 2c20 5472 7565 293a 0a20  write", True):. 
-00011020: 2020 2020 2020 2020 2020 2061 7267 732e             args.
-00011030: 6170 7065 6e64 2822 2d2d 636f 6e66 6972  append("--confir
-00011040: 6d2d 6f76 6572 7772 6974 6522 290a 0a20  m-overwrite").. 
-00011050: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
-00011060: 3d20 636c 732e 5f63 616c 6c28 6172 6773  = cls._call(args
-00011070: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00011080: 2066 696c 656e 616d 653a 0a20 2020 2020   filename:.     
-00011090: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000110a0: 6e65 0a0a 2020 2020 2020 2020 7265 7475  ne..        retu
-000110b0: 726e 2066 696c 656e 616d 650a 0a20 2020  rn filename..   
-000110c0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-000110d0: 2020 6465 6620 6173 6b64 6972 6563 746f    def askdirecto
-000110e0: 7279 2863 6c73 2c20 2a2a 6f70 7469 6f6e  ry(cls, **option
-000110f0: 7329 3a0a 2020 2020 2020 2020 6172 6773  s):.        args
-00011100: 203d 2063 6c73 2e5f 636f 6e76 6572 745f   = cls._convert_
-00011110: 636f 6d6d 6f6e 5f6f 7074 696f 6e73 2822  common_options("
-00011120: 5365 6c65 6374 2064 6972 6563 746f 7279  Select directory
-00011130: 222c 202a 2a6f 7074 696f 6e73 290a 2020  ", **options).  
-00011140: 2020 2020 2020 6172 6773 2e61 7070 656e        args.appen
-00011150: 6428 222d 2d64 6972 6563 746f 7279 2229  d("--directory")
-00011160: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011170: 636c 732e 5f63 616c 6c28 6172 6773 290a  cls._call(args).
-00011180: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00011190: 640a 2020 2020 6465 6620 5f63 6f6e 7665  d.    def _conve
-000111a0: 7274 5f63 6f6d 6d6f 6e5f 6f70 7469 6f6e  rt_common_option
-000111b0: 7328 636c 732c 2064 6566 6175 6c74 5f74  s(cls, default_t
-000111c0: 6974 6c65 2c20 2a2a 6f70 7469 6f6e 7329  itle, **options)
-000111d0: 3a0a 2020 2020 2020 2020 6172 6773 203d  :.        args =
-000111e0: 205b 222d 2d66 696c 652d 7365 6c65 6374   ["--file-select
-000111f0: 696f 6e22 2c20 222d 2d74 6974 6c65 3d25  ion", "--title=%
-00011200: 7322 2025 206f 7074 696f 6e73 2e67 6574  s" % options.get
-00011210: 2822 7469 746c 6522 2c20 6465 6661 756c  ("title", defaul
-00011220: 745f 7469 746c 6529 5d0a 0a20 2020 2020  t_title)]..     
-00011230: 2020 2066 696c 656e 616d 6520 3d20 5f6f     filename = _o
-00011240: 7074 696f 6e73 5f74 6f5f 7a65 6e69 7479  ptions_to_zenity
-00011250: 5f66 696c 656e 616d 6528 6f70 7469 6f6e  _filename(option
-00011260: 7329 0a20 2020 2020 2020 2069 6620 6669  s).        if fi
-00011270: 6c65 6e61 6d65 3a0a 2020 2020 2020 2020  lename:.        
-00011280: 2020 2020 6172 6773 2e61 7070 656e 6428      args.append(
-00011290: 222d 2d66 696c 656e 616d 653d 2573 2220  "--filename=%s" 
-000112a0: 2520 6669 6c65 6e61 6d65 290a 0a20 2020  % filename)..   
-000112b0: 2020 2020 2070 6172 656e 7420 3d20 6f70       parent = op
-000112c0: 7469 6f6e 732e 6765 7428 2270 6172 656e  tions.get("paren
-000112d0: 7422 2c20 6f70 7469 6f6e 732e 6765 7428  t", options.get(
-000112e0: 226d 6173 7465 7222 2c20 4e6f 6e65 2929  "master", None))
-000112f0: 0a20 2020 2020 2020 2069 6620 7061 7265  .        if pare
-00011300: 6e74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nt is not None:.
-00011310: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00011320: 2e61 7070 656e 6428 222d 2d6d 6f64 616c  .append("--modal
-00011330: 2229 0a20 2020 2020 2020 2020 2020 2061  ").            a
-00011340: 7267 732e 6170 7065 6e64 2822 2d2d 6174  rgs.append("--at
-00011350: 7461 6368 3d25 7322 2025 2068 6578 2870  tach=%s" % hex(p
-00011360: 6172 656e 742e 7769 6e66 6f5f 6964 2829  arent.winfo_id()
-00011370: 2929 0a0a 2020 2020 2020 2020 666f 7220  ))..        for 
-00011380: 6465 7363 2c20 7061 7474 6572 6e20 696e  desc, pattern in
-00011390: 206f 7074 696f 6e73 2e67 6574 2822 6669   options.get("fi
-000113a0: 6c65 7479 7065 7322 2c20 2829 293a 0a20  letypes", ()):. 
-000113b0: 2020 2020 2020 2020 2020 2023 207a 656e             # zen
-000113c0: 6974 7920 7265 7175 6972 6573 2073 7461  ity requires sta
-000113d0: 7220 6265 666f 7265 2065 7874 656e 7369  r before extensi
-000113e0: 6f6e 0a20 2020 2020 2020 2020 2020 2070  on.            p
-000113f0: 6174 7465 726e 203d 2070 6174 7465 726e  attern = pattern
-00011400: 2e72 6570 6c61 6365 2822 202e 222c 2022  .replace(" .", "
-00011410: 202a 2e22 290a 2020 2020 2020 2020 2020   *.").          
-00011420: 2020 6966 2070 6174 7465 726e 2e73 7461    if pattern.sta
-00011430: 7274 7377 6974 6828 222e 2229 3a0a 2020  rtswith("."):.  
-00011440: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00011450: 7474 6572 6e20 3d20 222a 2220 2b20 7061  ttern = "*" + pa
-00011460: 7474 6572 6e0a 0a20 2020 2020 2020 2020  ttern..         
-00011470: 2020 2069 6620 7061 7474 6572 6e20 3d3d     if pattern ==
-00011480: 2022 2a2e 2a22 3a0a 2020 2020 2020 2020   "*.*":.        
-00011490: 2020 2020 2020 2020 2320 222e 2a22 2077          # ".*" w
-000114a0: 6173 2070 726f 7669 6465 6420 746f 206d  as provided to m
-000114b0: 616b 6520 7468 6520 7061 7474 6572 6e20  ake the pattern 
-000114c0: 7361 6665 2066 6f72 2054 6b20 6469 616c  safe for Tk dial
-000114d0: 6f67 0a20 2020 2020 2020 2020 2020 2020  og.             
-000114e0: 2020 2023 206e 6f74 2072 6571 7569 7265     # not require
-000114f0: 6420 7769 7468 205a 656e 6974 790a 2020  d with Zenity.  
-00011500: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00011510: 7474 6572 6e20 3d20 222a 220a 0a20 2020  ttern = "*"..   
-00011520: 2020 2020 2020 2020 2061 7267 732e 6170           args.ap
-00011530: 7065 6e64 2822 2d2d 6669 6c65 2d66 696c  pend("--file-fil
-00011540: 7465 723d 2573 207c 2025 7322 2025 2028  ter=%s | %s" % (
-00011550: 6465 7363 2c20 7061 7474 6572 6e29 290a  desc, pattern)).
-00011560: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011570: 6172 6773 0a0a 2020 2020 4063 6c61 7373  args..    @class
-00011580: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
-00011590: 6361 6c6c 2863 6c73 2c20 6172 6773 293a  call(cls, args):
-000115a0: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
-000115b0: 5b22 7a65 6e69 7479 222c 2022 2d2d 6e61  ["zenity", "--na
-000115c0: 6d65 3d54 686f 6e6e 7922 2c20 222d 2d63  me=Thonny", "--c
-000115d0: 6c61 7373 3d54 686f 6e6e 7922 5d20 2b20  lass=Thonny"] + 
-000115e0: 6172 6773 0a20 2020 2020 2020 2072 6573  args.        res
-000115f0: 756c 7420 3d20 7375 6270 726f 6365 7373  ult = subprocess
-00011600: 2e72 756e 280a 2020 2020 2020 2020 2020  .run(.          
-00011610: 2020 6172 6773 2c20 7374 646f 7574 3d73    args, stdout=s
-00011620: 7562 7072 6f63 6573 732e 5049 5045 2c20  ubprocess.PIPE, 
-00011630: 7374 6465 7272 3d73 7562 7072 6f63 6573  stderr=subproces
-00011640: 732e 5049 5045 2c20 756e 6976 6572 7361  s.PIPE, universa
-00011650: 6c5f 6e65 776c 696e 6573 3d54 7275 650a  l_newlines=True.
-00011660: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011670: 2020 6966 2072 6573 756c 742e 7265 7475    if result.retu
-00011680: 726e 636f 6465 203d 3d20 303a 0a20 2020  rncode == 0:.   
-00011690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000116a0: 7265 7375 6c74 2e73 7464 6f75 742e 7374  result.stdout.st
-000116b0: 7269 7028 290a 2020 2020 2020 2020 656c  rip().        el
-000116c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000116d0: 6c6f 6767 6572 2e77 6172 6e69 6e67 280a  logger.warning(.
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116f0: 225a 656e 6974 7920 7265 7475 726e 6564  "Zenity returned
-00011700: 2063 6f64 6520 2572 2061 6e64 2073 7464   code %r and std
-00011710: 6572 7220 2572 222c 2072 6573 756c 742e  err %r", result.
-00011720: 7265 7475 726e 636f 6465 2c20 7265 7375  returncode, resu
-00011730: 6c74 2e73 7464 6572 720a 2020 2020 2020  lt.stderr.      
-00011740: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00011750: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00011760: 0a0a 6465 6620 5f6f 7074 696f 6e73 5f74  ..def _options_t
-00011770: 6f5f 7a65 6e69 7479 5f66 696c 656e 616d  o_zenity_filenam
-00011780: 6528 6f70 7469 6f6e 7329 3a0a 2020 2020  e(options):.    
-00011790: 6966 206f 7074 696f 6e73 2e67 6574 2822  if options.get("
-000117a0: 696e 6974 6961 6c64 6972 2229 3a0a 2020  initialdir"):.  
-000117b0: 2020 2020 2020 6966 206f 7074 696f 6e73        if options
-000117c0: 2e67 6574 2822 696e 6974 6961 6c66 696c  .get("initialfil
-000117d0: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-000117e0: 2072 6574 7572 6e20 6f73 2e70 6174 682e   return os.path.
-000117f0: 6a6f 696e 286f 7074 696f 6e73 5b22 696e  join(options["in
-00011800: 6974 6961 6c64 6972 225d 2c20 6f70 7469  itialdir"], opti
-00011810: 6f6e 735b 2269 6e69 7469 616c 6669 6c65  ons["initialfile
-00011820: 225d 290a 2020 2020 2020 2020 656c 7365  "]).        else
-00011830: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00011840: 7475 726e 206f 7074 696f 6e73 5b22 696e  turn options["in
-00011850: 6974 6961 6c64 6972 225d 202b 206f 732e  itialdir"] + os.
-00011860: 7061 7468 2e73 6570 0a0a 2020 2020 7265  path.sep..    re
-00011870: 7475 726e 204e 6f6e 650a 0a0a 6465 6620  turn None...def 
-00011880: 7265 6769 7374 6572 5f6c 6174 696e 5f73  register_latin_s
-00011890: 686f 7274 6375 7428 0a20 2020 2072 6567  hortcut(.    reg
-000118a0: 6973 7472 792c 2073 6571 7565 6e63 653a  istry, sequence:
-000118b0: 2073 7472 2c20 6861 6e64 6c65 723a 2043   str, handler: C
-000118c0: 616c 6c61 626c 652c 2074 6573 7465 723a  allable, tester:
-000118d0: 204f 7074 696f 6e61 6c5b 4361 6c6c 6162   Optional[Callab
-000118e0: 6c65 5d0a 2920 2d3e 204e 6f6e 653a 0a20  le].) -> None:. 
-000118f0: 2020 2072 6573 203d 2073 6571 7565 6e63     res = sequenc
-00011900: 655f 746f 5f65 7665 6e74 5f73 7461 7465  e_to_event_state
-00011910: 5f61 6e64 5f6b 6579 636f 6465 2873 6571  _and_keycode(seq
-00011920: 7565 6e63 6529 0a20 2020 2069 6620 7265  uence).    if re
-00011930: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00011940: 2020 2020 2020 2069 6620 7265 7320 6e6f         if res no
-00011950: 7420 696e 2072 6567 6973 7472 793a 0a20  t in registry:. 
-00011960: 2020 2020 2020 2020 2020 2072 6567 6973             regis
-00011970: 7472 795b 7265 735d 203d 205b 5d0a 2020  try[res] = [].  
-00011980: 2020 2020 2020 7265 6769 7374 7279 5b72        registry[r
-00011990: 6573 5d2e 6170 7065 6e64 2828 6861 6e64  es].append((hand
-000119a0: 6c65 722c 2074 6573 7465 7229 290a 0a0a  ler, tester))...
-000119b0: 6465 6620 6861 6e64 6c65 5f6d 6973 7472  def handle_mistr
-000119c0: 6561 7465 645f 6c61 7469 6e5f 7368 6f72  eated_latin_shor
-000119d0: 7463 7574 7328 7265 6769 7374 7279 2c20  tcuts(registry, 
-000119e0: 6576 656e 7429 3a0a 2020 2020 2320 7472  event):.    # tr
-000119f0: 6965 7320 746f 2068 616e 646c 6520 4374  ies to handle Ct
-00011a00: 726c 2b4c 6174 696e 4c65 7474 6572 2073  rl+LatinLetter s
-00011a10: 686f 7274 6375 7473 0a20 2020 2023 2067  hortcuts.    # g
-00011a20: 6976 656e 2066 726f 6d20 6e6f 6e2d 4c61  iven from non-La
-00011a30: 7469 6e20 6b65 7962 6f61 7264 730a 2020  tin keyboards.  
-00011a40: 2020 2320 5365 653a 2068 7474 7073 3a2f    # See: https:/
-00011a50: 2f62 6974 6275 636b 6574 2e6f 7267 2f70  /bitbucket.org/p
-00011a60: 6c61 732f 7468 6f6e 6e79 2f69 7373 7565  las/thonny/issue
-00011a70: 732f 3432 322f 6564 6974 2d6b 6579 626f  s/422/edit-keybo
-00011a80: 6172 642d 7368 6f72 7463 7574 732d 6374  ard-shortcuts-ct
-00011a90: 726c 2d63 2d63 7472 6c2d 762d 6574 630a  rl-c-ctrl-v-etc.
-00011aa0: 0a20 2020 2023 206f 6e6c 7920 636f 6e73  .    # only cons
-00011ab0: 6964 6572 2065 7665 6e74 7320 7769 7468  ider events with
-00011ac0: 2043 6f6e 7472 6f6c 2068 656c 640a 2020   Control held.  
-00011ad0: 2020 6966 206e 6f74 2065 7665 6e74 2e73    if not event.s
-00011ae0: 7461 7465 2026 2030 7830 343a 0a20 2020  tate & 0x04:.   
-00011af0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00011b00: 2069 6620 7275 6e6e 696e 675f 6f6e 5f6d   if running_on_m
-00011b10: 6163 5f6f 7328 293a 0a20 2020 2020 2020  ac_os():.       
-00011b20: 2072 6574 7572 6e0a 0a20 2020 2023 2063   return..    # c
-00011b30: 6f6e 7369 6465 7220 6f6e 6c79 2070 6172  onsider only par
-00011b40: 7420 6f66 2074 6865 2073 7461 7465 2c0a  t of the state,.
-00011b50: 2020 2020 2320 6265 6361 7573 6520 6174      # because at
-00011b60: 206c 6561 7374 206f 6e20 5769 6e64 6f77   least on Window
-00011b70: 732c 2043 7472 6c2d 7368 6f72 7463 7574  s, Ctrl-shortcut
-00011b80: 7327 2073 7461 7465 0a20 2020 2023 2068  s' state.    # h
-00011b90: 6173 2073 6f6d 6574 6869 6e67 2065 7874  as something ext
-00011ba0: 7261 0a20 2020 2073 696d 706c 6966 6965  ra.    simplifie
-00011bb0: 645f 7374 6174 6520 3d20 3078 3034 0a20  d_state = 0x04. 
-00011bc0: 2020 2069 6620 7368 6966 745f 6973 5f70     if shift_is_p
-00011bd0: 7265 7373 6564 2865 7665 6e74 293a 0a20  ressed(event):. 
-00011be0: 2020 2020 2020 2073 696d 706c 6966 6965         simplifie
-00011bf0: 645f 7374 6174 6520 7c3d 2030 7830 310a  d_state |= 0x01.
-00011c00: 0a20 2020 2023 2070 7269 6e74 2873 696d  .    # print(sim
-00011c10: 706c 6966 6965 645f 7374 6174 652c 2065  plified_state, e
-00011c20: 7665 6e74 2e6b 6579 636f 6465 290a 2020  vent.keycode).  
-00011c30: 2020 6966 2028 7369 6d70 6c69 6669 6564    if (simplified
-00011c40: 5f73 7461 7465 2c20 6576 656e 742e 6b65  _state, event.ke
-00011c50: 7963 6f64 6529 2069 6e20 7265 6769 7374  ycode) in regist
-00011c60: 7279 3a0a 2020 2020 2020 2020 6966 2065  ry:.        if e
-00011c70: 7665 6e74 2e6b 6579 636f 6465 2021 3d20  vent.keycode != 
-00011c80: 6f72 6428 6576 656e 742e 6368 6172 2920  ord(event.char) 
-00011c90: 616e 6420 6576 656e 742e 6b65 7973 796d  and event.keysym
-00011ca0: 2069 6e20 284e 6f6e 652c 2022 3f3f 2229   in (None, "??")
-00011cb0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00011cc0: 6b65 7963 6f64 6520 616e 6420 6368 6172  keycode and char
-00011cd0: 2064 6f65 736e 2774 206d 6174 6368 2c0a   doesn't match,.
-00011ce0: 2020 2020 2020 2020 2020 2020 2320 7468              # th
-00011cf0: 6973 206d 6561 6e73 206e 6f6e 2d6c 6174  is means non-lat
-00011d00: 696e 206b 6579 626f 6172 640a 2020 2020  in keyboard.    
-00011d10: 2020 2020 2020 2020 666f 7220 6861 6e64          for hand
-00011d20: 6c65 722c 2074 6573 7465 7220 696e 2072  ler, tester in r
-00011d30: 6567 6973 7472 795b 2873 696d 706c 6966  egistry[(simplif
-00011d40: 6965 645f 7374 6174 652c 2065 7665 6e74  ied_state, event
-00011d50: 2e6b 6579 636f 6465 295d 3a0a 2020 2020  .keycode)]:.    
-00011d60: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00011d70: 6573 7465 7220 6973 204e 6f6e 6520 6f72  ester is None or
-00011d80: 2074 6573 7465 7228 293a 0a20 2020 2020   tester():.     
-00011d90: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00011da0: 616e 646c 6572 2829 0a0a 0a64 6566 2073  andler()...def s
-00011db0: 686f 775f 6469 616c 6f67 2864 6c67 2c20  how_dialog(dlg, 
-00011dc0: 6d61 7374 6572 3d4e 6f6e 652c 2077 6964  master=None, wid
-00011dd0: 7468 3d4e 6f6e 652c 2068 6569 6768 743d  th=None, height=
-00011de0: 4e6f 6e65 2c20 6d6f 6461 6c3d 5472 7565  None, modal=True
-00011df0: 293a 0a20 2020 2069 6620 6765 7461 7474  ):.    if getatt
-00011e00: 7228 646c 672c 2022 636c 6f73 6564 222c  r(dlg, "closed",
-00011e10: 2046 616c 7365 293a 0a20 2020 2020 2020   False):.       
-00011e20: 2072 6574 7572 6e0a 0a20 2020 2069 6620   return..    if 
-00011e30: 6d61 7374 6572 2069 7320 4e6f 6e65 3a0a  master is None:.
-00011e40: 2020 2020 2020 2020 6d61 7374 6572 203d          master =
-00011e50: 2067 6574 6174 7472 2864 6c67 2c20 2270   getattr(dlg, "p
-00011e60: 6172 656e 7422 2c20 4e6f 6e65 2920 6f72  arent", None) or
-00011e70: 2067 6574 6174 7472 2864 6c67 2c20 226d   getattr(dlg, "m
-00011e80: 6173 7465 7222 2c20 4e6f 6e65 2920 6f72  aster", None) or
-00011e90: 2074 6b2e 5f64 6566 6175 6c74 5f72 6f6f   tk._default_roo
-00011ea0: 740a 0a20 2020 206d 6173 7465 7220 3d20  t..    master = 
-00011eb0: 6d61 7374 6572 2e77 696e 666f 5f74 6f70  master.winfo_top
-00011ec0: 6c65 7665 6c28 290a 0a20 2020 2067 6574  level()..    get
-00011ed0: 5f77 6f72 6b62 656e 6368 2829 2e65 7665  _workbench().eve
-00011ee0: 6e74 5f67 656e 6572 6174 6528 2257 696e  nt_generate("Win
-00011ef0: 646f 7746 6f63 7573 4f75 7422 290a 2020  dowFocusOut").  
-00011f00: 2020 2320 666f 6c6c 6f77 696e 6720 6f72    # following or
-00011f10: 6465 7220 7365 656d 7320 746f 2067 6976  der seems to giv
-00011f20: 6520 6d6f 7374 2073 6d6f 6f74 6820 6170  e most smooth ap
-00011f30: 7065 6172 616e 6365 0a20 2020 206f 6c64  pearance.    old
-00011f40: 5f66 6f63 7573 6564 5f77 6964 6765 7420  _focused_widget 
-00011f50: 3d20 6d61 7374 6572 2e66 6f63 7573 5f67  = master.focus_g
-00011f60: 6574 2829 0a20 2020 2069 6620 6d61 7374  et().    if mast
-00011f70: 6572 2e77 696e 666f 5f74 6f70 6c65 7665  er.winfo_topleve
-00011f80: 6c28 292e 7769 6e66 6f5f 7669 6577 6162  l().winfo_viewab
-00011f90: 6c65 2829 3a0a 2020 2020 2020 2020 646c  le():.        dl
-00011fa0: 672e 7472 616e 7369 656e 7428 6d61 7374  g.transient(mast
-00011fb0: 6572 2e77 696e 666f 5f74 6f70 6c65 7665  er.winfo_topleve
-00011fc0: 6c28 2929 0a0a 2020 2020 7361 7665 645f  l())..    saved_
-00011fd0: 7369 7a65 203d 2067 6574 5f77 6f72 6b62  size = get_workb
-00011fe0: 656e 6368 2829 2e67 6574 5f6f 7074 696f  ench().get_optio
-00011ff0: 6e28 6765 745f 7369 7a65 5f6f 7074 696f  n(get_size_optio
-00012000: 6e5f 6e61 6d65 2864 6c67 2929 0a20 2020  n_name(dlg)).   
-00012010: 2069 6620 7361 7665 645f 7369 7a65 3a0a   if saved_size:.
-00012020: 2020 2020 2020 2020 7769 6474 6820 3d20          width = 
-00012030: 6d69 6e28 6d61 7828 7361 7665 645f 7369  min(max(saved_si
-00012040: 7a65 5b30 5d2c 2065 6d73 5f74 6f5f 7069  ze[0], ems_to_pi
-00012050: 7865 6c73 2831 3029 292c 2065 6d73 5f74  xels(10)), ems_t
-00012060: 6f5f 7069 7865 6c73 2835 3030 2929 0a20  o_pixels(500)). 
-00012070: 2020 2020 2020 2068 6569 6768 7420 3d20         height = 
-00012080: 6d69 6e28 6d61 7828 7361 7665 645f 7369  min(max(saved_si
-00012090: 7a65 5b31 5d2c 2065 6d73 5f74 6f5f 7069  ze[1], ems_to_pi
-000120a0: 7865 6c73 2838 2929 2c20 656d 735f 746f  xels(8)), ems_to
-000120b0: 5f70 6978 656c 7328 3330 3029 290a 0a20  _pixels(300)).. 
-000120c0: 2020 205f 706c 6163 655f 7769 6e64 6f77     _place_window
-000120d0: 2864 6c67 2c20 6d61 7374 6572 2c20 7769  (dlg, master, wi
-000120e0: 6474 683d 7769 6474 682c 2068 6569 6768  dth=width, heigh
-000120f0: 743d 6865 6967 6874 290a 0a20 2020 2064  t=height)..    d
-00012100: 6c67 2e6c 6966 7428 290a 2020 2020 646c  lg.lift().    dl
-00012110: 672e 7761 6974 5f76 6973 6962 696c 6974  g.wait_visibilit
-00012120: 7928 290a 0a20 2020 2069 6620 6d6f 6461  y()..    if moda
-00012130: 6c3a 0a20 2020 2020 2020 2074 7279 3a0a  l:.        try:.
-00012140: 2020 2020 2020 2020 2020 2020 646c 672e              dlg.
-00012150: 6772 6162 5f73 6574 2829 0a20 2020 2020  grab_set().     
-00012160: 2020 2065 7863 6570 7420 5463 6c45 7272     except TclErr
-00012170: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-00012180: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-00012190: 696e 6728 2243 616e 2774 2067 7261 623a  ing("Can't grab:
-000121a0: 2025 7322 2c20 6529 0a0a 2020 2020 646c   %s", e)..    dl
-000121b0: 672e 7570 6461 7465 5f69 646c 6574 6173  g.update_idletas
-000121c0: 6b73 2829 0a20 2020 2064 6c67 2e66 6f63  ks().    dlg.foc
-000121d0: 7573 5f73 6574 2829 0a20 2020 2069 6620  us_set().    if 
-000121e0: 6861 7361 7474 7228 646c 672c 2022 7365  hasattr(dlg, "se
-000121f0: 745f 696e 6974 6961 6c5f 666f 6375 7322  t_initial_focus"
-00012200: 293a 0a20 2020 2020 2020 2064 6c67 2e73  ):.        dlg.s
-00012210: 6574 5f69 6e69 7469 616c 5f66 6f63 7573  et_initial_focus
-00012220: 2829 0a0a 2020 2020 646c 672e 7761 6974  ()..    dlg.wait
-00012230: 5f77 696e 646f 7728 646c 6729 0a20 2020  _window(dlg).   
-00012240: 2064 6c67 2e67 7261 625f 7265 6c65 6173   dlg.grab_releas
-00012250: 6528 290a 2020 2020 6d61 7374 6572 2e77  e().    master.w
-00012260: 696e 666f 5f74 6f70 6c65 7665 6c28 292e  info_toplevel().
-00012270: 6c69 6674 2829 0a20 2020 206d 6173 7465  lift().    maste
-00012280: 722e 7769 6e66 6f5f 746f 706c 6576 656c  r.winfo_toplevel
-00012290: 2829 2e66 6f63 7573 5f66 6f72 6365 2829  ().focus_force()
-000122a0: 0a20 2020 206d 6173 7465 722e 7769 6e66  .    master.winf
-000122b0: 6f5f 746f 706c 6576 656c 2829 2e67 7261  o_toplevel().gra
-000122c0: 625f 7365 7428 290a 2020 2020 6966 2072  b_set().    if r
-000122d0: 756e 6e69 6e67 5f6f 6e5f 6d61 635f 6f73  unning_on_mac_os
-000122e0: 2829 3a0a 2020 2020 2020 2020 6d61 7374  ():.        mast
-000122f0: 6572 2e77 696e 666f 5f74 6f70 6c65 7665  er.winfo_topleve
-00012300: 6c28 292e 6772 6162 5f72 656c 6561 7365  l().grab_release
-00012310: 2829 0a0a 2020 2020 6966 206f 6c64 5f66  ()..    if old_f
-00012320: 6f63 7573 6564 5f77 6964 6765 7420 6973  ocused_widget is
-00012330: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00012340: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00012350: 2020 2020 6f6c 645f 666f 6375 7365 645f      old_focused_
-00012360: 7769 6467 6574 2e66 6f63 7573 5f66 6f72  widget.focus_for
-00012370: 6365 2829 0a20 2020 2020 2020 2065 7863  ce().        exc
-00012380: 6570 7420 5463 6c45 7272 6f72 3a0a 2020  ept TclError:.  
-00012390: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
-000123a0: 0a64 6566 2070 6f70 656e 5f77 6974 685f  .def popen_with_
-000123b0: 7569 5f74 6872 6561 645f 6361 6c6c 6261  ui_thread_callba
-000123c0: 636b 282a 506f 7065 6e5f 6172 6773 2c20  ck(*Popen_args, 
-000123d0: 6f6e 5f63 6f6d 706c 6574 696f 6e2c 2070  on_completion, p
-000123e0: 6f6c 6c5f 6465 6c61 793d 302e 312c 202a  oll_delay=0.1, *
-000123f0: 2a50 6f70 656e 5f6b 7761 7267 7329 3a0a  *Popen_kwargs):.
-00012400: 2020 2020 6966 2022 656e 636f 6469 6e67      if "encoding
-00012410: 2220 6e6f 7420 696e 2050 6f70 656e 5f6b  " not in Popen_k
-00012420: 7761 7267 733a 0a20 2020 2020 2020 2069  wargs:.        i
-00012430: 6620 2265 6e76 2220 6e6f 7420 696e 2050  f "env" not in P
-00012440: 6f70 656e 5f6b 7761 7267 733a 0a20 2020  open_kwargs:.   
-00012450: 2020 2020 2020 2020 2050 6f70 656e 5f6b           Popen_k
-00012460: 7761 7267 735b 2265 6e76 225d 203d 206f  wargs["env"] = o
-00012470: 732e 656e 7669 726f 6e2e 636f 7079 2829  s.environ.copy()
-00012480: 0a20 2020 2020 2020 2050 6f70 656e 5f6b  .        Popen_k
-00012490: 7761 7267 735b 2265 6e76 225d 5b22 5059  wargs["env"]["PY
-000124a0: 5448 4f4e 494f 454e 434f 4449 4e47 225d  THONIOENCODING"]
-000124b0: 203d 2022 7574 662d 3822 0a20 2020 2020   = "utf-8".     
-000124c0: 2020 2069 6620 7379 732e 7665 7273 696f     if sys.versio
-000124d0: 6e5f 696e 666f 203e 3d20 2833 2c20 3629  n_info >= (3, 6)
-000124e0: 3a0a 2020 2020 2020 2020 2020 2020 506f  :.            Po
-000124f0: 7065 6e5f 6b77 6172 6773 5b22 656e 636f  pen_kwargs["enco
-00012500: 6469 6e67 225d 203d 2022 7574 662d 3822  ding"] = "utf-8"
-00012510: 0a0a 2020 2020 7072 6f63 203d 2073 7562  ..    proc = sub
-00012520: 7072 6f63 6573 732e 506f 7065 6e28 2a50  process.Popen(*P
-00012530: 6f70 656e 5f61 7267 732c 202a 2a50 6f70  open_args, **Pop
-00012540: 656e 5f6b 7761 7267 7329 0a0a 2020 2020  en_kwargs)..    
-00012550: 2320 4e65 6564 2074 6f20 7265 6164 2069  # Need to read i
-00012560: 6e20 7468 7265 6164 2069 6e20 6f72 6465  n thread in orde
-00012570: 7220 746f 2061 766f 6964 2062 6c6f 636b  r to avoid block
-00012580: 696e 6720 6265 6361 7573 650a 2020 2020  ing because.    
-00012590: 2320 6f66 2066 756c 6c20 7069 7065 2062  # of full pipe b
-000125a0: 7566 6665 7220 2873 6565 2068 7474 7073  uffer (see https
-000125b0: 3a2f 2f62 7567 732e 7079 7468 6f6e 2e6f  ://bugs.python.o
-000125c0: 7267 2f69 7373 7565 3132 3536 290a 2020  rg/issue1256).  
-000125d0: 2020 6f75 745f 6c69 6e65 7320 3d20 5b5d    out_lines = []
-000125e0: 0a20 2020 2065 7272 5f6c 696e 6573 203d  .    err_lines =
-000125f0: 205b 5d0a 0a20 2020 2064 6566 2072 6561   []..    def rea
-00012600: 645f 7374 7265 616d 2873 7472 6561 6d2c  d_stream(stream,
-00012610: 2074 6172 6765 745f 6c69 7374 293a 0a20   target_list):. 
-00012620: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-00012630: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-00012640: 696e 6520 3d20 7374 7265 616d 2e72 6561  ine = stream.rea
-00012650: 646c 696e 6528 290a 2020 2020 2020 2020  dline().        
-00012660: 2020 2020 6966 206c 696e 653a 0a20 2020      if line:.   
-00012670: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00012680: 6765 745f 6c69 7374 2e61 7070 656e 6428  get_list.append(
-00012690: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
-000126a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000126b0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-000126c0: 2020 2074 5f6f 7574 203d 2074 6872 6561     t_out = threa
-000126d0: 6469 6e67 2e54 6872 6561 6428 7461 7267  ding.Thread(targ
-000126e0: 6574 3d72 6561 645f 7374 7265 616d 2c20  et=read_stream, 
-000126f0: 6461 656d 6f6e 3d54 7275 652c 2061 7267  daemon=True, arg
-00012700: 733d 2870 726f 632e 7374 646f 7574 2c20  s=(proc.stdout, 
-00012710: 6f75 745f 6c69 6e65 7329 290a 2020 2020  out_lines)).    
-00012720: 745f 6572 7220 3d20 7468 7265 6164 696e  t_err = threadin
-00012730: 672e 5468 7265 6164 2874 6172 6765 743d  g.Thread(target=
-00012740: 7265 6164 5f73 7472 6561 6d2c 2064 6165  read_stream, dae
-00012750: 6d6f 6e3d 5472 7565 2c20 6172 6773 3d28  mon=True, args=(
-00012760: 7072 6f63 2e73 7464 6572 722c 2065 7272  proc.stderr, err
-00012770: 5f6c 696e 6573 2929 0a20 2020 2074 5f6f  _lines)).    t_o
-00012780: 7574 2e73 7461 7274 2829 0a20 2020 2074  ut.start().    t
-00012790: 5f65 7272 2e73 7461 7274 2829 0a0a 2020  _err.start()..  
-000127a0: 2020 6465 6620 706f 6c6c 2829 3a0a 2020    def poll():.  
-000127b0: 2020 2020 2020 6966 2070 726f 632e 706f        if proc.po
-000127c0: 6c6c 2829 2069 7320 6e6f 7420 4e6f 6e65  ll() is not None
-000127d0: 3a0a 2020 2020 2020 2020 2020 2020 745f  :.            t_
-000127e0: 6f75 742e 6a6f 696e 2833 290a 2020 2020  out.join(3).    
-000127f0: 2020 2020 2020 2020 745f 6572 722e 6a6f          t_err.jo
-00012800: 696e 2833 290a 2020 2020 2020 2020 2020  in(3).          
-00012810: 2020 6f6e 5f63 6f6d 706c 6574 696f 6e28    on_completion(
-00012820: 7072 6f63 2c20 6f75 745f 6c69 6e65 732c  proc, out_lines,
-00012830: 2065 7272 5f6c 696e 6573 290a 2020 2020   err_lines).    
-00012840: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00012850: 2020 2020 2020 2020 746b 2e5f 6465 6661          tk._defa
-00012860: 756c 745f 726f 6f74 2e61 6674 6572 2869  ult_root.after(i
-00012870: 6e74 2870 6f6c 6c5f 6465 6c61 7920 2a20  nt(poll_delay * 
-00012880: 3130 3030 292c 2070 6f6c 6c29 0a0a 2020  1000), poll)..  
-00012890: 2020 706f 6c6c 2829 0a20 2020 2072 6574    poll().    ret
-000128a0: 7572 6e20 7072 6f63 0a0a 0a63 6c61 7373  urn proc...class
-000128b0: 204d 656e 7545 7828 746b 2e4d 656e 7529   MenuEx(tk.Menu)
-000128c0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000128d0: 5f5f 2873 656c 662c 2074 6172 6765 7429  __(self, target)
-000128e0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-000128f0: 7465 7374 6572 7320 3d20 7b7d 0a20 2020  testers = {}.   
-00012900: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00012910: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-00012920: 2020 2074 6172 6765 742c 2074 6561 726f     target, tearo
-00012930: 6666 3d46 616c 7365 2c20 706f 7374 636f  ff=False, postco
-00012940: 6d6d 616e 643d 7365 6c66 2e6f 6e5f 706f  mmand=self.on_po
-00012950: 7374 2c20 2a2a 6765 745f 7374 796c 655f  st, **get_style_
-00012960: 636f 6e66 6967 7572 6174 696f 6e28 224d  configuration("M
-00012970: 656e 7522 290a 2020 2020 2020 2020 290a  enu").        ).
-00012980: 0a20 2020 2064 6566 206f 6e5f 706f 7374  .    def on_post
-00012990: 2873 656c 662c 202a 6172 6773 293a 0a20  (self, *args):. 
-000129a0: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-000129b0: 7465 5f69 7465 6d5f 6176 6169 6c61 6269  te_item_availabi
-000129c0: 6c69 7479 2829 0a0a 2020 2020 6465 6620  lity()..    def 
-000129d0: 7570 6461 7465 5f69 7465 6d5f 6176 6169  update_item_avai
-000129e0: 6c61 6269 6c69 7479 2873 656c 6629 3a0a  lability(self):.
-000129f0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00012a00: 2072 616e 6765 2873 656c 662e 696e 6465   range(self.inde
-00012a10: 7828 2265 6e64 2229 202b 2031 293a 0a20  x("end") + 1):. 
-00012a20: 2020 2020 2020 2020 2020 2069 7465 6d5f             item_
-00012a30: 6461 7461 203d 2073 656c 662e 656e 7472  data = self.entr
-00012a40: 7963 6f6e 6669 6775 7265 2869 290a 2020  yconfigure(i).  
-00012a50: 2020 2020 2020 2020 2020 6966 2022 6c61            if "la
-00012a60: 6265 6c22 2069 6e20 6974 656d 5f64 6174  bel" in item_dat
-00012a70: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-00012a80: 2020 2074 6573 7465 7220 3d20 7365 6c66     tester = self
-00012a90: 2e5f 7465 7374 6572 732e 6765 7428 6974  ._testers.get(it
-00012aa0: 656d 5f64 6174 615b 226c 6162 656c 225d  em_data["label"]
-00012ab0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012ac0: 2020 6966 2074 6573 7465 7220 616e 6420    if tester and 
-00012ad0: 6e6f 7420 7465 7374 6572 2829 3a0a 2020  not tester():.  
+0000e8f0: 2020 2020 2020 6f73 2e66 7379 6e63 2866        os.fsync(f
+0000e900: 6473 7429 0a20 2020 2020 2020 2020 2020  dst).           
+0000e910: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e920: 662e 5f62 7974 6573 5f63 6f70 6965 6420  f._bytes_copied 
+0000e930: 2b3d 206c 656e 2862 7566 290a 0a20 2020  += len(buf)..   
+0000e940: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
+0000e950: 6f6e 6520 3d20 5472 7565 0a0a 2020 2020  one = True..    
+0000e960: 2020 2020 7468 7265 6164 696e 672e 5468      threading.Th
+0000e970: 7265 6164 2874 6172 6765 743d 776f 726b  read(target=work
+0000e980: 2c20 6461 656d 6f6e 3d54 7275 6529 2e73  , daemon=True).s
+0000e990: 7461 7274 2829 0a0a 2020 2020 6465 6620  tart()..    def 
+0000e9a0: 5f75 7064 6174 655f 7072 6f67 7265 7373  _update_progress
+0000e9b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e9c0: 6966 2073 656c 662e 5f64 6f6e 653a 0a20  if self._done:. 
+0000e9d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000e9e0: 7420 7365 6c66 2e5f 636c 6f73 6564 3a0a  t self._closed:.
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea00: 7365 6c66 2e5f 636c 6f73 6528 290a 2020  self._close().  
+0000ea10: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ea20: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0000ea30: 6261 722e 7374 6570 2873 656c 662e 5f62  bar.step(self._b
+0000ea40: 7974 6573 5f63 6f70 6965 6420 2d20 7365  ytes_copied - se
+0000ea50: 6c66 2e5f 6f6c 645f 6279 7465 735f 636f  lf._old_bytes_co
+0000ea60: 7069 6564 290a 2020 2020 2020 2020 7365  pied).        se
+0000ea70: 6c66 2e5f 6f6c 645f 6279 7465 735f 636f  lf._old_bytes_co
+0000ea80: 7069 6564 203d 2073 656c 662e 5f62 7974  pied = self._byt
+0000ea90: 6573 5f63 6f70 6965 640a 0a20 2020 2020  es_copied..     
+0000eaa0: 2020 2073 656c 662e 6166 7465 7228 3130     self.after(10
+0000eab0: 302c 2073 656c 662e 5f75 7064 6174 655f  0, self._update_
+0000eac0: 7072 6f67 7265 7373 290a 0a20 2020 2064  progress)..    d
+0000ead0: 6566 205f 636c 6f73 6528 7365 6c66 293a  ef _close(self):
+0000eae0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
+0000eaf0: 7374 726f 7928 290a 2020 2020 2020 2020  stroy().        
+0000eb00: 7365 6c66 2e5f 636c 6f73 6564 203d 2054  self._closed = T
+0000eb10: 7275 650a 0a20 2020 2064 6566 205f 6361  rue..    def _ca
+0000eb20: 6e63 656c 2873 656c 662c 2065 7665 6e74  ncel(self, event
+0000eb30: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000eb40: 7365 6c66 2e5f 6361 6e63 656c 6c65 6420  self._cancelled 
+0000eb50: 3d20 5472 7565 0a20 2020 2020 2020 2073  = True.        s
+0000eb60: 656c 662e 5f63 6c6f 7365 2829 0a0a 0a63  elf._close()...c
+0000eb70: 6c61 7373 2043 686f 6963 6544 6961 6c6f  lass ChoiceDialo
+0000eb80: 6728 436f 6d6d 6f6e 4469 616c 6f67 4578  g(CommonDialogEx
+0000eb90: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0000eba0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0000ebb0: 662c 0a20 2020 2020 2020 206d 6173 7465  f,.        maste
+0000ebc0: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
+0000ebd0: 7469 746c 653d 2243 686f 6f73 6520 6f6e  title="Choose on
+0000ebe0: 6522 2c0a 2020 2020 2020 2020 7175 6573  e",.        ques
+0000ebf0: 7469 6f6e 3a20 7374 7220 3d20 2243 686f  tion: str = "Cho
+0000ec00: 6f73 6520 6f6e 653a 222c 0a20 2020 2020  ose one:",.     
+0000ec10: 2020 2063 686f 6963 6573 3d5b 5d2c 0a20     choices=[],. 
+0000ec20: 2020 2020 2020 2069 6e69 7469 616c 5f63         initial_c
+0000ec30: 686f 6963 655f 696e 6465 783d 4e6f 6e65  hoice_index=None
+0000ec40: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+0000ec50: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0000ec60: 7375 6c74 203d 204e 6f6e 650a 2020 2020  sult = None.    
+0000ec70: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0000ec80: 6974 5f5f 286d 6173 7465 723d 6d61 7374  it__(master=mast
+0000ec90: 6572 290a 0a20 2020 2020 2020 2073 656c  er)..        sel
+0000eca0: 662e 7469 746c 6528 7469 746c 6529 0a20  f.title(title). 
+0000ecb0: 2020 2020 2020 2073 656c 662e 7265 7369         self.resi
+0000ecc0: 7a61 626c 6528 4661 6c73 652c 2046 616c  zable(False, Fal
+0000ecd0: 7365 290a 0a20 2020 2020 2020 2073 656c  se)..        sel
+0000ece0: 662e 6d61 696e 5f66 7261 6d65 2e63 6f6c  f.main_frame.col
+0000ecf0: 756d 6e63 6f6e 6669 6775 7265 2830 2c20  umnconfigure(0, 
+0000ed00: 7765 6967 6874 3d31 290a 0a20 2020 2020  weight=1)..     
+0000ed10: 2020 2072 6f77 203d 2030 0a20 2020 2020     row = 0.     
+0000ed20: 2020 2071 7565 7374 696f 6e5f 6c61 6265     question_labe
+0000ed30: 6c20 3d20 7474 6b2e 4c61 6265 6c28 7365  l = ttk.Label(se
+0000ed40: 6c66 2e6d 6169 6e5f 6672 616d 652c 2074  lf.main_frame, t
+0000ed50: 6578 743d 7175 6573 7469 6f6e 290a 2020  ext=question).  
+0000ed60: 2020 2020 2020 7175 6573 7469 6f6e 5f6c        question_l
+0000ed70: 6162 656c 2e67 7269 6428 726f 773d 726f  abel.grid(row=ro
+0000ed80: 772c 2063 6f6c 756d 6e3d 302c 2063 6f6c  w, column=0, col
+0000ed90: 756d 6e73 7061 6e3d 322c 2073 7469 636b  umnspan=2, stick
+0000eda0: 793d 2277 222c 2070 6164 783d 3230 2c20  y="w", padx=20, 
+0000edb0: 7061 6479 3d32 3029 0a20 2020 2020 2020  pady=20).       
+0000edc0: 2072 6f77 202b 3d20 310a 0a20 2020 2020   row += 1..     
+0000edd0: 2020 2073 656c 662e 7661 7220 3d20 746b     self.var = tk
+0000ede0: 2e53 7472 696e 6756 6172 2876 616c 7565  .StringVar(value
+0000edf0: 3d22 2229 0a20 2020 2020 2020 2069 6620  ="").        if 
+0000ee00: 696e 6974 6961 6c5f 6368 6f69 6365 5f69  initial_choice_i
+0000ee10: 6e64 6578 2069 7320 6e6f 7420 4e6f 6e65  ndex is not None
+0000ee20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000ee30: 6c66 2e76 6172 2e73 6574 2863 686f 6963  lf.var.set(choic
+0000ee40: 6573 5b69 6e69 7469 616c 5f63 686f 6963  es[initial_choic
+0000ee50: 655f 696e 6465 785d 290a 2020 2020 2020  e_index]).      
+0000ee60: 2020 666f 7220 6368 6f69 6365 2069 6e20    for choice in 
+0000ee70: 6368 6f69 6365 733a 0a20 2020 2020 2020  choices:.       
+0000ee80: 2020 2020 2072 6220 3d20 7474 6b2e 5261       rb = ttk.Ra
+0000ee90: 6469 6f62 7574 746f 6e28 7365 6c66 2e6d  diobutton(self.m
+0000eea0: 6169 6e5f 6672 616d 652c 2074 6578 743d  ain_frame, text=
+0000eeb0: 6368 6f69 6365 2c20 7661 7269 6162 6c65  choice, variable
+0000eec0: 3d73 656c 662e 7661 722c 2076 616c 7565  =self.var, value
+0000eed0: 3d63 686f 6963 6529 0a20 2020 2020 2020  =choice).       
+0000eee0: 2020 2020 2072 622e 6772 6964 2872 6f77       rb.grid(row
+0000eef0: 3d72 6f77 2c20 636f 6c75 6d6e 3d30 2c20  =row, column=0, 
+0000ef00: 636f 6c75 6d6e 7370 616e 3d32 2c20 7374  columnspan=2, st
+0000ef10: 6963 6b79 3d22 7722 2c20 7061 6478 3d32  icky="w", padx=2
+0000ef20: 3029 0a20 2020 2020 2020 2020 2020 2072  0).            r
+0000ef30: 6f77 202b 3d20 310a 0a20 2020 2020 2020  ow += 1..       
+0000ef40: 206f 6b5f 6275 7474 6f6e 203d 2074 746b   ok_button = ttk
+0000ef50: 2e42 7574 746f 6e28 7365 6c66 2e6d 6169  .Button(self.mai
+0000ef60: 6e5f 6672 616d 652c 2074 6578 743d 7472  n_frame, text=tr
+0000ef70: 2822 4f4b 2229 2c20 636f 6d6d 616e 643d  ("OK"), command=
+0000ef80: 7365 6c66 2e5f 6f6b 2c20 6465 6661 756c  self._ok, defaul
+0000ef90: 743d 2261 6374 6976 6522 290a 2020 2020  t="active").    
+0000efa0: 2020 2020 6f6b 5f62 7574 746f 6e2e 6772      ok_button.gr
+0000efb0: 6964 2872 6f77 3d72 6f77 2c20 636f 6c75  id(row=row, colu
+0000efc0: 6d6e 3d30 2c20 7374 6963 6b79 3d22 6522  mn=0, sticky="e"
+0000efd0: 2c20 7061 6479 3d32 3029 0a0a 2020 2020  , pady=20)..    
+0000efe0: 2020 2020 6361 6e63 656c 5f62 7574 746f      cancel_butto
+0000eff0: 6e20 3d20 7474 6b2e 4275 7474 6f6e 2873  n = ttk.Button(s
+0000f000: 656c 662e 6d61 696e 5f66 7261 6d65 2c20  elf.main_frame, 
+0000f010: 7465 7874 3d74 7228 2243 616e 6365 6c22  text=tr("Cancel"
+0000f020: 292c 2063 6f6d 6d61 6e64 3d73 656c 662e  ), command=self.
+0000f030: 5f63 616e 6365 6c29 0a20 2020 2020 2020  _cancel).       
+0000f040: 2063 616e 6365 6c5f 6275 7474 6f6e 2e67   cancel_button.g
+0000f050: 7269 6428 726f 773d 726f 772c 2063 6f6c  rid(row=row, col
+0000f060: 756d 6e3d 312c 2073 7469 636b 793d 2265  umn=1, sticky="e
+0000f070: 222c 2070 6164 783d 3230 2c20 7061 6479  ", padx=20, pady
+0000f080: 3d32 3029 0a0a 2020 2020 2020 2020 7365  =20)..        se
+0000f090: 6c66 2e62 696e 6428 223c 4573 6361 7065  lf.bind("<Escape
+0000f0a0: 3e22 2c20 7365 6c66 2e5f 6361 6e63 656c  >", self._cancel
+0000f0b0: 2c20 5472 7565 290a 2020 2020 2020 2020  , True).        
+0000f0c0: 7365 6c66 2e62 696e 6428 223c 5265 7475  self.bind("<Retu
+0000f0d0: 726e 3e22 2c20 7365 6c66 2e5f 6f6b 2c20  rn>", self._ok, 
+0000f0e0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+0000f0f0: 6c66 2e70 726f 746f 636f 6c28 2257 4d5f  lf.protocol("WM_
+0000f100: 4445 4c45 5445 5f57 494e 444f 5722 2c20  DELETE_WINDOW", 
+0000f110: 7365 6c66 2e5f 6361 6e63 656c 290a 0a20  self._cancel).. 
+0000f120: 2020 2064 6566 205f 6f6b 2873 656c 6629     def _ok(self)
+0000f130: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
+0000f140: 6573 756c 7420 3d20 7365 6c66 2e76 6172  esult = self.var
+0000f150: 2e67 6574 2829 0a20 2020 2020 2020 2069  .get().        i
+0000f160: 6620 6e6f 7420 7365 6c66 2e72 6573 756c  f not self.resul
+0000f170: 743a 0a20 2020 2020 2020 2020 2020 2073  t:.            s
+0000f180: 656c 662e 7265 7375 6c74 203d 204e 6f6e  elf.result = Non
+0000f190: 650a 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+0000f1a0: 6465 7374 726f 7928 290a 0a20 2020 2064  destroy()..    d
+0000f1b0: 6566 205f 6361 6e63 656c 2873 656c 6629  ef _cancel(self)
+0000f1c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
+0000f1d0: 6573 756c 7420 3d20 4e6f 6e65 0a20 2020  esult = None.   
+0000f1e0: 2020 2020 2073 656c 662e 6465 7374 726f       self.destro
+0000f1f0: 7928 290a 0a0a 636c 6173 7320 4c6f 6e67  y()...class Long
+0000f200: 5465 7874 4469 616c 6f67 2843 6f6d 6d6f  TextDialog(Commo
+0000f210: 6e44 6961 6c6f 6729 3a0a 2020 2020 6465  nDialog):.    de
+0000f220: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0000f230: 2074 6974 6c65 2c20 7465 7874 5f63 6f6e   title, text_con
+0000f240: 7465 6e74 2c20 7061 7265 6e74 3d4e 6f6e  tent, parent=Non
+0000f250: 6529 3a0a 2020 2020 2020 2020 6966 2070  e):.        if p
+0000f260: 6172 656e 7420 6973 204e 6f6e 653a 0a20  arent is None:. 
+0000f270: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+0000f280: 7420 3d20 746b 2e5f 6465 6661 756c 745f  t = tk._default_
+0000f290: 726f 6f74 0a0a 2020 2020 2020 2020 7375  root..        su
+0000f2a0: 7065 7228 292e 5f5f 696e 6974 5f5f 286d  per().__init__(m
+0000f2b0: 6173 7465 723d 7061 7265 6e74 290a 2020  aster=parent).  
+0000f2c0: 2020 2020 2020 7365 6c66 2e74 6974 6c65        self.title
+0000f2d0: 2874 6974 6c65 290a 0a20 2020 2020 2020  (title)..       
+0000f2e0: 206d 6169 6e5f 6672 616d 6520 3d20 7474   main_frame = tt
+0000f2f0: 6b2e 4672 616d 6528 7365 6c66 290a 2020  k.Frame(self).  
+0000f300: 2020 2020 2020 6d61 696e 5f66 7261 6d65        main_frame
+0000f310: 2e67 7269 6428 726f 773d 302c 2063 6f6c  .grid(row=0, col
+0000f320: 756d 6e3d 302c 2073 7469 636b 793d 226e  umn=0, sticky="n
+0000f330: 7365 7722 290a 2020 2020 2020 2020 7365  sew").        se
+0000f340: 6c66 2e63 6f6c 756d 6e63 6f6e 6669 6775  lf.columnconfigu
+0000f350: 7265 2830 2c20 7765 6967 6874 3d31 290a  re(0, weight=1).
+0000f360: 2020 2020 2020 2020 7365 6c66 2e72 6f77          self.row
+0000f370: 636f 6e66 6967 7572 6528 302c 2077 6569  configure(0, wei
+0000f380: 6768 743d 3129 0a0a 2020 2020 2020 2020  ght=1)..        
+0000f390: 6465 6661 756c 745f 666f 6e74 203d 2074  default_font = t
+0000f3a0: 6b2e 666f 6e74 2e6e 616d 6574 6f66 6f6e  k.font.nametofon
+0000f3b0: 7428 2254 6b44 6566 6175 6c74 466f 6e74  t("TkDefaultFont
+0000f3c0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000f3d0: 5f74 6578 7420 3d20 746b 7465 7874 6578  _text = tktextex
+0000f3e0: 742e 5465 7874 4672 616d 6528 0a20 2020  t.TextFrame(.   
+0000f3f0: 2020 2020 2020 2020 206d 6169 6e5f 6672           main_fr
+0000f400: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0000f410: 2072 6561 645f 6f6e 6c79 3d54 7275 652c   read_only=True,
+0000f420: 0a20 2020 2020 2020 2020 2020 2077 7261  .            wra
+0000f430: 703d 226e 6f6e 6522 2c0a 2020 2020 2020  p="none",.      
+0000f440: 2020 2020 2020 666f 6e74 3d64 6566 6175        font=defau
+0000f450: 6c74 5f66 6f6e 742c 0a20 2020 2020 2020  lt_font,.       
+0000f460: 2020 2020 2077 6964 7468 3d38 302c 0a20       width=80,. 
+0000f470: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+0000f480: 743d 3130 2c0a 2020 2020 2020 2020 2020  t=10,.          
+0000f490: 2020 7265 6c69 6566 3d22 7375 6e6b 656e    relief="sunken
+0000f4a0: 222c 0a20 2020 2020 2020 2020 2020 2062  ",.            b
+0000f4b0: 6f72 6465 7277 6964 7468 3d31 2c0a 2020  orderwidth=1,.  
+0000f4c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000f4d0: 7365 6c66 2e5f 7465 7874 2e67 7269 6428  self._text.grid(
+0000f4e0: 726f 773d 312c 2063 6f6c 756d 6e3d 302c  row=1, column=0,
+0000f4f0: 2063 6f6c 756d 6e73 7061 6e3d 322c 2073   columnspan=2, s
+0000f500: 7469 636b 793d 226e 7365 7722 2c20 7061  ticky="nsew", pa
+0000f510: 6478 3d32 302c 2070 6164 793d 3230 290a  dx=20, pady=20).
+0000f520: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+0000f530: 7874 2e74 6578 742e 6469 7265 6374 5f69  xt.text.direct_i
+0000f540: 6e73 6572 7428 2231 2e30 222c 2074 6578  nsert("1.0", tex
+0000f550: 745f 636f 6e74 656e 7429 0a20 2020 2020  t_content).     
+0000f560: 2020 2073 656c 662e 5f74 6578 742e 7465     self._text.te
+0000f570: 7874 2e73 6565 2822 312e 3022 290a 0a20  xt.see("1.0").. 
+0000f580: 2020 2020 2020 2063 6f70 795f 6275 7474         copy_butt
+0000f590: 6f6e 203d 2074 746b 2e42 7574 746f 6e28  on = ttk.Button(
+0000f5a0: 0a20 2020 2020 2020 2020 2020 206d 6169  .            mai
+0000f5b0: 6e5f 6672 616d 652c 2063 6f6d 6d61 6e64  n_frame, command
+0000f5c0: 3d73 656c 662e 5f63 6f70 792c 2074 6578  =self._copy, tex
+0000f5d0: 743d 7472 2822 436f 7079 2074 6f20 636c  t=tr("Copy to cl
+0000f5e0: 6970 626f 6172 6422 292c 2077 6964 7468  ipboard"), width
+0000f5f0: 3d32 300a 2020 2020 2020 2020 290a 2020  =20.        ).  
+0000f600: 2020 2020 2020 636f 7079 5f62 7574 746f        copy_butto
+0000f610: 6e2e 6772 6964 2872 6f77 3d32 2c20 636f  n.grid(row=2, co
+0000f620: 6c75 6d6e 3d30 2c20 7374 6963 6b79 3d22  lumn=0, sticky="
+0000f630: 7722 2c20 7061 6478 3d32 302c 2070 6164  w", padx=20, pad
+0000f640: 793d 2830 2c20 3230 2929 0a0a 2020 2020  y=(0, 20))..    
+0000f650: 2020 2020 636c 6f73 655f 6275 7474 6f6e      close_button
+0000f660: 203d 2074 746b 2e42 7574 746f 6e28 0a20   = ttk.Button(. 
+0000f670: 2020 2020 2020 2020 2020 206d 6169 6e5f             main_
+0000f680: 6672 616d 652c 2063 6f6d 6d61 6e64 3d73  frame, command=s
+0000f690: 656c 662e 5f63 6c6f 7365 2c20 7465 7874  elf._close, text
+0000f6a0: 3d74 7228 2243 6c6f 7365 2229 2c20 6465  =tr("Close"), de
+0000f6b0: 6661 756c 743d 2261 6374 6976 6522 0a20  fault="active". 
+0000f6c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000f6d0: 2063 6c6f 7365 5f62 7574 746f 6e2e 6772   close_button.gr
+0000f6e0: 6964 2872 6f77 3d32 2c20 636f 6c75 6d6e  id(row=2, column
+0000f6f0: 3d31 2c20 7374 6963 6b79 3d22 7722 2c20  =1, sticky="w", 
+0000f700: 7061 6478 3d32 302c 2070 6164 793d 2830  padx=20, pady=(0
+0000f710: 2c20 3230 2929 0a20 2020 2020 2020 2063  , 20)).        c
+0000f720: 6c6f 7365 5f62 7574 746f 6e2e 666f 6375  lose_button.focu
+0000f730: 735f 7365 7428 290a 0a20 2020 2020 2020  s_set()..       
+0000f740: 206d 6169 6e5f 6672 616d 652e 636f 6c75   main_frame.colu
+0000f750: 6d6e 636f 6e66 6967 7572 6528 302c 2077  mnconfigure(0, w
+0000f760: 6569 6768 743d 3129 0a20 2020 2020 2020  eight=1).       
+0000f770: 206d 6169 6e5f 6672 616d 652e 726f 7763   main_frame.rowc
+0000f780: 6f6e 6669 6775 7265 2831 2c20 7765 6967  onfigure(1, weig
+0000f790: 6874 3d31 290a 0a20 2020 2020 2020 2073  ht=1)..        s
+0000f7a0: 656c 662e 7072 6f74 6f63 6f6c 2822 574d  elf.protocol("WM
+0000f7b0: 5f44 454c 4554 455f 5749 4e44 4f57 222c  _DELETE_WINDOW",
+0000f7c0: 2073 656c 662e 5f63 6c6f 7365 290a 2020   self._close).  
+0000f7d0: 2020 2020 2020 7365 6c66 2e62 696e 6428        self.bind(
+0000f7e0: 223c 4573 6361 7065 3e22 2c20 7365 6c66  "<Escape>", self
+0000f7f0: 2e5f 636c 6f73 652c 2054 7275 6529 0a0a  ._close, True)..
+0000f800: 2020 2020 6465 6620 5f63 6f70 7928 7365      def _copy(se
+0000f810: 6c66 2c20 6576 656e 743d 4e6f 6e65 293a  lf, event=None):
+0000f820: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+0000f830: 6970 626f 6172 645f 636c 6561 7228 290a  ipboard_clear().
+0000f840: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+0000f850: 7062 6f61 7264 5f61 7070 656e 6428 7365  pboard_append(se
+0000f860: 6c66 2e5f 7465 7874 2e74 6578 742e 6765  lf._text.text.ge
+0000f870: 7428 2231 2e30 222c 2022 656e 6422 2929  t("1.0", "end"))
+0000f880: 0a0a 2020 2020 6465 6620 5f63 6c6f 7365  ..    def _close
+0000f890: 2873 656c 662c 2065 7665 6e74 3d4e 6f6e  (self, event=Non
+0000f8a0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+0000f8b0: 2e64 6573 7472 6f79 2829 0a0a 0a64 6566  .destroy()...def
+0000f8c0: 2061 736b 5f6f 6e65 5f66 726f 6d5f 6368   ask_one_from_ch
+0000f8d0: 6f69 6365 7328 0a20 2020 206d 6173 7465  oices(.    maste
+0000f8e0: 723d 4e6f 6e65 2c0a 2020 2020 7469 746c  r=None,.    titl
+0000f8f0: 653d 2243 686f 6f73 6520 6f6e 6522 2c0a  e="Choose one",.
+0000f900: 2020 2020 7175 6573 7469 6f6e 3a20 7374      question: st
+0000f910: 7220 3d20 2243 686f 6f73 6520 6f6e 653a  r = "Choose one:
+0000f920: 222c 0a20 2020 2063 686f 6963 6573 3d5b  ",.    choices=[
+0000f930: 5d2c 0a20 2020 2069 6e69 7469 616c 5f63  ],.    initial_c
+0000f940: 686f 6963 655f 696e 6465 783d 4e6f 6e65  hoice_index=None
+0000f950: 2c0a 293a 0a20 2020 2064 6c67 203d 2043  ,.):.    dlg = C
+0000f960: 686f 6963 6544 6961 6c6f 6728 6d61 7374  hoiceDialog(mast
+0000f970: 6572 2c20 7469 746c 652c 2071 7565 7374  er, title, quest
+0000f980: 696f 6e2c 2063 686f 6963 6573 2c20 696e  ion, choices, in
+0000f990: 6974 6961 6c5f 6368 6f69 6365 5f69 6e64  itial_choice_ind
+0000f9a0: 6578 290a 2020 2020 7368 6f77 5f64 6961  ex).    show_dia
+0000f9b0: 6c6f 6728 646c 672c 206d 6173 7465 7229  log(dlg, master)
+0000f9c0: 0a20 2020 2072 6574 7572 6e20 646c 672e  .    return dlg.
+0000f9d0: 7265 7375 6c74 0a0a 0a64 6566 2067 6574  result...def get
+0000f9e0: 5f62 7573 795f 6375 7273 6f72 2829 3a0a  _busy_cursor():.
+0000f9f0: 2020 2020 6966 2072 756e 6e69 6e67 5f6f      if running_o
+0000fa00: 6e5f 7769 6e64 6f77 7328 293a 0a20 2020  n_windows():.   
+0000fa10: 2020 2020 2072 6574 7572 6e20 2277 6169       return "wai
+0000fa20: 7422 0a20 2020 2065 6c69 6620 7275 6e6e  t".    elif runn
+0000fa30: 696e 675f 6f6e 5f6d 6163 5f6f 7328 293a  ing_on_mac_os():
+0000fa40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000fa50: 2273 7069 6e6e 696e 6722 0a20 2020 2065  "spinning".    e
+0000fa60: 6c73 653a 0a20 2020 2020 2020 2072 6574  lse:.        ret
+0000fa70: 7572 6e20 2277 6174 6368 220a 0a0a 6465  urn "watch"...de
+0000fa80: 6620 6765 745f 746b 5f76 6572 7369 6f6e  f get_tk_version
+0000fa90: 5f73 7472 2829 3a0a 2020 2020 7265 7475  _str():.    retu
+0000faa0: 726e 2074 6b2e 5f64 6566 6175 6c74 5f72  rn tk._default_r
+0000fab0: 6f6f 742e 746b 2e63 616c 6c28 2269 6e66  oot.tk.call("inf
+0000fac0: 6f22 2c20 2270 6174 6368 6c65 7665 6c22  o", "patchlevel"
+0000fad0: 290a 0a0a 6465 6620 6765 745f 746b 5f76  )...def get_tk_v
+0000fae0: 6572 7369 6f6e 5f69 6e66 6f28 293a 0a20  ersion_info():. 
+0000faf0: 2020 2072 6573 756c 7420 3d20 5b5d 0a20     result = []. 
+0000fb00: 2020 2066 6f72 2070 6172 7420 696e 2067     for part in g
+0000fb10: 6574 5f74 6b5f 7665 7273 696f 6e5f 7374  et_tk_version_st
+0000fb20: 7228 292e 7370 6c69 7428 222e 2229 3a0a  r().split("."):.
+0000fb30: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000fb40: 2020 2020 2020 2020 2072 6573 756c 742e           result.
+0000fb50: 6170 7065 6e64 2869 6e74 2870 6172 7429  append(int(part)
+0000fb60: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+0000fb70: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
+0000fb80: 2020 2020 2020 2020 7265 7375 6c74 2e61          result.a
+0000fb90: 7070 656e 6428 3029 0a20 2020 2072 6574  ppend(0).    ret
+0000fba0: 7572 6e20 7475 706c 6528 7265 7375 6c74  urn tuple(result
+0000fbb0: 290a 0a0a 6465 6620 6765 745f 7374 796c  )...def get_styl
+0000fbc0: 655f 636f 6e66 6967 7572 6174 696f 6e28  e_configuration(
+0000fbd0: 7374 796c 655f 6e61 6d65 2c20 6465 6661  style_name, defa
+0000fbe0: 756c 743d 7b7d 293a 0a20 2020 2073 7479  ult={}):.    sty
+0000fbf0: 6c65 203d 2074 746b 2e53 7479 6c65 2829  le = ttk.Style()
+0000fc00: 0a20 2020 2023 204e 4221 2073 7479 6c65  .    # NB! style
+0000fc10: 2e63 6f6e 6669 6775 7265 2073 6565 6d73  .configure seems
+0000fc20: 2074 6f20 7265 7573 6520 7468 6520 7265   to reuse the re
+0000fc30: 7475 726e 6564 2064 6963 740a 2020 2020  turned dict.    
+0000fc40: 2320 446f 6e27 7420 6368 616e 6765 2069  # Don't change i
+0000fc50: 7420 7769 7468 6f75 7420 636f 7079 696e  t without copyin
+0000fc60: 6720 6669 7273 740a 2020 2020 7265 7375  g first.    resu
+0000fc70: 6c74 203d 2073 7479 6c65 2e63 6f6e 6669  lt = style.confi
+0000fc80: 6775 7265 2873 7479 6c65 5f6e 616d 6529  gure(style_name)
+0000fc90: 0a20 2020 2069 6620 7265 7375 6c74 2069  .    if result i
+0000fca0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000fcb0: 7265 7475 726e 2064 6566 6175 6c74 0a20  return default. 
+0000fcc0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000fcd0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0000fce0: 0a64 6566 206c 6f6f 6b75 705f 7374 796c  .def lookup_styl
+0000fcf0: 655f 6f70 7469 6f6e 2873 7479 6c65 5f6e  e_option(style_n
+0000fd00: 616d 652c 206f 7074 696f 6e5f 6e61 6d65  ame, option_name
+0000fd10: 2c20 6465 6661 756c 743d 4e6f 6e65 293a  , default=None):
+0000fd20: 0a20 2020 2073 7479 6c65 203d 2074 746b  .    style = ttk
+0000fd30: 2e53 7479 6c65 2829 0a20 2020 2073 6574  .Style().    set
+0000fd40: 7469 6e67 203d 2073 7479 6c65 2e6c 6f6f  ting = style.loo
+0000fd50: 6b75 7028 7374 796c 655f 6e61 6d65 2c20  kup(style_name, 
+0000fd60: 6f70 7469 6f6e 5f6e 616d 6529 0a20 2020  option_name).   
+0000fd70: 2069 6620 7365 7474 696e 6720 696e 205b   if setting in [
+0000fd80: 4e6f 6e65 2c20 2222 5d3a 0a20 2020 2020  None, ""]:.     
+0000fd90: 2020 2072 6574 7572 6e20 6465 6661 756c     return defaul
+0000fda0: 740a 2020 2020 656c 6966 2073 6574 7469  t.    elif setti
+0000fdb0: 6e67 203d 3d20 2254 7275 6522 3a0a 2020  ng == "True":.  
+0000fdc0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000fdd0: 650a 2020 2020 656c 6966 2073 6574 7469  e.    elif setti
+0000fde0: 6e67 203d 3d20 2246 616c 7365 223a 0a20  ng == "False":. 
+0000fdf0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0000fe00: 6c73 650a 2020 2020 656c 7365 3a0a 2020  lse.    else:.  
+0000fe10: 2020 2020 2020 7265 7475 726e 2073 6574        return set
+0000fe20: 7469 6e67 0a0a 0a64 6566 2073 6361 6c65  ting...def scale
+0000fe30: 2876 616c 7565 293a 0a20 2020 2072 6574  (value):.    ret
+0000fe40: 7572 6e20 6765 745f 776f 726b 6265 6e63  urn get_workbenc
+0000fe50: 6828 292e 7363 616c 6528 7661 6c75 6529  h().scale(value)
+0000fe60: 0a0a 0a64 6566 206f 7065 6e5f 7061 7468  ...def open_path
+0000fe70: 5f69 6e5f 7379 7374 656d 5f66 696c 655f  _in_system_file_
+0000fe80: 6d61 6e61 6765 7228 7061 7468 293a 0a20  manager(path):. 
+0000fe90: 2020 2069 6620 7275 6e6e 696e 675f 6f6e     if running_on
+0000fea0: 5f6d 6163 5f6f 7328 293a 0a20 2020 2020  _mac_os():.     
+0000feb0: 2020 2023 2068 7474 703a 2f2f 7374 6163     # http://stac
+0000fec0: 6b6f 7665 7266 6c6f 772e 636f 6d2f 612f  koverflow.com/a/
+0000fed0: 3335 3230 3639 332f 3236 3131 3831 0a20  3520693/261181. 
+0000fee0: 2020 2020 2020 2023 202d 5220 646f 6573         # -R does
+0000fef0: 6e27 7420 616c 6c6f 7720 7368 6f77 696e  n't allow showin
+0000ff00: 6720 6869 6464 656e 2066 6f6c 6465 7273  g hidden folders
+0000ff10: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
+0000ff20: 6573 732e 506f 7065 6e28 5b22 6f70 656e  ess.Popen(["open
+0000ff30: 222c 2070 6174 685d 290a 2020 2020 656c  ", path]).    el
+0000ff40: 6966 2072 756e 6e69 6e67 5f6f 6e5f 6c69  if running_on_li
+0000ff50: 6e75 7828 293a 0a20 2020 2020 2020 2073  nux():.        s
+0000ff60: 7562 7072 6f63 6573 732e 506f 7065 6e28  ubprocess.Popen(
+0000ff70: 5b22 7864 672d 6f70 656e 222c 2070 6174  ["xdg-open", pat
+0000ff80: 685d 290a 2020 2020 656c 7365 3a0a 2020  h]).    else:.  
+0000ff90: 2020 2020 2020 6173 7365 7274 2072 756e        assert run
+0000ffa0: 6e69 6e67 5f6f 6e5f 7769 6e64 6f77 7328  ning_on_windows(
+0000ffb0: 290a 2020 2020 2020 2020 7375 6270 726f  ).        subpro
+0000ffc0: 6365 7373 2e50 6f70 656e 285b 2265 7870  cess.Popen(["exp
+0000ffd0: 6c6f 7265 7222 2c20 7061 7468 5d29 0a0a  lorer", path])..
+0000ffe0: 0a64 6566 205f 6765 745f 6469 616c 6f67  .def _get_dialog
+0000fff0: 5f70 726f 7669 6465 7228 293a 0a20 2020  _provider():.   
+00010000: 2069 6620 706c 6174 666f 726d 2e73 7973   if platform.sys
+00010010: 7465 6d28 2920 213d 2022 4c69 6e75 7822  tem() != "Linux"
+00010020: 206f 7220 6765 745f 776f 726b 6265 6e63   or get_workbenc
+00010030: 6828 292e 6765 745f 6f70 7469 6f6e 2822  h().get_option("
+00010040: 6669 6c65 2e61 766f 6964 5f7a 656e 6974  file.avoid_zenit
+00010050: 7922 293a 0a20 2020 2020 2020 2072 6574  y"):.        ret
+00010060: 7572 6e20 6669 6c65 6469 616c 6f67 0a0a  urn filedialog..
+00010070: 2020 2020 696d 706f 7274 2073 6875 7469      import shuti
+00010080: 6c0a 0a20 2020 2069 6620 7368 7574 696c  l..    if shutil
+00010090: 2e77 6869 6368 2822 7a65 6e69 7479 2229  .which("zenity")
+000100a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000100b0: 205f 5a65 6e69 7479 4469 616c 6f67 5072   _ZenityDialogPr
+000100c0: 6f76 6964 6572 0a0a 2020 2020 2320 6661  ovider..    # fa
+000100d0: 6c6c 6261 636b 0a20 2020 2072 6574 7572  llback.    retur
+000100e0: 6e20 6669 6c65 6469 616c 6f67 0a0a 0a64  n filedialog...d
+000100f0: 6566 2074 7279 5f72 6573 746f 7265 5f66  ef try_restore_f
+00010100: 6f63 7573 5f61 6674 6572 5f66 696c 655f  ocus_after_file_
+00010110: 6469 616c 6f67 2864 6961 6c6f 675f 7061  dialog(dialog_pa
+00010120: 7265 6e74 293a 0a20 2020 2069 6620 6469  rent):.    if di
+00010130: 616c 6f67 5f70 6172 656e 7420 6973 204e  alog_parent is N
+00010140: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
+00010150: 7572 6e0a 0a20 2020 206c 6f67 6765 722e  urn..    logger.
+00010160: 696e 666f 2822 5265 7374 6f72 696e 6720  info("Restoring 
+00010170: 666f 6375 7320 746f 2025 7322 2c20 6469  focus to %s", di
+00010180: 616c 6f67 5f70 6172 656e 7429 0a20 2020  alog_parent).   
+00010190: 206f 6c64 5f66 6f63 7573 6564 5f77 6964   old_focused_wid
+000101a0: 6765 7420 3d20 6469 616c 6f67 5f70 6172  get = dialog_par
+000101b0: 656e 742e 7769 6e66 6f5f 746f 706c 6576  ent.winfo_toplev
+000101c0: 656c 2829 2e66 6f63 7573 5f67 6574 2829  el().focus_get()
+000101d0: 0a0a 2020 2020 6469 616c 6f67 5f70 6172  ..    dialog_par
+000101e0: 656e 742e 7769 6e66 6f5f 746f 706c 6576  ent.winfo_toplev
+000101f0: 656c 2829 2e6c 6966 7428 290a 2020 2020  el().lift().    
+00010200: 6469 616c 6f67 5f70 6172 656e 742e 7769  dialog_parent.wi
+00010210: 6e66 6f5f 746f 706c 6576 656c 2829 2e66  nfo_toplevel().f
+00010220: 6f63 7573 5f66 6f72 6365 2829 0a20 2020  ocus_force().   
+00010230: 2064 6961 6c6f 675f 7061 7265 6e74 2e77   dialog_parent.w
+00010240: 696e 666f 5f74 6f70 6c65 7665 6c28 292e  info_toplevel().
+00010250: 6772 6162 5f73 6574 2829 0a20 2020 2069  grab_set().    i
+00010260: 6620 7275 6e6e 696e 675f 6f6e 5f6d 6163  f running_on_mac
+00010270: 5f6f 7328 293a 0a20 2020 2020 2020 2064  _os():.        d
+00010280: 6961 6c6f 675f 7061 7265 6e74 2e77 696e  ialog_parent.win
+00010290: 666f 5f74 6f70 6c65 7665 6c28 292e 6772  fo_toplevel().gr
+000102a0: 6162 5f72 656c 6561 7365 2829 0a0a 2020  ab_release()..  
+000102b0: 2020 6966 206f 6c64 5f66 6f63 7573 6564    if old_focused
+000102c0: 5f77 6964 6765 7420 6973 206e 6f74 204e  _widget is not N
+000102d0: 6f6e 653a 0a20 2020 2020 2020 2074 7279  one:.        try
+000102e0: 3a0a 2020 2020 2020 2020 2020 2020 6f6c  :.            ol
+000102f0: 645f 666f 6375 7365 645f 7769 6467 6574  d_focused_widget
+00010300: 2e66 6f63 7573 5f66 6f72 6365 2829 0a20  .focus_force(). 
+00010310: 2020 2020 2020 2065 7863 6570 7420 5463         except Tc
+00010320: 6c45 7272 6f72 3a0a 2020 2020 2020 2020  lError:.        
+00010330: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+00010340: 6e67 2822 436f 756c 6420 6e6f 7420 7265  ng("Could not re
+00010350: 7374 6f72 6520 666f 6375 7320 746f 2025  store focus to %
+00010360: 7222 2c20 6f6c 645f 666f 6375 7365 645f  r", old_focused_
+00010370: 7769 6467 6574 290a 0a0a 6465 6620 6173  widget)...def as
+00010380: 6b73 6176 6561 7366 696c 656e 616d 6528  ksaveasfilename(
+00010390: 2a2a 6f70 7469 6f6e 7329 3a0a 2020 2020  **options):.    
+000103a0: 2320 6874 7470 733a 2f2f 7463 6c2e 746b  # https://tcl.tk
+000103b0: 2f6d 616e 2f74 636c 382e 362f 546b 436d  /man/tcl8.6/TkCm
+000103c0: 642f 6765 744f 7065 6e46 696c 652e 6874  d/getOpenFile.ht
+000103d0: 6d0a 2020 2020 7061 7265 6e74 203d 205f  m.    parent = _
+000103e0: 6368 6563 6b5f 6469 616c 6f67 5f70 6172  check_dialog_par
+000103f0: 656e 7428 6f70 7469 6f6e 7329 0a20 2020  ent(options).   
+00010400: 2074 7279 3a0a 2020 2020 2020 2020 7265   try:.        re
+00010410: 7475 726e 205f 6765 745f 6469 616c 6f67  turn _get_dialog
+00010420: 5f70 726f 7669 6465 7228 292e 6173 6b73  _provider().asks
+00010430: 6176 6561 7366 696c 656e 616d 6528 2a2a  aveasfilename(**
+00010440: 6f70 7469 6f6e 7329 0a20 2020 2066 696e  options).    fin
+00010450: 616c 6c79 3a0a 2020 2020 2020 2020 7472  ally:.        tr
+00010460: 795f 7265 7374 6f72 655f 666f 6375 735f  y_restore_focus_
+00010470: 6166 7465 725f 6669 6c65 5f64 6961 6c6f  after_file_dialo
+00010480: 6728 7061 7265 6e74 290a 0a0a 6465 6620  g(parent)...def 
+00010490: 6173 6b6f 7065 6e66 696c 656e 616d 6528  askopenfilename(
+000104a0: 2a2a 6f70 7469 6f6e 7329 3a0a 2020 2020  **options):.    
+000104b0: 2320 6874 7470 733a 2f2f 7463 6c2e 746b  # https://tcl.tk
+000104c0: 2f6d 616e 2f74 636c 382e 362f 546b 436d  /man/tcl8.6/TkCm
+000104d0: 642f 6765 744f 7065 6e46 696c 652e 6874  d/getOpenFile.ht
+000104e0: 6d0a 2020 2020 7061 7265 6e74 203d 205f  m.    parent = _
+000104f0: 6368 6563 6b5f 6469 616c 6f67 5f70 6172  check_dialog_par
+00010500: 656e 7428 6f70 7469 6f6e 7329 0a20 2020  ent(options).   
+00010510: 2074 7279 3a0a 2020 2020 2020 2020 7265   try:.        re
+00010520: 7475 726e 205f 6765 745f 6469 616c 6f67  turn _get_dialog
+00010530: 5f70 726f 7669 6465 7228 292e 6173 6b6f  _provider().asko
+00010540: 7065 6e66 696c 656e 616d 6528 2a2a 6f70  penfilename(**op
+00010550: 7469 6f6e 7329 0a20 2020 2066 696e 616c  tions).    final
+00010560: 6c79 3a0a 2020 2020 2020 2020 7472 795f  ly:.        try_
+00010570: 7265 7374 6f72 655f 666f 6375 735f 6166  restore_focus_af
+00010580: 7465 725f 6669 6c65 5f64 6961 6c6f 6728  ter_file_dialog(
+00010590: 7061 7265 6e74 290a 0a0a 6465 6620 6173  parent)...def as
+000105a0: 6b6f 7065 6e66 696c 656e 616d 6573 282a  kopenfilenames(*
+000105b0: 2a6f 7074 696f 6e73 293a 0a20 2020 2023  *options):.    #
+000105c0: 2068 7474 7073 3a2f 2f74 636c 2e74 6b2f   https://tcl.tk/
+000105d0: 6d61 6e2f 7463 6c38 2e36 2f54 6b43 6d64  man/tcl8.6/TkCmd
+000105e0: 2f67 6574 4f70 656e 4669 6c65 2e68 746d  /getOpenFile.htm
+000105f0: 0a20 2020 2070 6172 656e 7420 3d20 5f63  .    parent = _c
+00010600: 6865 636b 5f64 6961 6c6f 675f 7061 7265  heck_dialog_pare
+00010610: 6e74 286f 7074 696f 6e73 290a 2020 2020  nt(options).    
+00010620: 7472 793a 0a20 2020 2020 2020 2072 6574  try:.        ret
+00010630: 7572 6e20 5f67 6574 5f64 6961 6c6f 675f  urn _get_dialog_
+00010640: 7072 6f76 6964 6572 2829 2e61 736b 6f70  provider().askop
+00010650: 656e 6669 6c65 6e61 6d65 7328 2a2a 6f70  enfilenames(**op
+00010660: 7469 6f6e 7329 0a20 2020 2066 696e 616c  tions).    final
+00010670: 6c79 3a0a 2020 2020 2020 2020 7472 795f  ly:.        try_
+00010680: 7265 7374 6f72 655f 666f 6375 735f 6166  restore_focus_af
+00010690: 7465 725f 6669 6c65 5f64 6961 6c6f 6728  ter_file_dialog(
+000106a0: 7061 7265 6e74 290a 0a0a 6465 6620 6173  parent)...def as
+000106b0: 6b64 6972 6563 746f 7279 282a 2a6f 7074  kdirectory(**opt
+000106c0: 696f 6e73 293a 0a20 2020 2023 2068 7474  ions):.    # htt
+000106d0: 7073 3a2f 2f74 636c 2e74 6b2f 6d61 6e2f  ps://tcl.tk/man/
+000106e0: 7463 6c38 2e36 2f54 6b43 6d64 2f63 686f  tcl8.6/TkCmd/cho
+000106f0: 6f73 6544 6972 6563 746f 7279 2e68 746d  oseDirectory.htm
+00010700: 0a20 2020 2070 6172 656e 7420 3d20 5f63  .    parent = _c
+00010710: 6865 636b 5f64 6961 6c6f 675f 7061 7265  heck_dialog_pare
+00010720: 6e74 286f 7074 696f 6e73 290a 2020 2020  nt(options).    
+00010730: 7472 793a 0a20 2020 2020 2020 2072 6574  try:.        ret
+00010740: 7572 6e20 5f67 6574 5f64 6961 6c6f 675f  urn _get_dialog_
+00010750: 7072 6f76 6964 6572 2829 2e61 736b 6469  provider().askdi
+00010760: 7265 6374 6f72 7928 2a2a 6f70 7469 6f6e  rectory(**option
+00010770: 7329 0a20 2020 2066 696e 616c 6c79 3a0a  s).    finally:.
+00010780: 2020 2020 2020 2020 7472 795f 7265 7374          try_rest
+00010790: 6f72 655f 666f 6375 735f 6166 7465 725f  ore_focus_after_
+000107a0: 6669 6c65 5f64 6961 6c6f 6728 7061 7265  file_dialog(pare
+000107b0: 6e74 290a 0a0a 6465 6620 5f63 6865 636b  nt)...def _check
+000107c0: 5f64 6961 6c6f 675f 7061 7265 6e74 286f  _dialog_parent(o
+000107d0: 7074 696f 6e73 293a 0a20 2020 2069 6620  ptions):.    if 
+000107e0: 6f70 7469 6f6e 732e 6765 7428 2270 6172  options.get("par
+000107f0: 656e 7422 2920 616e 6420 6f70 7469 6f6e  ent") and option
+00010800: 732e 6765 7428 226d 6173 7465 7222 293a  s.get("master"):
+00010810: 0a20 2020 2020 2020 2070 6172 656e 7420  .        parent 
+00010820: 3d20 6f70 7469 6f6e 735b 2270 6172 656e  = options["paren
+00010830: 7422 5d2e 7769 6e66 6f5f 746f 706c 6576  t"].winfo_toplev
+00010840: 656c 2829 0a20 2020 2020 2020 206d 6173  el().        mas
+00010850: 7465 7220 3d20 6f70 7469 6f6e 735b 226d  ter = options["m
+00010860: 6173 7465 7222 5d2e 7769 6e66 6f5f 746f  aster"].winfo_to
+00010870: 706c 6576 656c 2829 0a20 2020 2020 2020  plevel().       
+00010880: 2069 6620 7061 7265 6e74 2069 7320 6e6f   if parent is no
+00010890: 7420 6d61 7374 6572 3a0a 2020 2020 2020  t master:.      
+000108a0: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+000108b0: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
+000108c0: 2020 2020 2020 2244 6961 6c6f 6720 7769        "Dialog wi
+000108d0: 7468 2064 6966 6665 7265 6e74 2070 6172  th different par
+000108e0: 656e 742f 6d61 7374 6572 2074 6f70 6c65  ent/master tople
+000108f0: 7665 6c73 3a5c 6e25 7322 2c0a 2020 2020  vels:\n%s",.    
+00010900: 2020 2020 2020 2020 2020 2020 2222 2e6a              "".j
+00010910: 6f69 6e28 7472 6163 6562 6163 6b2e 666f  oin(traceback.fo
+00010920: 726d 6174 5f73 7461 636b 2829 292c 0a20  rmat_stack()),. 
+00010930: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010940: 2065 6c69 6620 6f70 7469 6f6e 732e 6765   elif options.ge
+00010950: 7428 2270 6172 656e 7422 293a 0a20 2020  t("parent"):.   
+00010960: 2020 2020 2070 6172 656e 7420 3d20 6f70       parent = op
+00010970: 7469 6f6e 735b 2270 6172 656e 7422 5d2e  tions["parent"].
+00010980: 7769 6e66 6f5f 746f 706c 6576 656c 2829  winfo_toplevel()
+00010990: 0a20 2020 2020 2020 206d 6173 7465 7220  .        master 
+000109a0: 3d20 6f70 7469 6f6e 735b 2270 6172 656e  = options["paren
+000109b0: 7422 5d2e 7769 6e66 6f5f 746f 706c 6576  t"].winfo_toplev
+000109c0: 656c 2829 0a20 2020 2065 6c69 6620 6f70  el().    elif op
+000109d0: 7469 6f6e 732e 6765 7428 226d 6173 7465  tions.get("maste
+000109e0: 7222 293a 0a20 2020 2020 2020 2070 6172  r"):.        par
+000109f0: 656e 7420 3d20 6f70 7469 6f6e 735b 226d  ent = options["m
+00010a00: 6173 7465 7222 5d2e 7769 6e66 6f5f 746f  aster"].winfo_to
+00010a10: 706c 6576 656c 2829 0a20 2020 2020 2020  plevel().       
+00010a20: 206d 6173 7465 7220 3d20 6f70 7469 6f6e   master = option
+00010a30: 735b 226d 6173 7465 7222 5d2e 7769 6e66  s["master"].winf
+00010a40: 6f5f 746f 706c 6576 656c 2829 0a20 2020  o_toplevel().   
+00010a50: 2065 6c73 653a 0a20 2020 2020 2020 206c   else:.        l
+00010a60: 6f67 6765 722e 7761 726e 696e 6728 2244  ogger.warning("D
+00010a70: 6961 6c6f 6720 7769 7468 6f75 7420 7061  ialog without pa
+00010a80: 7265 6e74 3a5c 6e25 7322 2c20 2222 2e6a  rent:\n%s", "".j
+00010a90: 6f69 6e28 7472 6163 6562 6163 6b2e 666f  oin(traceback.fo
+00010aa0: 726d 6174 5f73 7461 636b 2829 2929 0a20  rmat_stack())). 
+00010ab0: 2020 2020 2020 2070 6172 656e 7420 3d20         parent = 
+00010ac0: 746b 2e5f 6465 6661 756c 745f 726f 6f74  tk._default_root
+00010ad0: 0a20 2020 2020 2020 206d 6173 7465 7220  .        master 
+00010ae0: 3d20 746b 2e5f 6465 6661 756c 745f 726f  = tk._default_ro
+00010af0: 6f74 0a0a 2020 2020 6f70 7469 6f6e 735b  ot..    options[
+00010b00: 2270 6172 656e 7422 5d20 3d20 7061 7265  "parent"] = pare
+00010b10: 6e74 0a20 2020 206f 7074 696f 6e73 5b22  nt.    options["
+00010b20: 6d61 7374 6572 225d 203d 206d 6173 7465  master"] = maste
+00010b30: 720a 0a20 2020 2069 6620 7275 6e6e 696e  r..    if runnin
+00010b40: 675f 6f6e 5f6d 6163 5f6f 7328 293a 0a20  g_on_mac_os():. 
+00010b50: 2020 2020 2020 2023 2075 7365 6420 746f         # used to
+00010b60: 2072 6571 7569 7265 206d 6173 7465 722f   require master/
+00010b70: 7061 7265 6e74 2028 6874 7470 733a 2f2f  parent (https://
+00010b80: 6275 6773 2e70 7974 686f 6e2e 6f72 672f  bugs.python.org/
+00010b90: 6973 7375 6533 3439 3237 290a 2020 2020  issue34927).    
+00010ba0: 2020 2020 2320 6275 7420 7468 6973 2069      # but this i
+00010bb0: 7320 6465 7072 6563 6174 6564 2069 6e20  s deprecated in 
+00010bc0: 4361 7461 6c69 6e61 2028 6874 7470 733a  Catalina (https:
+00010bd0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 686f  //github.com/tho
+00010be0: 6e6e 792f 7468 6f6e 6e79 2f69 7373 7565  nny/thonny/issue
+00010bf0: 732f 3834 3029 0a20 2020 2020 2020 2023  s/840).        #
+00010c00: 2054 4f44 4f3a 2043 6f6e 7369 6465 7220   TODO: Consider 
+00010c10: 7265 6d6f 7669 6e67 2074 6869 7320 7768  removing this wh
+00010c20: 656e 2075 7067 7261 6469 6e67 2066 726f  en upgrading fro
+00010c30: 6d20 546b 2038 2e36 2e38 0a20 2020 2020  m Tk 8.6.8.     
+00010c40: 2020 2064 656c 206f 7074 696f 6e73 5b22     del options["
+00010c50: 6d61 7374 6572 225d 0a20 2020 2020 2020  master"].       
+00010c60: 2064 656c 206f 7074 696f 6e73 5b22 7061   del options["pa
+00010c70: 7265 6e74 225d 0a0a 2020 2020 7265 7475  rent"]..    retu
+00010c80: 726e 2070 6172 656e 740a 0a0a 636c 6173  rn parent...clas
+00010c90: 7320 5f5a 656e 6974 7944 6961 6c6f 6750  s _ZenityDialogP
+00010ca0: 726f 7669 6465 723a 0a20 2020 2023 2068  rovider:.    # h
+00010cb0: 7474 7073 3a2f 2f77 7777 2e77 7269 7465  ttps://www.write
+00010cc0: 6261 7368 2e63 6f6d 2f62 6173 682d 6775  bash.com/bash-gu
+00010cd0: 692f 7a65 6e69 7479 2d63 7265 6174 652d  i/zenity-create-
+00010ce0: 6669 6c65 2d73 656c 6563 7469 6f6e 2d64  file-selection-d
+00010cf0: 6961 6c6f 672d 3232 342e 6874 6d6c 0a20  ialog-224.html. 
+00010d00: 2020 2023 2068 7474 703a 2f2f 6c69 6e75     # http://linu
+00010d10: 782e 6279 6578 616d 706c 6573 2e63 6f6d  x.byexamples.com
+00010d20: 2f61 7263 6869 7665 732f 3235 392f 612d  /archives/259/a-
+00010d30: 636f 6d70 6c65 7465 2d7a 656e 6974 792d  complete-zenity-
+00010d40: 6469 616c 6f67 2d65 7861 6d70 6c65 732d  dialog-examples-
+00010d50: 312f 0a20 2020 2023 2068 7474 703a 2f2f  1/.    # http://
+00010d60: 6c69 6e75 782e 6279 6578 616d 706c 6573  linux.byexamples
+00010d70: 2e63 6f6d 2f61 7263 6869 7665 732f 3236  .com/archives/26
+00010d80: 352f 612d 636f 6d70 6c65 7465 2d7a 656e  5/a-complete-zen
+00010d90: 6974 792d 6469 616c 6f67 2d65 7861 6d70  ity-dialog-examp
+00010da0: 6c65 732d 322f 0a0a 2020 2020 2320 616e  les-2/..    # an
+00010db0: 6f74 6865 7220 706f 7373 6962 696c 6974  other possibilit
+00010dc0: 7920 6973 2074 6f20 7573 6520 5079 476f  y is to use PyGo
+00010dd0: 626a 6563 743a 2068 7474 7073 3a2f 2f67  bject: https://g
+00010de0: 6974 6875 622e 636f 6d2f 706f 756c 702f  ithub.com/poulp/
+00010df0: 7a65 6e69 7079 0a0a 2020 2020 4063 6c61  zenipy..    @cla
+00010e00: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00010e10: 2061 736b 6f70 656e 6669 6c65 6e61 6d65   askopenfilename
+00010e20: 2863 6c73 2c20 2a2a 6f70 7469 6f6e 7329  (cls, **options)
+00010e30: 3a0a 2020 2020 2020 2020 6172 6773 203d  :.        args =
+00010e40: 2063 6c73 2e5f 636f 6e76 6572 745f 636f   cls._convert_co
+00010e50: 6d6d 6f6e 5f6f 7074 696f 6e73 2822 4f70  mmon_options("Op
+00010e60: 656e 2066 696c 6522 2c20 2a2a 6f70 7469  en file", **opti
+00010e70: 6f6e 7329 0a20 2020 2020 2020 2072 6574  ons).        ret
+00010e80: 7572 6e20 636c 732e 5f63 616c 6c28 6172  urn cls._call(ar
+00010e90: 6773 290a 0a20 2020 2040 636c 6173 736d  gs)..    @classm
+00010ea0: 6574 686f 640a 2020 2020 6465 6620 6173  ethod.    def as
+00010eb0: 6b6f 7065 6e66 696c 656e 616d 6573 2863  kopenfilenames(c
+00010ec0: 6c73 2c20 2a2a 6f70 7469 6f6e 7329 3a0a  ls, **options):.
+00010ed0: 2020 2020 2020 2020 6172 6773 203d 2063          args = c
+00010ee0: 6c73 2e5f 636f 6e76 6572 745f 636f 6d6d  ls._convert_comm
+00010ef0: 6f6e 5f6f 7074 696f 6e73 2822 4f70 656e  on_options("Open
+00010f00: 2066 696c 6573 222c 202a 2a6f 7074 696f   files", **optio
+00010f10: 6e73 290a 2020 2020 2020 2020 7265 7475  ns).        retu
+00010f20: 726e 2063 6c73 2e5f 6361 6c6c 2861 7267  rn cls._call(arg
+00010f30: 7320 2b20 5b22 2d2d 6d75 6c74 6970 6c65  s + ["--multiple
+00010f40: 225d 292e 7370 6c69 7428 227c 2229 0a0a  "]).split("|")..
+00010f50: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00010f60: 0a20 2020 2064 6566 2061 736b 7361 7665  .    def asksave
+00010f70: 6173 6669 6c65 6e61 6d65 2863 6c73 2c20  asfilename(cls, 
+00010f80: 2a2a 6f70 7469 6f6e 7329 3a0a 2020 2020  **options):.    
+00010f90: 2020 2020 6172 6773 203d 2063 6c73 2e5f      args = cls._
+00010fa0: 636f 6e76 6572 745f 636f 6d6d 6f6e 5f6f  convert_common_o
+00010fb0: 7074 696f 6e73 2822 5361 7665 2061 7322  ptions("Save as"
+00010fc0: 2c20 2a2a 6f70 7469 6f6e 7329 0a20 2020  , **options).   
+00010fd0: 2020 2020 2061 7267 732e 6170 7065 6e64       args.append
+00010fe0: 2822 2d2d 7361 7665 2229 0a20 2020 2020  ("--save").     
+00010ff0: 2020 2069 6620 6f70 7469 6f6e 732e 6765     if options.ge
+00011000: 7428 2263 6f6e 6669 726d 6f76 6572 7772  t("confirmoverwr
+00011010: 6974 6522 2c20 5472 7565 293a 0a20 2020  ite", True):.   
+00011020: 2020 2020 2020 2020 2061 7267 732e 6170           args.ap
+00011030: 7065 6e64 2822 2d2d 636f 6e66 6972 6d2d  pend("--confirm-
+00011040: 6f76 6572 7772 6974 6522 290a 0a20 2020  overwrite")..   
+00011050: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
+00011060: 636c 732e 5f63 616c 6c28 6172 6773 290a  cls._call(args).
+00011070: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
+00011080: 696c 656e 616d 653a 0a20 2020 2020 2020  ilename:.       
+00011090: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000110a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000110b0: 2066 696c 656e 616d 650a 0a20 2020 2040   filename..    @
+000110c0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+000110d0: 6465 6620 6173 6b64 6972 6563 746f 7279  def askdirectory
+000110e0: 2863 6c73 2c20 2a2a 6f70 7469 6f6e 7329  (cls, **options)
+000110f0: 3a0a 2020 2020 2020 2020 6172 6773 203d  :.        args =
+00011100: 2063 6c73 2e5f 636f 6e76 6572 745f 636f   cls._convert_co
+00011110: 6d6d 6f6e 5f6f 7074 696f 6e73 2822 5365  mmon_options("Se
+00011120: 6c65 6374 2064 6972 6563 746f 7279 222c  lect directory",
+00011130: 202a 2a6f 7074 696f 6e73 290a 2020 2020   **options).    
+00011140: 2020 2020 6172 6773 2e61 7070 656e 6428      args.append(
+00011150: 222d 2d64 6972 6563 746f 7279 2229 0a20  "--directory"). 
+00011160: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
+00011170: 732e 5f63 616c 6c28 6172 6773 290a 0a20  s._call(args).. 
+00011180: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00011190: 2020 2020 6465 6620 5f63 6f6e 7665 7274      def _convert
+000111a0: 5f63 6f6d 6d6f 6e5f 6f70 7469 6f6e 7328  _common_options(
+000111b0: 636c 732c 2064 6566 6175 6c74 5f74 6974  cls, default_tit
+000111c0: 6c65 2c20 2a2a 6f70 7469 6f6e 7329 3a0a  le, **options):.
+000111d0: 2020 2020 2020 2020 6172 6773 203d 205b          args = [
+000111e0: 222d 2d66 696c 652d 7365 6c65 6374 696f  "--file-selectio
+000111f0: 6e22 2c20 222d 2d74 6974 6c65 3d25 7322  n", "--title=%s"
+00011200: 2025 206f 7074 696f 6e73 2e67 6574 2822   % options.get("
+00011210: 7469 746c 6522 2c20 6465 6661 756c 745f  title", default_
+00011220: 7469 746c 6529 5d0a 0a20 2020 2020 2020  title)]..       
+00011230: 2066 696c 656e 616d 6520 3d20 5f6f 7074   filename = _opt
+00011240: 696f 6e73 5f74 6f5f 7a65 6e69 7479 5f66  ions_to_zenity_f
+00011250: 696c 656e 616d 6528 6f70 7469 6f6e 7329  ilename(options)
+00011260: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
+00011270: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+00011280: 2020 6172 6773 2e61 7070 656e 6428 222d    args.append("-
+00011290: 2d66 696c 656e 616d 653d 2573 2220 2520  -filename=%s" % 
+000112a0: 6669 6c65 6e61 6d65 290a 0a20 2020 2020  filename)..     
+000112b0: 2020 2070 6172 656e 7420 3d20 6f70 7469     parent = opti
+000112c0: 6f6e 732e 6765 7428 2270 6172 656e 7422  ons.get("parent"
+000112d0: 2c20 6f70 7469 6f6e 732e 6765 7428 226d  , options.get("m
+000112e0: 6173 7465 7222 2c20 4e6f 6e65 2929 0a20  aster", None)). 
+000112f0: 2020 2020 2020 2069 6620 7061 7265 6e74         if parent
+00011300: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011310: 2020 2020 2020 2020 2020 6172 6773 2e61            args.a
+00011320: 7070 656e 6428 222d 2d6d 6f64 616c 2229  ppend("--modal")
+00011330: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00011340: 732e 6170 7065 6e64 2822 2d2d 6174 7461  s.append("--atta
+00011350: 6368 3d25 7322 2025 2068 6578 2870 6172  ch=%s" % hex(par
+00011360: 656e 742e 7769 6e66 6f5f 6964 2829 2929  ent.winfo_id()))
+00011370: 0a0a 2020 2020 2020 2020 666f 7220 6465  ..        for de
+00011380: 7363 2c20 7061 7474 6572 6e20 696e 206f  sc, pattern in o
+00011390: 7074 696f 6e73 2e67 6574 2822 6669 6c65  ptions.get("file
+000113a0: 7479 7065 7322 2c20 2829 293a 0a20 2020  types", ()):.   
+000113b0: 2020 2020 2020 2020 2023 207a 656e 6974           # zenit
+000113c0: 7920 7265 7175 6972 6573 2073 7461 7220  y requires star 
+000113d0: 6265 666f 7265 2065 7874 656e 7369 6f6e  before extension
+000113e0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+000113f0: 7465 726e 203d 2070 6174 7465 726e 2e72  tern = pattern.r
+00011400: 6570 6c61 6365 2822 202e 222c 2022 202a  eplace(" .", " *
+00011410: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00011420: 6966 2070 6174 7465 726e 2e73 7461 7274  if pattern.start
+00011430: 7377 6974 6828 222e 2229 3a0a 2020 2020  swith("."):.    
+00011440: 2020 2020 2020 2020 2020 2020 7061 7474              patt
+00011450: 6572 6e20 3d20 222a 2220 2b20 7061 7474  ern = "*" + patt
+00011460: 6572 6e0a 0a20 2020 2020 2020 2020 2020  ern..           
+00011470: 2069 6620 7061 7474 6572 6e20 3d3d 2022   if pattern == "
+00011480: 2a2e 2a22 3a0a 2020 2020 2020 2020 2020  *.*":.          
+00011490: 2020 2020 2020 2320 222e 2a22 2077 6173        # ".*" was
+000114a0: 2070 726f 7669 6465 6420 746f 206d 616b   provided to mak
+000114b0: 6520 7468 6520 7061 7474 6572 6e20 7361  e the pattern sa
+000114c0: 6665 2066 6f72 2054 6b20 6469 616c 6f67  fe for Tk dialog
+000114d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114e0: 2023 206e 6f74 2072 6571 7569 7265 6420   # not required 
+000114f0: 7769 7468 205a 656e 6974 790a 2020 2020  with Zenity.    
+00011500: 2020 2020 2020 2020 2020 2020 7061 7474              patt
+00011510: 6572 6e20 3d20 222a 220a 0a20 2020 2020  ern = "*"..     
+00011520: 2020 2020 2020 2061 7267 732e 6170 7065         args.appe
+00011530: 6e64 2822 2d2d 6669 6c65 2d66 696c 7465  nd("--file-filte
+00011540: 723d 2573 207c 2025 7322 2025 2028 6465  r=%s | %s" % (de
+00011550: 7363 2c20 7061 7474 6572 6e29 290a 0a20  sc, pattern)).. 
+00011560: 2020 2020 2020 2072 6574 7572 6e20 6172         return ar
+00011570: 6773 0a0a 2020 2020 4063 6c61 7373 6d65  gs..    @classme
+00011580: 7468 6f64 0a20 2020 2064 6566 205f 6361  thod.    def _ca
+00011590: 6c6c 2863 6c73 2c20 6172 6773 293a 0a20  ll(cls, args):. 
+000115a0: 2020 2020 2020 2061 7267 7320 3d20 5b22         args = ["
+000115b0: 7a65 6e69 7479 222c 2022 2d2d 6e61 6d65  zenity", "--name
+000115c0: 3d54 686f 6e6e 7922 2c20 222d 2d63 6c61  =Thonny", "--cla
+000115d0: 7373 3d54 686f 6e6e 7922 5d20 2b20 6172  ss=Thonny"] + ar
+000115e0: 6773 0a20 2020 2020 2020 2072 6573 756c  gs.        resul
+000115f0: 7420 3d20 7375 6270 726f 6365 7373 2e72  t = subprocess.r
+00011600: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
+00011610: 6172 6773 2c20 7374 646f 7574 3d73 7562  args, stdout=sub
+00011620: 7072 6f63 6573 732e 5049 5045 2c20 7374  process.PIPE, st
+00011630: 6465 7272 3d73 7562 7072 6f63 6573 732e  derr=subprocess.
+00011640: 5049 5045 2c20 756e 6976 6572 7361 6c5f  PIPE, universal_
+00011650: 6e65 776c 696e 6573 3d54 7275 650a 2020  newlines=True.  
+00011660: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00011670: 6966 2072 6573 756c 742e 7265 7475 726e  if result.return
+00011680: 636f 6465 203d 3d20 303a 0a20 2020 2020  code == 0:.     
+00011690: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000116a0: 7375 6c74 2e73 7464 6f75 742e 7374 7269  sult.stdout.stri
+000116b0: 7028 290a 2020 2020 2020 2020 656c 7365  p().        else
+000116c0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+000116d0: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
+000116e0: 2020 2020 2020 2020 2020 2020 2020 225a                "Z
+000116f0: 656e 6974 7920 7265 7475 726e 6564 2063  enity returned c
+00011700: 6f64 6520 2572 2061 6e64 2073 7464 6572  ode %r and stder
+00011710: 7220 2572 222c 2072 6573 756c 742e 7265  r %r", result.re
+00011720: 7475 726e 636f 6465 2c20 7265 7375 6c74  turncode, result
+00011730: 2e73 7464 6572 720a 2020 2020 2020 2020  .stderr.        
+00011740: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00011750: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
+00011760: 6465 6620 5f6f 7074 696f 6e73 5f74 6f5f  def _options_to_
+00011770: 7a65 6e69 7479 5f66 696c 656e 616d 6528  zenity_filename(
+00011780: 6f70 7469 6f6e 7329 3a0a 2020 2020 6966  options):.    if
+00011790: 206f 7074 696f 6e73 2e67 6574 2822 696e   options.get("in
+000117a0: 6974 6961 6c64 6972 2229 3a0a 2020 2020  itialdir"):.    
+000117b0: 2020 2020 6966 206f 7074 696f 6e73 2e67      if options.g
+000117c0: 6574 2822 696e 6974 6961 6c66 696c 6522  et("initialfile"
+000117d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000117e0: 6574 7572 6e20 6f73 2e70 6174 682e 6a6f  eturn os.path.jo
+000117f0: 696e 286f 7074 696f 6e73 5b22 696e 6974  in(options["init
+00011800: 6961 6c64 6972 225d 2c20 6f70 7469 6f6e  ialdir"], option
+00011810: 735b 2269 6e69 7469 616c 6669 6c65 225d  s["initialfile"]
+00011820: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00011830: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011840: 726e 206f 7074 696f 6e73 5b22 696e 6974  rn options["init
+00011850: 6961 6c64 6972 225d 202b 206f 732e 7061  ialdir"] + os.pa
+00011860: 7468 2e73 6570 0a0a 2020 2020 7265 7475  th.sep..    retu
+00011870: 726e 204e 6f6e 650a 0a0a 6465 6620 7265  rn None...def re
+00011880: 6769 7374 6572 5f6c 6174 696e 5f73 686f  gister_latin_sho
+00011890: 7274 6375 7428 0a20 2020 2072 6567 6973  rtcut(.    regis
+000118a0: 7472 792c 2073 6571 7565 6e63 653a 2073  try, sequence: s
+000118b0: 7472 2c20 6861 6e64 6c65 723a 2043 616c  tr, handler: Cal
+000118c0: 6c61 626c 652c 2074 6573 7465 723a 204f  lable, tester: O
+000118d0: 7074 696f 6e61 6c5b 4361 6c6c 6162 6c65  ptional[Callable
+000118e0: 5d0a 2920 2d3e 204e 6f6e 653a 0a20 2020  ].) -> None:.   
+000118f0: 2072 6573 203d 2073 6571 7565 6e63 655f   res = sequence_
+00011900: 746f 5f65 7665 6e74 5f73 7461 7465 5f61  to_event_state_a
+00011910: 6e64 5f6b 6579 636f 6465 2873 6571 7565  nd_keycode(seque
+00011920: 6e63 6529 0a20 2020 2069 6620 7265 7320  nce).    if res 
+00011930: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00011940: 2020 2020 2069 6620 7265 7320 6e6f 7420       if res not 
+00011950: 696e 2072 6567 6973 7472 793a 0a20 2020  in registry:.   
+00011960: 2020 2020 2020 2020 2072 6567 6973 7472           registr
+00011970: 795b 7265 735d 203d 205b 5d0a 2020 2020  y[res] = [].    
+00011980: 2020 2020 7265 6769 7374 7279 5b72 6573      registry[res
+00011990: 5d2e 6170 7065 6e64 2828 6861 6e64 6c65  ].append((handle
+000119a0: 722c 2074 6573 7465 7229 290a 0a0a 6465  r, tester))...de
+000119b0: 6620 6861 6e64 6c65 5f6d 6973 7472 6561  f handle_mistrea
+000119c0: 7465 645f 6c61 7469 6e5f 7368 6f72 7463  ted_latin_shortc
+000119d0: 7574 7328 7265 6769 7374 7279 2c20 6576  uts(registry, ev
+000119e0: 656e 7429 3a0a 2020 2020 2320 7472 6965  ent):.    # trie
+000119f0: 7320 746f 2068 616e 646c 6520 4374 726c  s to handle Ctrl
+00011a00: 2b4c 6174 696e 4c65 7474 6572 2073 686f  +LatinLetter sho
+00011a10: 7274 6375 7473 0a20 2020 2023 2067 6976  rtcuts.    # giv
+00011a20: 656e 2066 726f 6d20 6e6f 6e2d 4c61 7469  en from non-Lati
+00011a30: 6e20 6b65 7962 6f61 7264 730a 2020 2020  n keyboards.    
+00011a40: 2320 5365 653a 2068 7474 7073 3a2f 2f62  # See: https://b
+00011a50: 6974 6275 636b 6574 2e6f 7267 2f70 6c61  itbucket.org/pla
+00011a60: 732f 7468 6f6e 6e79 2f69 7373 7565 732f  s/thonny/issues/
+00011a70: 3432 322f 6564 6974 2d6b 6579 626f 6172  422/edit-keyboar
+00011a80: 642d 7368 6f72 7463 7574 732d 6374 726c  d-shortcuts-ctrl
+00011a90: 2d63 2d63 7472 6c2d 762d 6574 630a 0a20  -c-ctrl-v-etc.. 
+00011aa0: 2020 2023 206f 6e6c 7920 636f 6e73 6964     # only consid
+00011ab0: 6572 2065 7665 6e74 7320 7769 7468 2043  er events with C
+00011ac0: 6f6e 7472 6f6c 2068 656c 640a 2020 2020  ontrol held.    
+00011ad0: 6966 206e 6f74 2065 7665 6e74 2e73 7461  if not event.sta
+00011ae0: 7465 2026 2030 7830 343a 0a20 2020 2020  te & 0x04:.     
+00011af0: 2020 2072 6574 7572 6e0a 0a20 2020 2069     return..    i
+00011b00: 6620 7275 6e6e 696e 675f 6f6e 5f6d 6163  f running_on_mac
+00011b10: 5f6f 7328 293a 0a20 2020 2020 2020 2072  _os():.        r
+00011b20: 6574 7572 6e0a 0a20 2020 2023 2063 6f6e  eturn..    # con
+00011b30: 7369 6465 7220 6f6e 6c79 2070 6172 7420  sider only part 
+00011b40: 6f66 2074 6865 2073 7461 7465 2c0a 2020  of the state,.  
+00011b50: 2020 2320 6265 6361 7573 6520 6174 206c    # because at l
+00011b60: 6561 7374 206f 6e20 5769 6e64 6f77 732c  east on Windows,
+00011b70: 2043 7472 6c2d 7368 6f72 7463 7574 7327   Ctrl-shortcuts'
+00011b80: 2073 7461 7465 0a20 2020 2023 2068 6173   state.    # has
+00011b90: 2073 6f6d 6574 6869 6e67 2065 7874 7261   something extra
+00011ba0: 0a20 2020 2073 696d 706c 6966 6965 645f  .    simplified_
+00011bb0: 7374 6174 6520 3d20 3078 3034 0a20 2020  state = 0x04.   
+00011bc0: 2069 6620 7368 6966 745f 6973 5f70 7265   if shift_is_pre
+00011bd0: 7373 6564 2865 7665 6e74 293a 0a20 2020  ssed(event):.   
+00011be0: 2020 2020 2073 696d 706c 6966 6965 645f       simplified_
+00011bf0: 7374 6174 6520 7c3d 2030 7830 310a 0a20  state |= 0x01.. 
+00011c00: 2020 2023 2070 7269 6e74 2873 696d 706c     # print(simpl
+00011c10: 6966 6965 645f 7374 6174 652c 2065 7665  ified_state, eve
+00011c20: 6e74 2e6b 6579 636f 6465 290a 2020 2020  nt.keycode).    
+00011c30: 6966 2028 7369 6d70 6c69 6669 6564 5f73  if (simplified_s
+00011c40: 7461 7465 2c20 6576 656e 742e 6b65 7963  tate, event.keyc
+00011c50: 6f64 6529 2069 6e20 7265 6769 7374 7279  ode) in registry
+00011c60: 3a0a 2020 2020 2020 2020 6966 2065 7665  :.        if eve
+00011c70: 6e74 2e6b 6579 636f 6465 2021 3d20 6f72  nt.keycode != or
+00011c80: 6428 6576 656e 742e 6368 6172 2920 616e  d(event.char) an
+00011c90: 6420 6576 656e 742e 6b65 7973 796d 2069  d event.keysym i
+00011ca0: 6e20 284e 6f6e 652c 2022 3f3f 2229 3a0a  n (None, "??"):.
+00011cb0: 2020 2020 2020 2020 2020 2020 2320 6b65              # ke
+00011cc0: 7963 6f64 6520 616e 6420 6368 6172 2064  ycode and char d
+00011cd0: 6f65 736e 2774 206d 6174 6368 2c0a 2020  oesn't match,.  
+00011ce0: 2020 2020 2020 2020 2020 2320 7468 6973            # this
+00011cf0: 206d 6561 6e73 206e 6f6e 2d6c 6174 696e   means non-latin
+00011d00: 206b 6579 626f 6172 640a 2020 2020 2020   keyboard.      
+00011d10: 2020 2020 2020 666f 7220 6861 6e64 6c65        for handle
+00011d20: 722c 2074 6573 7465 7220 696e 2072 6567  r, tester in reg
+00011d30: 6973 7472 795b 2873 696d 706c 6966 6965  istry[(simplifie
+00011d40: 645f 7374 6174 652c 2065 7665 6e74 2e6b  d_state, event.k
+00011d50: 6579 636f 6465 295d 3a0a 2020 2020 2020  eycode)]:.      
+00011d60: 2020 2020 2020 2020 2020 6966 2074 6573            if tes
+00011d70: 7465 7220 6973 204e 6f6e 6520 6f72 2074  ter is None or t
+00011d80: 6573 7465 7228 293a 0a20 2020 2020 2020  ester():.       
+00011d90: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00011da0: 646c 6572 2829 0a0a 0a64 6566 2073 686f  dler()...def sho
+00011db0: 775f 6469 616c 6f67 2864 6c67 2c20 6d61  w_dialog(dlg, ma
+00011dc0: 7374 6572 3d4e 6f6e 652c 2077 6964 7468  ster=None, width
+00011dd0: 3d4e 6f6e 652c 2068 6569 6768 743d 4e6f  =None, height=No
+00011de0: 6e65 2c20 6d6f 6461 6c3d 5472 7565 293a  ne, modal=True):
+00011df0: 0a20 2020 2069 6620 6765 7461 7474 7228  .    if getattr(
+00011e00: 646c 672c 2022 636c 6f73 6564 222c 2046  dlg, "closed", F
+00011e10: 616c 7365 293a 0a20 2020 2020 2020 2072  alse):.        r
+00011e20: 6574 7572 6e0a 0a20 2020 2069 6620 6d61  eturn..    if ma
+00011e30: 7374 6572 2069 7320 4e6f 6e65 3a0a 2020  ster is None:.  
+00011e40: 2020 2020 2020 6d61 7374 6572 203d 2067        master = g
+00011e50: 6574 6174 7472 2864 6c67 2c20 2270 6172  etattr(dlg, "par
+00011e60: 656e 7422 2c20 4e6f 6e65 2920 6f72 2067  ent", None) or g
+00011e70: 6574 6174 7472 2864 6c67 2c20 226d 6173  etattr(dlg, "mas
+00011e80: 7465 7222 2c20 4e6f 6e65 2920 6f72 2074  ter", None) or t
+00011e90: 6b2e 5f64 6566 6175 6c74 5f72 6f6f 740a  k._default_root.
+00011ea0: 0a20 2020 206d 6173 7465 7220 3d20 6d61  .    master = ma
+00011eb0: 7374 6572 2e77 696e 666f 5f74 6f70 6c65  ster.winfo_tople
+00011ec0: 7665 6c28 290a 0a20 2020 2067 6574 5f77  vel()..    get_w
+00011ed0: 6f72 6b62 656e 6368 2829 2e65 7665 6e74  orkbench().event
+00011ee0: 5f67 656e 6572 6174 6528 2257 696e 646f  _generate("Windo
+00011ef0: 7746 6f63 7573 4f75 7422 290a 2020 2020  wFocusOut").    
+00011f00: 2320 666f 6c6c 6f77 696e 6720 6f72 6465  # following orde
+00011f10: 7220 7365 656d 7320 746f 2067 6976 6520  r seems to give 
+00011f20: 6d6f 7374 2073 6d6f 6f74 6820 6170 7065  most smooth appe
+00011f30: 6172 616e 6365 0a20 2020 206f 6c64 5f66  arance.    old_f
+00011f40: 6f63 7573 6564 5f77 6964 6765 7420 3d20  ocused_widget = 
+00011f50: 6d61 7374 6572 2e66 6f63 7573 5f67 6574  master.focus_get
+00011f60: 2829 0a20 2020 2069 6620 6d61 7374 6572  ().    if master
+00011f70: 2e77 696e 666f 5f74 6f70 6c65 7665 6c28  .winfo_toplevel(
+00011f80: 292e 7769 6e66 6f5f 7669 6577 6162 6c65  ).winfo_viewable
+00011f90: 2829 3a0a 2020 2020 2020 2020 646c 672e  ():.        dlg.
+00011fa0: 7472 616e 7369 656e 7428 6d61 7374 6572  transient(master
+00011fb0: 2e77 696e 666f 5f74 6f70 6c65 7665 6c28  .winfo_toplevel(
+00011fc0: 2929 0a0a 2020 2020 7361 7665 645f 7369  ))..    saved_si
+00011fd0: 7a65 203d 2067 6574 5f77 6f72 6b62 656e  ze = get_workben
+00011fe0: 6368 2829 2e67 6574 5f6f 7074 696f 6e28  ch().get_option(
+00011ff0: 6765 745f 7369 7a65 5f6f 7074 696f 6e5f  get_size_option_
+00012000: 6e61 6d65 2864 6c67 2929 0a20 2020 2069  name(dlg)).    i
+00012010: 6620 7361 7665 645f 7369 7a65 3a0a 2020  f saved_size:.  
+00012020: 2020 2020 2020 7769 6474 6820 3d20 6d69        width = mi
+00012030: 6e28 6d61 7828 7361 7665 645f 7369 7a65  n(max(saved_size
+00012040: 5b30 5d2c 2065 6d73 5f74 6f5f 7069 7865  [0], ems_to_pixe
+00012050: 6c73 2831 3029 292c 2065 6d73 5f74 6f5f  ls(10)), ems_to_
+00012060: 7069 7865 6c73 2835 3030 2929 0a20 2020  pixels(500)).   
+00012070: 2020 2020 2068 6569 6768 7420 3d20 6d69       height = mi
+00012080: 6e28 6d61 7828 7361 7665 645f 7369 7a65  n(max(saved_size
+00012090: 5b31 5d2c 2065 6d73 5f74 6f5f 7069 7865  [1], ems_to_pixe
+000120a0: 6c73 2838 2929 2c20 656d 735f 746f 5f70  ls(8)), ems_to_p
+000120b0: 6978 656c 7328 3330 3029 290a 0a20 2020  ixels(300))..   
+000120c0: 205f 706c 6163 655f 7769 6e64 6f77 2864   _place_window(d
+000120d0: 6c67 2c20 6d61 7374 6572 2c20 7769 6474  lg, master, widt
+000120e0: 683d 7769 6474 682c 2068 6569 6768 743d  h=width, height=
+000120f0: 6865 6967 6874 290a 0a20 2020 2064 6c67  height)..    dlg
+00012100: 2e6c 6966 7428 290a 2020 2020 646c 672e  .lift().    dlg.
+00012110: 7761 6974 5f76 6973 6962 696c 6974 7928  wait_visibility(
+00012120: 290a 0a20 2020 2069 6620 6d6f 6461 6c3a  )..    if modal:
+00012130: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00012140: 2020 2020 2020 2020 2020 646c 672e 6772            dlg.gr
+00012150: 6162 5f73 6574 2829 0a20 2020 2020 2020  ab_set().       
+00012160: 2065 7863 6570 7420 5463 6c45 7272 6f72   except TclError
+00012170: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00012180: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+00012190: 6728 2243 616e 2774 2067 7261 623a 2025  g("Can't grab: %
+000121a0: 7322 2c20 6529 0a0a 2020 2020 646c 672e  s", e)..    dlg.
+000121b0: 7570 6461 7465 5f69 646c 6574 6173 6b73  update_idletasks
+000121c0: 2829 0a20 2020 2064 6c67 2e66 6f63 7573  ().    dlg.focus
+000121d0: 5f73 6574 2829 0a20 2020 2069 6620 6861  _set().    if ha
+000121e0: 7361 7474 7228 646c 672c 2022 7365 745f  sattr(dlg, "set_
+000121f0: 696e 6974 6961 6c5f 666f 6375 7322 293a  initial_focus"):
+00012200: 0a20 2020 2020 2020 2064 6c67 2e73 6574  .        dlg.set
+00012210: 5f69 6e69 7469 616c 5f66 6f63 7573 2829  _initial_focus()
+00012220: 0a0a 2020 2020 646c 672e 7761 6974 5f77  ..    dlg.wait_w
+00012230: 696e 646f 7728 646c 6729 0a20 2020 2064  indow(dlg).    d
+00012240: 6c67 2e67 7261 625f 7265 6c65 6173 6528  lg.grab_release(
+00012250: 290a 2020 2020 6d61 7374 6572 2e77 696e  ).    master.win
+00012260: 666f 5f74 6f70 6c65 7665 6c28 292e 6c69  fo_toplevel().li
+00012270: 6674 2829 0a20 2020 206d 6173 7465 722e  ft().    master.
+00012280: 7769 6e66 6f5f 746f 706c 6576 656c 2829  winfo_toplevel()
+00012290: 2e66 6f63 7573 5f66 6f72 6365 2829 0a20  .focus_force(). 
+000122a0: 2020 206d 6173 7465 722e 7769 6e66 6f5f     master.winfo_
+000122b0: 746f 706c 6576 656c 2829 2e67 7261 625f  toplevel().grab_
+000122c0: 7365 7428 290a 2020 2020 6966 2072 756e  set().    if run
+000122d0: 6e69 6e67 5f6f 6e5f 6d61 635f 6f73 2829  ning_on_mac_os()
+000122e0: 3a0a 2020 2020 2020 2020 6d61 7374 6572  :.        master
+000122f0: 2e77 696e 666f 5f74 6f70 6c65 7665 6c28  .winfo_toplevel(
+00012300: 292e 6772 6162 5f72 656c 6561 7365 2829  ).grab_release()
+00012310: 0a0a 2020 2020 6966 206f 6c64 5f66 6f63  ..    if old_foc
+00012320: 7573 6564 5f77 6964 6765 7420 6973 206e  used_widget is n
+00012330: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00012340: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00012350: 2020 6f6c 645f 666f 6375 7365 645f 7769    old_focused_wi
+00012360: 6467 6574 2e66 6f63 7573 5f66 6f72 6365  dget.focus_force
+00012370: 2829 0a20 2020 2020 2020 2065 7863 6570  ().        excep
+00012380: 7420 5463 6c45 7272 6f72 3a0a 2020 2020  t TclError:.    
+00012390: 2020 2020 2020 2020 7061 7373 0a0a 0a64          pass...d
+000123a0: 6566 2070 6f70 656e 5f77 6974 685f 7569  ef popen_with_ui
+000123b0: 5f74 6872 6561 645f 6361 6c6c 6261 636b  _thread_callback
+000123c0: 282a 506f 7065 6e5f 6172 6773 2c20 6f6e  (*Popen_args, on
+000123d0: 5f63 6f6d 706c 6574 696f 6e2c 2070 6f6c  _completion, pol
+000123e0: 6c5f 6465 6c61 793d 302e 312c 202a 2a50  l_delay=0.1, **P
+000123f0: 6f70 656e 5f6b 7761 7267 7329 3a0a 2020  open_kwargs):.  
+00012400: 2020 6966 2022 656e 636f 6469 6e67 2220    if "encoding" 
+00012410: 6e6f 7420 696e 2050 6f70 656e 5f6b 7761  not in Popen_kwa
+00012420: 7267 733a 0a20 2020 2020 2020 2069 6620  rgs:.        if 
+00012430: 2265 6e76 2220 6e6f 7420 696e 2050 6f70  "env" not in Pop
+00012440: 656e 5f6b 7761 7267 733a 0a20 2020 2020  en_kwargs:.     
+00012450: 2020 2020 2020 2050 6f70 656e 5f6b 7761         Popen_kwa
+00012460: 7267 735b 2265 6e76 225d 203d 206f 732e  rgs["env"] = os.
+00012470: 656e 7669 726f 6e2e 636f 7079 2829 0a20  environ.copy(). 
+00012480: 2020 2020 2020 2050 6f70 656e 5f6b 7761         Popen_kwa
+00012490: 7267 735b 2265 6e76 225d 5b22 5059 5448  rgs["env"]["PYTH
+000124a0: 4f4e 494f 454e 434f 4449 4e47 225d 203d  ONIOENCODING"] =
+000124b0: 2022 7574 662d 3822 0a20 2020 2020 2020   "utf-8".       
+000124c0: 2069 6620 7379 732e 7665 7273 696f 6e5f   if sys.version_
+000124d0: 696e 666f 203e 3d20 2833 2c20 3629 3a0a  info >= (3, 6):.
+000124e0: 2020 2020 2020 2020 2020 2020 506f 7065              Pope
+000124f0: 6e5f 6b77 6172 6773 5b22 656e 636f 6469  n_kwargs["encodi
+00012500: 6e67 225d 203d 2022 7574 662d 3822 0a0a  ng"] = "utf-8"..
+00012510: 2020 2020 7072 6f63 203d 2073 7562 7072      proc = subpr
+00012520: 6f63 6573 732e 506f 7065 6e28 2a50 6f70  ocess.Popen(*Pop
+00012530: 656e 5f61 7267 732c 202a 2a50 6f70 656e  en_args, **Popen
+00012540: 5f6b 7761 7267 7329 0a0a 2020 2020 2320  _kwargs)..    # 
+00012550: 4e65 6564 2074 6f20 7265 6164 2069 6e20  Need to read in 
+00012560: 7468 7265 6164 2069 6e20 6f72 6465 7220  thread in order 
+00012570: 746f 2061 766f 6964 2062 6c6f 636b 696e  to avoid blockin
+00012580: 6720 6265 6361 7573 650a 2020 2020 2320  g because.    # 
+00012590: 6f66 2066 756c 6c20 7069 7065 2062 7566  of full pipe buf
+000125a0: 6665 7220 2873 6565 2068 7474 7073 3a2f  fer (see https:/
+000125b0: 2f62 7567 732e 7079 7468 6f6e 2e6f 7267  /bugs.python.org
+000125c0: 2f69 7373 7565 3132 3536 290a 2020 2020  /issue1256).    
+000125d0: 6f75 745f 6c69 6e65 7320 3d20 5b5d 0a20  out_lines = []. 
+000125e0: 2020 2065 7272 5f6c 696e 6573 203d 205b     err_lines = [
+000125f0: 5d0a 0a20 2020 2064 6566 2072 6561 645f  ]..    def read_
+00012600: 7374 7265 616d 2873 7472 6561 6d2c 2074  stream(stream, t
+00012610: 6172 6765 745f 6c69 7374 293a 0a20 2020  arget_list):.   
+00012620: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
+00012630: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+00012640: 6520 3d20 7374 7265 616d 2e72 6561 646c  e = stream.readl
+00012650: 696e 6528 290a 2020 2020 2020 2020 2020  ine().          
+00012660: 2020 6966 206c 696e 653a 0a20 2020 2020    if line:.     
+00012670: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00012680: 745f 6c69 7374 2e61 7070 656e 6428 6c69  t_list.append(li
+00012690: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+000126a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000126b0: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
+000126c0: 2074 5f6f 7574 203d 2074 6872 6561 6469   t_out = threadi
+000126d0: 6e67 2e54 6872 6561 6428 7461 7267 6574  ng.Thread(target
+000126e0: 3d72 6561 645f 7374 7265 616d 2c20 6461  =read_stream, da
+000126f0: 656d 6f6e 3d54 7275 652c 2061 7267 733d  emon=True, args=
+00012700: 2870 726f 632e 7374 646f 7574 2c20 6f75  (proc.stdout, ou
+00012710: 745f 6c69 6e65 7329 290a 2020 2020 745f  t_lines)).    t_
+00012720: 6572 7220 3d20 7468 7265 6164 696e 672e  err = threading.
+00012730: 5468 7265 6164 2874 6172 6765 743d 7265  Thread(target=re
+00012740: 6164 5f73 7472 6561 6d2c 2064 6165 6d6f  ad_stream, daemo
+00012750: 6e3d 5472 7565 2c20 6172 6773 3d28 7072  n=True, args=(pr
+00012760: 6f63 2e73 7464 6572 722c 2065 7272 5f6c  oc.stderr, err_l
+00012770: 696e 6573 2929 0a20 2020 2074 5f6f 7574  ines)).    t_out
+00012780: 2e73 7461 7274 2829 0a20 2020 2074 5f65  .start().    t_e
+00012790: 7272 2e73 7461 7274 2829 0a0a 2020 2020  rr.start()..    
+000127a0: 6465 6620 706f 6c6c 2829 3a0a 2020 2020  def poll():.    
+000127b0: 2020 2020 6966 2070 726f 632e 706f 6c6c      if proc.poll
+000127c0: 2829 2069 7320 6e6f 7420 4e6f 6e65 3a0a  () is not None:.
+000127d0: 2020 2020 2020 2020 2020 2020 745f 6f75              t_ou
+000127e0: 742e 6a6f 696e 2833 290a 2020 2020 2020  t.join(3).      
+000127f0: 2020 2020 2020 745f 6572 722e 6a6f 696e        t_err.join
+00012800: 2833 290a 2020 2020 2020 2020 2020 2020  (3).            
+00012810: 6f6e 5f63 6f6d 706c 6574 696f 6e28 7072  on_completion(pr
+00012820: 6f63 2c20 6f75 745f 6c69 6e65 732c 2065  oc, out_lines, e
+00012830: 7272 5f6c 696e 6573 290a 2020 2020 2020  rr_lines).      
+00012840: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00012850: 2020 2020 2020 746b 2e5f 6465 6661 756c        tk._defaul
+00012860: 745f 726f 6f74 2e61 6674 6572 2869 6e74  t_root.after(int
+00012870: 2870 6f6c 6c5f 6465 6c61 7920 2a20 3130  (poll_delay * 10
+00012880: 3030 292c 2070 6f6c 6c29 0a0a 2020 2020  00), poll)..    
+00012890: 706f 6c6c 2829 0a20 2020 2072 6574 7572  poll().    retur
+000128a0: 6e20 7072 6f63 0a0a 0a63 6c61 7373 204d  n proc...class M
+000128b0: 656e 7545 7828 746b 2e4d 656e 7529 3a0a  enuEx(tk.Menu):.
+000128c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000128d0: 2873 656c 662c 2074 6172 6765 7429 3a0a  (self, target):.
+000128e0: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+000128f0: 7374 6572 7320 3d20 7b7d 0a20 2020 2020  sters = {}.     
+00012900: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00012910: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
+00012920: 2074 6172 6765 742c 2074 6561 726f 6666   target, tearoff
+00012930: 3d46 616c 7365 2c20 706f 7374 636f 6d6d  =False, postcomm
+00012940: 616e 643d 7365 6c66 2e6f 6e5f 706f 7374  and=self.on_post
+00012950: 2c20 2a2a 6765 745f 7374 796c 655f 636f  , **get_style_co
+00012960: 6e66 6967 7572 6174 696f 6e28 224d 656e  nfiguration("Men
+00012970: 7522 290a 2020 2020 2020 2020 290a 0a20  u").        ).. 
+00012980: 2020 2064 6566 206f 6e5f 706f 7374 2873     def on_post(s
+00012990: 656c 662c 202a 6172 6773 293a 0a20 2020  elf, *args):.   
+000129a0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+000129b0: 5f69 7465 6d5f 6176 6169 6c61 6269 6c69  _item_availabili
+000129c0: 7479 2829 0a0a 2020 2020 6465 6620 7570  ty()..    def up
+000129d0: 6461 7465 5f69 7465 6d5f 6176 6169 6c61  date_item_availa
+000129e0: 6269 6c69 7479 2873 656c 6629 3a0a 2020  bility(self):.  
+000129f0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00012a00: 616e 6765 2873 656c 662e 696e 6465 7828  ange(self.index(
+00012a10: 2265 6e64 2229 202b 2031 293a 0a20 2020  "end") + 1):.   
+00012a20: 2020 2020 2020 2020 2069 7465 6d5f 6461           item_da
+00012a30: 7461 203d 2073 656c 662e 656e 7472 7963  ta = self.entryc
+00012a40: 6f6e 6669 6775 7265 2869 290a 2020 2020  onfigure(i).    
+00012a50: 2020 2020 2020 2020 6966 2022 6c61 6265          if "labe
+00012a60: 6c22 2069 6e20 6974 656d 5f64 6174 613a  l" in item_data:
+00012a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a80: 2074 6573 7465 7220 3d20 7365 6c66 2e5f   tester = self._
+00012a90: 7465 7374 6572 732e 6765 7428 6974 656d  testers.get(item
+00012aa0: 5f64 6174 615b 226c 6162 656c 225d 290a  _data["label"]).
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 6966 2074 6573 7465 7220 616e 6420 6e6f  if tester and no
+00012ad0: 7420 7465 7374 6572 2829 3a0a 2020 2020  t tester():.    
 00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 2020 7365 6c66 2e65 6e74 7279 636f 6e66    self.entryconf
-00012b00: 6967 7572 6528 692c 2073 7461 7465 3d74  igure(i, state=t
-00012b10: 6b2e 4449 5341 424c 4544 290a 2020 2020  k.DISABLED).    
-00012b20: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00012b30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012b40: 2020 2020 2020 7365 6c66 2e65 6e74 7279        self.entry
-00012b50: 636f 6e66 6967 7572 6528 692c 2073 7461  configure(i, sta
-00012b60: 7465 3d74 6b2e 4e4f 524d 414c 290a 0a20  te=tk.NORMAL).. 
-00012b70: 2020 2064 6566 2061 6464 2873 656c 662c     def add(self,
-00012b80: 2069 7465 6d54 7970 652c 2063 6e66 3d7b   itemType, cnf={
-00012b90: 7d2c 202a 2a6b 7729 3a0a 2020 2020 2020  }, **kw):.      
-00012ba0: 2020 636e 6620 3d20 636e 6620 6f72 206b    cnf = cnf or k
-00012bb0: 770a 2020 2020 2020 2020 7465 7374 6572  w.        tester
-00012bc0: 203d 2063 6e66 2e67 6574 2822 7465 7374   = cnf.get("test
-00012bd0: 6572 2229 0a20 2020 2020 2020 2069 6620  er").        if 
-00012be0: 2274 6573 7465 7222 2069 6e20 636e 663a  "tester" in cnf:
-00012bf0: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-00012c00: 2063 6e66 5b22 7465 7374 6572 225d 0a0a   cnf["tester"]..
-00012c10: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00012c20: 6164 6428 6974 656d 5479 7065 2c20 636e  add(itemType, cn
-00012c30: 6629 0a0a 2020 2020 2020 2020 6974 656d  f)..        item
-00012c40: 6461 7461 203d 2073 656c 662e 656e 7472  data = self.entr
-00012c50: 7963 6f6e 6669 6775 7265 2873 656c 662e  yconfigure(self.
-00012c60: 696e 6465 7828 2265 6e64 2229 290a 2020  index("end")).  
-00012c70: 2020 2020 2020 6c61 6265 6c64 6174 6120        labeldata 
-00012c80: 3d20 6974 656d 6461 7461 2e67 6574 2822  = itemdata.get("
-00012c90: 6c61 6265 6c22 290a 2020 2020 2020 2020  label").        
-00012ca0: 6966 206c 6162 656c 6461 7461 3a0a 2020  if labeldata:.  
-00012cb0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00012cc0: 7465 7374 6572 735b 6c61 6265 6c64 6174  testers[labeldat
-00012cd0: 615d 203d 2074 6573 7465 720a 0a0a 636c  a] = tester...cl
-00012ce0: 6173 7320 5465 7874 4d65 6e75 284d 656e  ass TextMenu(Men
-00012cf0: 7545 7829 3a0a 2020 2020 6465 6620 5f5f  uEx):.    def __
-00012d00: 696e 6974 5f5f 2873 656c 662c 2074 6172  init__(self, tar
-00012d10: 6765 7429 3a0a 2020 2020 2020 2020 7365  get):.        se
-00012d20: 6c66 2e74 6578 7420 3d20 7461 7267 6574  lf.text = target
-00012d30: 0a20 2020 2020 2020 204d 656e 7545 782e  .        MenuEx.
-00012d40: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
-00012d50: 6172 6765 7429 0a20 2020 2020 2020 2073  arget).        s
-00012d60: 656c 662e 6164 645f 6261 7369 635f 6974  elf.add_basic_it
-00012d70: 656d 7328 290a 2020 2020 2020 2020 7365  ems().        se
-00012d80: 6c66 2e61 6464 5f65 7874 7261 5f69 7465  lf.add_extra_ite
-00012d90: 6d73 2829 0a0a 2020 2020 6465 6620 6164  ms()..    def ad
-00012da0: 645f 6261 7369 635f 6974 656d 7328 7365  d_basic_items(se
-00012db0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00012dc0: 662e 6164 645f 636f 6d6d 616e 6428 6c61  f.add_command(la
-00012dd0: 6265 6c3d 7472 2822 4375 7422 292c 2063  bel=tr("Cut"), c
-00012de0: 6f6d 6d61 6e64 3d73 656c 662e 6f6e 5f63  ommand=self.on_c
-00012df0: 7574 2c20 7465 7374 6572 3d73 656c 662e  ut, tester=self.
-00012e00: 6361 6e5f 6375 7429 0a20 2020 2020 2020  can_cut).       
-00012e10: 2073 656c 662e 6164 645f 636f 6d6d 616e   self.add_comman
-00012e20: 6428 6c61 6265 6c3d 7472 2822 436f 7079  d(label=tr("Copy
-00012e30: 2229 2c20 636f 6d6d 616e 643d 7365 6c66  "), command=self
-00012e40: 2e6f 6e5f 636f 7079 2c20 7465 7374 6572  .on_copy, tester
-00012e50: 3d73 656c 662e 6361 6e5f 636f 7079 290a  =self.can_copy).
-00012e60: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-00012e70: 5f63 6f6d 6d61 6e64 286c 6162 656c 3d74  _command(label=t
-00012e80: 7228 2250 6173 7465 2229 2c20 636f 6d6d  r("Paste"), comm
-00012e90: 616e 643d 7365 6c66 2e6f 6e5f 7061 7374  and=self.on_past
-00012ea0: 652c 2074 6573 7465 723d 7365 6c66 2e63  e, tester=self.c
-00012eb0: 616e 5f70 6173 7465 290a 0a20 2020 2064  an_paste)..    d
-00012ec0: 6566 2061 6464 5f65 7874 7261 5f69 7465  ef add_extra_ite
-00012ed0: 6d73 2873 656c 6629 3a0a 2020 2020 2020  ms(self):.      
-00012ee0: 2020 7365 6c66 2e61 6464 5f73 6570 6172    self.add_separ
-00012ef0: 6174 6f72 2829 0a20 2020 2020 2020 2073  ator().        s
-00012f00: 656c 662e 6164 645f 636f 6d6d 616e 6428  elf.add_command(
-00012f10: 6c61 6265 6c3d 7472 2822 5365 6c65 6374  label=tr("Select
-00012f20: 2041 6c6c 2229 2c20 636f 6d6d 616e 643d   All"), command=
-00012f30: 7365 6c66 2e6f 6e5f 7365 6c65 6374 5f61  self.on_select_a
-00012f40: 6c6c 290a 0a20 2020 2064 6566 206f 6e5f  ll)..    def on_
-00012f50: 6375 7428 7365 6c66 293a 0a20 2020 2020  cut(self):.     
-00012f60: 2020 2073 656c 662e 7465 7874 2e65 7665     self.text.eve
-00012f70: 6e74 5f67 656e 6572 6174 6528 223c 3c43  nt_generate("<<C
-00012f80: 7574 3e3e 2229 0a0a 2020 2020 6465 6620  ut>>")..    def 
-00012f90: 6f6e 5f63 6f70 7928 7365 6c66 293a 0a20  on_copy(self):. 
-00012fa0: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00012fb0: 2e65 7665 6e74 5f67 656e 6572 6174 6528  .event_generate(
-00012fc0: 223c 3c43 6f70 793e 3e22 290a 0a20 2020  "<<Copy>>")..   
-00012fd0: 2064 6566 206f 6e5f 7061 7374 6528 7365   def on_paste(se
-00012fe0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00012ff0: 662e 7465 7874 2e65 7665 6e74 5f67 656e  f.text.event_gen
-00013000: 6572 6174 6528 223c 3c50 6173 7465 3e3e  erate("<<Paste>>
-00013010: 2229 0a0a 2020 2020 6465 6620 6f6e 5f73  ")..    def on_s
-00013020: 656c 6563 745f 616c 6c28 7365 6c66 293a  elect_all(self):
-00013030: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
-00013040: 7874 2e65 7665 6e74 5f67 656e 6572 6174  xt.event_generat
-00013050: 6528 223c 3c53 656c 6563 7441 6c6c 3e3e  e("<<SelectAll>>
-00013060: 2229 0a0a 2020 2020 6465 6620 6361 6e5f  ")..    def can_
-00013070: 6375 7428 7365 6c66 293a 0a20 2020 2020  cut(self):.     
-00013080: 2020 2072 6574 7572 6e20 7365 6c66 2e67     return self.g
-00013090: 6574 5f73 656c 6563 7465 645f 7465 7874  et_selected_text
-000130a0: 2829 2061 6e64 206e 6f74 2073 656c 662e  () and not self.
-000130b0: 7365 6c65 6374 696f 6e5f 6973 5f72 6561  selection_is_rea
-000130c0: 645f 6f6e 6c79 2829 0a0a 2020 2020 6465  d_only()..    de
-000130d0: 6620 6361 6e5f 636f 7079 2873 656c 6629  f can_copy(self)
-000130e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000130f0: 2073 656c 662e 6765 745f 7365 6c65 6374   self.get_select
-00013100: 6564 5f74 6578 7428 290a 0a20 2020 2064  ed_text()..    d
-00013110: 6566 2063 616e 5f70 6173 7465 2873 656c  ef can_paste(sel
-00013120: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00013130: 726e 206e 6f74 2073 656c 662e 7365 6c65  rn not self.sele
-00013140: 6374 696f 6e5f 6973 5f72 6561 645f 6f6e  ction_is_read_on
-00013150: 6c79 2829 0a0a 2020 2020 6465 6620 6765  ly()..    def ge
-00013160: 745f 7365 6c65 6374 6564 5f74 6578 7428  t_selected_text(
-00013170: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-00013180: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00013190: 7265 7475 726e 2073 656c 662e 7465 7874  return self.text
-000131a0: 2e67 6574 2822 7365 6c2e 6669 7273 7422  .get("sel.first"
-000131b0: 2c20 2273 656c 2e6c 6173 7422 290a 2020  , "sel.last").  
-000131c0: 2020 2020 2020 6578 6365 7074 2054 636c        except Tcl
-000131d0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-000131e0: 2020 2072 6574 7572 6e20 2222 0a0a 2020     return ""..  
-000131f0: 2020 6465 6620 7365 6c65 6374 696f 6e5f    def selection_
-00013200: 6973 5f72 6561 645f 6f6e 6c79 2873 656c  is_read_only(sel
-00013210: 6629 3a0a 2020 2020 2020 2020 6966 2068  f):.        if h
-00013220: 6173 6174 7472 2873 656c 662e 7465 7874  asattr(self.text
-00013230: 2c20 2269 735f 7265 6164 5f6f 6e6c 7922  , "is_read_only"
-00013240: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00013250: 6574 7572 6e20 7365 6c66 2e74 6578 742e  eturn self.text.
-00013260: 6973 5f72 6561 645f 6f6e 6c79 2829 0a0a  is_read_only()..
-00013270: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00013280: 616c 7365 0a0a 0a64 6566 2063 7265 6174  alse...def creat
-00013290: 655f 7572 6c5f 6c61 6265 6c28 6d61 7374  e_url_label(mast
-000132a0: 6572 2c20 7572 6c2c 2074 6578 743d 4e6f  er, url, text=No
-000132b0: 6e65 2c20 2a2a 6b77 293a 0a20 2020 2069  ne, **kw):.    i
-000132c0: 6d70 6f72 7420 7765 6262 726f 7773 6572  mport webbrowser
-000132d0: 0a0a 2020 2020 7265 7475 726e 2063 7265  ..    return cre
-000132e0: 6174 655f 6163 7469 6f6e 5f6c 6162 656c  ate_action_label
-000132f0: 286d 6173 7465 722c 2074 6578 7420 6f72  (master, text or
-00013300: 2075 726c 2c20 6c61 6d62 6461 205f 3a20   url, lambda _: 
-00013310: 7765 6262 726f 7773 6572 2e6f 7065 6e28  webbrowser.open(
-00013320: 7572 6c29 2c20 2a2a 6b77 290a 0a0a 6465  url), **kw)...de
-00013330: 6620 6372 6561 7465 5f61 6374 696f 6e5f  f create_action_
-00013340: 6c61 6265 6c28 6d61 7374 6572 2c20 7465  label(master, te
-00013350: 7874 2c20 636c 6963 6b5f 6861 6e64 6c65  xt, click_handle
-00013360: 722c 202a 2a6b 7729 3a0a 2020 2020 7572  r, **kw):.    ur
-00013370: 6c5f 666f 6e74 203d 2074 6b69 6e74 6572  l_font = tkinter
-00013380: 2e66 6f6e 742e 6e61 6d65 746f 666f 6e74  .font.nametofont
-00013390: 2822 546b 4465 6661 756c 7446 6f6e 7422  ("TkDefaultFont"
-000133a0: 292e 636f 7079 2829 0a20 2020 2075 726c  ).copy().    url
-000133b0: 5f66 6f6e 742e 636f 6e66 6967 7572 6528  _font.configure(
-000133c0: 756e 6465 726c 696e 653d 3129 0a20 2020  underline=1).   
-000133d0: 2075 726c 5f6c 6162 656c 203d 2074 746b   url_label = ttk
-000133e0: 2e4c 6162 656c 280a 2020 2020 2020 2020  .Label(.        
-000133f0: 6d61 7374 6572 2c20 7465 7874 3d74 6578  master, text=tex
-00013400: 742c 2073 7479 6c65 3d22 5572 6c2e 544c  t, style="Url.TL
-00013410: 6162 656c 222c 2063 7572 736f 723d 6765  abel", cursor=ge
-00013420: 745f 6879 7065 726c 696e 6b5f 6375 7273  t_hyperlink_curs
-00013430: 6f72 2829 2c20 666f 6e74 3d75 726c 5f66  or(), font=url_f
-00013440: 6f6e 742c 202a 2a6b 770a 2020 2020 290a  ont, **kw.    ).
-00013450: 2020 2020 7572 6c5f 6c61 6265 6c2e 6269      url_label.bi
-00013460: 6e64 2822 3c42 7574 746f 6e2d 313e 222c  nd("<Button-1>",
-00013470: 2063 6c69 636b 5f68 616e 646c 6572 290a   click_handler).
-00013480: 2020 2020 7265 7475 726e 2075 726c 5f6c      return url_l
-00013490: 6162 656c 0a0a 0a64 6566 2067 6574 5f73  abel...def get_s
-000134a0: 697a 655f 6f70 7469 6f6e 5f6e 616d 6528  ize_option_name(
-000134b0: 7769 6e64 6f77 293a 0a20 2020 2072 6574  window):.    ret
-000134c0: 7572 6e20 226c 6179 6f75 742e 2220 2b20  urn "layout." + 
-000134d0: 7479 7065 2877 696e 646f 7729 2e5f 5f6e  type(window).__n
-000134e0: 616d 655f 5f20 2b20 225f 7369 7a65 220a  ame__ + "_size".
-000134f0: 0a0a 6465 6620 6765 745f 6465 6661 756c  ..def get_defaul
-00013500: 745f 6261 7369 635f 7468 656d 6528 293a  t_basic_theme():
-00013510: 0a20 2020 2069 6620 7275 6e6e 696e 675f  .    if running_
-00013520: 6f6e 5f77 696e 646f 7773 2829 3a0a 2020  on_windows():.  
-00013530: 2020 2020 2020 7265 7475 726e 2022 7669        return "vi
-00013540: 7374 6122 0a20 2020 2065 6c73 653a 0a20  sta".    else:. 
-00013550: 2020 2020 2020 2072 6574 7572 6e20 2263         return "c
-00013560: 6c61 6d22 0a0a 0a45 4d5f 5749 4454 4820  lam"...EM_WIDTH 
-00013570: 3d20 4e6f 6e65 0a0a 0a64 6566 2065 6d73  = None...def ems
-00013580: 5f74 6f5f 7069 7865 6c73 2878 3a20 666c  _to_pixels(x: fl
-00013590: 6f61 7429 202d 3e20 696e 743a 0a20 2020  oat) -> int:.   
-000135a0: 2067 6c6f 6261 6c20 454d 5f57 4944 5448   global EM_WIDTH
-000135b0: 0a20 2020 2069 6620 454d 5f57 4944 5448  .    if EM_WIDTH
-000135c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000135d0: 2020 454d 5f57 4944 5448 203d 2074 6b69    EM_WIDTH = tki
-000135e0: 6e74 6572 2e66 6f6e 742e 6e61 6d65 746f  nter.font.nameto
-000135f0: 666f 6e74 2822 546b 4465 6661 756c 7446  font("TkDefaultF
-00013600: 6f6e 7422 292e 6d65 6173 7572 6528 226d  ont").measure("m
-00013610: 2229 0a20 2020 2072 6574 7572 6e20 696e  ").    return in
-00013620: 7428 454d 5f57 4944 5448 202a 2078 290a  t(EM_WIDTH * x).
-00013630: 0a0a 5f62 746e 5f70 6164 6469 6e67 203d  .._btn_padding =
-00013640: 204e 6f6e 650a 0a0a 6465 6620 7365 745f   None...def set_
-00013650: 7465 7874 5f69 665f 6469 6666 6572 656e  text_if_differen
-00013660: 7428 7769 6467 6574 2c20 7465 7874 2920  t(widget, text) 
-00013670: 2d3e 2062 6f6f 6c3a 0a20 2020 2069 6620  -> bool:.    if 
-00013680: 7769 6467 6574 5b22 7465 7874 225d 2021  widget["text"] !
-00013690: 3d20 7465 7874 3a0a 2020 2020 2020 2020  = text:.        
-000136a0: 7769 6467 6574 5b22 7465 7874 225d 203d  widget["text"] =
-000136b0: 2074 6578 740a 2020 2020 2020 2020 7265   text.        re
-000136c0: 7475 726e 2054 7275 650a 2020 2020 656c  turn True.    el
-000136d0: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-000136e0: 726e 2046 616c 7365 0a0a 0a64 6566 2074  rn False...def t
-000136f0: 725f 6274 6e28 7329 3a0a 2020 2020 2222  r_btn(s):.    ""
-00013700: 2254 7261 6e73 6c61 7465 7320 6275 7474  "Translates butt
-00013710: 6f6e 2063 6170 7469 6f6e 2c20 6164 6473  on caption, adds
-00013720: 2070 6164 6469 6e67 2074 6f20 6d61 6b65   padding to make
-00013730: 2073 7572 6520 7465 7874 2066 6974 7322   sure text fits"
-00013740: 2222 0a20 2020 2067 6c6f 6261 6c20 5f62  "".    global _b
-00013750: 746e 5f70 6164 6469 6e67 0a20 2020 2069  tn_padding.    i
-00013760: 6620 5f62 746e 5f70 6164 6469 6e67 2069  f _btn_padding i
-00013770: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00013780: 5f62 746e 5f70 6164 6469 6e67 203d 2067  _btn_padding = g
-00013790: 6574 5f62 7574 746f 6e5f 7061 6464 696e  et_button_paddin
-000137a0: 6728 290a 0a20 2020 2072 6574 7572 6e20  g()..    return 
-000137b0: 5f62 746e 5f70 6164 6469 6e67 202b 2074  _btn_padding + t
-000137c0: 7228 7329 202b 205f 6274 6e5f 7061 6464  r(s) + _btn_padd
-000137d0: 696e 670a 0a0a 6465 6620 6164 645f 6d65  ing...def add_me
-000137e0: 7373 6167 6562 6f78 5f70 6172 656e 745f  ssagebox_parent_
-000137f0: 6368 6563 6b65 7228 293a 0a20 2020 2064  checker():.    d
-00013800: 6566 2077 7261 705f 7769 7468 5f70 6172  ef wrap_with_par
-00013810: 656e 745f 6368 6563 6b65 7228 6f72 6967  ent_checker(orig
-00013820: 696e 616c 293a 0a20 2020 2020 2020 2064  inal):.        d
-00013830: 6566 2077 7261 7070 6572 282a 6172 6773  ef wrapper(*args
-00013840: 2c20 2a2a 6f70 7469 6f6e 7329 3a0a 2020  , **options):.  
-00013850: 2020 2020 2020 2020 2020 5f63 6865 636b            _check
-00013860: 5f64 6961 6c6f 675f 7061 7265 6e74 286f  _dialog_parent(o
-00013870: 7074 696f 6e73 290a 2020 2020 2020 2020  ptions).        
-00013880: 2020 2020 7265 7475 726e 206f 7269 6769      return origi
-00013890: 6e61 6c28 2a61 7267 732c 202a 2a6f 7074  nal(*args, **opt
-000138a0: 696f 6e73 290a 0a20 2020 2020 2020 2072  ions)..        r
-000138b0: 6574 7572 6e20 7772 6170 7065 720a 0a20  eturn wrapper.. 
-000138c0: 2020 2066 726f 6d20 746b 696e 7465 7220     from tkinter 
-000138d0: 696d 706f 7274 206d 6573 7361 6765 626f  import messagebo
-000138e0: 780a 0a20 2020 2066 6f72 206e 616d 6520  x..    for name 
-000138f0: 696e 205b 0a20 2020 2020 2020 2022 7368  in [.        "sh
-00013900: 6f77 696e 666f 222c 0a20 2020 2020 2020  owinfo",.       
-00013910: 2022 7368 6f77 7761 726e 696e 6722 2c0a   "showwarning",.
-00013920: 2020 2020 2020 2020 2273 686f 7765 7272          "showerr
-00013930: 6f72 222c 0a20 2020 2020 2020 2022 6173  or",.        "as
-00013940: 6b71 7565 7374 696f 6e22 2c0a 2020 2020  kquestion",.    
-00013950: 2020 2020 2261 736b 6f6b 6361 6e63 656c      "askokcancel
-00013960: 222c 0a20 2020 2020 2020 2022 6173 6b79  ",.        "asky
-00013970: 6573 6e6f 222c 0a20 2020 2020 2020 2022  esno",.        "
-00013980: 6173 6b79 6573 6e6f 6361 6e63 656c 222c  askyesnocancel",
-00013990: 0a20 2020 2020 2020 2022 6173 6b72 6574  .        "askret
-000139a0: 7279 6361 6e63 656c 222c 0a20 2020 205d  rycancel",.    ]
-000139b0: 3a0a 2020 2020 2020 2020 6675 6e20 3d20  :.        fun = 
-000139c0: 6765 7461 7474 7228 6d65 7373 6167 6562  getattr(messageb
-000139d0: 6f78 2c20 6e61 6d65 290a 2020 2020 2020  ox, name).      
-000139e0: 2020 7365 7461 7474 7228 6d65 7373 6167    setattr(messag
-000139f0: 6562 6f78 2c20 6e61 6d65 2c20 7772 6170  ebox, name, wrap
-00013a00: 5f77 6974 685f 7061 7265 6e74 5f63 6865  _with_parent_che
-00013a10: 636b 6572 2866 756e 2929 0a0a 0a64 6566  cker(fun))...def
-00013a20: 2072 6570 6c61 6365 5f75 6e73 7570 706f   replace_unsuppo
-00013a30: 7274 6564 5f63 6861 7273 2874 6578 743a  rted_chars(text:
-00013a40: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
-00013a50: 2020 6966 2067 6574 5f74 6b5f 7665 7273    if get_tk_vers
-00013a60: 696f 6e5f 696e 666f 2829 203c 2028 382c  ion_info() < (8,
-00013a70: 2036 2c20 3132 293a 0a20 2020 2020 2020   6, 12):.       
-00013a80: 2023 2063 616e 2063 7261 7368 2077 6974   # can crash wit
-00013a90: 6820 656d 6f6a 6973 0a20 2020 2020 2020  h emojis.       
-00013aa0: 2072 6574 7572 6e20 2222 2e6a 6f69 6e28   return "".join(
-00013ab0: 6320 6966 2063 203c 2022 5c55 3030 3031  c if c < "\U0001
-00013ac0: 3030 3030 2220 656c 7365 2022 e296 a122  0000" else "..."
-00013ad0: 2066 6f72 2063 2069 6e20 7465 7874 290a   for c in text).
-00013ae0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00013af0: 2020 7265 7475 726e 2074 6578 740a 0a0a    return text...
-00013b00: 6465 6620 7769 6e64 6f77 735f 6b6e 6f77  def windows_know
-00013b10: 6e5f 6578 7465 6e73 696f 6e73 5f61 7265  n_extensions_are
-00013b20: 5f68 6964 6465 6e28 2920 2d3e 2062 6f6f  _hidden() -> boo
-00013b30: 6c3a 0a20 2020 2061 7373 6572 7420 7275  l:.    assert ru
-00013b40: 6e6e 696e 675f 6f6e 5f77 696e 646f 7773  nning_on_windows
-00013b50: 2829 0a20 2020 2069 6d70 6f72 7420 7769  ().    import wi
-00013b60: 6e72 6567 0a0a 2020 2020 7265 675f 6b65  nreg..    reg_ke
-00013b70: 7920 3d20 7769 6e72 6567 2e4f 7065 6e4b  y = winreg.OpenK
-00013b80: 6579 280a 2020 2020 2020 2020 7769 6e72  ey(.        winr
-00013b90: 6567 2e48 4b45 595f 4355 5252 454e 545f  eg.HKEY_CURRENT_
-00013ba0: 5553 4552 2c0a 2020 2020 2020 2020 7222  USER,.        r"
-00013bb0: 534f 4654 5741 5245 5c4d 6963 726f 736f  SOFTWARE\Microso
-00013bc0: 6674 5c57 696e 646f 7773 5c43 7572 7265  ft\Windows\Curre
-00013bd0: 6e74 5665 7273 696f 6e5c 4578 706c 6f72  ntVersion\Explor
-00013be0: 6572 5c41 6476 616e 6365 6422 2c0a 2020  er\Advanced",.  
-00013bf0: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
-00013c00: 2077 696e 7265 672e 4b45 595f 5245 4144   winreg.KEY_READ
-00013c10: 2c0a 2020 2020 290a 2020 2020 7472 793a  ,.    ).    try:
-00013c20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013c30: 7769 6e72 6567 2e51 7565 7279 5661 6c75  winreg.QueryValu
-00013c40: 6545 7828 7265 675f 6b65 792c 2022 4869  eEx(reg_key, "Hi
-00013c50: 6465 4669 6c65 4578 7422 295b 305d 203d  deFileExt")[0] =
-00013c60: 3d20 310a 2020 2020 6669 6e61 6c6c 793a  = 1.    finally:
-00013c70: 0a20 2020 2020 2020 2072 6567 5f6b 6579  .        reg_key
-00013c80: 2e43 6c6f 7365 2829 0a0a 0a63 6c61 7373  .Close()...class
-00013c90: 204d 6170 7069 6e67 436f 6d62 6f62 6f78   MappingCombobox
-00013ca0: 2874 746b 2e43 6f6d 626f 626f 7829 3a0a  (ttk.Combobox):.
-00013cb0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00013cc0: 2873 656c 662c 206d 6173 7465 722c 206d  (self, master, m
-00013cd0: 6170 7069 6e67 3d4e 6f6e 652c 202a 2a6b  apping=None, **k
-00013ce0: 7729 3a0a 2020 2020 2020 2020 7375 7065  w):.        supe
-00013cf0: 7228 292e 5f5f 696e 6974 5f5f 286d 6173  r().__init__(mas
-00013d00: 7465 722c 202a 2a6b 7729 0a0a 2020 2020  ter, **kw)..    
-00013d10: 2020 2020 6966 206d 6170 7069 6e67 2069      if mapping i
-00013d20: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00013d30: 2020 2020 6d61 7070 696e 6720 3d20 7b7d      mapping = {}
-00013d40: 0a0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-00013d50: 6170 7069 6e67 3a20 4469 6374 5b73 7472  apping: Dict[str
-00013d60: 2c20 416e 795d 0a20 2020 2020 2020 2073  , Any].        s
-00013d70: 656c 662e 7365 745f 6d61 7070 696e 6728  elf.set_mapping(
-00013d80: 6d61 7070 696e 6729 0a20 2020 2020 2020  mapping).       
-00013d90: 2073 656c 662e 6d61 7070 696e 675f 6465   self.mapping_de
-00013da0: 7363 5f76 6172 6961 626c 6520 3d20 746b  sc_variable = tk
-00013db0: 2e53 7472 696e 6756 6172 2876 616c 7565  .StringVar(value
-00013dc0: 3d22 2229 0a20 2020 2020 2020 2073 656c  ="").        sel
-00013dd0: 662e 636f 6e66 6967 7572 6528 7465 7874  f.configure(text
-00013de0: 7661 7269 6162 6c65 3d73 656c 662e 6d61  variable=self.ma
-00013df0: 7070 696e 675f 6465 7363 5f76 6172 6961  pping_desc_varia
-00013e00: 626c 6529 0a0a 2020 2020 2020 2020 6966  ble)..        if
-00013e10: 206b 772e 6765 7428 2273 7461 7465 222c   kw.get("state",
-00013e20: 204e 6f6e 6529 203d 3d20 2264 6973 6162   None) == "disab
-00013e30: 6c65 6422 3a0a 2020 2020 2020 2020 2020  led":.          
-00013e40: 2020 7365 6c66 2e73 7461 7465 285b 2272    self.state(["r
-00013e50: 6561 646f 6e6c 7922 5d29 0a20 2020 2020  eadonly"]).     
-00013e60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00013e70: 2020 2020 2073 656c 662e 7374 6174 6528       self.state(
-00013e80: 5b22 2164 6973 6162 6c65 6422 2c20 2272  ["!disabled", "r
-00013e90: 6561 646f 6e6c 7922 5d29 0a0a 2020 2020  eadonly"])..    
-00013ea0: 6465 6620 7365 745f 6d61 7070 696e 6728  def set_mapping(
-00013eb0: 7365 6c66 2c20 6d61 7070 696e 673a 2044  self, mapping: D
-00013ec0: 6963 745b 7374 722c 2041 6e79 5d29 3a0a  ict[str, Any]):.
-00013ed0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-00013ee0: 7069 6e67 203d 206d 6170 7069 6e67 0a20  ping = mapping. 
-00013ef0: 2020 2020 2020 2073 656c 665b 2276 616c         self["val
-00013f00: 7565 7322 5d20 3d20 6c69 7374 286d 6170  ues"] = list(map
-00013f10: 7069 6e67 290a 0a20 2020 2064 6566 2067  ping)..    def g
-00013f20: 6574 5f73 656c 6563 7465 645f 7661 6c75  et_selected_valu
-00013f30: 6528 7365 6c66 2920 2d3e 2041 6e79 3a0a  e(self) -> Any:.
-00013f40: 2020 2020 2020 2020 6465 7363 203d 2073          desc = s
-00013f50: 656c 662e 6d61 7070 696e 675f 6465 7363  elf.mapping_desc
-00013f60: 5f76 6172 6961 626c 652e 6765 7428 290a  _variable.get().
-00013f70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013f80: 656c 662e 6d61 7070 696e 672e 6765 7428  elf.mapping.get(
-00013f90: 6465 7363 2c20 4e6f 6e65 290a 0a20 2020  desc, None)..   
-00013fa0: 2064 6566 2073 656c 6563 745f 7661 6c75   def select_valu
-00013fb0: 6528 7365 6c66 2c20 7661 6c75 6529 202d  e(self, value) -
-00013fc0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00013fd0: 666f 7220 6465 7363 2069 6e20 7365 6c66  for desc in self
-00013fe0: 2e6d 6170 7069 6e67 3a0a 2020 2020 2020  .mapping:.      
-00013ff0: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
-00014000: 7070 696e 675b 6465 7363 5d20 3d3d 2076  pping[desc] == v
-00014010: 616c 7565 3a0a 2020 2020 2020 2020 2020  alue:.          
-00014020: 2020 2020 2020 7365 6c66 2e73 6574 2864        self.set(d
-00014030: 6573 6329 0a0a 2020 2020 6465 6620 7365  esc)..    def se
-00014040: 6c65 6374 5f6e 6f6e 6528 7365 6c66 2920  lect_none(self) 
-00014050: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00014060: 2073 656c 662e 6d61 7070 696e 675f 6465   self.mapping_de
-00014070: 7363 5f76 6172 6961 626c 652e 7365 7428  sc_variable.set(
-00014080: 2222 290a 0a0a 636c 6173 7320 4164 7661  "")...class Adva
-00014090: 6e63 6564 4c61 6265 6c28 7474 6b2e 4c61  ncedLabel(ttk.La
-000140a0: 6265 6c29 3a0a 2020 2020 6465 6620 5f5f  bel):.    def __
-000140b0: 696e 6974 5f5f 2873 656c 662c 206d 6173  init__(self, mas
-000140c0: 7465 722c 202a 2a6b 7729 3a0a 2020 2020  ter, **kw):.    
-000140d0: 2020 2020 7365 6c66 2e5f 6465 6661 756c      self._defaul
-000140e0: 745f 666f 6e74 203d 2074 6b69 6e74 6572  t_font = tkinter
-000140f0: 2e66 6f6e 742e 6e61 6d65 746f 666f 6e74  .font.nametofont
-00014100: 2822 546b 4465 6661 756c 7446 6f6e 7422  ("TkDefaultFont"
-00014110: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00014120: 7572 6c5f 666f 6e74 203d 2073 656c 662e  url_font = self.
-00014130: 5f64 6566 6175 6c74 5f66 6f6e 742e 636f  _default_font.co
-00014140: 7079 2829 0a20 2020 2020 2020 2073 656c  py().        sel
-00014150: 662e 5f75 726c 5f66 6f6e 742e 636f 6e66  f._url_font.conf
-00014160: 6967 7572 6528 756e 6465 726c 696e 653d  igure(underline=
-00014170: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-00014180: 5f75 726c 203d 204e 6f6e 650a 2020 2020  _url = None.    
-00014190: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-000141a0: 6974 5f5f 286d 6173 7465 722c 202a 2a6b  it__(master, **k
-000141b0: 7729 0a20 2020 2020 2020 2073 656c 662e  w).        self.
-000141c0: 6269 6e64 2822 3c42 7574 746f 6e2d 313e  bind("<Button-1>
-000141d0: 222c 2073 656c 662e 5f6f 6e5f 636c 6963  ", self._on_clic
-000141e0: 6b2c 2054 7275 6529 0a0a 2020 2020 6465  k, True)..    de
-000141f0: 6620 7365 745f 7572 6c28 7365 6c66 2c20  f set_url(self, 
-00014200: 7572 6c3a 204f 7074 696f 6e61 6c5b 7374  url: Optional[st
-00014210: 725d 2920 2d3e 204e 6f6e 653a 0a20 2020  r]) -> None:.   
-00014220: 2020 2020 2069 6620 7365 6c66 2e5f 7572       if self._ur
-00014230: 6c20 3d3d 2075 726c 3a0a 2020 2020 2020  l == url:.      
-00014240: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
-00014250: 2020 2020 2020 7365 6c66 2e5f 7572 6c20        self._url 
-00014260: 3d20 7572 6c0a 2020 2020 2020 2020 6966  = url.        if
-00014270: 2075 726c 3a0a 2020 2020 2020 2020 2020   url:.          
-00014280: 2020 7365 6c66 2e63 6f6e 6669 6775 7265    self.configure
-00014290: 2873 7479 6c65 3d22 5572 6c2e 544c 6162  (style="Url.TLab
-000142a0: 656c 222c 2063 7572 736f 723d 6765 745f  el", cursor=get_
-000142b0: 6879 7065 726c 696e 6b5f 6375 7273 6f72  hyperlink_cursor
-000142c0: 2829 2c20 666f 6e74 3d73 656c 662e 5f75  (), font=self._u
-000142d0: 726c 5f66 6f6e 7429 0a20 2020 2020 2020  rl_font).       
-000142e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000142f0: 2020 2073 656c 662e 636f 6e66 6967 7572     self.configur
-00014300: 6528 7374 796c 653d 2254 4c61 6265 6c22  e(style="TLabel"
-00014310: 2c20 6375 7273 6f72 3d22 222c 2066 6f6e  , cursor="", fon
-00014320: 743d 7365 6c66 2e5f 6465 6661 756c 745f  t=self._default_
-00014330: 666f 6e74 290a 0a20 2020 2064 6566 2067  font)..    def g
-00014340: 6574 5f75 726c 2873 656c 6629 202d 3e20  et_url(self) -> 
-00014350: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
-00014360: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00014370: 6c66 2e5f 7572 6c0a 0a20 2020 2064 6566  lf._url..    def
-00014380: 205f 6f6e 5f63 6c69 636b 2873 656c 662c   _on_click(self,
-00014390: 202a 6576 656e 7429 3a0a 2020 2020 2020   *event):.      
-000143a0: 2020 6966 2073 656c 662e 5f75 726c 3a0a    if self._url:.
-000143b0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-000143c0: 7274 2077 6562 6272 6f77 7365 720a 0a20  rt webbrowser.. 
-000143d0: 2020 2020 2020 2020 2020 2077 6562 6272             webbr
-000143e0: 6f77 7365 722e 6f70 656e 2873 656c 662e  owser.open(self.
-000143f0: 5f75 726c 290a 0a0a 6966 205f 5f6e 616d  _url)...if __nam
-00014400: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-00014410: 223a 0a20 2020 2070 7269 6e74 2877 696e  ":.    print(win
-00014420: 646f 7773 5f6b 6e6f 776e 5f65 7874 656e  dows_known_exten
-00014430: 7369 6f6e 735f 6172 655f 6869 6464 656e  sions_are_hidden
-00014440: 2829 290a                                ()).
+00012af0: 7365 6c66 2e65 6e74 7279 636f 6e66 6967  self.entryconfig
+00012b00: 7572 6528 692c 2073 7461 7465 3d74 6b2e  ure(i, state=tk.
+00012b10: 4449 5341 424c 4544 290a 2020 2020 2020  DISABLED).      
+00012b20: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b40: 2020 2020 7365 6c66 2e65 6e74 7279 636f      self.entryco
+00012b50: 6e66 6967 7572 6528 692c 2073 7461 7465  nfigure(i, state
+00012b60: 3d74 6b2e 4e4f 524d 414c 290a 0a20 2020  =tk.NORMAL)..   
+00012b70: 2064 6566 2061 6464 2873 656c 662c 2069   def add(self, i
+00012b80: 7465 6d54 7970 652c 2063 6e66 3d7b 7d2c  temType, cnf={},
+00012b90: 202a 2a6b 7729 3a0a 2020 2020 2020 2020   **kw):.        
+00012ba0: 636e 6620 3d20 636e 6620 6f72 206b 770a  cnf = cnf or kw.
+00012bb0: 2020 2020 2020 2020 7465 7374 6572 203d          tester =
+00012bc0: 2063 6e66 2e67 6574 2822 7465 7374 6572   cnf.get("tester
+00012bd0: 2229 0a20 2020 2020 2020 2069 6620 2274  ").        if "t
+00012be0: 6573 7465 7222 2069 6e20 636e 663a 0a20  ester" in cnf:. 
+00012bf0: 2020 2020 2020 2020 2020 2064 656c 2063             del c
+00012c00: 6e66 5b22 7465 7374 6572 225d 0a0a 2020  nf["tester"]..  
+00012c10: 2020 2020 2020 7375 7065 7228 292e 6164        super().ad
+00012c20: 6428 6974 656d 5479 7065 2c20 636e 6629  d(itemType, cnf)
+00012c30: 0a0a 2020 2020 2020 2020 6974 656d 6461  ..        itemda
+00012c40: 7461 203d 2073 656c 662e 656e 7472 7963  ta = self.entryc
+00012c50: 6f6e 6669 6775 7265 2873 656c 662e 696e  onfigure(self.in
+00012c60: 6465 7828 2265 6e64 2229 290a 2020 2020  dex("end")).    
+00012c70: 2020 2020 6c61 6265 6c64 6174 6120 3d20      labeldata = 
+00012c80: 6974 656d 6461 7461 2e67 6574 2822 6c61  itemdata.get("la
+00012c90: 6265 6c22 290a 2020 2020 2020 2020 6966  bel").        if
+00012ca0: 206c 6162 656c 6461 7461 3a0a 2020 2020   labeldata:.    
+00012cb0: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00012cc0: 7374 6572 735b 6c61 6265 6c64 6174 615d  sters[labeldata]
+00012cd0: 203d 2074 6573 7465 720a 0a0a 636c 6173   = tester...clas
+00012ce0: 7320 5465 7874 4d65 6e75 284d 656e 7545  s TextMenu(MenuE
+00012cf0: 7829 3a0a 2020 2020 6465 6620 5f5f 696e  x):.    def __in
+00012d00: 6974 5f5f 2873 656c 662c 2074 6172 6765  it__(self, targe
+00012d10: 7429 3a0a 2020 2020 2020 2020 7365 6c66  t):.        self
+00012d20: 2e74 6578 7420 3d20 7461 7267 6574 0a20  .text = target. 
+00012d30: 2020 2020 2020 204d 656e 7545 782e 5f5f         MenuEx.__
+00012d40: 696e 6974 5f5f 2873 656c 662c 2074 6172  init__(self, tar
+00012d50: 6765 7429 0a20 2020 2020 2020 2073 656c  get).        sel
+00012d60: 662e 6164 645f 6261 7369 635f 6974 656d  f.add_basic_item
+00012d70: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
+00012d80: 2e61 6464 5f65 7874 7261 5f69 7465 6d73  .add_extra_items
+00012d90: 2829 0a0a 2020 2020 6465 6620 6164 645f  ()..    def add_
+00012da0: 6261 7369 635f 6974 656d 7328 7365 6c66  basic_items(self
+00012db0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00012dc0: 6164 645f 636f 6d6d 616e 6428 6c61 6265  add_command(labe
+00012dd0: 6c3d 7472 2822 4375 7422 292c 2063 6f6d  l=tr("Cut"), com
+00012de0: 6d61 6e64 3d73 656c 662e 6f6e 5f63 7574  mand=self.on_cut
+00012df0: 2c20 7465 7374 6572 3d73 656c 662e 6361  , tester=self.ca
+00012e00: 6e5f 6375 7429 0a20 2020 2020 2020 2073  n_cut).        s
+00012e10: 656c 662e 6164 645f 636f 6d6d 616e 6428  elf.add_command(
+00012e20: 6c61 6265 6c3d 7472 2822 436f 7079 2229  label=tr("Copy")
+00012e30: 2c20 636f 6d6d 616e 643d 7365 6c66 2e6f  , command=self.o
+00012e40: 6e5f 636f 7079 2c20 7465 7374 6572 3d73  n_copy, tester=s
+00012e50: 656c 662e 6361 6e5f 636f 7079 290a 2020  elf.can_copy).  
+00012e60: 2020 2020 2020 7365 6c66 2e61 6464 5f63        self.add_c
+00012e70: 6f6d 6d61 6e64 286c 6162 656c 3d74 7228  ommand(label=tr(
+00012e80: 2250 6173 7465 2229 2c20 636f 6d6d 616e  "Paste"), comman
+00012e90: 643d 7365 6c66 2e6f 6e5f 7061 7374 652c  d=self.on_paste,
+00012ea0: 2074 6573 7465 723d 7365 6c66 2e63 616e   tester=self.can
+00012eb0: 5f70 6173 7465 290a 0a20 2020 2064 6566  _paste)..    def
+00012ec0: 2061 6464 5f65 7874 7261 5f69 7465 6d73   add_extra_items
+00012ed0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00012ee0: 7365 6c66 2e61 6464 5f73 6570 6172 6174  self.add_separat
+00012ef0: 6f72 2829 0a20 2020 2020 2020 2073 656c  or().        sel
+00012f00: 662e 6164 645f 636f 6d6d 616e 6428 6c61  f.add_command(la
+00012f10: 6265 6c3d 7472 2822 5365 6c65 6374 2041  bel=tr("Select A
+00012f20: 6c6c 2229 2c20 636f 6d6d 616e 643d 7365  ll"), command=se
+00012f30: 6c66 2e6f 6e5f 7365 6c65 6374 5f61 6c6c  lf.on_select_all
+00012f40: 290a 0a20 2020 2064 6566 206f 6e5f 6375  )..    def on_cu
+00012f50: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00012f60: 2073 656c 662e 7465 7874 2e65 7665 6e74   self.text.event
+00012f70: 5f67 656e 6572 6174 6528 223c 3c43 7574  _generate("<<Cut
+00012f80: 3e3e 2229 0a0a 2020 2020 6465 6620 6f6e  >>")..    def on
+00012f90: 5f63 6f70 7928 7365 6c66 293a 0a20 2020  _copy(self):.   
+00012fa0: 2020 2020 2073 656c 662e 7465 7874 2e65       self.text.e
+00012fb0: 7665 6e74 5f67 656e 6572 6174 6528 223c  vent_generate("<
+00012fc0: 3c43 6f70 793e 3e22 290a 0a20 2020 2064  <Copy>>")..    d
+00012fd0: 6566 206f 6e5f 7061 7374 6528 7365 6c66  ef on_paste(self
+00012fe0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00012ff0: 7465 7874 2e65 7665 6e74 5f67 656e 6572  text.event_gener
+00013000: 6174 6528 223c 3c50 6173 7465 3e3e 2229  ate("<<Paste>>")
+00013010: 0a0a 2020 2020 6465 6620 6f6e 5f73 656c  ..    def on_sel
+00013020: 6563 745f 616c 6c28 7365 6c66 293a 0a20  ect_all(self):. 
+00013030: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
+00013040: 2e65 7665 6e74 5f67 656e 6572 6174 6528  .event_generate(
+00013050: 223c 3c53 656c 6563 7441 6c6c 3e3e 2229  "<<SelectAll>>")
+00013060: 0a0a 2020 2020 6465 6620 6361 6e5f 6375  ..    def can_cu
+00013070: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00013080: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+00013090: 5f73 656c 6563 7465 645f 7465 7874 2829  _selected_text()
+000130a0: 2061 6e64 206e 6f74 2073 656c 662e 7365   and not self.se
+000130b0: 6c65 6374 696f 6e5f 6973 5f72 6561 645f  lection_is_read_
+000130c0: 6f6e 6c79 2829 0a0a 2020 2020 6465 6620  only()..    def 
+000130d0: 6361 6e5f 636f 7079 2873 656c 6629 3a0a  can_copy(self):.
+000130e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000130f0: 656c 662e 6765 745f 7365 6c65 6374 6564  elf.get_selected
+00013100: 5f74 6578 7428 290a 0a20 2020 2064 6566  _text()..    def
+00013110: 2063 616e 5f70 6173 7465 2873 656c 6629   can_paste(self)
+00013120: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00013130: 206e 6f74 2073 656c 662e 7365 6c65 6374   not self.select
+00013140: 696f 6e5f 6973 5f72 6561 645f 6f6e 6c79  ion_is_read_only
+00013150: 2829 0a0a 2020 2020 6465 6620 6765 745f  ()..    def get_
+00013160: 7365 6c65 6374 6564 5f74 6578 7428 7365  selected_text(se
+00013170: 6c66 293a 0a20 2020 2020 2020 2074 7279  lf):.        try
+00013180: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00013190: 7475 726e 2073 656c 662e 7465 7874 2e67  turn self.text.g
+000131a0: 6574 2822 7365 6c2e 6669 7273 7422 2c20  et("sel.first", 
+000131b0: 2273 656c 2e6c 6173 7422 290a 2020 2020  "sel.last").    
+000131c0: 2020 2020 6578 6365 7074 2054 636c 4572      except TclEr
+000131d0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+000131e0: 2072 6574 7572 6e20 2222 0a0a 2020 2020   return ""..    
+000131f0: 6465 6620 7365 6c65 6374 696f 6e5f 6973  def selection_is
+00013200: 5f72 6561 645f 6f6e 6c79 2873 656c 6629  _read_only(self)
+00013210: 3a0a 2020 2020 2020 2020 6966 2068 6173  :.        if has
+00013220: 6174 7472 2873 656c 662e 7465 7874 2c20  attr(self.text, 
+00013230: 2269 735f 7265 6164 5f6f 6e6c 7922 293a  "is_read_only"):
+00013240: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013250: 7572 6e20 7365 6c66 2e74 6578 742e 6973  urn self.text.is
+00013260: 5f72 6561 645f 6f6e 6c79 2829 0a0a 2020  _read_only()..  
+00013270: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00013280: 7365 0a0a 0a64 6566 2063 7265 6174 655f  se...def create_
+00013290: 7572 6c5f 6c61 6265 6c28 6d61 7374 6572  url_label(master
+000132a0: 2c20 7572 6c2c 2074 6578 743d 4e6f 6e65  , url, text=None
+000132b0: 2c20 2a2a 6b77 293a 0a20 2020 2069 6d70  , **kw):.    imp
+000132c0: 6f72 7420 7765 6262 726f 7773 6572 0a0a  ort webbrowser..
+000132d0: 2020 2020 7265 7475 726e 2063 7265 6174      return creat
+000132e0: 655f 6163 7469 6f6e 5f6c 6162 656c 286d  e_action_label(m
+000132f0: 6173 7465 722c 2074 6578 7420 6f72 2075  aster, text or u
+00013300: 726c 2c20 6c61 6d62 6461 205f 3a20 7765  rl, lambda _: we
+00013310: 6262 726f 7773 6572 2e6f 7065 6e28 7572  bbrowser.open(ur
+00013320: 6c29 2c20 2a2a 6b77 290a 0a0a 6465 6620  l), **kw)...def 
+00013330: 6372 6561 7465 5f61 6374 696f 6e5f 6c61  create_action_la
+00013340: 6265 6c28 6d61 7374 6572 2c20 7465 7874  bel(master, text
+00013350: 2c20 636c 6963 6b5f 6861 6e64 6c65 722c  , click_handler,
+00013360: 202a 2a6b 7729 3a0a 2020 2020 7572 6c5f   **kw):.    url_
+00013370: 666f 6e74 203d 2074 6b69 6e74 6572 2e66  font = tkinter.f
+00013380: 6f6e 742e 6e61 6d65 746f 666f 6e74 2822  ont.nametofont("
+00013390: 546b 4465 6661 756c 7446 6f6e 7422 292e  TkDefaultFont").
+000133a0: 636f 7079 2829 0a20 2020 2075 726c 5f66  copy().    url_f
+000133b0: 6f6e 742e 636f 6e66 6967 7572 6528 756e  ont.configure(un
+000133c0: 6465 726c 696e 653d 3129 0a20 2020 2075  derline=1).    u
+000133d0: 726c 5f6c 6162 656c 203d 2074 746b 2e4c  rl_label = ttk.L
+000133e0: 6162 656c 280a 2020 2020 2020 2020 6d61  abel(.        ma
+000133f0: 7374 6572 2c20 7465 7874 3d74 6578 742c  ster, text=text,
+00013400: 2073 7479 6c65 3d22 5572 6c2e 544c 6162   style="Url.TLab
+00013410: 656c 222c 2063 7572 736f 723d 6765 745f  el", cursor=get_
+00013420: 6879 7065 726c 696e 6b5f 6375 7273 6f72  hyperlink_cursor
+00013430: 2829 2c20 666f 6e74 3d75 726c 5f66 6f6e  (), font=url_fon
+00013440: 742c 202a 2a6b 770a 2020 2020 290a 2020  t, **kw.    ).  
+00013450: 2020 7572 6c5f 6c61 6265 6c2e 6269 6e64    url_label.bind
+00013460: 2822 3c42 7574 746f 6e2d 313e 222c 2063  ("<Button-1>", c
+00013470: 6c69 636b 5f68 616e 646c 6572 290a 2020  lick_handler).  
+00013480: 2020 7265 7475 726e 2075 726c 5f6c 6162    return url_lab
+00013490: 656c 0a0a 0a64 6566 2067 6574 5f73 697a  el...def get_siz
+000134a0: 655f 6f70 7469 6f6e 5f6e 616d 6528 7769  e_option_name(wi
+000134b0: 6e64 6f77 293a 0a20 2020 2072 6574 7572  ndow):.    retur
+000134c0: 6e20 226c 6179 6f75 742e 2220 2b20 7479  n "layout." + ty
+000134d0: 7065 2877 696e 646f 7729 2e5f 5f6e 616d  pe(window).__nam
+000134e0: 655f 5f20 2b20 225f 7369 7a65 220a 0a0a  e__ + "_size"...
+000134f0: 6465 6620 6765 745f 6465 6661 756c 745f  def get_default_
+00013500: 6261 7369 635f 7468 656d 6528 293a 0a20  basic_theme():. 
+00013510: 2020 2069 6620 7275 6e6e 696e 675f 6f6e     if running_on
+00013520: 5f77 696e 646f 7773 2829 3a0a 2020 2020  _windows():.    
+00013530: 2020 2020 7265 7475 726e 2022 7669 7374      return "vist
+00013540: 6122 0a20 2020 2065 6c73 653a 0a20 2020  a".    else:.   
+00013550: 2020 2020 2072 6574 7572 6e20 2263 6c61       return "cla
+00013560: 6d22 0a0a 0a45 4d5f 5749 4454 4820 3d20  m"...EM_WIDTH = 
+00013570: 4e6f 6e65 0a0a 0a64 6566 2065 6d73 5f74  None...def ems_t
+00013580: 6f5f 7069 7865 6c73 2878 3a20 666c 6f61  o_pixels(x: floa
+00013590: 7429 202d 3e20 696e 743a 0a20 2020 2067  t) -> int:.    g
+000135a0: 6c6f 6261 6c20 454d 5f57 4944 5448 0a20  lobal EM_WIDTH. 
+000135b0: 2020 2069 6620 454d 5f57 4944 5448 2069     if EM_WIDTH i
+000135c0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000135d0: 454d 5f57 4944 5448 203d 2074 6b69 6e74  EM_WIDTH = tkint
+000135e0: 6572 2e66 6f6e 742e 6e61 6d65 746f 666f  er.font.nametofo
+000135f0: 6e74 2822 546b 4465 6661 756c 7446 6f6e  nt("TkDefaultFon
+00013600: 7422 292e 6d65 6173 7572 6528 226d 2229  t").measure("m")
+00013610: 0a20 2020 2072 6574 7572 6e20 696e 7428  .    return int(
+00013620: 454d 5f57 4944 5448 202a 2078 290a 0a0a  EM_WIDTH * x)...
+00013630: 5f62 746e 5f70 6164 6469 6e67 203d 204e  _btn_padding = N
+00013640: 6f6e 650a 0a0a 6465 6620 7365 745f 7465  one...def set_te
+00013650: 7874 5f69 665f 6469 6666 6572 656e 7428  xt_if_different(
+00013660: 7769 6467 6574 2c20 7465 7874 2920 2d3e  widget, text) ->
+00013670: 2062 6f6f 6c3a 0a20 2020 2069 6620 7769   bool:.    if wi
+00013680: 6467 6574 5b22 7465 7874 225d 2021 3d20  dget["text"] != 
+00013690: 7465 7874 3a0a 2020 2020 2020 2020 7769  text:.        wi
+000136a0: 6467 6574 5b22 7465 7874 225d 203d 2074  dget["text"] = t
+000136b0: 6578 740a 2020 2020 2020 2020 7265 7475  ext.        retu
+000136c0: 726e 2054 7275 650a 2020 2020 656c 7365  rn True.    else
+000136d0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000136e0: 2046 616c 7365 0a0a 0a64 6566 2074 725f   False...def tr_
+000136f0: 6274 6e28 7329 3a0a 2020 2020 2222 2254  btn(s):.    """T
+00013700: 7261 6e73 6c61 7465 7320 6275 7474 6f6e  ranslates button
+00013710: 2063 6170 7469 6f6e 2c20 6164 6473 2070   caption, adds p
+00013720: 6164 6469 6e67 2074 6f20 6d61 6b65 2073  adding to make s
+00013730: 7572 6520 7465 7874 2066 6974 7322 2222  ure text fits"""
+00013740: 0a20 2020 2067 6c6f 6261 6c20 5f62 746e  .    global _btn
+00013750: 5f70 6164 6469 6e67 0a20 2020 2069 6620  _padding.    if 
+00013760: 5f62 746e 5f70 6164 6469 6e67 2069 7320  _btn_padding is 
+00013770: 4e6f 6e65 3a0a 2020 2020 2020 2020 5f62  None:.        _b
+00013780: 746e 5f70 6164 6469 6e67 203d 2067 6574  tn_padding = get
+00013790: 5f62 7574 746f 6e5f 7061 6464 696e 6728  _button_padding(
+000137a0: 290a 0a20 2020 2072 6574 7572 6e20 5f62  )..    return _b
+000137b0: 746e 5f70 6164 6469 6e67 202b 2074 7228  tn_padding + tr(
+000137c0: 7329 202b 205f 6274 6e5f 7061 6464 696e  s) + _btn_paddin
+000137d0: 670a 0a0a 6465 6620 6164 645f 6d65 7373  g...def add_mess
+000137e0: 6167 6562 6f78 5f70 6172 656e 745f 6368  agebox_parent_ch
+000137f0: 6563 6b65 7228 293a 0a20 2020 2064 6566  ecker():.    def
+00013800: 2077 7261 705f 7769 7468 5f70 6172 656e   wrap_with_paren
+00013810: 745f 6368 6563 6b65 7228 6f72 6967 696e  t_checker(origin
+00013820: 616c 293a 0a20 2020 2020 2020 2064 6566  al):.        def
+00013830: 2077 7261 7070 6572 282a 6172 6773 2c20   wrapper(*args, 
+00013840: 2a2a 6f70 7469 6f6e 7329 3a0a 2020 2020  **options):.    
+00013850: 2020 2020 2020 2020 5f63 6865 636b 5f64          _check_d
+00013860: 6961 6c6f 675f 7061 7265 6e74 286f 7074  ialog_parent(opt
+00013870: 696f 6e73 290a 2020 2020 2020 2020 2020  ions).          
+00013880: 2020 7265 7475 726e 206f 7269 6769 6e61    return origina
+00013890: 6c28 2a61 7267 732c 202a 2a6f 7074 696f  l(*args, **optio
+000138a0: 6e73 290a 0a20 2020 2020 2020 2072 6574  ns)..        ret
+000138b0: 7572 6e20 7772 6170 7065 720a 0a20 2020  urn wrapper..   
+000138c0: 2066 726f 6d20 746b 696e 7465 7220 696d   from tkinter im
+000138d0: 706f 7274 206d 6573 7361 6765 626f 780a  port messagebox.
+000138e0: 0a20 2020 2066 6f72 206e 616d 6520 696e  .    for name in
+000138f0: 205b 0a20 2020 2020 2020 2022 7368 6f77   [.        "show
+00013900: 696e 666f 222c 0a20 2020 2020 2020 2022  info",.        "
+00013910: 7368 6f77 7761 726e 696e 6722 2c0a 2020  showwarning",.  
+00013920: 2020 2020 2020 2273 686f 7765 7272 6f72        "showerror
+00013930: 222c 0a20 2020 2020 2020 2022 6173 6b71  ",.        "askq
+00013940: 7565 7374 696f 6e22 2c0a 2020 2020 2020  uestion",.      
+00013950: 2020 2261 736b 6f6b 6361 6e63 656c 222c    "askokcancel",
+00013960: 0a20 2020 2020 2020 2022 6173 6b79 6573  .        "askyes
+00013970: 6e6f 222c 0a20 2020 2020 2020 2022 6173  no",.        "as
+00013980: 6b79 6573 6e6f 6361 6e63 656c 222c 0a20  kyesnocancel",. 
+00013990: 2020 2020 2020 2022 6173 6b72 6574 7279         "askretry
+000139a0: 6361 6e63 656c 222c 0a20 2020 205d 3a0a  cancel",.    ]:.
+000139b0: 2020 2020 2020 2020 6675 6e20 3d20 6765          fun = ge
+000139c0: 7461 7474 7228 6d65 7373 6167 6562 6f78  tattr(messagebox
+000139d0: 2c20 6e61 6d65 290a 2020 2020 2020 2020  , name).        
+000139e0: 7365 7461 7474 7228 6d65 7373 6167 6562  setattr(messageb
+000139f0: 6f78 2c20 6e61 6d65 2c20 7772 6170 5f77  ox, name, wrap_w
+00013a00: 6974 685f 7061 7265 6e74 5f63 6865 636b  ith_parent_check
+00013a10: 6572 2866 756e 2929 0a0a 0a64 6566 2072  er(fun))...def r
+00013a20: 6570 6c61 6365 5f75 6e73 7570 706f 7274  eplace_unsupport
+00013a30: 6564 5f63 6861 7273 2874 6578 743a 2073  ed_chars(text: s
+00013a40: 7472 2920 2d3e 2073 7472 3a0a 2020 2020  tr) -> str:.    
+00013a50: 6966 2067 6574 5f74 6b5f 7665 7273 696f  if get_tk_versio
+00013a60: 6e5f 696e 666f 2829 203c 2028 382c 2036  n_info() < (8, 6
+00013a70: 2c20 3132 293a 0a20 2020 2020 2020 2023  , 12):.        #
+00013a80: 2063 616e 2063 7261 7368 2077 6974 6820   can crash with 
+00013a90: 656d 6f6a 6973 0a20 2020 2020 2020 2072  emojis.        r
+00013aa0: 6574 7572 6e20 2222 2e6a 6f69 6e28 6320  eturn "".join(c 
+00013ab0: 6966 2063 203c 2022 5c55 3030 3031 3030  if c < "\U000100
+00013ac0: 3030 2220 656c 7365 2022 e296 a122 2066  00" else "..." f
+00013ad0: 6f72 2063 2069 6e20 7465 7874 290a 2020  or c in text).  
+00013ae0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00013af0: 7265 7475 726e 2074 6578 740a 0a0a 6465  return text...de
+00013b00: 6620 7769 6e64 6f77 735f 6b6e 6f77 6e5f  f windows_known_
+00013b10: 6578 7465 6e73 696f 6e73 5f61 7265 5f68  extensions_are_h
+00013b20: 6964 6465 6e28 2920 2d3e 2062 6f6f 6c3a  idden() -> bool:
+00013b30: 0a20 2020 2061 7373 6572 7420 7275 6e6e  .    assert runn
+00013b40: 696e 675f 6f6e 5f77 696e 646f 7773 2829  ing_on_windows()
+00013b50: 0a20 2020 2069 6d70 6f72 7420 7769 6e72  .    import winr
+00013b60: 6567 0a0a 2020 2020 7265 675f 6b65 7920  eg..    reg_key 
+00013b70: 3d20 7769 6e72 6567 2e4f 7065 6e4b 6579  = winreg.OpenKey
+00013b80: 280a 2020 2020 2020 2020 7769 6e72 6567  (.        winreg
+00013b90: 2e48 4b45 595f 4355 5252 454e 545f 5553  .HKEY_CURRENT_US
+00013ba0: 4552 2c0a 2020 2020 2020 2020 7222 534f  ER,.        r"SO
+00013bb0: 4654 5741 5245 5c4d 6963 726f 736f 6674  FTWARE\Microsoft
+00013bc0: 5c57 696e 646f 7773 5c43 7572 7265 6e74  \Windows\Current
+00013bd0: 5665 7273 696f 6e5c 4578 706c 6f72 6572  Version\Explorer
+00013be0: 5c41 6476 616e 6365 6422 2c0a 2020 2020  \Advanced",.    
+00013bf0: 2020 2020 302c 0a20 2020 2020 2020 2077      0,.        w
+00013c00: 696e 7265 672e 4b45 595f 5245 4144 2c0a  inreg.KEY_READ,.
+00013c10: 2020 2020 290a 2020 2020 7472 793a 0a20      ).    try:. 
+00013c20: 2020 2020 2020 2072 6574 7572 6e20 7769         return wi
+00013c30: 6e72 6567 2e51 7565 7279 5661 6c75 6545  nreg.QueryValueE
+00013c40: 7828 7265 675f 6b65 792c 2022 4869 6465  x(reg_key, "Hide
+00013c50: 4669 6c65 4578 7422 295b 305d 203d 3d20  FileExt")[0] == 
+00013c60: 310a 2020 2020 6669 6e61 6c6c 793a 0a20  1.    finally:. 
+00013c70: 2020 2020 2020 2072 6567 5f6b 6579 2e43         reg_key.C
+00013c80: 6c6f 7365 2829 0a0a 0a63 6c61 7373 204d  lose()...class M
+00013c90: 6170 7069 6e67 436f 6d62 6f62 6f78 2874  appingCombobox(t
+00013ca0: 746b 2e43 6f6d 626f 626f 7829 3a0a 2020  tk.Combobox):.  
+00013cb0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00013cc0: 656c 662c 206d 6173 7465 722c 206d 6170  elf, master, map
+00013cd0: 7069 6e67 3d4e 6f6e 652c 202a 2a6b 7729  ping=None, **kw)
+00013ce0: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00013cf0: 292e 5f5f 696e 6974 5f5f 286d 6173 7465  ).__init__(maste
+00013d00: 722c 202a 2a6b 7729 0a0a 2020 2020 2020  r, **kw)..      
+00013d10: 2020 6966 206d 6170 7069 6e67 2069 7320    if mapping is 
+00013d20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00013d30: 2020 6d61 7070 696e 6720 3d20 7b7d 0a0a    mapping = {}..
+00013d40: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+00013d50: 7069 6e67 3a20 4469 6374 5b73 7472 2c20  ping: Dict[str, 
+00013d60: 416e 795d 0a20 2020 2020 2020 2073 656c  Any].        sel
+00013d70: 662e 7365 745f 6d61 7070 696e 6728 6d61  f.set_mapping(ma
+00013d80: 7070 696e 6729 0a20 2020 2020 2020 2073  pping).        s
+00013d90: 656c 662e 6d61 7070 696e 675f 6465 7363  elf.mapping_desc
+00013da0: 5f76 6172 6961 626c 6520 3d20 746b 2e53  _variable = tk.S
+00013db0: 7472 696e 6756 6172 2876 616c 7565 3d22  tringVar(value="
+00013dc0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00013dd0: 636f 6e66 6967 7572 6528 7465 7874 7661  configure(textva
+00013de0: 7269 6162 6c65 3d73 656c 662e 6d61 7070  riable=self.mapp
+00013df0: 696e 675f 6465 7363 5f76 6172 6961 626c  ing_desc_variabl
+00013e00: 6529 0a0a 2020 2020 2020 2020 6966 206b  e)..        if k
+00013e10: 772e 6765 7428 2273 7461 7465 222c 204e  w.get("state", N
+00013e20: 6f6e 6529 203d 3d20 2264 6973 6162 6c65  one) == "disable
+00013e30: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
+00013e40: 7365 6c66 2e73 7461 7465 285b 2272 6561  self.state(["rea
+00013e50: 646f 6e6c 7922 5d29 0a20 2020 2020 2020  donly"]).       
+00013e60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013e70: 2020 2073 656c 662e 7374 6174 6528 5b22     self.state(["
+00013e80: 2164 6973 6162 6c65 6422 2c20 2272 6561  !disabled", "rea
+00013e90: 646f 6e6c 7922 5d29 0a0a 2020 2020 6465  donly"])..    de
+00013ea0: 6620 7365 745f 6d61 7070 696e 6728 7365  f set_mapping(se
+00013eb0: 6c66 2c20 6d61 7070 696e 673a 2044 6963  lf, mapping: Dic
+00013ec0: 745b 7374 722c 2041 6e79 5d29 3a0a 2020  t[str, Any]):.  
+00013ed0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+00013ee0: 6e67 203d 206d 6170 7069 6e67 0a20 2020  ng = mapping.   
+00013ef0: 2020 2020 2073 656c 665b 2276 616c 7565       self["value
+00013f00: 7322 5d20 3d20 6c69 7374 286d 6170 7069  s"] = list(mappi
+00013f10: 6e67 290a 0a20 2020 2064 6566 2067 6574  ng)..    def get
+00013f20: 5f73 656c 6563 7465 645f 7661 6c75 6528  _selected_value(
+00013f30: 7365 6c66 2920 2d3e 2041 6e79 3a0a 2020  self) -> Any:.  
+00013f40: 2020 2020 2020 6465 7363 203d 2073 656c        desc = sel
+00013f50: 662e 6d61 7070 696e 675f 6465 7363 5f76  f.mapping_desc_v
+00013f60: 6172 6961 626c 652e 6765 7428 290a 2020  ariable.get().  
+00013f70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00013f80: 662e 6d61 7070 696e 672e 6765 7428 6465  f.mapping.get(de
+00013f90: 7363 2c20 4e6f 6e65 290a 0a20 2020 2064  sc, None)..    d
+00013fa0: 6566 2073 656c 6563 745f 7661 6c75 6528  ef select_value(
+00013fb0: 7365 6c66 2c20 7661 6c75 6529 202d 3e20  self, value) -> 
+00013fc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 666f  None:.        fo
+00013fd0: 7220 6465 7363 2069 6e20 7365 6c66 2e6d  r desc in self.m
+00013fe0: 6170 7069 6e67 3a0a 2020 2020 2020 2020  apping:.        
+00013ff0: 2020 2020 6966 2073 656c 662e 6d61 7070      if self.mapp
+00014000: 696e 675b 6465 7363 5d20 3d3d 2076 616c  ing[desc] == val
+00014010: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00014020: 2020 2020 7365 6c66 2e73 6574 2864 6573      self.set(des
+00014030: 6329 0a0a 2020 2020 6465 6620 7365 6c65  c)..    def sele
+00014040: 6374 5f6e 6f6e 6528 7365 6c66 2920 2d3e  ct_none(self) ->
+00014050: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+00014060: 656c 662e 6d61 7070 696e 675f 6465 7363  elf.mapping_desc
+00014070: 5f76 6172 6961 626c 652e 7365 7428 2222  _variable.set(""
+00014080: 290a 0a0a 636c 6173 7320 4164 7661 6e63  )...class Advanc
+00014090: 6564 4c61 6265 6c28 7474 6b2e 4c61 6265  edLabel(ttk.Labe
+000140a0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000140b0: 6974 5f5f 2873 656c 662c 206d 6173 7465  it__(self, maste
+000140c0: 722c 202a 2a6b 7729 3a0a 2020 2020 2020  r, **kw):.      
+000140d0: 2020 7365 6c66 2e5f 6465 6661 756c 745f    self._default_
+000140e0: 666f 6e74 203d 2074 6b69 6e74 6572 2e66  font = tkinter.f
+000140f0: 6f6e 742e 6e61 6d65 746f 666f 6e74 2822  ont.nametofont("
+00014100: 546b 4465 6661 756c 7446 6f6e 7422 290a  TkDefaultFont").
+00014110: 2020 2020 2020 2020 7365 6c66 2e5f 7572          self._ur
+00014120: 6c5f 666f 6e74 203d 2073 656c 662e 5f64  l_font = self._d
+00014130: 6566 6175 6c74 5f66 6f6e 742e 636f 7079  efault_font.copy
+00014140: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00014150: 5f75 726c 5f66 6f6e 742e 636f 6e66 6967  _url_font.config
+00014160: 7572 6528 756e 6465 726c 696e 653d 3129  ure(underline=1)
+00014170: 0a20 2020 2020 2020 2073 656c 662e 5f75  .        self._u
+00014180: 726c 203d 204e 6f6e 650a 2020 2020 2020  rl = None.      
+00014190: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+000141a0: 5f5f 286d 6173 7465 722c 202a 2a6b 7729  __(master, **kw)
+000141b0: 0a20 2020 2020 2020 2073 656c 662e 6269  .        self.bi
+000141c0: 6e64 2822 3c42 7574 746f 6e2d 313e 222c  nd("<Button-1>",
+000141d0: 2073 656c 662e 5f6f 6e5f 636c 6963 6b2c   self._on_click,
+000141e0: 2054 7275 6529 0a0a 2020 2020 6465 6620   True)..    def 
+000141f0: 7365 745f 7572 6c28 7365 6c66 2c20 7572  set_url(self, ur
+00014200: 6c3a 204f 7074 696f 6e61 6c5b 7374 725d  l: Optional[str]
+00014210: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00014220: 2020 2069 6620 7365 6c66 2e5f 7572 6c20     if self._url 
+00014230: 3d3d 2075 726c 3a0a 2020 2020 2020 2020  == url:.        
+00014240: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00014250: 2020 2020 7365 6c66 2e5f 7572 6c20 3d20      self._url = 
+00014260: 7572 6c0a 2020 2020 2020 2020 6966 2075  url.        if u
+00014270: 726c 3a0a 2020 2020 2020 2020 2020 2020  rl:.            
+00014280: 7365 6c66 2e63 6f6e 6669 6775 7265 2873  self.configure(s
+00014290: 7479 6c65 3d22 5572 6c2e 544c 6162 656c  tyle="Url.TLabel
+000142a0: 222c 2063 7572 736f 723d 6765 745f 6879  ", cursor=get_hy
+000142b0: 7065 726c 696e 6b5f 6375 7273 6f72 2829  perlink_cursor()
+000142c0: 2c20 666f 6e74 3d73 656c 662e 5f75 726c  , font=self._url
+000142d0: 5f66 6f6e 7429 0a20 2020 2020 2020 2065  _font).        e
+000142e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000142f0: 2073 656c 662e 636f 6e66 6967 7572 6528   self.configure(
+00014300: 7374 796c 653d 2254 4c61 6265 6c22 2c20  style="TLabel", 
+00014310: 6375 7273 6f72 3d22 222c 2066 6f6e 743d  cursor="", font=
+00014320: 7365 6c66 2e5f 6465 6661 756c 745f 666f  self._default_fo
+00014330: 6e74 290a 0a20 2020 2064 6566 2067 6574  nt)..    def get
+00014340: 5f75 726c 2873 656c 6629 202d 3e20 4f70  _url(self) -> Op
+00014350: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
+00014360: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00014370: 2e5f 7572 6c0a 0a20 2020 2064 6566 205f  ._url..    def _
+00014380: 6f6e 5f63 6c69 636b 2873 656c 662c 202a  on_click(self, *
+00014390: 6576 656e 7429 3a0a 2020 2020 2020 2020  event):.        
+000143a0: 6966 2073 656c 662e 5f75 726c 3a0a 2020  if self._url:.  
+000143b0: 2020 2020 2020 2020 2020 6966 206f 732e            if os.
+000143c0: 7061 7468 2e69 7364 6972 2873 656c 662e  path.isdir(self.
+000143d0: 5f75 726c 293a 0a20 2020 2020 2020 2020  _url):.         
+000143e0: 2020 2020 2020 206f 7065 6e5f 7769 7468         open_with
+000143f0: 5f64 6566 6175 6c74 5f61 7070 2873 656c  _default_app(sel
+00014400: 662e 5f75 726c 290a 2020 2020 2020 2020  f._url).        
+00014410: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014420: 2020 2020 2020 2020 2020 696d 706f 7274            import
+00014430: 2077 6562 6272 6f77 7365 720a 0a20 2020   webbrowser..   
+00014440: 2020 2020 2020 2020 2020 2020 2077 6562               web
+00014450: 6272 6f77 7365 722e 6f70 656e 2873 656c  browser.open(sel
+00014460: 662e 5f75 726c 290a 0a0a 6465 6620 6f70  f._url)...def op
+00014470: 656e 5f77 6974 685f 6465 6661 756c 745f  en_with_default_
+00014480: 6170 7028 7061 7468 293a 0a20 2020 2069  app(path):.    i
+00014490: 6620 7275 6e6e 696e 675f 6f6e 5f77 696e  f running_on_win
+000144a0: 646f 7773 2829 3a0a 2020 2020 2020 2020  dows():.        
+000144b0: 6f73 2e73 7461 7274 6669 6c65 2870 6174  os.startfile(pat
+000144c0: 6829 0a20 2020 2065 6c69 6620 7275 6e6e  h).    elif runn
+000144d0: 696e 675f 6f6e 5f6d 6163 5f6f 7328 293a  ing_on_mac_os():
+000144e0: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
+000144f0: 6573 732e 7275 6e28 5b22 6f70 656e 222c  ess.run(["open",
+00014500: 2070 6174 685d 290a 2020 2020 656c 7365   path]).    else
+00014510: 3a0a 2020 2020 2020 2020 7375 6270 726f  :.        subpro
+00014520: 6365 7373 2e72 756e 285b 2278 6467 2d6f  cess.run(["xdg-o
+00014530: 7065 6e22 2c20 7061 7468 5d29 0a0a 0a69  pen", path])...i
+00014540: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+00014550: 5f6d 6169 6e5f 5f22 3a0a 2020 2020 7072  _main__":.    pr
+00014560: 696e 7428 7769 6e64 6f77 735f 6b6e 6f77  int(windows_know
+00014570: 6e5f 6578 7465 6e73 696f 6e73 5f61 7265  n_extensions_are
+00014580: 5f68 6964 6465 6e28 2929 0a              _hidden()).
```

### Comparing `thonny-4.0.2/thonny/vendored_libs/filelock/__init__.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/filelock/_api.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/filelock/_soft.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/filelock/_unix.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/filelock/_util.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/filelock/_windows.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/__init__.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__init__.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/__main__.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#!/usr/bin/env python3
 """
 MIT License
 
-Copyright (c) 2022 Aivar Annamaa
+Copyright (c) 2023 Aivar Annamaa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/adapters.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/adapters.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/bare_metal.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/bare_metal.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/connection.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/parser.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/parser.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/proxy.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#!/usr/bin/env python3
 """
 MIT License
 
-Copyright (c) 2022 Aivar Annamaa
+Copyright (c) 2023 Aivar Annamaa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/serial_connection.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/serial_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/session.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/session.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/util.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/util.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/vendored_libs/pipkin/webrepl_connection.py` & `thonny-4.1.0b1.dev0/thonny/vendored_libs/pipkin/webrepl_connection.py`

 * *Files identical despite different names*

### Comparing `thonny-4.0.2/thonny/workbench.py` & `thonny-4.1.0b1.dev0/thonny/workbench.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             if self.get_ui_mode() != "simple":
                 self._menubar.grid(row=0, sticky="nsew")
         else:
             opts = get_style_configuration("Menubar")
             if "custom" in opts:
                 del opts["custom"]
             self._menubar = tk.Menu(self, **opts)
-            if self.get_ui_mode() != "simple":
+            if self.get_ui_mode() != "simple" or running_on_mac_os():
                 self["menu"] = self._menubar
         self._menus = {}  # type: Dict[str, tk.Menu]
         self._menu_item_specs = (
             {}
         )  # type: Dict[Tuple[str, str], MenuItem] # key is pair (menu_name, command_label)
 
         # create standard menus in correct order
@@ -580,15 +580,14 @@
             server_socket.bind(thonny.get_ipc_file_path())
             secret = ""
 
         os.chmod(thonny.get_ipc_file_path(), 0o600)
         return server_socket, secret
 
     def _init_commands(self) -> None:
-
         self.add_command(
             "exit",
             "file",
             tr("Exit"),
             self._on_close,
             default_sequence=select_sequence("<Alt-F4>", "<Command-q>", "<Control-q>"),
             extra_sequences=["<Alt-F4>"]
@@ -603,15 +602,15 @@
         self.createcommand("::tk::mac::Quit", self._mac_quit)
 
         self.add_command(
             "increase_font_size",
             "view",
             tr("Increase font size"),
             lambda: self._change_font_size(1),
-            default_sequence=select_sequence("<Control-plus>", "<Command-Shift-plus>"),
+            default_sequence=select_sequence("<Control-plus>", "<Command-plus>"),
             extra_sequences=["<Control-KP_Add>"],
             group=60,
         )
 
         self.add_command(
             "decrease_font_size",
             "view",
@@ -639,15 +638,14 @@
             tr("Focus shell"),
             self._cmd_focus_shell,
             default_sequence=select_sequence("<Alt-s>", "<Command-Alt-s>"),
             group=70,
         )
 
         if self.get_ui_mode() == "expert":
-
             self.add_command(
                 "toggle_maximize_view",
                 "view",
                 tr("Maximize view"),
                 self._cmd_toggle_maximize_view,
                 flag_name="view.maximize_view",
                 default_sequence=None,
@@ -702,15 +700,14 @@
         if thonny.in_debug_mode():
             self.bind_all("<Control-Shift-Alt-D>", self._print_state_for_debugging, True)
 
     def _print_state_for_debugging(self, event) -> None:
         print(get_runner()._postponed_commands)
 
     def _init_containers(self) -> None:
-
         margin = ems_to_pixels(0.6)
         # Main frame functions as
         # - a background behind padding of main_pw, without this OS X leaves white border
         # - a container to be hidden, when a view is maximized and restored when view is back home
         main_frame = ttk.Frame(self)  #
         self._main_frame = main_frame
         main_frame.grid(row=1, column=0, sticky=tk.NSEW)
@@ -798,15 +795,14 @@
         )
         ukraine_label.grid(row=1, column=1, sticky="wsn")
 
     def _support_ukraine(self, event=None) -> None:
         webbrowser.open("https://github.com/thonny/thonny/wiki/Support-Ukraine")
 
     def _init_backend_switcher(self):
-
         # Set up the menu
         self._backend_conf_variable = tk.StringVar(value="{}")
 
         if running_on_mac_os():
             menu_conf = {}
         else:
             menu_conf = get_style_configuration("Menu")
@@ -1401,15 +1397,14 @@
     def get_default_syntax_theme(self) -> str:
         if self.uses_dark_ui_theme():
             return "Default Dark"
         else:
             return "Default Light"
 
     def uses_dark_ui_theme(self) -> bool:
-
         name = self._style.theme_use()
         while True:
             if "dark" in name.lower():
                 return True
             try:
                 name, _, _ = self._ui_themes[name]
             except KeyError:
@@ -1639,15 +1634,14 @@
     def get_package_dir(self):
         """Returns thonny package directory"""
         return os.path.dirname(sys.modules["thonny"].__file__)
 
     def get_image(
         self, filename: str, tk_name: Optional[str] = None, disabled=False
     ) -> tk.PhotoImage:
-
         if filename in self._image_mapping_by_theme[self._current_theme_name]:
             filename = self._image_mapping_by_theme[self._current_theme_name][filename]
 
         if filename in self._default_image_mapping:
             filename = self._default_image_mapping[filename]
 
         # if path is relative then interpret it as living in res folder
@@ -1977,15 +1971,14 @@
         caption: str,
         alternative_caption: str,
         accelerator: Optional[str],
         handler: Callable[[], None],
         tester: Optional[Callable[[], bool]],
         toolbar_group: int,
     ) -> None:
-
         assert caption is not None and len(caption) > 0, (
             "Missing caption for '%s'. Toolbar commands must have caption." % command_label
         )
         slaves = self._toolbar.grid_slaves(0, toolbar_group)
         if len(slaves) == 0:
             group_frame = ttk.Frame(self._toolbar)
             if self.in_simple_mode():
@@ -2096,15 +2089,14 @@
         self._change_font_size(new_size - current_size)
 
         new_width = min(widths[new_size], self.winfo_screenwidth())
         geo = re.findall(r"\d+", self.wm_geometry())
         self.geometry("{0}x{1}+{2}+{3}".format(new_width, geo[1], geo[2], geo[3]))
 
     def _change_font_size(self, delta: int) -> None:
-
         if delta != 0:
             editor_font_size = self.get_option("view.editor_font_size")
             editor_font_size += delta
             self.set_option("view.editor_font_size", self._guard_font_size(editor_font_size))
             io_font_size = self.get_option("view.io_font_size")
             io_font_size += delta
             self.set_option("view.io_font_size", self._guard_font_size(io_font_size))
@@ -2255,15 +2247,14 @@
 
                 if enabled:
                     menu.entryconfigure(i, state=tk.NORMAL)
                 else:
                     menu.entryconfigure(i, state=tk.DISABLED)
 
     def _find_location_for_menu_item(self, menu_name: str, command_label: str) -> Union[str, int]:
-
         menu = self.get_menu(menu_name)
 
         if menu.index("end") == None:  # menu is empty
             return "end"
 
         specs = self._menu_item_specs[(menu_name, command_label)]
```

### Comparing `thonny-4.0.2/thonny/workdlg.py` & `thonny-4.1.0b1.dev0/thonny/workdlg.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 import tkinter as tk
 from logging import getLogger
 from tkinter import messagebox, ttk
 from typing import Optional
 
 from thonny import tktextext
 from thonny.languages import tr
-from thonny.misc_utils import running_on_windows
-from thonny.ui_utils import CommonDialog, create_action_label, ems_to_pixels, set_text_if_different
+from thonny.misc_utils import running_on_mac_os, running_on_windows
+from thonny.ui_utils import (
+    CommonDialog,
+    create_action_label,
+    ems_to_pixels,
+    get_style_configuration,
+    set_text_if_different,
+)
 
 logger = getLogger(__name__)
 
 
 class WorkDialog(CommonDialog):
     def __init__(self, master, autostart=False):
         super(WorkDialog, self).__init__(master)
@@ -94,18 +100,34 @@
             width=round(self.get_action_text_max_length() * 1.1),
             click_handler=self.toggle_log_frame,
         )
         self._current_action_label.grid(
             row=1, column=2, sticky="we", pady=padding, padx=(0, intpad)
         )
 
+        self._menu_button = ttk.Button(
+            self.action_frame,
+            text="☰",
+            command=self.post_action_menu,
+            # style="Toolbutton"
+            width=3,
+        )
+        if self.has_action_menu():
+            self._menu_button.grid(column=3, row=1, pady=padding, padx=(0, intpad))
+
+        if running_on_mac_os():
+            menu_conf = {}
+        else:
+            menu_conf = get_style_configuration("Menu")
+        self._action_menu = tk.Menu(self, tearoff=False, **menu_conf)
+
         self._ok_button = ttk.Button(
             self.action_frame,
             text=self.get_ok_text(),
-            command=self.start_work_and_update_ui,
+            command=self.on_click_ok_button,
             state="disabled",
             default="active",
         )
         if not self._autostart:
             self._ok_button.grid(column=4, row=1, pady=padding, padx=(0, intpad))
 
         self._cancel_button = ttk.Button(
@@ -113,30 +135,49 @@
             text=self.get_cancel_text(),
             command=self.on_cancel,
         )
         self._cancel_button.grid(column=5, row=1, padx=(0, padding), pady=padding)
 
         self.action_frame.columnconfigure(2, weight=1)
 
+    def on_click_ok_button(self):
+        self.start_work_and_update_ui()
+
+    def has_action_menu(self) -> bool:
+        return False
+
+    def populate_action_menu(self, action_menu: tk.Menu) -> None:
+        pass
+
+    def post_action_menu(self) -> None:
+        self._action_menu.delete(0, "end")
+        post_x = self._menu_button.winfo_rootx()
+        post_y = self._menu_button.winfo_rooty() + self._menu_button.winfo_height()
+        self.populate_action_menu(self._action_menu)
+        self._action_menu.tk_popup(post_x, post_y)
+
     def get_action_text_max_length(self):
         return 35
 
+    def get_initial_log_line_count(self):
+        return 5
+
     def init_log_frame(self):
         self.log_frame = ttk.Frame(self)
         self.log_frame.columnconfigure(1, weight=1)
         self.log_frame.rowconfigure(1, weight=1)
         fixed_font = tk.font.nametofont("TkFixedFont")
         font = fixed_font.copy()
         font.configure(size=round(fixed_font.cget("size") * 0.8))
         self.log_text = tktextext.TextFrame(
             self.log_frame,
             horizontal_scrollbar=False,
             wrap="word",
             borderwidth=1,
-            height=5,
+            height=self.get_initial_log_line_count(),
             width=20,
             font=font,
             read_only=True,
         )
 
         padding = self.get_large_padding()
         self.log_text.grid(row=1, column=1, sticky="nsew", padx=padding, pady=(0, padding))
@@ -190,21 +231,30 @@
     def cancel_work(self):
         # worker should periodically check this value
         self._state = "cancelling"
         self.set_action_text(tr("Cancelling"))
 
     def toggle_log_frame(self, event=None):
         if self.log_frame.winfo_ismapped():
-            self.log_frame.grid_forget()
-            self.rowconfigure(2, weight=1)
-            self.rowconfigure(4, weight=0)
+            self.hide_log_frame()
         else:
-            self.log_frame.grid(row=4, column=0, sticky="nsew")
-            self.rowconfigure(2, weight=0)
-            self.rowconfigure(4, weight=1)
+            self.show_log_frame()
+
+    def show_log_frame(self):
+        self.log_frame.grid(row=4, column=0, sticky="nsew")
+        self.rowconfigure(2, weight=0)
+        self.rowconfigure(4, weight=1)
+
+    def hide_log_frame(self):
+        self.log_frame.grid_forget()
+        self.rowconfigure(2, weight=1)
+        self.rowconfigure(4, weight=0)
+
+    def clear_log(self) -> None:
+        self.log_text.text.direct_delete("1.0", "end")
 
     def get_ok_text(self):
         return tr("OK")
 
     def get_cancel_text(self):
         return tr("Cancel")
 
@@ -252,15 +302,15 @@
         setattr(self, stream_name, getattr(self, stream_name) + text)
 
     def replace_last_line(self, text: str, stream_name="stdout") -> None:
         """Replaces last line in the details box. May be called from another thread."""
         self._work_events_queue.put(("replace", (text, stream_name)))
         setattr(self, stream_name, getattr(self, stream_name) + text)
 
-    def report_progress(self, value: float, maximum: float) -> None:
+    def report_progress(self, value: Optional[float], maximum: Optional[float]) -> None:
         """Updates progress bar. May be called from another thread."""
         self._work_events_queue.put(("progress", (value, maximum)))
 
     def set_action_text(self, text: str) -> None:
         """Updates text above the progress bar. May be called from another thread."""
         self._work_events_queue.put(("action", (text,)))
 
@@ -296,43 +346,43 @@
                 if self._progress_bar["mode"] != "determinate":
                     self._progress_bar["mode"] = "determinate"
                     self._progress_bar.stop()
                 self._progress_bar.configure(value=value, maximum=maximum)
         elif type == "done":
             self.on_done(args[0])
 
+    def allow_single_success(self) -> bool:
+        return True
+
     def on_done(self, success):
         """NB! Don't call from non-ui thread!"""
         self.success = success
-        if self.success:
-            self._state = "done"
-            self._cancel_button.focus_set()
-            self._cancel_button["default"] = "active"
-            self._ok_button["default"] = "normal"
-        elif self._autostart:
-            # Can't try again if failed with autostart
+        if self.success and self.allow_single_success() or self._autostart:
             self._state = "done"
             self._cancel_button.focus_set()
             self._cancel_button["default"] = "active"
             self._ok_button["default"] = "normal"
         else:
-            # allows trying again when failed
-            self._state = "idle"
-            self._ok_button.focus_set()
-            self._ok_button["default"] = "active"
-            self._cancel_button["default"] = "normal"
+            # allows trying again when failed or wasn't final action
+            self.allow_new_work()
 
         self._progress_bar.stop()
         # need to put to determinate mode, otherwise it looks half done
         self._progress_bar["mode"] = "determinate"
         if self.success and self._autostart and not self.log_frame.winfo_ismapped():
             self.close()
 
-        if not self.success and not self.log_frame.winfo_ismapped():
-            self.toggle_log_frame()
+        if not self.success:
+            self.show_log_frame()
+
+    def allow_new_work(self):
+        self._state = "idle"
+        self._ok_button.focus_set()
+        self._ok_button["default"] = "active"
+        self._cancel_button["default"] = "normal"
 
 
 class SubprocessDialog(WorkDialog):
     """Shows incrementally the output of given subprocess.
     Allows cancelling"""
 
     def __init__(self, master, proc, title, long_description=None, autostart=True):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `thonny-4.0.2/thonny.egg-info/PKG-INFO` & `thonny-4.1.0b1.dev0/thonny.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thonny
-Version: 4.0.2
+Version: 4.1.0b1.dev0
 Summary: Python IDE for beginners
 Home-page: https://thonny.org
 Author: Aivar Annamaa and others
 Author-email: thonny@googlegroups.com
 License: MIT
 Project-URL: Source code, https://github.com/thonny/thonny
 Project-URL: Bug tracker, https://github.com/thonny/thonny/issues
@@ -28,14 +28,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Text Editors
 Requires-Python: >=3.8
 License-File: LICENSE.txt
```

### Comparing `thonny-4.0.2/thonny.egg-info/SOURCES.txt` & `thonny-4.1.0b1.dev0/thonny.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,26 @@
 thonny/roughparse.py
 thonny/rst_utils.py
 thonny/running.py
 thonny/shell.py
 thonny/terminal.py
 thonny/tktextext.py
 thonny/token_utils.py
+thonny/udisks.py
 thonny/ui_utils.py
 thonny/workbench.py
 thonny/workdlg.py
 thonny.egg-info/PKG-INFO
 thonny.egg-info/SOURCES.txt
 thonny.egg-info/dependency_links.txt
 thonny.egg-info/entry_points.txt
 thonny.egg-info/requires.txt
 thonny.egg-info/top_level.txt
+thonny/dbus/org.freedesktop.DBus.ObjectManager.xml
+thonny/dbus/org.freedesktop.UDisks2.xml
 thonny/locale/compile_mo.bat
 thonny/locale/register_updates.py
 thonny/locale/thonny.pot
 thonny/locale/update_pot.bat
 thonny/locale/ar_AR/LC_MESSAGES/thonny.mo
 thonny/locale/ar_AR/LC_MESSAGES/thonny.po
 thonny/locale/cs_CZ/LC_MESSAGES/thonny.mo
@@ -129,14 +132,28 @@
 thonny/locale/nb_NO/LC_MESSAGES/thonny.po
 thonny/locale/nl_NL/LC_MESSAGES/thonny.mo
 thonny/locale/nl_NL/LC_MESSAGES/thonny.po
 thonny/locale/nn_NO/LC_MESSAGES/thonny.mo
 thonny/locale/nn_NO/LC_MESSAGES/thonny.po
 thonny/locale/pl_PL/LC_MESSAGES/thonny.mo
 thonny/locale/pl_PL/LC_MESSAGES/thonny.po
+thonny/locale/pt_BR/HELP_CONTENT/assistant.rst
+thonny/locale/pt_BR/HELP_CONTENT/birdseye.rst
+thonny/locale/pt_BR/HELP_CONTENT/debuggers.rst
+thonny/locale/pt_BR/HELP_CONTENT/debugging.rst
+thonny/locale/pt_BR/HELP_CONTENT/dock.rst
+thonny/locale/pt_BR/HELP_CONTENT/errors.rst
+thonny/locale/pt_BR/HELP_CONTENT/flask.rst
+thonny/locale/pt_BR/HELP_CONTENT/index.rst
+thonny/locale/pt_BR/HELP_CONTENT/modes.rst
+thonny/locale/pt_BR/HELP_CONTENT/packages.rst
+thonny/locale/pt_BR/HELP_CONTENT/plotter.rst
+thonny/locale/pt_BR/HELP_CONTENT/program_arguments.rst
+thonny/locale/pt_BR/HELP_CONTENT/shell.rst
+thonny/locale/pt_BR/HELP_CONTENT/turtle.rst
 thonny/locale/pt_BR/LC_MESSAGES/thonny.mo
 thonny/locale/pt_BR/LC_MESSAGES/thonny.po
 thonny/locale/pt_PT/LC_MESSAGES/thonny.mo
 thonny/locale/pt_PT/LC_MESSAGES/thonny.po
 thonny/locale/ro_RO/LC_MESSAGES/thonny.mo
 thonny/locale/ro_RO/LC_MESSAGES/thonny.po
 thonny/locale/ru_RU/LC_MESSAGES/thonny.mo
@@ -253,15 +270,14 @@
 thonny/plugins/help/shell.rst
 thonny/plugins/help/turtle.rst
 thonny/plugins/microbit/__init__.py
 thonny/plugins/microbit/microbit_back.py
 thonny/plugins/microbit/api_stubs/antigravity.pyi
 thonny/plugins/microbit/api_stubs/array.pyi
 thonny/plugins/microbit/api_stubs/audio.pyi
-thonny/plugins/microbit/api_stubs/builtins.py
 thonny/plugins/microbit/api_stubs/collections.py
 thonny/plugins/microbit/api_stubs/gc.py
 thonny/plugins/microbit/api_stubs/love.pyi
 thonny/plugins/microbit/api_stubs/machine.py
 thonny/plugins/microbit/api_stubs/math.py
 thonny/plugins/microbit/api_stubs/microbit.pyi
 thonny/plugins/microbit/api_stubs/micropython.py
@@ -277,15 +293,17 @@
 thonny/plugins/microbit/api_stubs/time.py
 thonny/plugins/microbit/api_stubs/uarray.pyi
 thonny/plugins/microbit/api_stubs/ucollections.py
 thonny/plugins/microbit/api_stubs/ustruct.pyi
 thonny/plugins/microbit/api_stubs/utime.pyi
 thonny/plugins/micropython/__init__.py
 thonny/plugins/micropython/bare_metal_backend.py
+thonny/plugins/micropython/base_flashing_dialog.py
 thonny/plugins/micropython/connection.py
+thonny/plugins/micropython/esptool_dialog.py
 thonny/plugins/micropython/miniterm_wrapper.py
 thonny/plugins/micropython/mp_back.py
 thonny/plugins/micropython/mp_common.py
 thonny/plugins/micropython/mp_front.py
 thonny/plugins/micropython/os_mp_backend.py
 thonny/plugins/micropython/pip_gui.py
 thonny/plugins/micropython/serial_connection.py
```

