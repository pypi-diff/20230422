# Comparing `tmp/wwdtm-2.0.8.tar.gz` & `tmp/wwdtm-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwdtm-2.0.8.tar", last modified: Sun Nov 13 00:18:10 2022, max compression
+gzip compressed data, was "wwdtm-2.0.9.tar", last modified: Sat Apr 22 18:05:29 2023, max compression
```

## Comparing `wwdtm-2.0.8.tar` & `wwdtm-2.0.9.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.357632 wwdtm-2.0.8/
--rw-r--r--   0 lpham      (501) staff       (20)    10142 2021-10-14 22:42:34.000000 wwdtm-2.0.8/LICENSE
--rw-r--r--   0 lpham      (501) staff       (20)      267 2022-01-03 00:36:38.000000 wwdtm-2.0.8/MANIFEST.in
--rw-r--r--   0 lpham      (501) staff       (20)     4229 2022-11-13 00:18:10.357716 wwdtm-2.0.8/PKG-INFO
--rw-r--r--   0 lpham      (501) staff       (20)     3409 2022-11-13 00:18:03.000000 wwdtm-2.0.8/README.rst
--rw-r--r--   0 lpham      (501) staff       (20)      344 2022-03-17 03:36:18.000000 wwdtm-2.0.8/config.json.dist
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.348599 wwdtm-2.0.8/docs/
--rw-r--r--   0 lpham      (501) staff       (20)      686 2021-10-14 22:42:34.000000 wwdtm-2.0.8/docs/Makefile
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.341136 wwdtm-2.0.8/docs/_static/
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.348744 wwdtm-2.0.8/docs/_static/css/
--rw-r--r--   0 lpham      (501) staff       (20)     1168 2022-08-19 03:49:52.000000 wwdtm-2.0.8/docs/_static/css/custom.css
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.348958 wwdtm-2.0.8/docs/_templates/
--rw-r--r--   0 lpham      (501) staff       (20)      193 2021-10-14 22:42:34.000000 wwdtm-2.0.8/docs/_templates/layout.html
--rw-r--r--   0 lpham      (501) staff       (20)     1711 2022-08-19 03:49:52.000000 wwdtm-2.0.8/docs/conf.py
--rw-r--r--   0 lpham      (501) staff       (20)      223 2022-11-13 00:18:03.000000 wwdtm-2.0.8/docs/environment.yaml
--rw-r--r--   0 lpham      (501) staff       (20)     1225 2022-08-19 03:49:52.000000 wwdtm-2.0.8/docs/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2927 2022-11-13 00:18:03.000000 wwdtm-2.0.8/docs/known_issues.rst
--rw-r--r--   0 lpham      (501) staff       (20)      795 2021-10-14 22:42:34.000000 wwdtm-2.0.8/docs/make.bat
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.350218 wwdtm-2.0.8/docs/migrating/
--rw-r--r--   0 lpham      (501) staff       (20)     1886 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/migrating/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1854 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/migrating/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2895 2022-11-13 00:18:03.000000 wwdtm-2.0.8/docs/migrating/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2320 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/migrating/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     3802 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/migrating/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2050 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/migrating/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)     2572 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/migrating/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      318 2022-11-13 00:18:03.000000 wwdtm-2.0.8/docs/requirements.txt
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.351532 wwdtm-2.0.8/docs/tests/
--rw-r--r--   0 lpham      (501) staff       (20)      633 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)      608 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)      300 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)      704 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)     1064 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)      783 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)      757 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      287 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/tests/validation.rst
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.353075 wwdtm-2.0.8/docs/wwdtm/
--rw-r--r--   0 lpham      (501) staff       (20)      467 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/guest.rst
--rw-r--r--   0 lpham      (501) staff       (20)      484 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/host.rst
--rw-r--r--   0 lpham      (501) staff       (20)      435 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/index.rst
--rw-r--r--   0 lpham      (501) staff       (20)      569 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/location.rst
--rw-r--r--   0 lpham      (501) staff       (20)      802 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/panelist.rst
--rw-r--r--   0 lpham      (501) staff       (20)      617 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/scorekeeper.rst
--rw-r--r--   0 lpham      (501) staff       (20)      581 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/show.rst
--rw-r--r--   0 lpham      (501) staff       (20)      195 2022-03-17 03:36:18.000000 wwdtm-2.0.8/docs/wwdtm/validation.rst
--rw-r--r--   0 lpham      (501) staff       (20)      185 2022-11-13 00:18:03.000000 wwdtm-2.0.8/pyproject.toml
--rw-r--r--   0 lpham      (501) staff       (20)      118 2021-11-06 23:15:47.000000 wwdtm-2.0.8/pytest.ini
--rw-r--r--   0 lpham      (501) staff       (20)     1116 2022-11-13 00:18:10.358115 wwdtm-2.0.8/setup.cfg
--rw-r--r--   0 lpham      (501) staff       (20)      436 2022-11-13 00:18:03.000000 wwdtm-2.0.8/setup.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.353252 wwdtm-2.0.8/tests/
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.353620 wwdtm-2.0.8/tests/guest/
--rw-r--r--   0 lpham      (501) staff       (20)     1936 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/guest/test_guest_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4114 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/guest/test_guest_guest.py
--rw-r--r--   0 lpham      (501) staff       (20)     4458 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/guest/test_guest_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.354133 wwdtm-2.0.8/tests/host/
--rw-r--r--   0 lpham      (501) staff       (20)     1927 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/host/test_host_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     3989 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/host/test_host_host.py
--rw-r--r--   0 lpham      (501) staff       (20)     4268 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/host/test_host_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.354609 wwdtm-2.0.8/tests/location/
--rw-r--r--   0 lpham      (501) staff       (20)     4466 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/location/test_location_location.py
--rw-r--r--   0 lpham      (501) staff       (20)     2040 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/location/test_location_recordings.py
--rw-r--r--   0 lpham      (501) staff       (20)     8662 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/location/test_location_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.355598 wwdtm-2.0.8/tests/panelist/
--rw-r--r--   0 lpham      (501) staff       (20)     3235 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/panelist/test_panelist_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4439 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/panelist/test_panelist_panelist.py
--rw-r--r--   0 lpham      (501) staff       (20)     6561 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/panelist/test_panelist_scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     4302 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/panelist/test_panelist_statistics.py
--rw-r--r--   0 lpham      (501) staff       (20)     4610 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/panelist/test_panelist_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.356194 wwdtm-2.0.8/tests/scorekeeper/
--rw-r--r--   0 lpham      (501) staff       (20)     2062 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/scorekeeper/test_scorekeeper_appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     4654 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/scorekeeper/test_scorekeeper_scorekeeper.py
--rw-r--r--   0 lpham      (501) staff       (20)     4942 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/scorekeeper/test_scorekeeper_utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.356877 wwdtm-2.0.8/tests/show/
--rw-r--r--   0 lpham      (501) staff       (20)     3549 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/show/test_show_info.py
--rw-r--r--   0 lpham      (501) staff       (20)     8448 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/show/test_show_info_multiple.py
--rw-r--r--   0 lpham      (501) staff       (20)    12570 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/show/test_show_show.py
--rw-r--r--   0 lpham      (501) staff       (20)     4970 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/show/test_show_utility.py
--rw-r--r--   0 lpham      (501) staff       (20)      881 2022-03-17 03:36:18.000000 wwdtm-2.0.8/tests/test_validation.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.343647 wwdtm-2.0.8/wwdtm/
--rw-r--r--   0 lpham      (501) staff       (20)      752 2022-11-13 00:18:03.000000 wwdtm-2.0.8/wwdtm/__init__.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.344322 wwdtm-2.0.8/wwdtm/guest/
--rw-r--r--   0 lpham      (501) staff       (20)      335 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/guest/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4967 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/guest/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     8434 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/guest/guest.py
--rw-r--r--   0 lpham      (501) staff       (20)     4074 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/guest/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.344909 wwdtm-2.0.8/wwdtm/host/
--rw-r--r--   0 lpham      (501) staff       (20)      327 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/host/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     4735 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/host/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     8296 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/host/host.py
--rw-r--r--   0 lpham      (501) staff       (20)     3974 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/host/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.345391 wwdtm-2.0.8/wwdtm/location/
--rw-r--r--   0 lpham      (501) staff       (20)      357 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/location/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    10545 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/location/location.py
--rw-r--r--   0 lpham      (501) staff       (20)     4558 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/location/recordings.py
--rw-r--r--   0 lpham      (501) staff       (20)     5474 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/location/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.346101 wwdtm-2.0.8/wwdtm/panelist/
--rw-r--r--   0 lpham      (501) staff       (20)      465 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/panelist/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     9176 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/panelist/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     9458 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/panelist/panelist.py
--rw-r--r--   0 lpham      (501) staff       (20)    12396 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/panelist/scores.py
--rw-r--r--   0 lpham      (501) staff       (20)     9318 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/panelist/statistics.py
--rw-r--r--   0 lpham      (501) staff       (20)     4283 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/panelist/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.346589 wwdtm-2.0.8/wwdtm/scorekeeper/
--rw-r--r--   0 lpham      (501) staff       (20)      383 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/scorekeeper/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)     5073 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/scorekeeper/appearances.py
--rw-r--r--   0 lpham      (501) staff       (20)     9109 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/scorekeeper/scorekeeper.py
--rw-r--r--   0 lpham      (501) staff       (20)     4495 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/scorekeeper/utility.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.347346 wwdtm-2.0.8/wwdtm/show/
--rw-r--r--   0 lpham      (501) staff       (20)      367 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/show/__init__.py
--rw-r--r--   0 lpham      (501) staff       (20)    11541 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/show/info.py
--rw-r--r--   0 lpham      (501) staff       (20)    22918 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/show/info_multiple.py
--rw-r--r--   0 lpham      (501) staff       (20)    29398 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/show/show.py
--rw-r--r--   0 lpham      (501) staff       (20)     4152 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/show/utility.py
--rw-r--r--   0 lpham      (501) staff       (20)      813 2022-03-17 03:36:18.000000 wwdtm-2.0.8/wwdtm/validation.py
-drwxr-xr-x   0 lpham      (501) staff       (20)        0 2022-11-13 00:18:10.357512 wwdtm-2.0.8/wwdtm.egg-info/
--rw-r--r--   0 lpham      (501) staff       (20)     4229 2022-11-13 00:18:10.000000 wwdtm-2.0.8/wwdtm.egg-info/PKG-INFO
--rw-r--r--   0 lpham      (501) staff       (20)     2586 2022-11-13 00:18:10.000000 wwdtm-2.0.8/wwdtm.egg-info/SOURCES.txt
--rw-r--r--   0 lpham      (501) staff       (20)        1 2022-11-13 00:18:10.000000 wwdtm-2.0.8/wwdtm.egg-info/dependency_links.txt
--rw-r--r--   0 lpham      (501) staff       (20)      103 2022-11-13 00:18:10.000000 wwdtm-2.0.8/wwdtm.egg-info/requires.txt
--rw-r--r--   0 lpham      (501) staff       (20)        6 2022-11-13 00:18:10.000000 wwdtm-2.0.8/wwdtm.egg-info/top_level.txt
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.457889 wwdtm-2.0.9/
+-rw-r--r--   0 lpham      (501) staff       (20)    10142 2021-10-14 22:42:34.000000 wwdtm-2.0.9/LICENSE
+-rw-r--r--   0 lpham      (501) staff       (20)      267 2022-01-03 00:36:38.000000 wwdtm-2.0.9/MANIFEST.in
+-rw-r--r--   0 lpham      (501) staff       (20)     4229 2023-04-22 18:05:29.457995 wwdtm-2.0.9/PKG-INFO
+-rw-r--r--   0 lpham      (501) staff       (20)     3409 2022-11-13 00:18:03.000000 wwdtm-2.0.9/README.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      344 2022-03-17 03:36:18.000000 wwdtm-2.0.9/config.json.dist
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.431612 wwdtm-2.0.9/docs/
+-rw-r--r--   0 lpham      (501) staff       (20)      686 2021-10-14 22:42:34.000000 wwdtm-2.0.9/docs/Makefile
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.422463 wwdtm-2.0.9/docs/_static/
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.431755 wwdtm-2.0.9/docs/_static/css/
+-rw-r--r--   0 lpham      (501) staff       (20)     1352 2023-04-22 18:04:32.000000 wwdtm-2.0.9/docs/_static/css/custom.css
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.431896 wwdtm-2.0.9/docs/_templates/
+-rw-r--r--   0 lpham      (501) staff       (20)      193 2021-10-14 22:42:34.000000 wwdtm-2.0.9/docs/_templates/layout.html
+-rw-r--r--   0 lpham      (501) staff       (20)     1713 2023-04-22 18:04:32.000000 wwdtm-2.0.9/docs/conf.py
+-rw-r--r--   0 lpham      (501) staff       (20)      223 2023-03-20 00:23:27.000000 wwdtm-2.0.9/docs/environment.yaml
+-rw-r--r--   0 lpham      (501) staff       (20)     1225 2022-08-19 03:49:52.000000 wwdtm-2.0.9/docs/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2927 2022-11-13 00:18:03.000000 wwdtm-2.0.9/docs/known_issues.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      795 2021-10-14 22:42:34.000000 wwdtm-2.0.9/docs/make.bat
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.433411 wwdtm-2.0.9/docs/migrating/
+-rw-r--r--   0 lpham      (501) staff       (20)     1886 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/migrating/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1854 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/migrating/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2895 2022-11-13 00:18:03.000000 wwdtm-2.0.9/docs/migrating/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2320 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/migrating/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     3802 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/migrating/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2050 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/migrating/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     2572 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/migrating/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      318 2023-04-22 18:04:32.000000 wwdtm-2.0.9/docs/requirements.txt
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.435056 wwdtm-2.0.9/docs/tests/
+-rw-r--r--   0 lpham      (501) staff       (20)      633 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      608 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      300 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      704 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)     1064 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      783 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      757 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      287 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/tests/validation.rst
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.436631 wwdtm-2.0.9/docs/wwdtm/
+-rw-r--r--   0 lpham      (501) staff       (20)      467 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/guest.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      484 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/host.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      435 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/index.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      569 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/location.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      802 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/panelist.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      617 2023-04-22 17:09:22.000000 wwdtm-2.0.9/docs/wwdtm/scorekeeper.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      581 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/show.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      195 2022-03-17 03:36:18.000000 wwdtm-2.0.9/docs/wwdtm/validation.rst
+-rw-r--r--   0 lpham      (501) staff       (20)      184 2023-04-22 18:04:32.000000 wwdtm-2.0.9/pyproject.toml
+-rw-r--r--   0 lpham      (501) staff       (20)      118 2021-11-06 23:15:47.000000 wwdtm-2.0.9/pytest.ini
+-rw-r--r--   0 lpham      (501) staff       (20)     1116 2023-04-22 18:05:29.460902 wwdtm-2.0.9/setup.cfg
+-rw-r--r--   0 lpham      (501) staff       (20)      436 2023-04-22 18:04:32.000000 wwdtm-2.0.9/setup.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.436861 wwdtm-2.0.9/tests/
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.437548 wwdtm-2.0.9/tests/guest/
+-rw-r--r--   0 lpham      (501) staff       (20)     1936 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/guest/test_guest_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4114 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/guest/test_guest_guest.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4458 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/guest/test_guest_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.438882 wwdtm-2.0.9/tests/host/
+-rw-r--r--   0 lpham      (501) staff       (20)     1927 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/host/test_host_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     3989 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/host/test_host_host.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4268 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/host/test_host_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.441986 wwdtm-2.0.9/tests/location/
+-rw-r--r--   0 lpham      (501) staff       (20)     4466 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/location/test_location_location.py
+-rw-r--r--   0 lpham      (501) staff       (20)     2040 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/location/test_location_recordings.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8662 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/location/test_location_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.447272 wwdtm-2.0.9/tests/panelist/
+-rw-r--r--   0 lpham      (501) staff       (20)     3235 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/panelist/test_panelist_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4439 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/panelist/test_panelist_panelist.py
+-rw-r--r--   0 lpham      (501) staff       (20)     6561 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/panelist/test_panelist_scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4302 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/panelist/test_panelist_statistics.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4610 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/panelist/test_panelist_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.447730 wwdtm-2.0.9/tests/scorekeeper/
+-rw-r--r--   0 lpham      (501) staff       (20)     2062 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/scorekeeper/test_scorekeeper_appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4654 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/scorekeeper/test_scorekeeper_scorekeeper.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4942 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/scorekeeper/test_scorekeeper_utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.448264 wwdtm-2.0.9/tests/show/
+-rw-r--r--   0 lpham      (501) staff       (20)     3549 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/show/test_show_info.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8448 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/show/test_show_info_multiple.py
+-rw-r--r--   0 lpham      (501) staff       (20)    12570 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/show/test_show_show.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4970 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/show/test_show_utility.py
+-rw-r--r--   0 lpham      (501) staff       (20)      881 2022-03-17 03:36:18.000000 wwdtm-2.0.9/tests/test_validation.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.425402 wwdtm-2.0.9/wwdtm/
+-rw-r--r--   0 lpham      (501) staff       (20)      752 2022-12-28 00:40:42.000000 wwdtm-2.0.9/wwdtm/__init__.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.425997 wwdtm-2.0.9/wwdtm/guest/
+-rw-r--r--   0 lpham      (501) staff       (20)      335 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/guest/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4967 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/guest/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8434 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/guest/guest.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4074 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/guest/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.426635 wwdtm-2.0.9/wwdtm/host/
+-rw-r--r--   0 lpham      (501) staff       (20)      327 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/host/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4735 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/host/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     8296 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/host/host.py
+-rw-r--r--   0 lpham      (501) staff       (20)     3974 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/host/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.427200 wwdtm-2.0.9/wwdtm/location/
+-rw-r--r--   0 lpham      (501) staff       (20)      357 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/location/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    10545 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/location/location.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4558 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/location/recordings.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5474 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/location/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.428140 wwdtm-2.0.9/wwdtm/panelist/
+-rw-r--r--   0 lpham      (501) staff       (20)      465 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/panelist/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9176 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/panelist/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9458 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/panelist/panelist.py
+-rw-r--r--   0 lpham      (501) staff       (20)    12396 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/panelist/scores.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9318 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/panelist/statistics.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4283 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/panelist/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.428943 wwdtm-2.0.9/wwdtm/scorekeeper/
+-rw-r--r--   0 lpham      (501) staff       (20)      383 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/scorekeeper/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)     5073 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/scorekeeper/appearances.py
+-rw-r--r--   0 lpham      (501) staff       (20)     9109 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/scorekeeper/scorekeeper.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4495 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/scorekeeper/utility.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.429994 wwdtm-2.0.9/wwdtm/show/
+-rw-r--r--   0 lpham      (501) staff       (20)      367 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/show/__init__.py
+-rw-r--r--   0 lpham      (501) staff       (20)    11541 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/show/info.py
+-rw-r--r--   0 lpham      (501) staff       (20)    22918 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/show/info_multiple.py
+-rw-r--r--   0 lpham      (501) staff       (20)    29398 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/show/show.py
+-rw-r--r--   0 lpham      (501) staff       (20)     4152 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/show/utility.py
+-rw-r--r--   0 lpham      (501) staff       (20)      813 2022-03-17 03:36:18.000000 wwdtm-2.0.9/wwdtm/validation.py
+drwxr-xr-x   0 lpham      (501) staff       (20)        0 2023-04-22 18:05:29.457773 wwdtm-2.0.9/wwdtm.egg-info/
+-rw-r--r--   0 lpham      (501) staff       (20)     4229 2023-04-22 18:05:29.000000 wwdtm-2.0.9/wwdtm.egg-info/PKG-INFO
+-rw-r--r--   0 lpham      (501) staff       (20)     2586 2023-04-22 18:05:29.000000 wwdtm-2.0.9/wwdtm.egg-info/SOURCES.txt
+-rw-r--r--   0 lpham      (501) staff       (20)        1 2023-04-22 18:05:29.000000 wwdtm-2.0.9/wwdtm.egg-info/dependency_links.txt
+-rw-r--r--   0 lpham      (501) staff       (20)      103 2023-04-22 18:05:29.000000 wwdtm-2.0.9/wwdtm.egg-info/requires.txt
+-rw-r--r--   0 lpham      (501) staff       (20)        6 2023-04-22 18:05:29.000000 wwdtm-2.0.9/wwdtm.egg-info/top_level.txt
```

### Comparing `wwdtm-2.0.8/LICENSE` & `wwdtm-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/PKG-INFO` & `wwdtm-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwdtm
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library used to query data from copy of Wait Wait Stats Database.
 Home-page: https://github.com/questionlp/wwdtm
 Author: Linh Pham
 Author-email: dev@wwdt.me
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/questionlp/wwdtm
 Project-URL: Issue Tracker, https://github.com/questionlp/wwdtm/issues
