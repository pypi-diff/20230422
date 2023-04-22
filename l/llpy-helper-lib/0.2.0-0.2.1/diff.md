# Comparing `tmp/llpy-helper-lib-0.2.0.tar.gz` & `tmp/llpy-helper-lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llpy-helper-lib-0.2.0.tar", last modified: Tue Apr  4 15:13:52 2023, max compression
+gzip compressed data, was "llpy-helper-lib-0.2.1.tar", last modified: Sat Apr 22 10:17:22 2023, max compression
```

## Comparing `llpy-helper-lib-0.2.0.tar` & `llpy-helper-lib-0.2.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0     1077 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/LICENSE
--rw-r--r--   0        0        0     1047 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/README.md
--rw-r--r--   0        0        0     4867 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/__init__.py
--rw-r--r--   0        0        0       48 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/directionangle/__init__.py
--rw-r--r--   0        0        0      813 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/directionangle/__init__.pyi
--rw-r--r--   0        0        0      338 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/enumdefine/__init__.pyi
--rw-r--r--   0        0        0       32 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/format/__init__.py
--rw-r--r--   0        0        0     1758 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/format/__init__.pyi
--rw-r--r--   0        0        0       68 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/pos/__init__.py
--rw-r--r--   0        0        0     1230 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/pos/__init__.pyi
--rw-r--r--   0        0        0      444 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/base/types.py
--rw-r--r--   0        0        0       59 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/block/__init__.py
--rw-r--r--   0        0        0     4230 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/block/__init__.pyi
--rw-r--r--   0        0        0       83 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/block/entity/__init__.py
--rw-r--r--   0        0        0     1039 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/block/entity/__init__.pyi
--rw-r--r--   0        0        0       67 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/__init__.py
--rw-r--r--   0        0        0     7037 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/__init__.pyi
--rw-r--r--   0        0        0      156 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/enums/__init__.py
--rw-r--r--   0        0        0     4983 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/enums/__init__.pyi
--rw-r--r--   0        0        0       91 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/origin/__init__.py
--rw-r--r--   0        0        0      873 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/origin/__init__.pyi
--rw-r--r--   0        0        0       91 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/output/__init__.py
--rw-r--r--   0        0        0     1754 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/output/__init__.pyi
--rw-r--r--   0        0        0     3381 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/command/types.py
--rw-r--r--   0        0        0       46 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/config/ini/__init__.py
--rw-r--r--   0        0        0     5673 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/config/ini/__init__.pyi
--rw-r--r--   0        0        0       48 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/config/json/__init__.py
--rw-r--r--   0        0        0     3738 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/config/json/__init__.pyi
--rw-r--r--   0        0        0      221 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/config/types.py
--rw-r--r--   0        0        0       75 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/container/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/container/__init__.pyi
--rw-r--r--   0        0        0       28 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/data/__init__.py
--rw-r--r--   0        0        0     4357 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/data/__init__.pyi
--rw-r--r--   0        0        0      330 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/data/types.py
--rw-r--r--   0        0        0       38 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/dbsession/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/dbsession/__init__.pyi
--rw-r--r--   0        0        0       32 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/dbstmt/__init__.py
--rw-r--r--   0        0        0     4663 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/dbstmt/__init__.pyi
--rw-r--r--   0        0        0       40 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/kvdb/__init__.py
--rw-r--r--   0        0        0     1657 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/kvdb/__init__.pyi
--rw-r--r--   0        0        0      570 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/db/types.py
--rw-r--r--   0        0        0       63 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/entity/__init__.py
--rw-r--r--   0        0        0    15776 2023-04-04 15:13:40.666202 llpy-helper-lib-0.2.0/llpy/classes/entity/__init__.pyi
--rw-r--r--   0        0        0       93 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/entity/damagecause/__init__.py
--rw-r--r--   0        0        0     3678 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/entity/damagecause/__init__.pyi
--rw-r--r--   0        0        0     1962 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/entity/types.py
--rw-r--r--   0        0        0       28 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/file/__init__.py
--rw-r--r--   0        0        0    12487 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/file/__init__.pyi
--rw-r--r--   0        0        0      208 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/file/types.py
--rw-r--r--   0        0        0       79 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/form/custom/__init__.py
--rw-r--r--   0        0        0     3106 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/form/custom/__init__.pyi
--rw-r--r--   0        0        0       79 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/form/simple/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/form/simple/__init__.pyi
--rw-r--r--   0        0        0       28 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/i18n/__init__.py
--rw-r--r--   0        0        0     3434 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/i18n/__init__.pyi
--rw-r--r--   0        0        0       43 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/i18n/types.py
--rw-r--r--   0        0        0       55 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/item/__init__.py
--rw-r--r--   0        0        0     4991 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/item/__init__.pyi
--rw-r--r--   0        0        0       24 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/ll/__init__.py
--rw-r--r--   0        0        0     7505 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/ll/__init__.pyi
--rw-r--r--   0        0        0      612 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/ll/types.py
--rw-r--r--   0        0        0       34 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/ll/version/__init__.py
--rw-r--r--   0        0        0      471 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/ll/version/__init__.pyi
--rw-r--r--   0        0        0       32 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/logger/__init__.py
--rw-r--r--   0        0        0     3440 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/logger/__init__.pyi
--rw-r--r--   0        0        0      431 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/logger/types.py
--rw-r--r--   0        0        0       24 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/mc/__init__.py
--rw-r--r--   0        0        0    82826 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/mc/__init__.pyi
--rw-r--r--   0        0        0     1930 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/mc/types.py
--rw-r--r--   0        0        0       30 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/money/__init__.py
--rw-r--r--   0        0        0     2537 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/money/__init__.pyi
--rw-r--r--   0        0        0      468 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/money/types.py
--rw-r--r--   0        0        0       42 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/enum/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/enum/__init__.pyi
--rw-r--r--   0        0        0       48 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/function/__init__.py
--rw-r--r--   0        0        0     2598 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/function/__init__.pyi
--rw-r--r--   0        0        0       46 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/globalpointer/__init__.py
--rw-r--r--   0        0        0      861 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/globalpointer/__init__.pyi
--rw-r--r--   0        0        0       40 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/hook/__init__.py
--rw-r--r--   0        0        0      700 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/hook/__init__.pyi
--rw-r--r--   0        0        0       42 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/patch/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/patch/__init__.pyi
--rw-r--r--   0        0        0       46 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/pointer/__init__.py
--rw-r--r--   0        0        0     4298 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/pointer/__init__.pyi
--rw-r--r--   0        0        0       50 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/stdstring/__init__.py
--rw-r--r--   0        0        0     1693 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/stdstring/__init__.pyi
--rw-r--r--   0        0        0      953 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/native/types.py
--rw-r--r--   0        0        0      324 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/base/__init__.py
--rw-r--r--   0        0        0     2021 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/base/__init__.pyi
--rw-r--r--   0        0        0       42 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/compound/__init__.py
--rw-r--r--   0        0        0     7453 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/compound/__init__.pyi
--rw-r--r--   0        0        0       34 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/list/__init__.py
--rw-r--r--   0        0        0     6992 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/list/__init__.pyi
--rw-r--r--   0        0        0       26 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/static/__init__.py
--rw-r--r--   0        0        0     2382 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/static/__init__.pyi
--rw-r--r--   0        0        0     1181 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/nbt/types.py
--rw-r--r--   0        0        0       34 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/__init__.py
--rw-r--r--   0        0        0     3497 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/__init__.pyi
--rw-r--r--   0        0        0       42 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/httprequest/__init__.py
--rw-r--r--   0        0        0     1289 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/httprequest/__init__.pyi
--rw-r--r--   0        0        0       44 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/httpresponse/__init__.py
--rw-r--r--   0        0        0     1291 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/httpresponse/__init__.pyi
--rw-r--r--   0        0        0       40 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/httpserver/__init__.py
--rw-r--r--   0        0        0     7655 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/httpserver/__init__.pyi
--rw-r--r--   0        0        0      833 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/types.py
--rw-r--r--   0        0        0       36 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/wsclient/__init__.py
--rw-r--r--   0        0        0     4258 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/network/wsclient/__init__.pyi
--rw-r--r--   0        0        0       75 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/objective/__init__.py
--rw-r--r--   0        0        0     3364 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/objective/__init__.pyi
--rw-r--r--   0        0        0      211 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/objective/types.py
--rw-r--r--   0        0        0      108 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/packet/__init__.py
--rw-r--r--   0        0        0     5149 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/packet/__init__.pyi
--rw-r--r--   0        0        0       46 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/color/__init__.py
--rw-r--r--   0        0        0     1724 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/color/__init__.pyi
--rw-r--r--   0        0        0       38 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/direction/__init__.py
--rw-r--r--   0        0        0      703 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/direction/__init__.pyi
--rw-r--r--   0        0        0       50 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/spawner/__init__.py
--rw-r--r--   0        0        0     5726 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/spawner/__init__.pyi
--rw-r--r--   0        0        0     1745 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/particle/types.py
--rw-r--r--   0        0        0       40 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/permission/__init__.py
--rw-r--r--   0        0        0     4827 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/permission/__init__.pyi
--rw-r--r--   0        0        0       28 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/permission/role/__init__.py
--rw-r--r--   0        0        0     5082 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/permission/role/__init__.pyi
--rw-r--r--   0        0        0      253 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/permission/types.py
--rw-r--r--   0        0        0       63 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/player/__init__.py
--rw-r--r--   0        0        0    45602 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/player/__init__.pyi
--rw-r--r--   0        0        0       63 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/player/device/__init__.py
--rw-r--r--   0        0        0     2342 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/player/device/__init__.pyi
--rw-r--r--   0        0        0     2684 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/player/types.py
--rw-r--r--   0        0        0       32 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/system/__init__.py
--rw-r--r--   0        0        0     2434 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/system/__init__.pyi
--rw-r--r--   0        0        0      380 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/classes/system/types.py
--rw-r--r--   0        0        0      260 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/functions/__init__.py
--rw-r--r--   0        0        0     2742 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/functions/__init__.pyi
--rw-r--r--   0        0        0      304 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/functions/types.py
--rw-r--r--   0        0        0    15844 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/llpy/types.py
--rw-r--r--   0        0        0     1101 2023-04-04 15:13:40.670202 llpy-helper-lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 llpy-helper-lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1047 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/README.md
+-rw-r--r--   0        0        0     4863 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/directionangle/__init__.py
+-rw-r--r--   0        0        0      813 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/directionangle/__init__.pyi
+-rw-r--r--   0        0        0      338 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/enumdefine/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/format/__init__.py
+-rw-r--r--   0        0        0     1758 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/format/__init__.pyi
+-rw-r--r--   0        0        0       68 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/pos/__init__.py
+-rw-r--r--   0        0        0     1230 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/pos/__init__.pyi
+-rw-r--r--   0        0        0      444 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/base/types.py
+-rw-r--r--   0        0        0       59 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/__init__.py
+-rw-r--r--   0        0        0     4230 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/__init__.pyi
+-rw-r--r--   0        0        0       83 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/entity/__init__.py
+-rw-r--r--   0        0        0     1039 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/block/entity/__init__.pyi
+-rw-r--r--   0        0        0       67 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/__init__.py
+-rw-r--r--   0        0        0     7199 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/__init__.pyi
+-rw-r--r--   0        0        0      156 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/enums/__init__.py
+-rw-r--r--   0        0        0     4983 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/enums/__init__.pyi
+-rw-r--r--   0        0        0       91 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/origin/__init__.py
+-rw-r--r--   0        0        0      873 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/origin/__init__.pyi
+-rw-r--r--   0        0        0       91 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/output/__init__.py
+-rw-r--r--   0        0        0     1754 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/output/__init__.pyi
+-rw-r--r--   0        0        0     3381 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/command/types.py
+-rw-r--r--   0        0        0       46 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/ini/__init__.py
+-rw-r--r--   0        0        0     5673 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/ini/__init__.pyi
+-rw-r--r--   0        0        0       48 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/json/__init__.py
+-rw-r--r--   0        0        0     3738 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/json/__init__.pyi
+-rw-r--r--   0        0        0      221 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/config/types.py
+-rw-r--r--   0        0        0       75 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/container/__init__.py
+-rw-r--r--   0        0        0     3611 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/container/__init__.pyi
+-rw-r--r--   0        0        0       28 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/data/__init__.py
+-rw-r--r--   0        0        0     4357 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/data/__init__.pyi
+-rw-r--r--   0        0        0      330 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/data/types.py
+-rw-r--r--   0        0        0       38 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbsession/__init__.py
+-rw-r--r--   0        0        0     2243 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbsession/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbstmt/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/dbstmt/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/kvdb/__init__.py
+-rw-r--r--   0        0        0     1657 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/kvdb/__init__.pyi
+-rw-r--r--   0        0        0      570 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/db/types.py
+-rw-r--r--   0        0        0       63 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/__init__.py
+-rw-r--r--   0        0        0    15776 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/__init__.pyi
+-rw-r--r--   0        0        0       93 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/damagecause/__init__.py
+-rw-r--r--   0        0        0     3678 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/damagecause/__init__.pyi
+-rw-r--r--   0        0        0     1962 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/entity/types.py
+-rw-r--r--   0        0        0       28 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/file/__init__.py
+-rw-r--r--   0        0        0    12487 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/file/__init__.pyi
+-rw-r--r--   0        0        0      208 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/file/types.py
+-rw-r--r--   0        0        0       79 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/custom/__init__.py
+-rw-r--r--   0        0        0     3106 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/custom/__init__.pyi
+-rw-r--r--   0        0        0       79 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/simple/__init__.py
+-rw-r--r--   0        0        0     1263 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/form/simple/__init__.pyi
+-rw-r--r--   0        0        0       28 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/i18n/__init__.py
+-rw-r--r--   0        0        0     3434 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/i18n/__init__.pyi
+-rw-r--r--   0        0        0       43 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/i18n/types.py
+-rw-r--r--   0        0        0       55 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/item/__init__.py
+-rw-r--r--   0        0        0     5079 2023-04-22 10:17:11.743157 llpy-helper-lib-0.2.1/llpy/classes/item/__init__.pyi
+-rw-r--r--   0        0        0       24 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/__init__.py
+-rw-r--r--   0        0        0     7505 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/__init__.pyi
+-rw-r--r--   0        0        0      612 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/types.py
+-rw-r--r--   0        0        0       34 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/version/__init__.py
+-rw-r--r--   0        0        0      471 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/ll/version/__init__.pyi
+-rw-r--r--   0        0        0       32 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/logger/__init__.py
+-rw-r--r--   0        0        0     3440 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/logger/__init__.pyi
+-rw-r--r--   0        0        0      431 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/logger/types.py
+-rw-r--r--   0        0        0       24 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/mc/__init__.py
+-rw-r--r--   0        0        0    82826 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/mc/__init__.pyi
+-rw-r--r--   0        0        0     1930 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/mc/types.py
+-rw-r--r--   0        0        0       30 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/money/__init__.py
+-rw-r--r--   0        0        0     2537 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/money/__init__.pyi
+-rw-r--r--   0        0        0      468 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/money/types.py
+-rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/enum/__init__.py
+-rw-r--r--   0        0        0     1047 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/enum/__init__.pyi
+-rw-r--r--   0        0        0       48 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/function/__init__.py
+-rw-r--r--   0        0        0     2598 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/function/__init__.pyi
+-rw-r--r--   0        0        0       46 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/globalpointer/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/globalpointer/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/hook/__init__.py
+-rw-r--r--   0        0        0      700 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/hook/__init__.pyi
+-rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/patch/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/patch/__init__.pyi
+-rw-r--r--   0        0        0       46 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/pointer/__init__.py
+-rw-r--r--   0        0        0     4298 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/pointer/__init__.pyi
+-rw-r--r--   0        0        0       50 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/stdstring/__init__.py
+-rw-r--r--   0        0        0     1693 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/stdstring/__init__.pyi
+-rw-r--r--   0        0        0      953 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/native/types.py
+-rw-r--r--   0        0        0      324 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/base/__init__.py
+-rw-r--r--   0        0        0     2021 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/base/__init__.pyi
+-rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/compound/__init__.py
+-rw-r--r--   0        0        0     7453 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/compound/__init__.pyi
+-rw-r--r--   0        0        0       34 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/list/__init__.py
+-rw-r--r--   0        0        0     6992 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/list/__init__.pyi
+-rw-r--r--   0        0        0       26 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/static/__init__.py
+-rw-r--r--   0        0        0     2382 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/static/__init__.pyi
+-rw-r--r--   0        0        0     1181 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/nbt/types.py
+-rw-r--r--   0        0        0       34 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/__init__.py
+-rw-r--r--   0        0        0     3497 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/__init__.pyi
+-rw-r--r--   0        0        0       42 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httprequest/__init__.py
+-rw-r--r--   0        0        0     1289 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httprequest/__init__.pyi
+-rw-r--r--   0        0        0       44 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpresponse/__init__.py
+-rw-r--r--   0        0        0     1291 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpresponse/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpserver/__init__.py
+-rw-r--r--   0        0        0     7655 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/httpserver/__init__.pyi
+-rw-r--r--   0        0        0      833 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/types.py
+-rw-r--r--   0        0        0       36 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/wsclient/__init__.py
+-rw-r--r--   0        0        0     4258 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/network/wsclient/__init__.pyi
+-rw-r--r--   0        0        0       75 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/objective/__init__.py
+-rw-r--r--   0        0        0     3364 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/objective/__init__.pyi
+-rw-r--r--   0        0        0      211 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/objective/types.py
+-rw-r--r--   0        0        0      108 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/packet/__init__.py
+-rw-r--r--   0        0        0     5149 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/packet/__init__.pyi
+-rw-r--r--   0        0        0       46 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/color/__init__.py
+-rw-r--r--   0        0        0     1724 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/color/__init__.pyi
+-rw-r--r--   0        0        0       38 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/direction/__init__.py
+-rw-r--r--   0        0        0      703 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/direction/__init__.pyi
+-rw-r--r--   0        0        0       50 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/spawner/__init__.py
+-rw-r--r--   0        0        0     5726 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/spawner/__init__.pyi
+-rw-r--r--   0        0        0     1745 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/particle/types.py
+-rw-r--r--   0        0        0       40 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/__init__.py
+-rw-r--r--   0        0        0     4827 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/__init__.pyi
+-rw-r--r--   0        0        0       28 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/role/__init__.py
+-rw-r--r--   0        0        0     5082 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/role/__init__.pyi
+-rw-r--r--   0        0        0      253 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/permission/types.py
+-rw-r--r--   0        0        0       63 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/__init__.py
+-rw-r--r--   0        0        0    45602 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/__init__.pyi
+-rw-r--r--   0        0        0       63 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/device/__init__.py
+-rw-r--r--   0        0        0     2342 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/device/__init__.pyi
+-rw-r--r--   0        0        0     2684 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/player/types.py
+-rw-r--r--   0        0        0       32 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/system/__init__.py
+-rw-r--r--   0        0        0     2434 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/system/__init__.pyi
+-rw-r--r--   0        0        0      380 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/classes/system/types.py
+-rw-r--r--   0        0        0      256 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/functions/__init__.py
+-rw-r--r--   0        0        0     2738 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/functions/__init__.pyi
+-rw-r--r--   0        0        0      304 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/functions/types.py
+-rw-r--r--   0        0        0    15844 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/llpy/types.py
+-rw-r--r--   0        0        0     1101 2023-04-22 10:17:11.747157 llpy-helper-lib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 llpy-helper-lib-0.2.1/PKG-INFO
```

### Comparing `llpy-helper-lib-0.2.0/LICENSE` & `llpy-helper-lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/README.md` & `llpy-helper-lib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/__init__.py` & `llpy-helper-lib-0.2.1/llpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,11 +78,11 @@
 from .classes.player import Player as Player
 from .classes.player.device import Device as Device
 from .classes.player.device import LLSE_Device as LLSE_Device
 from .classes.system import system as system
 from .functions import clearInterval as clearInterval
 from .functions import colorLog as colorLog
 from .functions import fastLog as fastLog
