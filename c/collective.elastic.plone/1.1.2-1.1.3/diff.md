# Comparing `tmp/collective.elastic.plone-1.1.2.tar.gz` & `tmp/collective.elastic.plone-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.elastic.plone-1.1.2.tar", last modified: Sat Mar  4 13:32:02 2023, max compression
+gzip compressed data, was "collective.elastic.plone-1.1.3.tar", last modified: Sat Apr 22 13:08:13 2023, max compression
```

## Comparing `collective.elastic.plone-1.1.2.tar` & `collective.elastic.plone-1.1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.501472 collective.elastic.plone-1.1.2/
--rw-r--r--   0 katjasuss   (501) staff       (20)      421 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/CHANGES.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      586 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/DEVELOP.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)    18092 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/LICENSE.GPL
--rw-r--r--   0 katjasuss   (501) staff       (20)      668 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/LICENSE.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      108 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/MANIFEST.in
--rw-r--r--   0 katjasuss   (501) staff       (20)     4223 2023-03-04 13:32:02.501601 collective.elastic.plone-1.1.2/PKG-INFO
--rw-r--r--   0 katjasuss   (501) staff       (20)     2567 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/README.rst
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.489264 collective.elastic.plone-1.1.2/docs/
--rw-r--r--   0 katjasuss   (501) staff       (20)     7931 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/docs/conf.py
--rw-r--r--   0 katjasuss   (501) staff       (20)       85 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/docs/index.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      471 2023-03-04 13:32:02.502349 collective.elastic.plone-1.1.2/setup.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)     2174 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/setup.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.484693 collective.elastic.plone-1.1.2/src/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.489493 collective.elastic.plone-1.1.2/src/collective/
--rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.491580 collective.elastic.plone-1.1.2/src/collective/elastic/
--rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.494081 collective.elastic.plone-1.1.2/src/collective/elastic/plone/
--rw-r--r--   0 katjasuss   (501) staff       (20)      484 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.494731 collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      521 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.494950 collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/static/
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/static/.gitkeep
--rw-r--r--   0 katjasuss   (501) staff       (20)      613 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/update.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1630 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)      936 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/eslib.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      447 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/interfaces.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.495989 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/
--rw-r--r--   0 katjasuss   (501) staff       (20)      611 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/README.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/collective.es.plone.pot
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.485666 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/en/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.496222 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/en/LC_MESSAGES/
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/en/LC_MESSAGES/collective.es.plone.po
--rw-r--r--   0 katjasuss   (501) staff       (20)     1581 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/update.py
--rwxr-xr-x   0 katjasuss   (501) staff       (20)      494 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/update.sh
--rw-r--r--   0 katjasuss   (501) staff       (20)      260 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/permissions.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.486066 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.496856 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/default/
--rw-r--r--   0 katjasuss   (501) staff       (20)      187 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/default/browserlayer.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)     2168 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/default/catalog.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      229 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/default/metadata.xml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.497303 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/uninstall/
--rw-r--r--   0 katjasuss   (501) staff       (20)      129 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      404 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/uninstall/catalog.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)    10231 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/proxyindex.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1587 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/queueprocessor.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.498412 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      965 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)     1676 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/expansions.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.499486 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      289 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)     5725 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/post.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     8685 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/request_example.json
--rw-r--r--   0 katjasuss   (501) staff       (20)    27847 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/response_example.json
--rw-r--r--   0 katjasuss   (501) staff       (20)     1693 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/schema.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      948 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/service.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      601 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/setuphandlers.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1345 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/testing.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.500402 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/
--rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.500625 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/robot/
--rw-r--r--   0 katjasuss   (501) staff       (20)     2007 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/robot/test_example.robot
--rw-r--r--   0 katjasuss   (501) staff       (20)     3408 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/test_proxyindex.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     9270 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/test_restapi.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     2134 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/test_setup.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      193 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/upgrades.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      393 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/upgrades.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.501292 collective.elastic.plone-1.1.2/src/collective/elastic/plone/www/
--rw-r--r--   0 katjasuss   (501) staff       (20)     2351 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/www/addIndex.zpt
--rw-r--r--   0 katjasuss   (501) staff       (20)      199 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/www/index.gif
--rw-r--r--   0 katjasuss   (501) staff       (20)     2172 2023-03-04 13:32:01.000000 collective.elastic.plone-1.1.2/src/collective/elastic/plone/www/manageIndex.zpt
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-04 13:32:02.491359 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/
--rw-r--r--   0 katjasuss   (501) staff       (20)     4223 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/PKG-INFO
--rw-r--r--   0 katjasuss   (501) staff       (20)     2869 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/SOURCES.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/dependency_links.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       40 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/entry_points.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       30 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/namespace_packages.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/not-zip-safe
--rw-r--r--   0 katjasuss   (501) staff       (20)       95 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/requires.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       11 2023-03-04 13:32:02.000000 collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/top_level.txt
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.027447 collective.elastic.plone-1.1.3/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      525 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/CHANGES.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      586 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/DEVELOP.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)    18092 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/LICENSE.GPL
+-rw-r--r--   0 katjasuss   (501) staff       (20)      668 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/LICENSE.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      108 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/MANIFEST.in
+-rw-r--r--   0 katjasuss   (501) staff       (20)     4327 2023-04-22 13:08:13.027593 collective.elastic.plone-1.1.3/PKG-INFO
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2567 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/README.rst
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.009856 collective.elastic.plone-1.1.3/docs/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     7931 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/docs/conf.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)       85 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/docs/index.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      471 2023-04-22 13:08:13.028451 collective.elastic.plone-1.1.3/setup.cfg
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2174 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/setup.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.004896 collective.elastic.plone-1.1.3/src/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.010108 collective.elastic.plone-1.1.3/src/collective/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.012302 collective.elastic.plone-1.1.3/src/collective/elastic/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.018042 collective.elastic.plone-1.1.3/src/collective/elastic/plone/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      484 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.019211 collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      521 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/configure.zcml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.019948 collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/static/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/static/.gitkeep
+-rw-r--r--   0 katjasuss   (501) staff       (20)      613 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/update.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1630 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/configure.zcml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      936 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/eslib.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      447 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/interfaces.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.021500 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      611 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/README.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/collective.es.plone.pot
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.005911 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/en/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.021743 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/en/LC_MESSAGES/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/en/LC_MESSAGES/collective.es.plone.po
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1581 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/update.py
+-rwxr-xr-x   0 katjasuss   (501) staff       (20)      494 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/update.sh
+-rw-r--r--   0 katjasuss   (501) staff       (20)      260 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/permissions.zcml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.006322 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.022436 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/default/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      187 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/default/browserlayer.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2168 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/default/catalog.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      229 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/default/metadata.xml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.022925 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/uninstall/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      129 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)      404 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/uninstall/catalog.xml
+-rw-r--r--   0 katjasuss   (501) staff       (20)    10231 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/proxyindex.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1587 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/queueprocessor.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.024106 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       24 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      965 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/configure.zcml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1676 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/expansions.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.025332 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      289 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/configure.zcml
+-rw-r--r--   0 katjasuss   (501) staff       (20)     5695 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/post.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     8685 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/request_example.json
+-rw-r--r--   0 katjasuss   (501) staff       (20)    27847 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/response_example.json
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1693 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/schema.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      948 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/service.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      601 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/setuphandlers.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1345 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/testing.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.026296 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/
+-rw-r--r--   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.026534 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/robot/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2007 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/robot/test_example.robot
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3408 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/test_proxyindex.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     9270 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/test_restapi.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2134 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/test_setup.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      193 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/upgrades.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      393 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/upgrades.zcml
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.027252 collective.elastic.plone-1.1.3/src/collective/elastic/plone/www/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2351 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/www/addIndex.zpt
+-rw-r--r--   0 katjasuss   (501) staff       (20)      199 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/www/index.gif
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2172 2023-04-22 13:08:11.000000 collective.elastic.plone-1.1.3/src/collective/elastic/plone/www/manageIndex.zpt
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-04-22 13:08:13.012060 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     4327 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/PKG-INFO
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2869 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/SOURCES.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/dependency_links.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       40 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/entry_points.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       30 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/namespace_packages.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/not-zip-safe
+-rw-r--r--   0 katjasuss   (501) staff       (20)       95 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/requires.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       11 2023-04-22 13:08:12.000000 collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/top_level.txt
```

### Comparing `collective.elastic.plone-1.1.2/DEVELOP.rst` & `collective.elastic.plone-1.1.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/LICENSE.GPL` & `collective.elastic.plone-1.1.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/LICENSE.rst` & `collective.elastic.plone-1.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/PKG-INFO` & `collective.elastic.plone-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.elastic.plone
-Version: 1.1.2
+Version: 1.1.3
 Summary: Addon for ElasticSearch integration with Plone
 Home-page: https://github.com/collective/collective.elastic.plone
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.plone
 Project-URL: Source, https://github.com/collective/collective.elastic.plone