```

### Comparing `wwdtm-2.0.8/README.rst` & `wwdtm-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/Makefile` & `wwdtm-2.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/_static/css/custom.css` & `wwdtm-2.0.9/docs/_static/css/custom.css`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 @import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Sans:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');
 @import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Serif:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');
 @import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');
 
 @media all {
-    body, input {
-        font-family: "IBM Plex Sans", "Fira Sans", Calibri, sans-serif;
+    body, input, div.sphinxsidebar input {
+        font-family: "IBM Plex Sans", -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
         font-size: 1.05rem;
     }
 
     h1, h2, h3, h4, h5, h6 {
-        font-family: "IBM Plex Serif", Georgia, Cambria, serif;
+        font-family: "IBM Plex Serif", Georgia, Cambria, "Times New Roman", serif;
     }
 
     code, kbd, pre, textarea {
-        font-family: "IBM Plex Mono", "Fira Code", Consolas, monospace;
+        font-family: "IBM Plex Mono", Menlo, Consolas, Monaco, "Liberation Mono", "Lucida Console", monospace;
         font-size: 1rem;
     }
 
     div.sphinxsidebar {
         font-size: 1rem;
     }
```

### Comparing `wwdtm-2.0.8/docs/conf.py` & `wwdtm-2.0.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # vim: set noai syntax=python ts=4 sw=4:
 #