-from .functions import listener as listener
+from .functions import handle as handle
 from .functions import log as log
 from .functions import setInterval as setInterval
 from .functions import setTimeout as setTimeout
```

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/base/directionangle/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/base/directionangle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/base/format/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/base/format/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/base/pos/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/base/pos/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/block/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/block/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/block/entity/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/block/entity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/command/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/command/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typing
-from typing import NoReturn, TypeVar
+from typing import Callable, NoReturn, TypeVar
 
 from .types import T_CommandCallback, T_ParamOption, T_ParamType
 
 _T_ArgCallback = TypeVar("_T_ArgCallback", bound=T_CommandCallback)
 
 class LLSE_Command:
     """指令对象"""
@@ -228,23 +228,29 @@
     def setSoftEnum(self, name: str, enums: str) -> str: ...
     def addSoftEnumValues(self, name: str, enums: str) -> bool: ...
     def removeSoftEnumValues(self, name: str, enums: str) -> bool: ...
     def getSoftEnumValues(self, name: str) -> list[str]: ...
     def getSoftEnumNames(self) -> list[str]: ...
 
     # BaseLib.py
-    def callback(self, func: _T_ArgCallback) -> _T_ArgCallback:
+    @typing.overload
+    def handle(
+        self,
+        func: None = None,
+    ) -> Callable[[_T_ArgCallback], _T_ArgCallback]: ...
+    @typing.overload
+    def handle(self, func: _T_ArgCallback) -> _T_ArgCallback:
         """
         指令回调装饰器
 
         来源：`BaseLib.py`
 
         用法：
 
         ```py