@@ -113,14 +113,20 @@
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
 
+1.1.3 (2023-04-22)
+------------------
+
+- Step back from ElasticSearch scroll API for deep pagination.
+
+
 1.1.2 (2023-03-04)
 ------------------
 
 -  Enhance response of @kitsearch on unavailable ElasticSearch or not found index [ksuess]
 
 
 1.1.1 (2023-03-03)
```

### Comparing `collective.elastic.plone-1.1.2/README.rst` & `collective.elastic.plone-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/docs/conf.py` & `collective.elastic.plone-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/setup.py` & `collective.elastic.plone-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     open('README.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='collective.elastic.plone',
-    version='1.1.2',
+    version='1.1.3',
     description="Addon for ElasticSearch integration with Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/configure.zcml` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/browser/update.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/browser/update.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/configure.zcml` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/eslib.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/eslib.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/README.rst` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/locales/update.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/profiles/default/catalog.xml` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/proxyindex.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/proxyindex.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/queueprocessor.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/queueprocessor.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/configure.zcml` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/expansions.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/expansions.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/post.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         elasticsearch_url = data.get("elasticsearch_url", "http://localhost:9200")
         elasticsearch_index = data.get("elasticsearch_index", "plone")
         query_body = data.get("elasticsearch_payload", {})
 
         es_kwargs = dict(
             index=elasticsearch_index,
             body=query_body,
-            scroll="1m",
             # _source_includes=["rid"],
         )
         if not query_body.get("size", None):
             es_kwargs["size"] = 10
         es = get_query_client(elasticsearch_url)
         try:
             result = es.search(**es_kwargs)
@@ -61,21 +60,20 @@
             self.request.response.setStatus(500)
             return dict(error=dict(message=e.message))
         except TransportError as e:
             self.request.response.setStatus(503)
             return dict(error=dict(message=e.message))
         except NotFoundError as e:
             self.request.response.setStatus(404)
-            return dict(error=dict(message=e.body['error']['reason']))
+            return dict(error=dict(message=e.body["error"]["reason"]))
         except Exception as e:
             self.request.response.setStatus(500)
             return dict(error=dict(message=e.message))
         # result is of type ObjectApiResponse
         return dict(result)
-    
 
     def has_permission_to_query_all(self):
         sm = getSecurityManager()
         return sm.checkPermission("Manage portal", self.context)
 
     def esQuery(self, data):
         """Extend query with roles, user and groups."""
```

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/request_example.json` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/request_example.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/kitsearch/response_example.json` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/kitsearch/response_example.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/schema.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/schema.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/restapi/service.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/restapi/service.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/setuphandlers.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/testing.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/testing.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/robot/test_example.robot` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/test_proxyindex.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/test_proxyindex.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/test_restapi.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/test_restapi.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/tests/test_setup.py` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/www/addIndex.zpt` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/www/addIndex.zpt`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective/elastic/plone/www/manageIndex.zpt` & `collective.elastic.plone-1.1.3/src/collective/elastic/plone/www/manageIndex.zpt`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/PKG-INFO` & `collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.elastic.plone
-Version: 1.1.2
+Version: 1.1.3
 Summary: Addon for ElasticSearch integration with Plone
 Home-page: https://github.com/collective/collective.elastic.plone
 Author: Jens W. Klein
 Author-email: jk@kleinundpartner.at
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.plone
 Project-URL: Source, https://github.com/collective/collective.elastic.plone
@@ -113,14 +113,20 @@
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
 
+1.1.3 (2023-04-22)
+------------------
+
+- Step back from ElasticSearch scroll API for deep pagination.
+
+
 1.1.2 (2023-03-04)
 ------------------
 
 -  Enhance response of @kitsearch on unavailable ElasticSearch or not found index [ksuess]
 
 
 1.1.1 (2023-03-03)
```

### Comparing `collective.elastic.plone-1.1.2/src/collective.elastic.plone.egg-info/SOURCES.txt` & `collective.elastic.plone-1.1.3/src/collective.elastic.plone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