-# Copyright (c) 2018-2022 Linh Pham
+# Copyright (c) 2018-2023 Linh Pham
 # wwdtm is released under the terms of the Apache License 2.0
 import os
 import sys
 
 from pallets_sphinx_themes import ProjectLink  # type: ignore
 
 sys.path.insert(0, os.path.abspath("../"))
@@ -54,15 +54,15 @@
     "index": [
         "globaltoc.html",
         "project.html",
         "searchbox.html",
     ],
     "**": [
         "globaltoc.html",
-        "localtoc.html",
+        # "localtoc.html",
         "relations.html",
         "project.html",
         "searchbox.html",
     ],
 }
 
 html_static_path = [
```

### Comparing `wwdtm-2.0.8/docs/index.rst` & `wwdtm-2.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/known_issues.rst` & `wwdtm-2.0.9/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/make.bat` & `wwdtm-2.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/guest.rst` & `wwdtm-2.0.9/docs/migrating/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/host.rst` & `wwdtm-2.0.9/docs/migrating/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/index.rst` & `wwdtm-2.0.9/docs/migrating/index.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/location.rst` & `wwdtm-2.0.9/docs/migrating/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/panelist.rst` & `wwdtm-2.0.9/docs/migrating/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/scorekeeper.rst` & `wwdtm-2.0.9/docs/migrating/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/migrating/show.rst` & `wwdtm-2.0.9/docs/migrating/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/tests/guest.rst` & `wwdtm-2.0.9/docs/tests/guest.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/tests/host.rst` & `wwdtm-2.0.9/docs/tests/host.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/tests/location.rst` & `wwdtm-2.0.9/docs/tests/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/tests/panelist.rst` & `wwdtm-2.0.9/docs/tests/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/tests/scorekeeper.rst` & `wwdtm-2.0.9/docs/tests/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/tests/show.rst` & `wwdtm-2.0.9/docs/tests/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/wwdtm/location.rst` & `wwdtm-2.0.9/docs/wwdtm/location.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/wwdtm/panelist.rst` & `wwdtm-2.0.9/docs/wwdtm/panelist.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/wwdtm/scorekeeper.rst` & `wwdtm-2.0.9/docs/wwdtm/scorekeeper.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/docs/wwdtm/show.rst` & `wwdtm-2.0.9/docs/wwdtm/show.rst`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/setup.cfg` & `wwdtm-2.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [options]
 package_dir = 
 	=.
 packages = find:
 include_package_data = true
 python_requires = >= 3.8
 install_requires = 
-	mysql-connector-python==8.0.31
-	numpy==1.23.5
+	mysql-connector-python==8.0.33
+	numpy==1.24.2
 	python-dateutil==2.8.2
-	python-slugify==6.1.2
-	pytz==2022.6
+	python-slugify==8.0.1
+	pytz==2023.3
 
 [options.packages.find]
 where = .
 
 [tool:pytest]
 testpaths = tests
 filterwarnings =
```

### Comparing `wwdtm-2.0.8/tests/guest/test_guest_appearances.py` & `wwdtm-2.0.9/tests/guest/test_guest_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/guest/test_guest_guest.py` & `wwdtm-2.0.9/tests/guest/test_guest_guest.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/guest/test_guest_utility.py` & `wwdtm-2.0.9/tests/guest/test_guest_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/host/test_host_appearances.py` & `wwdtm-2.0.9/tests/host/test_host_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/host/test_host_host.py` & `wwdtm-2.0.9/tests/host/test_host_host.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/host/test_host_utility.py` & `wwdtm-2.0.9/tests/host/test_host_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/location/test_location_location.py` & `wwdtm-2.0.9/tests/location/test_location_location.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/location/test_location_recordings.py` & `wwdtm-2.0.9/tests/location/test_location_recordings.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/location/test_location_utility.py` & `wwdtm-2.0.9/tests/location/test_location_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/panelist/test_panelist_appearances.py` & `wwdtm-2.0.9/tests/panelist/test_panelist_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/panelist/test_panelist_panelist.py` & `wwdtm-2.0.9/tests/panelist/test_panelist_panelist.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/panelist/test_panelist_scores.py` & `wwdtm-2.0.9/tests/panelist/test_panelist_scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/panelist/test_panelist_statistics.py` & `wwdtm-2.0.9/tests/panelist/test_panelist_statistics.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/panelist/test_panelist_utility.py` & `wwdtm-2.0.9/tests/panelist/test_panelist_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/scorekeeper/test_scorekeeper_appearances.py` & `wwdtm-2.0.9/tests/scorekeeper/test_scorekeeper_appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/scorekeeper/test_scorekeeper_scorekeeper.py` & `wwdtm-2.0.9/tests/scorekeeper/test_scorekeeper_scorekeeper.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/scorekeeper/test_scorekeeper_utility.py` & `wwdtm-2.0.9/tests/scorekeeper/test_scorekeeper_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/show/test_show_info.py` & `wwdtm-2.0.9/tests/show/test_show_info.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/show/test_show_info_multiple.py` & `wwdtm-2.0.9/tests/show/test_show_info_multiple.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/show/test_show_show.py` & `wwdtm-2.0.9/tests/show/test_show_show.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/show/test_show_utility.py` & `wwdtm-2.0.9/tests/show/test_show_utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/tests/test_validation.py` & `wwdtm-2.0.9/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/__init__.py` & `wwdtm-2.0.9/wwdtm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
     PanelistStatistics,
     PanelistUtility,
 )
 from wwdtm.scorekeeper import Scorekeeper, ScorekeeperAppearances, ScorekeeperUtility
 from wwdtm.show import Show, ShowInfo, ShowInfoMultiple, ShowUtility
 
 