-        @cmd.callback
+        @cmd.handle
         def _(_, ori: LLSE_CommandOrigin, out: LLSE_CommandOutput, result: dict[str, Any]):
             ...
         ```
         """
 
 Command = LLSE_Command
```

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/command/enums/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/command/enums/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/command/origin/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/command/origin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/command/output/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/command/output/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/command/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/command/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/config/ini/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/config/ini/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/config/json/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/config/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/container/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/container/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/data/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/db/dbsession/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/db/dbsession/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/db/dbstmt/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/db/dbstmt/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/db/kvdb/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/db/kvdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/db/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/db/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/entity/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/entity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/entity/damagecause/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/entity/damagecause/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/entity/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/entity/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/file/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/file/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/form/custom/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/form/custom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/form/simple/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/form/simple/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/i18n/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/i18n/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/item/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/item/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     @property
     def attackDamage(self) -> int:
         """物品攻击伤害"""
     @property
     def maxDamage(self) -> int:
         """物品最大耐久"""
     @property
+    def maxStackSize(self) -> int:
+        """物品最大堆叠数量"""
+    @property
     def isArmorItem(self) -> bool:
         """物品是否为盔甲"""
     @property
     def isBlock(self) -> bool:
         """物品是否为方块"""
     @property
     def isDamageableItem(self) -> bool:
