# Comparing `tmp/stormcatchments-0.3.1.tar.gz` & `tmp/stormcatchments-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormcatchments-0.3.1.tar", last modified: Sat Dec  3 21:53:34 2022, max compression
+gzip compressed data, was "stormcatchments-0.4.0.tar", last modified: Sat Apr 22 13:56:13 2023, max compression
```

## Comparing `stormcatchments-0.3.1.tar` & `stormcatchments-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.831744 stormcatchments-0.3.1/
--rw-r--r--   0 TommyOtt   (501) staff       (20)    35149 2022-12-02 11:46:18.000000 stormcatchments-0.3.1/LICENSE.txt
--rw-r--r--   0 TommyOtt   (501) staff       (20)      290 2022-11-06 13:56:33.000000 stormcatchments-0.3.1/MANIFEST.in
--rw-r--r--   0 TommyOtt   (501) staff       (20)     8125 2022-12-03 21:53:34.828707 stormcatchments-0.3.1/PKG-INFO
--rw-r--r--   0 TommyOtt   (501) staff       (20)     6414 2022-12-01 22:49:01.000000 stormcatchments-0.3.1/README.md
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.116108 stormcatchments-0.3.1/img/
--rw-r--r--   0 TommyOtt   (501) staff       (20)   581188 2022-11-19 14:46:38.000000 stormcatchments-0.3.1/img/example_stormcatchment.png
--rw-r--r--   0 TommyOtt   (501) staff       (20)       38 2022-12-03 21:53:34.832012 stormcatchments-0.3.1/setup.cfg
--rw-r--r--   0 TommyOtt   (501) staff       (20)     1110 2022-12-03 21:48:45.000000 stormcatchments-0.3.1/setup.py
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.491935 stormcatchments-0.3.1/stormcatchments/
--rw-r--r--   0 TommyOtt   (501) staff       (20)      138 2022-12-03 21:49:02.000000 stormcatchments-0.3.1/stormcatchments/__init__.py
--rw-r--r--   0 TommyOtt   (501) staff       (20)      130 2022-11-06 13:48:10.000000 stormcatchments-0.3.1/stormcatchments/constants.py
--rw-r--r--   0 TommyOtt   (501) staff       (20)     6561 2022-11-28 12:23:18.000000 stormcatchments-0.3.1/stormcatchments/delineate.py
--rw-r--r--   0 TommyOtt   (501) staff       (20)    23029 2022-11-19 14:24:58.000000 stormcatchments-0.3.1/stormcatchments/network.py
--rw-r--r--   0 TommyOtt   (501) staff       (20)     1520 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/stormcatchments/terrain.py
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.553829 stormcatchments-0.3.1/stormcatchments.egg-info/
--rw-r--r--   0 TommyOtt   (501) staff       (20)     8125 2022-12-03 21:53:31.000000 stormcatchments-0.3.1/stormcatchments.egg-info/PKG-INFO
--rw-r--r--   0 TommyOtt   (501) staff       (20)     1521 2022-12-03 21:53:31.000000 stormcatchments-0.3.1/stormcatchments.egg-info/SOURCES.txt
--rw-r--r--   0 TommyOtt   (501) staff       (20)        1 2022-12-03 21:53:31.000000 stormcatchments-0.3.1/stormcatchments.egg-info/dependency_links.txt
--rw-r--r--   0 TommyOtt   (501) staff       (20)       92 2022-12-03 21:53:31.000000 stormcatchments-0.3.1/stormcatchments.egg-info/requires.txt
--rw-r--r--   0 TommyOtt   (501) staff       (20)       16 2022-12-03 21:53:31.000000 stormcatchments-0.3.1/stormcatchments.egg-info/top_level.txt
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.594738 stormcatchments-0.3.1/tests/
--rw-r--r--   0 TommyOtt   (501) staff       (20)        0 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/__init__.py
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.068232 stormcatchments-0.3.1/tests/test_data/
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.766380 stormcatchments-0.3.1/tests/test_data/johnson_vt/
--rw-r--r--   0 TommyOtt   (501) staff       (20)  7035209 2022-12-03 21:46:39.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/dem.tif
--rw-r--r--   0 TommyOtt   (501) staff       (20)       10 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/initial_catchment.cpg
--rw-r--r--   0 TommyOtt   (501) staff       (20)       85 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/initial_catchment.dbf
--rw-r--r--   0 TommyOtt   (501) staff       (20)      439 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/initial_catchment.prj
--rw-r--r--   0 TommyOtt   (501) staff       (20)     7100 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/initial_catchment.shp
--rw-r--r--   0 TommyOtt   (501) staff       (20)      108 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/initial_catchment.shx
--rw-r--r--   0 TommyOtt   (501) staff       (20)       10 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.cpg
--rw-r--r--   0 TommyOtt   (501) staff       (20)    44739 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.dbf
--rw-r--r--   0 TommyOtt   (501) staff       (20)      446 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.prj
--rw-r--r--   0 TommyOtt   (501) staff       (20)     5852 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.shp
--rw-r--r--   0 TommyOtt   (501) staff       (20)      380 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.shx
--rw-r--r--   0 TommyOtt   (501) staff       (20)       10 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.cpg
--rw-r--r--   0 TommyOtt   (501) staff       (20)    34105 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.dbf
--rw-r--r--   0 TommyOtt   (501) staff       (20)      446 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.prj
--rw-r--r--   0 TommyOtt   (501) staff       (20)      912 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.shp
--rw-r--r--   0 TommyOtt   (501) staff       (20)      332 2022-10-09 20:18:33.000000 stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.shx
-drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2022-12-03 21:53:34.820533 stormcatchments-0.3.1/tests/test_data/synthetic/
--rw-r--r--   0 TommyOtt   (501) staff       (20)        5 2022-10-13 11:09:25.000000 stormcatchments-0.3.1/tests/test_data/synthetic/lines.cpg
--rw-r--r--   0 TommyOtt   (501) staff       (20)      553 2022-11-19 14:17:27.000000 stormcatchments-0.3.1/tests/test_data/synthetic/lines.dbf
--rw-r--r--   0 TommyOtt   (501) staff       (20)      425 2022-10-13 11:09:25.000000 stormcatchments-0.3.1/tests/test_data/synthetic/lines.prj
--rw-r--r--   0 TommyOtt   (501) staff       (20)      668 2022-11-19 14:17:27.000000 stormcatchments-0.3.1/tests/test_data/synthetic/lines.shp
--rw-r--r--   0 TommyOtt   (501) staff       (20)      140 2022-11-19 14:17:27.000000 stormcatchments-0.3.1/tests/test_data/synthetic/lines.shx
--rw-r--r--   0 TommyOtt   (501) staff       (20)        5 2022-10-13 11:06:19.000000 stormcatchments-0.3.1/tests/test_data/synthetic/pts.cpg
--rw-r--r--   0 TommyOtt   (501) staff       (20)      818 2022-10-13 11:39:45.000000 stormcatchments-0.3.1/tests/test_data/synthetic/pts.dbf
--rw-r--r--   0 TommyOtt   (501) staff       (20)      425 2022-10-13 11:06:19.000000 stormcatchments-0.3.1/tests/test_data/synthetic/pts.prj
--rw-r--r--   0 TommyOtt   (501) staff       (20)      548 2022-10-13 11:39:45.000000 stormcatchments-0.3.1/tests/test_data/synthetic/pts.shp
--rw-r--r--   0 TommyOtt   (501) staff       (20)      228 2022-10-13 11:39:45.000000 stormcatchments-0.3.1/tests/test_data/synthetic/pts.shx
--rw-r--r--   0 TommyOtt   (501) staff       (20)     1591 2022-11-06 13:48:10.000000 stormcatchments-0.3.1/tests/test_delineate.py
--rw-r--r--   0 TommyOtt   (501) staff       (20)     4948 2022-11-06 13:48:10.000000 stormcatchments-0.3.1/tests/test_network.py
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:13.686030 stormcatchments-0.4.0/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)    35149 2022-12-02 11:46:18.000000 stormcatchments-0.4.0/LICENSE.txt
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      290 2022-11-06 13:56:33.000000 stormcatchments-0.4.0/MANIFEST.in
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     8098 2023-04-22 13:56:13.685429 stormcatchments-0.4.0/PKG-INFO
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     7368 2023-04-22 13:23:07.000000 stormcatchments-0.4.0/README.md
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:11.095902 stormcatchments-0.4.0/img/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)   581188 2022-11-19 14:46:38.000000 stormcatchments-0.4.0/img/example_stormcatchment.png
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       38 2023-04-22 13:56:13.686174 stormcatchments-0.4.0/setup.cfg
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     1110 2023-04-22 13:24:02.000000 stormcatchments-0.4.0/setup.py
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:11.429293 stormcatchments-0.4.0/stormcatchments/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      148 2023-04-22 13:24:11.000000 stormcatchments-0.4.0/stormcatchments/__init__.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      130 2022-11-06 13:48:10.000000 stormcatchments-0.4.0/stormcatchments/constants.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     6570 2023-04-22 12:49:38.000000 stormcatchments-0.4.0/stormcatchments/delineate.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)    23030 2023-03-08 12:30:47.000000 stormcatchments-0.4.0/stormcatchments/network.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     1520 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/stormcatchments/terrain.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     3817 2023-01-30 12:40:08.000000 stormcatchments-0.4.0/stormcatchments/topology.py
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:11.489846 stormcatchments-0.4.0/stormcatchments.egg-info/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     8098 2023-04-22 13:56:10.000000 stormcatchments-0.4.0/stormcatchments.egg-info/PKG-INFO
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     1572 2023-04-22 13:56:10.000000 stormcatchments-0.4.0/stormcatchments.egg-info/SOURCES.txt
+-rw-r--r--   0 TommyOtt   (501) staff       (20)        1 2023-04-22 13:56:10.000000 stormcatchments-0.4.0/stormcatchments.egg-info/dependency_links.txt
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       92 2023-04-22 13:56:10.000000 stormcatchments-0.4.0/stormcatchments.egg-info/requires.txt
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       16 2023-04-22 13:56:10.000000 stormcatchments-0.4.0/stormcatchments.egg-info/top_level.txt
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:11.590795 stormcatchments-0.4.0/tests/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)        0 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/__init__.py
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:11.029313 stormcatchments-0.4.0/tests/test_data/
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:12.872914 stormcatchments-0.4.0/tests/test_data/johnson_vt/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)  7035209 2022-12-03 21:46:39.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/dem.tif
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       10 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/initial_catchment.cpg
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       85 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/initial_catchment.dbf
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      439 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/initial_catchment.prj
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     7100 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/initial_catchment.shp
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      108 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/initial_catchment.shx
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       10 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.cpg
+-rw-r--r--   0 TommyOtt   (501) staff       (20)    44739 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.dbf
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      446 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.prj
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     5852 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.shp
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      380 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.shx
+-rw-r--r--   0 TommyOtt   (501) staff       (20)       10 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.cpg
+-rw-r--r--   0 TommyOtt   (501) staff       (20)    34105 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.dbf
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      446 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.prj
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      912 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.shp
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      332 2022-10-09 20:18:33.000000 stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.shx
+drwxr-xr-x   0 TommyOtt   (501) staff       (20)        0 2023-04-22 13:56:13.684638 stormcatchments-0.4.0/tests/test_data/synthetic/
+-rw-r--r--   0 TommyOtt   (501) staff       (20)        5 2022-10-13 11:09:25.000000 stormcatchments-0.4.0/tests/test_data/synthetic/lines.cpg
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      735 2023-01-23 12:33:43.000000 stormcatchments-0.4.0/tests/test_data/synthetic/lines.dbf
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      425 2022-10-13 11:09:25.000000 stormcatchments-0.4.0/tests/test_data/synthetic/lines.prj
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      892 2023-01-23 12:33:43.000000 stormcatchments-0.4.0/tests/test_data/synthetic/lines.shp
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      156 2023-01-23 12:33:43.000000 stormcatchments-0.4.0/tests/test_data/synthetic/lines.shx
+-rw-r--r--   0 TommyOtt   (501) staff       (20)        5 2022-10-13 11:06:19.000000 stormcatchments-0.4.0/tests/test_data/synthetic/pts.cpg
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     1023 2023-01-23 12:33:43.000000 stormcatchments-0.4.0/tests/test_data/synthetic/pts.dbf
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      425 2022-10-13 11:06:19.000000 stormcatchments-0.4.0/tests/test_data/synthetic/pts.prj
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      688 2023-01-23 12:33:43.000000 stormcatchments-0.4.0/tests/test_data/synthetic/pts.shp
+-rw-r--r--   0 TommyOtt   (501) staff       (20)      268 2023-01-23 12:33:43.000000 stormcatchments-0.4.0/tests/test_data/synthetic/pts.shx
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     1591 2022-11-06 13:48:10.000000 stormcatchments-0.4.0/tests/test_delineate.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     4948 2022-11-06 13:48:10.000000 stormcatchments-0.4.0/tests/test_network.py
+-rw-r--r--   0 TommyOtt   (501) staff       (20)     1977 2023-01-30 12:40:08.000000 stormcatchments-0.4.0/tests/test_topology.py
```

### Comparing `stormcatchments-0.3.1/LICENSE.txt` & `stormcatchments-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/README.md` & `stormcatchments-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stormcatchments
 [![PyPi](https://img.shields.io/pypi/v/stormcatchments.svg)](https://pypi.python.org/pypi/stormcatchments)
+[![docs](https://readthedocs.org/projects/stormcatchments/badge)](https://stormcatchments.readthedocs.io/en/latest/)
 
 ## Stormwater network aware catchment delineation
 
 Converts existing stormwater infrastucture GIS feature data (points and lines) into a
 ```networkx``` directed graph (```DiGraph```) object, then utilizes the ```DiGraph``` to
 incorporate subsurface flows into urban stormwater catchment delineation.
 
@@ -116,7 +117,14 @@
 1) ```from_sources```: This is the default. This method traces networks upstream from their discharge points. This assumes that subnetworks are comprised of one or more flow sinks that flow to a single flow source. If multiple flow sources are connected to a given flow sink, this method will run into issues since determining which flow source is the terminal node in the graph would need to incorporate pipe elevation data somehow.
 2) ```vertex_order```: This defines the subsurface flow direction using the order of verticies in the line data (flowing from the first to last vertex).
 3) ```vertex_order_r```: This is the same as above, but in reverse (flowing from last to first vertex).
 
 Two other potential methods that are not yet implemented are:
 - Using surface elevation data as an analog for for subsurface pipe elevations. In flat urban settings this would likely have a lot of issues/inaccuracies.
 - Using pipe invert data from the attributes of point or line data. This would require manual preparation by the user but would be the most accurate method.
+
+## Validating network topology
+
+Several functions are available in ```stormcatchments.topology``` to assist in validating the topology of your input data. These include:
+- ```find_floating_points```: Returns points that aren't snapped to a line vertex. Floating points cannot be incorporated into the Network.
+- ```snap_points```: Returns an altered copy of a ```stormcatchments.Network``` in which any floating points are snapped to the nearest vertex, within a specified snapping tolerance.
+- ```find_multi_outlet```: Returns a ```GeoDataFrame``` containing geometry for subgraphs within a ```Network``` that have multiple flow sources (outlets). Delineation results may not be optimal in mutli-outlet subgraphs depending on how the directions are resolved within them. Having a single outlet ensures predictable delineation results.
```

### Comparing `stormcatchments-0.3.1/img/example_stormcatchment.png` & `stormcatchments-0.4.0/img/example_stormcatchment.png`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/setup.py` & `stormcatchments-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
   long_description = f.read()
 
 setup(
   name='stormcatchments',
-  version='0.3.1',
+  version='0.4.0',
   description='Stormwater network aware catchment delineation',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author='Thomas Ott',    
   author_email='tommy.ott617@gmail.com',
   license='GPLv3',
   url='https://github.com/t-ott/stormcatchments',
```

### Comparing `stormcatchments-0.3.1/stormcatchments/delineate.py` & `stormcatchments-0.4.0/stormcatchments/delineate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import copy
+from copy import deepcopy
+
 import geopandas as gpd
 import numpy as np
 import pysheds
 from shapely.geometry import Polygon
 
 from stormcatchments.network import Network
 
@@ -38,16 +39,16 @@
       The minimum accumulation threshold used during pour point snapping
     
     Returns
     -------
     catchment : gpd.GeoDataFrame
       A GeoDataFrame containing the newly delineated catchment polygon
     '''
-    # create a deep copy of the grid to not manipulate original grid
-    grid = copy.deepcopy(grid)
+    # create a deepcopy of the grid to not manipulate original grid
+    grid = deepcopy(grid)
     x, y = pour_pt
     x_snap, y_snap = grid.snap_to_mask(acc > acc_thresh, (x, y))
     catch = grid.catchment(x=x_snap, y=y_snap, fdir=fdir)
     grid.clip_to(catch)
     catch_view = grid.view(catch, dtype=np.uint8)
     catch_vec = grid.polygonize(catch_view)
```

### Comparing `stormcatchments-0.3.1/stormcatchments/network.py` & `stormcatchments-0.4.0/stormcatchments/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import namedtuple
+from typing import Optional
+import warnings
+
 import geopandas as gpd
-import pandas as pd
 import networkx as nx
-from typing import Optional
+import pandas as pd
 from shapely.geometry import LineString, MultiPoint, Point
-import warnings
 
 
 def get_point_coords(pt_geom, decimals: int=None) -> tuple:
     '''
     Get and x, y coordinate tuple from a Point or MultiPoint shapely geometry
 
     Parameters
```

### Comparing `stormcatchments-0.3.1/stormcatchments/terrain.py` & `stormcatchments-0.4.0/stormcatchments/terrain.py`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/stormcatchments.egg-info/SOURCES.txt` & `stormcatchments-0.4.0/stormcatchments.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 setup.py
 img/example_stormcatchment.png
 stormcatchments/__init__.py
 stormcatchments/constants.py
 stormcatchments/delineate.py
 stormcatchments/network.py
 stormcatchments/terrain.py
+stormcatchments/topology.py
 stormcatchments.egg-info/PKG-INFO
 stormcatchments.egg-info/SOURCES.txt
 stormcatchments.egg-info/dependency_links.txt
 stormcatchments.egg-info/requires.txt
 stormcatchments.egg-info/top_level.txt
 tests/__init__.py
 tests/test_delineate.py
 tests/test_network.py
+tests/test_topology.py
 tests/test_data/johnson_vt/dem.tif
 tests/test_data/johnson_vt/initial_catchment.cpg
 tests/test_data/johnson_vt/initial_catchment.dbf
 tests/test_data/johnson_vt/initial_catchment.prj
 tests/test_data/johnson_vt/initial_catchment.shp
 tests/test_data/johnson_vt/initial_catchment.shx
 tests/test_data/johnson_vt/storm_lines.cpg
```

### Comparing `stormcatchments-0.3.1/tests/test_data/johnson_vt/dem.tif` & `stormcatchments-0.4.0/tests/test_data/johnson_vt/dem.tif`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_data/johnson_vt/initial_catchment.shp` & `stormcatchments-0.4.0/tests/test_data/johnson_vt/initial_catchment.shp`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.dbf` & `stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.dbf`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_lines.shp` & `stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_lines.shp`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.dbf` & `stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.dbf`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_data/johnson_vt/storm_pts.shp` & `stormcatchments-0.4.0/tests/test_data/johnson_vt/storm_pts.shp`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_data/synthetic/lines.shp` & `stormcatchments-0.4.0/tests/test_data/synthetic/lines.shp`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 0000 270a 0000 0000 0000 0000 0000 0000  ..'.............
-00000010: 0000 0000 0000 0000 0000 014e e803 0000  ...........N....
-00000020: 0300 0000 784f 4d50 e5cd 5dc1 0160 f256  ....xOMP..]..`.V
+00000010: 0000 0000 0000 0000 0000 01be e803 0000  ................
+00000020: 0300 0000 d7db ecc4 f0cd 5dc1 0160 f256  ..........]..`.V
 00000030: eab4 5341 3b63 9a6c d8cd 5dc1 8606 38a1  ..SA;c.l..]...8.
 00000040: f8b4 5341 0000 0000 0000 0000 0000 0000  ..SA............
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0001 0000 0038 0300 0000  ...........8....
 00000070: f600 1b5d e4cd 5dc1 0160 f256 eab4 5341  ...]..]..`.V..SA
 00000080: 9514 2235 e0cd 5dc1 0e60 6649 edb4 5341  .."5..]..`fI..SA
 00000090: 0100 0000 0400 0000 0000 0000 f600 1b5d  ...............]
