# Comparing `tmp/ds-format-3.6.0.tar.gz` & `tmp/ds-format-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds-format-3.6.0.tar", last modified: Sat Apr  1 17:13:34 2023, max compression
+gzip compressed data, was "ds-format-3.6.1.tar", last modified: Fri Apr 21 22:03:28 2023, max compression
```

## Comparing `ds-format-3.6.0.tar` & `ds-format-3.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.683558 ds-format-3.6.0/
--rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-01 17:13:34.683558 ds-format-3.6.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      563 2023-04-01 17:10:21.000000 ds-format-3.6.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.679558 ds-format-3.6.0/bin/
--rwxr-xr-x   0 peter     (1000) peter     (1000)      247 2023-04-01 17:10:21.000000 ds-format-3.6.0/bin/ds
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.679558 ds-format-3.6.0/ds_format/
--rw-r--r--   0 peter     (1000) peter     (1000)      623 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.679558 ds-format-3.6.0/ds_format/cmd/
--rw-r--r--   0 peter     (1000) peter     (1000)      578 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1645 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/attrs.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/cat.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1212 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/dims.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2565 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/ls.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5039 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/merge.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1335 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/meta.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3076 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/rename.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1231 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/rename_dim.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2244 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/rm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2594 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/select.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5279 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/set_.py
--rw-r--r--   0 peter     (1000) peter     (1000)      850 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/size.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1953 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)      859 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/cmd/type_.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.679558 ds-format-3.6.0/ds_format/drivers/
--rw-r--r--   0 peter     (1000) peter     (1000)      179 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/drivers/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1655 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/drivers/csv.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5574 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/drivers/ds.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2768 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/drivers/hdf.py
--rw-r--r--   0 peter     (1000) peter     (1000)      602 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/drivers/json.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2361 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/drivers/netcdf.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4874 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/help.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8469 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/io.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5067 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/misc.py
--rw-r--r--   0 peter     (1000) peter     (1000)    34143 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/op.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1122 2023-04-01 17:10:21.000000 ds-format-3.6.0/ds_format/validate.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.679558 ds-format-3.6.0/ds_format.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-01 17:13:34.000000 ds-format-3.6.0/ds_format.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1139 2023-04-01 17:13:34.000000 ds-format-3.6.0/ds_format.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-01 17:13:34.000000 ds-format-3.6.0/ds_format.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      131 2023-04-01 17:13:34.000000 ds-format-3.6.0/ds_format.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       10 2023-04-01 17:13:34.000000 ds-format-3.6.0/ds_format.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-01 17:13:34.683558 ds-format-3.6.0/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     1186 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-attrs.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1407 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-cat.1
--rw-r--r--   0 peter     (1000) peter     (1000)      809 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-dims.1
--rw-r--r--   0 peter     (1000) peter     (1000)      299 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-get.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1599 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-ls.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2713 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-merge.1
--rw-r--r--   0 peter     (1000) peter     (1000)      877 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-meta.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1859 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-rename.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1023 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-rename_attr.1
--rw-r--r--   0 peter     (1000) peter     (1000)      912 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-rename_dim.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1388 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-rm.1
--rw-r--r--   0 peter     (1000) peter     (1000)      896 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-rm_attr.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2143 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-select.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3777 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-set.1
--rw-r--r--   0 peter     (1000) peter     (1000)      688 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-set_attrs.1
--rw-r--r--   0 peter     (1000) peter     (1000)      750 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-set_dims.1
--rw-r--r--   0 peter     (1000) peter     (1000)      542 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-size.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1243 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)      548 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-type.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1195 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds-write.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3353 2023-04-01 17:10:21.000000 ds-format-3.6.0/man/ds.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-01 17:13:34.683558 ds-format-3.6.0/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1089 2023-04-01 17:10:21.000000 ds-format-3.6.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.054612 ds-format-3.6.1/
+-rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-21 22:03:28.054612 ds-format-3.6.1/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      563 2023-04-21 22:00:10.000000 ds-format-3.6.1/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/bin/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      247 2023-04-21 22:00:10.000000 ds-format-3.6.1/bin/ds
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format/
+-rw-r--r--   0 peter     (1000) peter     (1000)      623 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format/cmd/
+-rw-r--r--   0 peter     (1000) peter     (1000)      578 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1645 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/attrs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/cat.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1212 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/dims.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2565 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/ls.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5039 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/merge.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1335 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/meta.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3076 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/rename.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1231 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/rename_dim.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2244 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/rm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2594 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/select.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5279 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/set_.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      850 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/size.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1984 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      859 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/type_.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format/drivers/
+-rw-r--r--   0 peter     (1000) peter     (1000)      179 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1655 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/csv.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5574 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/ds.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2768 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/hdf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      602 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/json.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2361 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/netcdf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4874 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/help.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8527 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/io.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5067 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/misc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    34168 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/op.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1122 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/validate.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1139 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      131 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       10 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.054612 ds-format-3.6.1/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1186 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-attrs.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1717 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-cat.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      809 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-dims.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      299 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-get.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1599 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-ls.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2713 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-merge.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      877 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-meta.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1859 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rename.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1023 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rename_attr.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      912 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rename_dim.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1388 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rm.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      896 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rm_attr.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2143 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-select.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3777 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-set.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      688 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-set_attrs.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      750 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-set_dims.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      542 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-size.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1278 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      548 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-type.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1195 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-write.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3353 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-21 22:03:28.054612 ds-format-3.6.1/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1089 2023-04-21 22:00:10.000000 ds-format-3.6.1/setup.py
```

### Comparing `ds-format-3.6.0/PKG-INFO` & `ds-format-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ds-format
-Version: 3.6.0
+Version: 3.6.1
 Summary: ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.
 Home-page: https://ds-format.peterkuma.net
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: dataset,netcdf,hdf,json,numpy
```

### Comparing `ds-format-3.6.0/README.md` & `ds-format-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/__init__.py` & `ds-format-3.6.1/ds_format/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.6.0'
+__version__ = '3.6.1'
 
 import os
 mode = os.environ.get('DS_MODE', 'soft')
 output = 'pst'
 
 from .misc import \
 	escape, \