-VERSION = "2.0.8"
+VERSION = "2.0.9"
```

### Comparing `wwdtm-2.0.8/wwdtm/guest/appearances.py` & `wwdtm-2.0.9/wwdtm/guest/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/guest/guest.py` & `wwdtm-2.0.9/wwdtm/guest/guest.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/guest/utility.py` & `wwdtm-2.0.9/wwdtm/guest/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/host/appearances.py` & `wwdtm-2.0.9/wwdtm/host/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/host/host.py` & `wwdtm-2.0.9/wwdtm/host/host.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/host/utility.py` & `wwdtm-2.0.9/wwdtm/host/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/location/location.py` & `wwdtm-2.0.9/wwdtm/location/location.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/location/recordings.py` & `wwdtm-2.0.9/wwdtm/location/recordings.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/location/utility.py` & `wwdtm-2.0.9/wwdtm/location/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/panelist/appearances.py` & `wwdtm-2.0.9/wwdtm/panelist/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/panelist/panelist.py` & `wwdtm-2.0.9/wwdtm/panelist/panelist.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/panelist/scores.py` & `wwdtm-2.0.9/wwdtm/panelist/scores.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/panelist/statistics.py` & `wwdtm-2.0.9/wwdtm/panelist/statistics.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/panelist/utility.py` & `wwdtm-2.0.9/wwdtm/panelist/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/scorekeeper/appearances.py` & `wwdtm-2.0.9/wwdtm/scorekeeper/appearances.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/scorekeeper/scorekeeper.py` & `wwdtm-2.0.9/wwdtm/scorekeeper/scorekeeper.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/scorekeeper/utility.py` & `wwdtm-2.0.9/wwdtm/scorekeeper/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/show/info.py` & `wwdtm-2.0.9/wwdtm/show/info.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/show/info_multiple.py` & `wwdtm-2.0.9/wwdtm/show/info_multiple.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/show/show.py` & `wwdtm-2.0.9/wwdtm/show/show.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/show/utility.py` & `wwdtm-2.0.9/wwdtm/show/utility.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm/validation.py` & `wwdtm-2.0.9/wwdtm/validation.py`

 * *Files identical despite different names*

### Comparing `wwdtm-2.0.8/wwdtm.egg-info/PKG-INFO` & `wwdtm-2.0.9/wwdtm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwdtm
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library used to query data from copy of Wait Wait Stats Database.
 Home-page: https://github.com/questionlp/wwdtm
 Author: Linh Pham
 Author-email: dev@wwdt.me
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/questionlp/wwdtm
 Project-URL: Issue Tracker, https://github.com/questionlp/wwdtm/issues
```

### Comparing `wwdtm-2.0.8/wwdtm.egg-info/SOURCES.txt` & `wwdtm-2.0.9/wwdtm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