@@ -35,8 +35,22 @@
 00000220: ebb4 5341 0000 0005 0000 0038 0300 0000  ..SA.......8....
 00000230: 784f 4d50 e5cd 5dc1 d1eb 3e46 f8b4 5341  xOMP..]...>F..SA
 00000240: 953b d019 ddcd 5dc1 8606 38a1 f8b4 5341  .;....]...8...SA
 00000250: 0100 0000 0400 0000 0000 0000 953b d019  .............;..
 00000260: ddcd 5dc1 d1eb 3e46 f8b4 5341 f12b 924c  ..]...>F..SA.+.L
 00000270: e0cd 5dc1 d1eb 3e46 f8b4 5341 2842 99dd  ..]...>F..SA(B..
 00000280: e2cd 5dc1 b8f4 9164 f8b4 5341 784f 4d50  ..]....d..SAxOMP
-00000290: e5cd 5dc1 8606 38a1 f8b4 5341            ..]...8...SA
+00000290: e5cd 5dc1 8606 38a1 f8b4 5341 0000 0006  ..]...8...SA....
+000002a0: 0000 0040 0300 0000 d7db ecc4 f0cd 5dc1  ...@..........].
+000002b0: aff8 2bfa eab4 5341 2ca3 1b95 ebcd 5dc1  ..+...SA,.....].
+000002c0: c740 4ce1 f5b4 5341 0100 0000 0500 0000  .@L...SA........
+000002d0: 0000 0000 d7db ecc4 f0cd 5dc1 c740 4ce1  ..........]..@L.
+000002e0: f5b4 5341 6952 ae46 edcd 5dc1 d3d2 aaa9  ..SAiR.F..].....
+000002f0: f4b4 5341 2ca3 1b95 ebcd 5dc1 041b 25cb  ..SA,.....]...%.
+00000300: efb4 5341 e3e7 3a54 edcd 5dc1 aff8 2bfa  ..SA..:T..]...+.
+00000310: eab4 5341 e3e7 3a54 edcd 5dc1 aff8 2bfa  ..SA..:T..]...+.
+00000320: eab4 5341 0000 0007 0000 0028 0300 0000  ..SA.......(....
+00000330: 6952 ae46 edcd 5dc1 d3d2 aaa9 f4b4 5341  iR.F..].......SA
+00000340: 75e4 0c0f eccd 5dc1 72b0 84bb f7b4 5341  u.....].r.....SA
+00000350: 0100 0000 0200 0000 0000 0000 75e4 0c0f  ............u...
+00000360: eccd 5dc1 72b0 84bb f7b4 5341 6952 ae46  ..].r.....SAiR.F
+00000370: edcd 5dc1 d3d2 aaa9 f4b4 5341            ..].......SA
```

### Comparing `stormcatchments-0.3.1/tests/test_data/synthetic/pts.dbf` & `stormcatchments-0.4.0/tests/test_data/synthetic/pts.dbf`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 037a 0a0d 1000 0000 a100 2900 0000 0000  .z........).....
+00000000: 037b 0116 1500 0000 a100 2900 0000 0000  .{........).....
 00000010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 6964 0000 0000 0000 0000 004e 0000 0000  id.........N....
 00000030: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
 00000040: 4953 5f53 4f55 5243 4500 004e 0000 0000  IS_SOURCE..N....
 00000050: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 4953 5f53 494e 4b00 0000 004e 0000 0000  IS_SINK....N....
 00000070: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
@@ -45,8 +45,20 @@
 000002c0: 3420 2020 2020 2020 2020 3120 2020 2020  4         1     
 000002d0: 2020 2020 3063 6f6e 7365 635f 6f75 7420      0consec_out 
 000002e0: 2020 2020 2020 2020 3135 2020 2020 2020          15      
 000002f0: 2020 2030 2020 2020 2020 2020 2031 636f     0         1co
 00000300: 6e73 6563 5f6f 7574 2020 2020 2020 2020  nsec_out        
 00000310: 2031 3620 2020 2020 2020 2020 3020 2020   16         0   
 00000320: 2020 2020 2020 3163 6f6e 7365 635f 6f75        1consec_ou
-00000330: 741a                                     t.
+00000330: 7420 2020 2020 2020 2020 3137 2020 2020  t         17    
+00000340: 2020 2020 2030 2020 2020 2020 2020 2031       0         1
+00000350: 666c 6f61 7469 6e67 5f70 2020 2020 2020  floating_p      
+00000360: 2020 2031 3820 2020 2020 2020 2020 3020     18         0 
+00000370: 2020 2020 2020 2020 3166 6c6f 6174 696e          1floatin
+00000380: 675f 7020 2020 2020 2020 2020 3139 2020  g_p         19  
+00000390: 2020 2020 2020 2030 2020 2020 2020 2020         0        
+000003a0: 2031 666c 6f61 7469 6e67 5f70 2020 2020   1floating_p    
+000003b0: 2020 2020 2032 3020 2020 2020 2020 2020       20         
+000003c0: 3020 2020 2020 2020 2020 3166 6c6f 6174  0         1float
+000003d0: 696e 675f 7020 2020 2020 2020 2020 3231  ing_p         21
+000003e0: 2020 2020 2020 2020 2031 2020 2020 2020           1      
+000003f0: 2020 2030 666c 6f61 7469 6e67 5f70 1a       0floating_p.
```

### Comparing `stormcatchments-0.3.1/tests/test_delineate.py` & `stormcatchments-0.4.0/tests/test_delineate.py`

 * *Files identical despite different names*

### Comparing `stormcatchments-0.3.1/tests/test_network.py` & `stormcatchments-0.4.0/tests/test_network.py`

 * *Files identical despite different names*