```

### Comparing `ds-format-3.6.0/ds_format/cmd/__init__.py` & `ds-format-3.6.1/ds_format/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/attrs.py` & `ds-format-3.6.1/ds_format/cmd/attrs.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/cat.py` & `ds-format-3.6.1/ds_format/cmd/cat.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/dims.py` & `ds-format-3.6.1/ds_format/cmd/dims.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/ls.py` & `ds-format-3.6.1/ds_format/cmd/ls.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/main.py` & `ds-format-3.6.1/ds_format/cmd/main.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/merge.py` & `ds-format-3.6.1/ds_format/cmd/merge.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/meta.py` & `ds-format-3.6.1/ds_format/cmd/meta.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/rename.py` & `ds-format-3.6.1/ds_format/cmd/rename.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/rename_dim.py` & `ds-format-3.6.1/ds_format/cmd/rename_dim.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/rm.py` & `ds-format-3.6.1/ds_format/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/select.py` & `ds-format-3.6.1/ds_format/cmd/select.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/set_.py` & `ds-format-3.6.1/ds_format/cmd/set_.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/size.py` & `ds-format-3.6.1/ds_format/cmd/size.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/cmd/stats.py` & `ds-format-3.6.1/ds_format/cmd/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	}}
 	"Output description": {{
 		`count`: "Number of array elements."
 		`max`: "Maximum value."
 		`mean`: "Sample mean."
 		`median`: "Sample median."
 		`min`: "Minimum value."
+		`std`: "Standard deviation."
 		`p68`: "68% confidence interval calculated using percentiles."
 		`p95`: "95% confidence interval calculated using percentiles."
 		`p99`: "99% confidence interval calculated using percentiles."
 	}}
 	desc: "NaNs are ignored in all statistics except for `count`. The output is formatted as [PST](https://github.com/peterkuma/pst)."
 	examples: {{
 "Print statistics of variable temperature in dataset.nc.":
```

### Comparing `ds-format-3.6.0/ds_format/cmd/type_.py` & `ds-format-3.6.1/ds_format/cmd/type_.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/drivers/csv.py` & `ds-format-3.6.1/ds_format/drivers/csv.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/drivers/ds.py` & `ds-format-3.6.1/ds_format/drivers/ds.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/drivers/hdf.py` & `ds-format-3.6.1/ds_format/drivers/hdf.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/drivers/json.py` & `ds-format-3.6.1/ds_format/drivers/json.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/drivers/netcdf.py` & `ds-format-3.6.1/ds_format/drivers/netcdf.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/help.py` & `ds-format-3.6.1/ds_format/help.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/io.py` & `ds-format-3.6.1/ds_format/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,22 +85,22 @@
 				return d
 	raise IOError('%s: Unknown file format' % filename)
 
 def readdir_worker(args):
 	filename, extensions, variables, kwargs = args
 	warnings = []
 	if not os.path.isfile(filename) or not filename.endswith(extensions):
-		return
+		return None, warnings
 	try: d = ds.read(filename, variables=variables, **kwargs)
 	except Exception as e:
 		warnings += [(
 			'%s: %s' % (filename, e),
 			tb.format_exc()
 		)]
-		return
+		return None, warnings
 	ds.var(d, 'filename', filename)
 	ds.dims(d, 'filename', [])
 	return d, warnings
 
 def readdir(dirname, variables=None, merge=None, warnings=[], recursive=False,
 	parallel=False, executor=None, njobs=None, **kwargs):
 	'''
@@ -178,14 +178,16 @@
 			for filename in files
 		])
 	except Exception:
 		if ex is not None: ex.__exit__()
 		raise
 	dd = []
 	for d, w in res:
+		if d is None:
+			continue
 		dd += [d]
 		warnings += w
 	if merge is None:
 		return dd
 	else:
 		n = 0
 		for n, d in enumerate(dd):
```

### Comparing `ds-format-3.6.0/ds_format/misc.py` & `ds-format-3.6.1/ds_format/misc.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format/op.py` & `ds-format-3.6.1/ds_format/op.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,17 @@
 	check(d, 'd', dict)
 	check(attr, 'attr', str)
 	check(var, 'var', [str, None])
 	if len(value) == 0:
 		if require(d, 'attr', attr, var):
 			attrs = ds.attrs(d, var)
 			return attrs[attr]
-	if len(value) == 1:
+		else:
+			return None
+	elif len(value) == 1:
 		meta = ds.meta(d, '' if var is None else var, create=True)
 		meta[ds.escape(attr)] = value[0]
 	else:
 		raise TypeError('only one value argument is expected')
 
 def attrs(d, var=None, *value):
 	'''
```

### Comparing `ds-format-3.6.0/ds_format/validate.py` & `ds-format-3.6.1/ds_format/validate.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/ds_format.egg-info/PKG-INFO` & `ds-format-3.6.1/ds_format.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ds-format
-Version: 3.6.0
+Version: 3.6.1
 Summary: ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.
 Home-page: https://ds-format.peterkuma.net
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: dataset,netcdf,hdf,json,numpy
```

### Comparing `ds-format-3.6.0/ds_format.egg-info/SOURCES.txt` & `ds-format-3.6.1/ds_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-attrs.1` & `ds-format-3.6.1/man/ds-attrs.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-cat.1` & `ds-format-3.6.1/man/ds-cat.1`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 .SH "OPTIONS"
 .TP
 \fB\-h\fR
 Print human\-readable values (time as ISO 8601)\.
 .TP
 \fB\-\-jd\fR
 Convert time variables to Julian date (see Aquarius Time \fIhttps://github\.com/peterkuma/aquarius\-time\fR)\.
+.TP
+\fBsel: {\fR [\fIdim\fR: \fIindex\fR|\fImask\fR]\|\.\|\.\|\. \fB}\fR
+Select data by an index or a mask\. \fIdim\fR is a dimension name to subset along\. \fIindex\fR is an index or a list of indexes to select\. \fImask\fR is \fBtrue\fR or \fBfalse\fR or a list thereof, specifying which indexes to select\.
 .SH "EXAMPLES"
 Print temperature values in dataset\.nc\.
 .IP "" 4
 .nf
 $ ds cat temperature dataset\.nc
 temperature
 16\.000000
```

### Comparing `ds-format-3.6.0/man/ds-dims.1` & `ds-format-3.6.1/man/ds-dims.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-ls.1` & `ds-format-3.6.1/man/ds-ls.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-merge.1` & `ds-format-3.6.1/man/ds-merge.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-meta.1` & `ds-format-3.6.1/man/ds-meta.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-rename.1` & `ds-format-3.6.1/man/ds-rename.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-rename_attr.1` & `ds-format-3.6.1/man/ds-rename_attr.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-rename_dim.1` & `ds-format-3.6.1/man/ds-rename_dim.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-rm.1` & `ds-format-3.6.1/man/ds-rm.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-rm_attr.1` & `ds-format-3.6.1/man/ds-rm_attr.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-select.1` & `ds-format-3.6.1/man/ds-select.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-set.1` & `ds-format-3.6.1/man/ds-set.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-set_attrs.1` & `ds-format-3.6.1/man/ds-set_attrs.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-set_dims.1` & `ds-format-3.6.1/man/ds-set_dims.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-size.1` & `ds-format-3.6.1/man/ds-size.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-stats.1` & `ds-format-3.6.1/man/ds-stats.1`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 .TP
 \fBmedian\fR
 Sample median\.
 .TP
 \fBmin\fR
 Minimum value\.
 .TP
+\fBstd\fR
+Standard deviation\.
+.TP
 \fBp68\fR
 68% confidence interval calculated using percentiles\.
 .TP
 \fBp95\fR
 95% confidence interval calculated using percentiles\.
 .TP
 \fBp99\fR
```

### Comparing `ds-format-3.6.0/man/ds-type.1` & `ds-format-3.6.1/man/ds-type.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds-write.1` & `ds-format-3.6.1/man/ds-write.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/man/ds.1` & `ds-format-3.6.1/man/ds.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.0/setup.py` & `ds-format-3.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 from glob import glob
 
 setup(
 	name='ds-format',
-	version='3.6.0',
+	version='3.6.1',
 	scripts=['bin/ds'],
 	packages=find_packages(),
 	description='ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.',
 	author='Peter Kuma',
 	author_email='peter@peterkuma.net',
 	keywords=['dataset', 'netcdf', 'hdf', 'json', 'numpy'],
 	url='https://ds-format.peterkuma.net',
```