```

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/ll/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/ll/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/ll/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/ll/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/logger/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/logger/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/mc/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/mc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/mc/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/mc/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/money/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/money/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/enum/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/enum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/function/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/function/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/globalpointer/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/globalpointer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/hook/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/hook/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/patch/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/patch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/pointer/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/pointer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/stdstring/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/native/stdstring/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/native/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/native/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/nbt/base/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/nbt/base/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/nbt/compound/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/nbt/compound/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/nbt/list/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/nbt/list/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/nbt/static/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/nbt/static/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/nbt/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/nbt/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/network/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/network/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/network/httprequest/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/network/httprequest/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/network/httpresponse/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/network/httpresponse/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/network/httpserver/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/network/httpserver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/network/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/network/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/network/wsclient/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/network/wsclient/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/objective/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/objective/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/packet/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/packet/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/particle/color/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/particle/color/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/particle/direction/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/particle/direction/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/particle/spawner/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/particle/spawner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/particle/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/particle/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/permission/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/permission/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/permission/role/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/permission/role/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/player/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/player/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/player/device/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/player/device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/player/types.py` & `llpy-helper-lib-0.2.1/llpy/classes/player/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/classes/system/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/classes/system/__init__.pyi`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/llpy/functions/__init__.pyi` & `llpy-helper-lib-0.2.1/llpy/functions/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,24 +91,24 @@
     Returns:
         是否取消成功。如果返回Null，则代表取消任务失败
     """
 
 _T_Listener = TypeVar("_T_Listener", bound=Callable[..., Literal[False] | Any])
 
 # BaseLib.py
-def listener(event: str) -> Callable[[_T_Listener], _T_Listener]:
+def handle(event: str) -> Callable[[_T_Listener], _T_Listener]:
     """
     监听事件函数装饰器
 
     来源：`BaseLib.py`
 
     用法：
 
     ```py
-    @listener("onJoin")
+    @handle("onJoin")
     def _(player: LLSE_Player):
         log(f"{player.realName} joined the game!")
     ```
 
     Args:
         event: 要监听的事件名称
     """
```

### Comparing `llpy-helper-lib-0.2.0/llpy/types.py` & `llpy-helper-lib-0.2.1/llpy/types.py`

 * *Files identical despite different names*

### Comparing `llpy-helper-lib-0.2.0/pyproject.toml` & `llpy-helper-lib-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 "example.py" = [
     "F403",
     "F405",
 ]
 
 [project]
 name = "llpy-helper-lib"
-version = "0.2.0"
+version = "0.2.1"
 description = "A typing & util lib for LLSE Python runtime"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
 ]
```

### Comparing `llpy-helper-lib-0.2.0/PKG-INFO` & `llpy-helper-lib-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llpy-helper-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: A typing & util lib for LLSE Python runtime
 License: MIT
 Author-email: student_2333 <lgc2333@126.com>
 Requires-Python: >=3.10
 Provides-Extra: dev
 Description-Content-Type: text/markdown
```

