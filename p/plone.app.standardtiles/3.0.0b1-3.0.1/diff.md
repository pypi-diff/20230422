# Comparing `tmp/plone.app.standardtiles-3.0.0b1.tar.gz` & `tmp/plone.app.standardtiles-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.standardtiles-3.0.0b1.tar", last modified: Fri Jun 24 17:04:42 2022, max compression
+gzip compressed data, was "plone.app.standardtiles-3.0.1.tar", last modified: Sat Apr 22 13:58:37 2023, max compression
```

## Comparing `plone.app.standardtiles-3.0.0b1.tar` & `plone.app.standardtiles-3.0.1.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.576449 plone.app.standardtiles-3.0.0b1/
--rw-r--r--   0 maurits    (501) staff       (20)    10379 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      750 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      178 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    12493 2022-06-24 17:04:42.576566 plone.app.standardtiles-3.0.0b1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1061 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      289 2022-06-24 17:04:42.577142 plone.app.standardtiles-3.0.0b1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1921 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.547436 plone.app.standardtiles-3.0.0b1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.550419 plone.app.standardtiles-3.0.0b1/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.552636 plone.app.standardtiles-3.0.0b1/src/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.561164 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/
--rw-r--r--   0 maurits    (501) staff       (20)      122 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3764 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/attachment.py
--rw-r--r--   0 maurits    (501) staff       (20)    11201 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/common.py
--rw-r--r--   0 maurits    (501) staff       (20)     3914 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5249 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/content.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9084 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/contentlisting.py
--rw-r--r--   0 maurits    (501) staff       (20)     2330 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/discussion.py
--rw-r--r--   0 maurits    (501) staff       (20)      739 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/embed.py
--rw-r--r--   0 maurits    (501) staff       (20)     8463 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/existingcontent.py
--rw-r--r--   0 maurits    (501) staff       (20)     5775 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/field.py
--rw-r--r--   0 maurits    (501) staff       (20)     2182 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/head.py
--rw-r--r--   0 maurits    (501) staff       (20)     1909 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/head.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1426 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/html.py
--rw-r--r--   0 maurits    (501) staff       (20)      587 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     4359 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/layout.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1688 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/media.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1361 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)    11826 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/navigation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.565593 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3940 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/add.py
--rw-r--r--   0 maurits    (501) staff       (20)     1968 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/assignment.py
--rw-r--r--   0 maurits    (501) staff       (20)     2563 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      317 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     2282 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1799 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/portletmanager.py
--rw-r--r--   0 maurits    (501) staff       (20)     1970 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1720 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.548176 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.567211 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)     4540 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.568150 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      222 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
--rw-r--r--   0 maurits    (501) staff       (20)      129 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/uninstall/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1382 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/rawembed.py
--rw-r--r--   0 maurits    (501) staff       (20)     8427 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/rss.py
--rw-r--r--   0 maurits    (501) staff       (20)      780 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/sitemap.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.572996 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1761 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/attachment_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2251 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/configlets.pt
--rw-r--r--   0 maurits    (501) staff       (20)      728 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/contentlisting_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      457 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/description.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3905 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/existingcontent_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      762 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/image.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3433 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/listing_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5767 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/login.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1477 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/namedimage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1501 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/navigation.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2143 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/navigation_recurse.pt
--rw-r--r--   0 maurits    (501) staff       (20)      681 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/navigationlink.pt
--rw-r--r--   0 maurits    (501) staff       (20)      767 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/rawembed.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1689 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/rss.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5336 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/summary_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4803 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/tabular_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      368 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9747 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      698 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.576084 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     2938 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/RSS.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      746 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      969 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/funky_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7293 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)    14645 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_existing_content.py
--rw-r--r--   0 maurits    (501) staff       (20)    10897 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_field.py
--rw-r--r--   0 maurits    (501) staff       (20)     6241 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_head.py
--rw-r--r--   0 maurits    (501) staff       (20)    15107 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     7409 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_media.py
--rw-r--r--   0 maurits    (501) staff       (20)     1650 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      272 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      746 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1854 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2489 2022-06-24 17:04:40.000000 plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/viewletmanager.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-06-24 17:04:42.552392 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    12493 2022-06-24 17:04:41.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3919 2022-06-24 17:04:42.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-06-24 17:04:42.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2022-06-24 17:04:42.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-06-24 17:04:42.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-06-24 17:04:41.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      264 2022-06-24 17:04:42.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-06-24 17:04:42.000000 plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.537007 plone.app.standardtiles-3.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    10731 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      750 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      178 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    12898 2023-04-22 13:58:37.537156 plone.app.standardtiles-3.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1061 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      289 2023-04-22 13:58:37.537680 plone.app.standardtiles-3.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1994 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.508303 plone.app.standardtiles-3.0.1/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.512329 plone.app.standardtiles-3.0.1/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.514949 plone.app.standardtiles-3.0.1/src/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.523966 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3764 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/attachment.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11183 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4184 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5249 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/content.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9084 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/contentlisting.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2330 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/discussion.py
+-rw-r--r--   0 maurits    (501) staff       (20)      739 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/embed.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8463 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/existingcontent.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5775 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/field.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2182 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1909 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1426 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/html.py
+-rw-r--r--   0 maurits    (501) staff       (20)      587 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4359 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/layout.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/linkintegrity.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1688 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/media.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1361 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11827 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/navigation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.526970 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3940 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/add.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1968 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/assignment.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2563 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      317 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/delete.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2282 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1799 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portletmanager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1970 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1720 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.509155 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.527799 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      207 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     4557 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.528537 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      239 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/uninstall/portlets..xml
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1382 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rawembed.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8427 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rss.py
+-rw-r--r--   0 maurits    (501) staff       (20)      780 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/sitemap.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.533534 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1761 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/attachment_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2251 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/configlets.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/contentlisting_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      457 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/description.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3905 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/existingcontent_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      762 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3433 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/listing_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5767 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/login.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1477 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/namedimage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2143 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation_recurse.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      681 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigationlink.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rawembed.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1689 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rss.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5336 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/summary_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4803 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/tabular_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      368 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/title.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9747 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      698 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.536771 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     2921 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/RSS.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      746 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      969 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/funky_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7293 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14645 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_existing_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10897 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_field.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6241 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_head.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15107 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7409 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_media.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1650 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      746 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1854 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2489 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/viewletmanager.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-22 13:58:37.514706 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    12898 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3964 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      259 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-22 13:58:37.000000 plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/top_level.txt
```

### Comparing `plone.app.standardtiles-3.0.0b1/CHANGES.rst` & `plone.app.standardtiles-3.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Changelog
 =========
 
+3.0.1 (2023-04-22)
+------------------
+
+- Fix broken CMFDynamicViewFTI import.
+  [thet]
+
+- Fix byline viewlet name
+  [frapell]
+
+
+3.0.0 (2022-12-05)
+------------------
+
+- Added linkintegrity for html and existingcontent tile.
+  Code is ported form version 2.5.0, and is only active when
+  plone.app.blocks version 6.0.2 or higher is used.
+  [petschki]
+
+
 3.0.0b1 (2022-06-24)
 --------------------
 
 - Fix ``isDefaultPage`` import which was moved to ``plone.base.defaultpage``
   [petschki]
 
 - Cleanup and fix ExistingContentTile in 5.2
```

#### html2text {}

```diff
@@ -1,12 +1,17 @@
-Changelog ========= 3.0.0b1 (2022-06-24) -------------------- - Fix
-``isDefaultPage`` import which was moved to ``plone.base.defaultpage``
-[petschki] - Cleanup and fix ExistingContentTile in 5.2 [gotcha, Mychae1]
-3.0.0a2 (2022-04-01) -------------------- - Fixed KeyError ``results`` in
-tabular view. Should have been ``batch``. Fixes `issue 122
+Changelog ========= 3.0.1 (2023-04-22) ------------------ - Fix broken
+CMFDynamicViewFTI import. [thet] - Fix byline viewlet name [frapell] 3.0.0
+(2022-12-05) ------------------ - Added linkintegrity for html and
+existingcontent tile. Code is ported form version 2.5.0, and is only active
+when plone.app.blocks version 6.0.2 or higher is used. [petschki] 3.0.0b1
+(2022-06-24) -------------------- - Fix ``isDefaultPage`` import which was
+moved to ``plone.base.defaultpage`` [petschki] - Cleanup and fix
+ExistingContentTile in 5.2 [gotcha, Mychae1] 3.0.0a2 (2022-04-01) -------------
+------- - Fixed KeyError ``results`` in tabular view. Should have been
+``batch``. Fixes `issue 122
 github.com/plone/plone.app.standardtiles/issues/122>`_. [maurits] 3.0.0a1
 (2022-03-23) -------------------- - Fix showing private content while editing a
 tile. Fixes `issue 100
 github.com/plone/plone.app.standardtiles/issues/100>`_. [maurits] - Fix tests
 to respect BS5 Markup of Plone 6. [jensens] - Fix membertools tile [agitator] -
 Breaking: Drop code marked as deprecated for 3.0. This includes
 ``plone.app.standardtiles.image``. If anyone for any reason has still these
```

### Comparing `plone.app.standardtiles-3.0.0b1/LICENSE.GPL` & `plone.app.standardtiles-3.0.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/LICENSE.txt` & `plone.app.standardtiles-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/PKG-INFO` & `plone.app.standardtiles-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.0.0b1
+Version: 3.0.1
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: attachment
 License-File: LICENSE.GPL
 License-File: LICENSE.txt
 
 Plone Standard Tiles
 ====================
@@ -57,14 +58,33 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.0.1 (2023-04-22)
+------------------
+
+- Fix broken CMFDynamicViewFTI import.
+  [thet]
+
+- Fix byline viewlet name
+  [frapell]
+
+
+3.0.0 (2022-12-05)
+------------------
+
+- Added linkintegrity for html and existingcontent tile.
+  Code is ported form version 2.5.0, and is only active when
+  plone.app.blocks version 6.0.2 or higher is used.
+  [petschki]
+
+
 3.0.0b1 (2022-06-24)
 --------------------
 
 - Fix ``isDefaultPage`` import which was moved to ``plone.base.defaultpage``
   [petschki]
 
 - Cleanup and fix ExistingContentTile in 5.2
@@ -493,9 +513,7 @@
   smaller than width columns
   [datakurre]
 
 1.0a1 (2015-05-25)
 ------------------
 
 - First alpha release.
-
-
```

### Comparing `plone.app.standardtiles-3.0.0b1/README.rst` & `plone.app.standardtiles-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/setup.py` & `plone.app.standardtiles-3.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.0b1"
+version = "3.0.1"
 
 
 setup(
     name="plone.app.standardtiles",
     version=version,
     description="Tiles for plone.app.blocks page composition",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
@@ -14,36 +14,38 @@
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 6.0",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="tiles content plone",
     author="Rob Gietema",
     author_email="rob@fourdigits.nl",
     url="https://github.com/plone/plone.app.standardtiles",
     license="GPL",
     packages=find_packages("src"),
     package_dir={"": "src"},
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
         "plone.app.blocks",
         "plone.app.tiles>=3.1.2",
         "plone.subrequest",
-        "plone.tiles>=1.8.0.dev0",
+        "plone.tiles>=1.8.0",
         "Products.CMFPlone>=6.0.0a3",
         "requests",
         "setuptools",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/attachment.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/attachment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/common.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     viewlet = "plone.globalstatusmessage"
 
 
 class DocumentBylineTile(ProxyViewletTile):
     """A document byline tile."""
 
     manager = "plone.belowcontenttitle"
-    viewlet = "plone.belowcontenttitle.documentbyline"
+    viewlet = "plone.documentbyline"
 
 
 class LockInfoTile(ProxyViewletTile):
     """A lockinfo tile."""
 
     manager = "plone.abovecontent"
     viewlet = "plone.lockinfo"
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/configure.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -122,10 +122,16 @@
       name="display"
       />
   <adapter
       factory=".field.namedImageDisplayTemplate"
       name="display"
       />
 
+  <!-- Linkintegrity in plone.app.blocks is available since 6.0.2. -->
+  <configure zcml:condition="installed plone.app.blocks.linkintegrity">
+    <adapter factory=".linkintegrity.HTMLTile" />
+    <adapter factory=".linkintegrity.ExistingContentTile" />
+  </configure>
+
   <include file="upgrades.zcml" />
 
 </configure>
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/content.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/content.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/contentlisting.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/contentlisting.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/discussion.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/embed.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/embed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/existingcontent.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/existingcontent.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/field.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/field.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/head.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/head.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/head.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/html.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/html.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/interfaces.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/layout.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/layout.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/media.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/media.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/metadata.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/navigation.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/navigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from plone.i18n.normalizer.interfaces import IIDNormalizer
 from plone.memoize.instance import memoize
 from plone.supermodel.model import Schema
 from plone.tiles import Tile
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.interfaces import IFolderish
 from Products.CMFCore.utils import getToolByName
-from Products.CMFDynamicViewFTI.interface import IBrowserDefault
+from Products.CMFDynamicViewFTI.interfaces import IBrowserDefault
 from Products.CMFPlone.browser.navtree import NavtreeQueryBuilder
 from Products.CMFPlone.browser.navtree import SitemapNavtreeStrategy
 from Products.CMFPlone.interfaces import INonStructuralFolder
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from z3c.form.interfaces import IValue
 from z3c.form.util import getSpecification
 from zope import schema
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/add.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/add.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/assignment.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/assignment.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/configure.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/edit.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/edit.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/portlet.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/portletmanager.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/portletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/utils.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/portlets/vocabularies.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/portlets/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/profiles/default/registry.xml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/profiles/default/registry.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 4% similar despite different names*

```diff
@@ -1,284 +1,285 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 223f 3e0a 3c72 6567 6973 7472 793e  .0"?>.<registry>
-00000020: 0a20 203c 7265 636f 7264 206e 616d 653d  .  <record name=
-00000030: 2270 6c6f 6e65 2e61 7070 2e74 696c 6573  "plone.app.tiles
-00000040: 223e 0a20 2020 203c 6669 656c 6420 7479  ">.    <field ty
-00000050: 7065 3d22 706c 6f6e 652e 7265 6769 7374  pe="plone.regist
-00000060: 7279 2e66 6965 6c64 2e4c 6973 7422 3e0a  ry.field.List">.
-00000070: 2020 2020 2020 3c74 6974 6c65 3e54 696c        <title>Til
-00000080: 6573 3c2f 7469 746c 653e 0a20 2020 2020  es</title>.     
-00000090: 203c 7661 6c75 655f 7479 7065 2074 7970   <value_type typ
-000000a0: 653d 2270 6c6f 6e65 2e72 6567 6973 7472  e="plone.registr
-000000b0: 792e 6669 656c 642e 5465 7874 4c69 6e65  y.field.TextLine
-000000c0: 2220 2f3e 0a20 2020 203c 2f66 6965 6c64  " />.    </field
-000000d0: 3e0a 2020 2020 3c76 616c 7565 2070 7572  >.    <value pur
-000000e0: 6765 3d22 6661 6c73 6522 3e0a 2020 2020  ge="false">.    
-000000f0: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
-00000100: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
-00000110: 6573 2e61 6e61 6c79 7469 6373 3c2f 656c  es.analytics</el
-00000120: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
-00000130: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-00000140: 7374 616e 6461 7264 7469 6c65 732e 616e  standardtiles.an
-00000150: 6f6e 746f 6f6c 733c 2f65 6c65 6d65 6e74  ontools</element
-00000160: 3e0a 2020 2020 2020 3c65 6c65 6d65 6e74  >.      <element
-00000170: 3e70 6c6f 6e65 2e61 7070 2e73 7461 6e64  >plone.app.stand
-00000180: 6172 6474 696c 6573 2e61 7574 686f 726c  ardtiles.authorl
-00000190: 696e 6b3c 2f65 6c65 6d65 6e74 3e0a 2020  ink</element>.  
-000001a0: 2020 2020 3c65 6c65 6d65 6e74 3e70 6c6f      <element>plo
-000001b0: 6e65 2e61 7070 2e73 7461 6e64 6172 6474  ne.app.standardt
-000001c0: 696c 6573 2e63 616e 6f6e 6963 616c 5f75  iles.canonical_u
-000001d0: 726c 3c2f 656c 656d 656e 743e 0a20 2020  rl</element>.   
-000001e0: 2020 203c 656c 656d 656e 743e 706c 6f6e     <element>plon
-000001f0: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
-00000200: 6c65 732e 636f 6c6f 7068 6f6e 3c2f 656c  les.colophon</el
-00000210: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
-00000220: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-00000230: 7374 616e 6461 7264 7469 6c65 732e 636f  standardtiles.co
-00000240: 6e74 656e 746c 6973 7469 6e67 3c2f 656c  ntentlisting</el
-00000250: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
-00000260: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-00000270: 7374 616e 6461 7264 7469 6c65 732e 6465  standardtiles.de
-00000280: 7363 7269 7074 696f 6e3c 2f65 6c65 6d65  scription</eleme
-00000290: 6e74 3e0a 2020 2020 2020 3c65 6c65 6d65  nt>.      <eleme
-000002a0: 6e74 3e70 6c6f 6e65 2e61 7070 2e73 7461  nt>plone.app.sta
-000002b0: 6e64 6172 6474 696c 6573 2e64 6973 6375  ndardtiles.discu
-000002c0: 7373 696f 6e3c 2f65 6c65 6d65 6e74 3e0a  ssion</element>.
-000002d0: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
-000002e0: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
-000002f0: 6474 696c 6573 2e64 6f63 756d 656e 745f  dtiles.document_
-00000300: 6163 7469 6f6e 733c 2f65 6c65 6d65 6e74  actions</element
-00000310: 3e0a 2020 2020 2020 3c65 6c65 6d65 6e74  >.      <element
-00000320: 3e70 6c6f 6e65 2e61 7070 2e73 7461 6e64  >plone.app.stand
-00000330: 6172 6474 696c 6573 2e64 6f63 756d 656e  ardtiles.documen
-00000340: 745f 6279 6c69 6e65 3c2f 656c 656d 656e  t_byline</elemen
-00000350: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
-00000360: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
-00000370: 6461 7264 7469 6c65 732e 6475 626c 696e  dardtiles.dublin
-00000380: 636f 7265 3c2f 656c 656d 656e 743e 0a20  core</element>. 
-00000390: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
-000003a0: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
-000003b0: 7469 6c65 732e 6564 6974 5f62 6172 3c2f  tiles.edit_bar</
-000003c0: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
-000003d0: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
-000003e0: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
-000003f0: 656d 6265 643c 2f65 6c65 6d65 6e74 3e0a  embed</element>.
-00000400: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
-00000410: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
-00000420: 6474 696c 6573 2e72 6177 656d 6265 643c  dtiles.rawembed<
-00000430: 2f65 6c65 6d65 6e74 3e0a 2020 2020 2020  /element>.      
-00000440: 3c65 6c65 6d65 6e74 3e70 6c6f 6e65 2e61  <element>plone.a
-00000450: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
-00000460: 2e65 7869 7374 696e 6763 6f6e 7465 6e74  .existingcontent
-00000470: 3c2f 656c 656d 656e 743e 0a20 2020 2020  </element>.     
-00000480: 203c 656c 656d 656e 743e 706c 6f6e 652e   <element>plone.
-00000490: 6170 702e 7374 616e 6461 7264 7469 6c65  app.standardtile
-000004a0: 732e 6661 7669 636f 6e6c 696e 6b3c 2f65  s.faviconlink</e
-000004b0: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
-000004c0: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
-000004d0: 2e73 7461 6e64 6172 6474 696c 6573 2e66  .standardtiles.f
-000004e0: 6965 6c64 3c2f 656c 656d 656e 743e 0a20  ield</element>. 
-000004f0: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
-00000500: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
-00000510: 7469 6c65 732e 666f 6f74 6572 3c2f 656c  tiles.footer</el
-00000520: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
-00000530: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-00000540: 7374 616e 6461 7264 7469 6c65 732e 676c  standardtiles.gl
-00000550: 6f62 616c 5f73 6563 7469 6f6e 733c 2f65  obal_sections</e
-00000560: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
-00000570: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
-00000580: 2e73 7461 6e64 6172 6474 696c 6573 2e68  .standardtiles.h
-00000590: 6561 6474 6974 6c65 3c2f 656c 656d 656e  eadtitle</elemen
-000005a0: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
-000005b0: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
-000005c0: 6461 7264 7469 6c65 732e 6869 7374 6f72  dardtiles.histor
-000005d0: 793c 2f65 6c65 6d65 6e74 3e0a 2020 2020  y</element>.    
-000005e0: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
-000005f0: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
-00000600: 6573 2e6a 6176 6173 6372 6970 7473 3c2f  es.javascripts</
-00000610: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
-00000620: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
-00000630: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
-00000640: 6b65 7977 6f72 6473 3c2f 656c 656d 656e  keywords</elemen
-00000650: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
-00000660: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
-00000670: 6461 7264 7469 6c65 732e 6c61 6e67 7561  dardtiles.langua
-00000680: 6765 7365 6c65 6374 6f72 3c2f 656c 656d  geselector</elem
-00000690: 656e 743e 0a20 2020 2020 203c 656c 656d  ent>.      <elem
-000006a0: 656e 743e 706c 6f6e 652e 6170 702e 7374  ent>plone.app.st
-000006b0: 616e 6461 7264 7469 6c65 732e 6c6f 636b  andardtiles.lock
-000006c0: 696e 666f 3c2f 656c 656d 656e 743e 0a20  info</element>. 
-000006d0: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
-000006e0: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
-000006f0: 7469 6c65 732e 6c6f 6769 6e3c 2f65 6c65  tiles.login</ele
-00000700: 6d65 6e74 3e0a 2020 2020 2020 3c65 6c65  ment>.      <ele
-00000710: 6d65 6e74 3e70 6c6f 6e65 2e61 7070 2e73  ment>plone.app.s
-00000720: 7461 6e64 6172 6474 696c 6573 2e6c 6f67  tandardtiles.log
-00000730: 6f3c 2f65 6c65 6d65 6e74 3e0a 2020 2020  o</element>.    
-00000740: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
-00000750: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
-00000760: 6573 2e6e 6176 6967 6174 696f 6e3c 2f65  es.navigation</e
-00000770: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
-00000780: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
-00000790: 2e73 7461 6e64 6172 6474 696c 6573 2e6e  .standardtiles.n
-000007a0: 6176 6967 6174 696f 6e6c 696e 6b3c 2f65  avigationlink</e
-000007b0: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
-000007c0: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
-000007d0: 2e73 7461 6e64 6172 6474 696c 6573 2e6e  .standardtiles.n
-000007e0: 6578 7470 7265 7669 6f75 733c 2f65 6c65  extprevious</ele
-000007f0: 6d65 6e74 3e0a 2020 2020 2020 3c65 6c65  ment>.      <ele
-00000800: 6d65 6e74 3e70 6c6f 6e65 2e61 7070 2e73  ment>plone.app.s
-00000810: 7461 6e64 6172 6474 696c 6573 2e70 6174  tandardtiles.pat
-00000820: 685f 6261 723c 2f65 6c65 6d65 6e74 3e0a  h_bar</element>.
-00000830: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
-00000840: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
-00000850: 6474 696c 6573 2e70 6572 736f 6e61 6c5f  dtiles.personal_
-00000860: 6261 723c 2f65 6c65 6d65 6e74 3e0a 2020  bar</element>.  
-00000870: 2020 2020 3c65 6c65 6d65 6e74 3e70 6c6f      <element>plo
-00000880: 6e65 2e61 7070 2e73 7461 6e64 6172 6474  ne.app.standardt
-00000890: 696c 6573 2e70 6f72 746c 6574 3c2f 656c  iles.portlet</el
-000008a0: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
-000008b0: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-000008c0: 7374 616e 6461 7264 7469 6c65 732e 706f  standardtiles.po
-000008d0: 7274 6c65 746d 616e 6167 6572 3c2f 656c  rtletmanager</el
-000008e0: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
-000008f0: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-00000900: 7374 616e 6461 7264 7469 6c65 732e 7265  standardtiles.re
-00000910: 6c61 7465 645f 6974 656d 733c 2f65 6c65  lated_items</ele
-00000920: 6d65 6e74 3e0a 2020 2020 2020 3c65 6c65  ment>.      <ele
-00000930: 6d65 6e74 3e70 6c6f 6e65 2e61 7070 2e73  ment>plone.app.s
-00000940: 7461 6e64 6172 6474 696c 6573 2e72 7373  tandardtiles.rss
-00000950: 3c2f 656c 656d 656e 743e 0a20 2020 2020  </element>.     
-00000960: 203c 656c 656d 656e 743e 706c 6f6e 652e   <element>plone.
-00000970: 6170 702e 7374 616e 6461 7264 7469 6c65  app.standardtile
-00000980: 732e 7273 736c 696e 6b3c 2f65 6c65 6d65  s.rsslink</eleme
-00000990: 6e74 3e0a 2020 2020 2020 3c65 6c65 6d65  nt>.      <eleme
-000009a0: 6e74 3e70 6c6f 6e65 2e61 7070 2e73 7461  nt>plone.app.sta
-000009b0: 6e64 6172 6474 696c 6573 2e73 6561 7263  ndardtiles.searc
-000009c0: 6862 6f78 3c2f 656c 656d 656e 743e 0a20  hbox</element>. 
-000009d0: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
-000009e0: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
-000009f0: 7469 6c65 732e 7365 6172 6368 6c69 6e6b  tiles.searchlink
-00000a00: 3c2f 656c 656d 656e 743e 0a20 2020 2020  </element>.     
-00000a10: 203c 656c 656d 656e 743e 706c 6f6e 652e   <element>plone.
-00000a20: 6170 702e 7374 616e 6461 7264 7469 6c65  app.standardtile
-00000a30: 732e 7369 7465 5f61 6374 696f 6e73 3c2f  s.site_actions</
-00000a40: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
-00000a50: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
-00000a60: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
-00000a70: 7369 7465 6d61 703c 2f65 6c65 6d65 6e74  sitemap</element
-00000a80: 3e0a 2020 2020 2020 3c65 6c65 6d65 6e74  >.      <element
-00000a90: 3e70 6c6f 6e65 2e61 7070 2e73 7461 6e64  >plone.app.stand
-00000aa0: 6172 6474 696c 6573 2e73 6b69 705f 6c69  ardtiles.skip_li
-00000ab0: 6e6b 733c 2f65 6c65 6d65 6e74 3e0a 2020  nks</element>.  
-00000ac0: 2020 2020 3c65 6c65 6d65 6e74 3e70 6c6f      <element>plo
-00000ad0: 6e65 2e61 7070 2e73 7461 6e64 6172 6474  ne.app.standardt
-00000ae0: 696c 6573 2e73 7479 6c65 7368 6565 7473  iles.stylesheets
-00000af0: 3c2f 656c 656d 656e 743e 0a20 2020 2020  </element>.     
-00000b00: 203c 656c 656d 656e 743e 706c 6f6e 652e   <element>plone.
-00000b10: 6170 702e 7374 616e 6461 7264 7469 6c65  app.standardtile
-00000b20: 732e 7461 626c 656f 6663 6f6e 7465 6e74  s.tableofcontent
-00000b30: 733c 2f65 6c65 6d65 6e74 3e0a 2020 2020  s</element>.    
-00000b40: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
-00000b50: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
-00000b60: 6573 2e74 6974 6c65 3c2f 656c 656d 656e  es.title</elemen
-00000b70: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
-00000b80: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
-00000b90: 6461 7264 7469 6c65 732e 746f 6f6c 6261  dardtiles.toolba
-00000ba0: 723c 2f65 6c65 6d65 6e74 3e0a 2020 2020  r</element>.    
-00000bb0: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
-00000bc0: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
-00000bd0: 6573 2e76 6965 776c 6574 6d61 6e61 6765  es.viewletmanage
-00000be0: 723c 2f65 6c65 6d65 6e74 3e0a 2020 2020  r</element>.    
-00000bf0: 3c2f 7661 6c75 653e 0a20 203c 2f72 6563  </value>.  </rec
-00000c00: 6f72 643e 0a0a 2020 3c72 6563 6f72 6420  ord>..  <record 
-00000c10: 6e61 6d65 3d22 706c 6f6e 652e 6170 702e  name="plone.app.
-00000c20: 7374 616e 6461 7264 7469 6c65 732e 6c69  standardtiles.li
-00000c30: 7374 696e 675f 7669 6577 7322 3e0a 2020  sting_views">.  
-00000c40: 2020 3c66 6965 6c64 2074 7970 653d 2270    <field type="p
-00000c50: 6c6f 6e65 2e72 6567 6973 7472 792e 6669  lone.registry.fi
-00000c60: 656c 642e 4469 6374 223e 0a20 2020 2020  eld.Dict">.     
-00000c70: 203c 7469 746c 653e 4c69 7374 696e 6720   <title>Listing 
-00000c80: 5669 6577 733c 2f74 6974 6c65 3e0a 2020  Views</title>.  
-00000c90: 2020 2020 3c6b 6579 5f74 7970 6520 7479      <key_type ty
-00000ca0: 7065 3d22 706c 6f6e 652e 7265 6769 7374  pe="plone.regist
-00000cb0: 7279 2e66 6965 6c64 2e54 6578 744c 696e  ry.field.TextLin
-00000cc0: 6522 202f 3e0a 2020 2020 2020 3c76 616c  e" />.      <val
-00000cd0: 7565 5f74 7970 6520 7479 7065 3d22 706c  ue_type type="pl
-00000ce0: 6f6e 652e 7265 6769 7374 7279 2e66 6965  one.registry.fie
-00000cf0: 6c64 2e54 6578 744c 696e 6522 202f 3e0a  ld.TextLine" />.
-00000d00: 2020 2020 3c2f 6669 656c 643e 0a20 2020      </field>.   
-00000d10: 203c 7661 6c75 6520 7075 7267 653d 2266   <value purge="f
-00000d20: 616c 7365 223e 0a20 2020 2020 203c 656c  alse">.      <el
-00000d30: 656d 656e 7420 6b65 793d 226c 6973 7469  ement key="listi
-00000d40: 6e67 5f76 6965 7722 3e4c 6973 7469 6e67  ng_view">Listing
-00000d50: 2076 6965 773c 2f65 6c65 6d65 6e74 3e0a   view</element>.
-00000d60: 2020 2020 2020 3c65 6c65 6d65 6e74 206b        <element k
-00000d70: 6579 3d22 7375 6d6d 6172 795f 7669 6577  ey="summary_view
-00000d80: 223e 5375 6d6d 6172 7920 7669 6577 3c2f  ">Summary view</
-00000d90: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
-00000da0: 656c 656d 656e 7420 6b65 793d 2274 6162  element key="tab
-00000db0: 756c 6172 5f76 6965 7722 3e54 6162 756c  ular_view">Tabul
-00000dc0: 6172 2076 6965 773c 2f65 6c65 6d65 6e74  ar view</element
-00000dd0: 3e0a 2020 2020 3c2f 7661 6c75 653e 0a20  >.    </value>. 
-00000de0: 203c 2f72 6563 6f72 643e 0a0a 2020 3c72   </record>..  <r
-00000df0: 6563 6f72 6420 6e61 6d65 3d22 706c 6f6e  ecord name="plon
-00000e00: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
-00000e10: 6c65 732e 636f 6e74 656e 745f 7669 6577  les.content_view
-00000e20: 7322 3e0a 2020 2020 3c66 6965 6c64 2074  s">.    <field t
-00000e30: 7970 653d 2270 6c6f 6e65 2e72 6567 6973  ype="plone.regis
-00000e40: 7472 792e 6669 656c 642e 4469 6374 223e  try.field.Dict">
-00000e50: 0a20 2020 2020 203c 7469 746c 653e 436f  .      <title>Co
-00000e60: 6e74 656e 7420 5669 6577 733c 2f74 6974  ntent Views</tit
-00000e70: 6c65 3e0a 2020 2020 2020 3c72 6571 7569  le>.      <requi
-00000e80: 7265 643e 4661 6c73 653c 2f72 6571 7569  red>False</requi
-00000e90: 7265 643e 0a20 2020 2020 203c 6b65 795f  red>.      <key_
-00000ea0: 7479 7065 2074 7970 653d 2270 6c6f 6e65  type type="plone
-00000eb0: 2e72 6567 6973 7472 792e 6669 656c 642e  .registry.field.
-00000ec0: 5465 7874 4c69 6e65 2220 2f3e 0a20 2020  TextLine" />.   
-00000ed0: 2020 203c 7661 6c75 655f 7479 7065 2074     <value_type t
-00000ee0: 7970 653d 2270 6c6f 6e65 2e72 6567 6973  ype="plone.regis
-00000ef0: 7472 792e 6669 656c 642e 5465 7874 4c69  try.field.TextLi
-00000f00: 6e65 2220 2f3e 0a20 2020 203c 2f66 6965  ne" />.    </fie
-00000f10: 6c64 3e0a 2020 3c2f 7265 636f 7264 3e0a  ld>.  </record>.
-00000f20: 0a20 203c 7265 636f 7264 7320 696e 7465  .  <records inte
-00000f30: 7266 6163 653d 2270 6c6f 6e65 2e61 7070  rface="plone.app
-00000f40: 2e71 7565 7279 7374 7269 6e67 2e69 6e74  .querystring.int
-00000f50: 6572 6661 6365 732e 4951 7565 7279 4669  erfaces.IQueryFi
-00000f60: 656c 6422 0a20 2020 2020 2020 2020 2020  eld".           
-00000f70: 7072 6566 6978 3d22 706c 6f6e 652e 6170  prefix="plone.ap
-00000f80: 702e 7175 6572 7973 7472 696e 672e 6669  p.querystring.fi
-00000f90: 656c 642e 6765 744f 626a 506f 7369 7469  eld.getObjPositi
-00000fa0: 6f6e 496e 5061 7265 6e74 220a 2020 3e0a  onInParent".  >.
-00000fb0: 2020 2020 3c76 616c 7565 206b 6579 3d22      <value key="
-00000fc0: 736f 7274 6162 6c65 223e 5472 7565 3c2f  sortable">True</
-00000fd0: 7661 6c75 653e 0a20 203c 2f72 6563 6f72  value>.  </recor
-00000fe0: 6473 3e0a 0a20 203c 7265 636f 7264 206e  ds>..  <record n
-00000ff0: 616d 653d 2270 6c6f 6e65 2e61 7070 2e70  ame="plone.app.p
-00001000: 6f72 746c 6574 732e 506f 7274 6c65 744d  ortlets.PortletM
-00001010: 616e 6167 6572 426c 6163 6b6c 6973 7422  anagerBlacklist"
-00001020: 3e0a 2020 2020 3c66 6965 6c64 2074 7970  >.    <field typ
-00001030: 653d 2270 6c6f 6e65 2e72 6567 6973 7472  e="plone.registr
-00001040: 792e 6669 656c 642e 4c69 7374 223e 0a20  y.field.List">. 
-00001050: 2020 2020 203c 7469 746c 653e 546f 6f6c       <title>Tool
-00001060: 6261 7220 506f 7274 6c65 7420 4d61 6e61  bar Portlet Mana
-00001070: 6765 7220 426c 6163 6b6c 6973 743c 2f74  ger Blacklist</t
-00001080: 6974 6c65 3e0a 2020 2020 2020 3c64 6573  itle>.      <des
-00001090: 6372 6970 7469 6f6e 3e41 206c 6973 7420  cription>A list 
-000010a0: 6f66 2070 6f72 746c 6574 206d 616e 6167  of portlet manag
-000010b0: 6572 206e 616d 6573 2074 6861 7420 7769  er names that wi
-000010c0: 6c6c 206e 6f74 2062 6520 7368 6f77 6e20  ll not be shown 
-000010d0: 696e 2074 6865 2074 6f6f 6c62 6172 2064  in the toolbar d
-000010e0: 726f 7064 6f77 6e3c 2f64 6573 6372 6970  ropdown</descrip
-000010f0: 7469 6f6e 3e0a 2020 2020 2020 3c76 616c  tion>.      <val
-00001100: 7565 5f74 7970 6520 7479 7065 3d22 706c  ue_type type="pl
-00001110: 6f6e 652e 7265 6769 7374 7279 2e66 6965  one.registry.fie
-00001120: 6c64 2e54 6578 744c 696e 6522 202f 3e0a  ld.TextLine" />.
-00001130: 2020 2020 3c2f 6669 656c 643e 0a20 2020      </field>.   
-00001140: 203c 7661 6c75 6520 7075 7267 653d 2266   <value purge="f
-00001150: 616c 7365 223e 0a20 2020 2020 203c 656c  alse">.      <el
-00001160: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
-00001170: 7374 616e 6461 7264 7469 6c65 732e 706f  standardtiles.po
-00001180: 7274 6c65 744d 616e 6167 6572 3c2f 656c  rtletManager</el
-00001190: 656d 656e 743e 0a20 2020 203c 2f76 616c  ement>.    </val
-000011a0: 7565 3e0a 2020 3c2f 7265 636f 7264 3e0a  ue>.  </record>.
-000011b0: 3c2f 7265 6769 7374 7279 3e0a            </registry>.
+00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
+00000020: 662d 3822 3f3e 0a3c 7265 6769 7374 7279  f-8"?>.<registry
+00000030: 3e0a 2020 3c72 6563 6f72 6420 6e61 6d65  >.  <record name
+00000040: 3d22 706c 6f6e 652e 6170 702e 7469 6c65  ="plone.app.tile
+00000050: 7322 3e0a 2020 2020 3c66 6965 6c64 2074  s">.    <field t
+00000060: 7970 653d 2270 6c6f 6e65 2e72 6567 6973  ype="plone.regis
+00000070: 7472 792e 6669 656c 642e 4c69 7374 223e  try.field.List">
+00000080: 0a20 2020 2020 203c 7469 746c 653e 5469  .      <title>Ti
+00000090: 6c65 733c 2f74 6974 6c65 3e0a 2020 2020  les</title>.    
+000000a0: 2020 3c76 616c 7565 5f74 7970 6520 7479    <value_type ty
+000000b0: 7065 3d22 706c 6f6e 652e 7265 6769 7374  pe="plone.regist
+000000c0: 7279 2e66 6965 6c64 2e54 6578 744c 696e  ry.field.TextLin
+000000d0: 6522 202f 3e0a 2020 2020 3c2f 6669 656c  e" />.    </fiel
+000000e0: 643e 0a20 2020 203c 7661 6c75 6520 7075  d>.    <value pu
+000000f0: 7267 653d 2266 616c 7365 223e 0a20 2020  rge="false">.   
+00000100: 2020 203c 656c 656d 656e 743e 706c 6f6e     <element>plon
+00000110: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
+00000120: 6c65 732e 616e 616c 7974 6963 733c 2f65  les.analytics</e
+00000130: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
+00000140: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+00000150: 2e73 7461 6e64 6172 6474 696c 6573 2e61  .standardtiles.a
+00000160: 6e6f 6e74 6f6f 6c73 3c2f 656c 656d 656e  nontools</elemen
+00000170: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
+00000180: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
+00000190: 6461 7264 7469 6c65 732e 6175 7468 6f72  dardtiles.author
+000001a0: 6c69 6e6b 3c2f 656c 656d 656e 743e 0a20  link</element>. 
+000001b0: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
+000001c0: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
+000001d0: 7469 6c65 732e 6361 6e6f 6e69 6361 6c5f  tiles.canonical_
+000001e0: 7572 6c3c 2f65 6c65 6d65 6e74 3e0a 2020  url</element>.  
+000001f0: 2020 2020 3c65 6c65 6d65 6e74 3e70 6c6f      <element>plo
+00000200: 6e65 2e61 7070 2e73 7461 6e64 6172 6474  ne.app.standardt
+00000210: 696c 6573 2e63 6f6c 6f70 686f 6e3c 2f65  iles.colophon</e
+00000220: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
+00000230: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+00000240: 2e73 7461 6e64 6172 6474 696c 6573 2e63  .standardtiles.c
+00000250: 6f6e 7465 6e74 6c69 7374 696e 673c 2f65  ontentlisting</e
+00000260: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
+00000270: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+00000280: 2e73 7461 6e64 6172 6474 696c 6573 2e64  .standardtiles.d
+00000290: 6573 6372 6970 7469 6f6e 3c2f 656c 656d  escription</elem
+000002a0: 656e 743e 0a20 2020 2020 203c 656c 656d  ent>.      <elem
+000002b0: 656e 743e 706c 6f6e 652e 6170 702e 7374  ent>plone.app.st
+000002c0: 616e 6461 7264 7469 6c65 732e 6469 7363  andardtiles.disc
+000002d0: 7573 7369 6f6e 3c2f 656c 656d 656e 743e  ussion</element>
+000002e0: 0a20 2020 2020 203c 656c 656d 656e 743e  .      <element>
+000002f0: 706c 6f6e 652e 6170 702e 7374 616e 6461  plone.app.standa
+00000300: 7264 7469 6c65 732e 646f 6375 6d65 6e74  rdtiles.document
+00000310: 5f61 6374 696f 6e73 3c2f 656c 656d 656e  _actions</elemen
+00000320: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
+00000330: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
+00000340: 6461 7264 7469 6c65 732e 646f 6375 6d65  dardtiles.docume
+00000350: 6e74 5f62 796c 696e 653c 2f65 6c65 6d65  nt_byline</eleme
+00000360: 6e74 3e0a 2020 2020 2020 3c65 6c65 6d65  nt>.      <eleme
+00000370: 6e74 3e70 6c6f 6e65 2e61 7070 2e73 7461  nt>plone.app.sta
+00000380: 6e64 6172 6474 696c 6573 2e64 7562 6c69  ndardtiles.dubli
+00000390: 6e63 6f72 653c 2f65 6c65 6d65 6e74 3e0a  ncore</element>.
+000003a0: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
+000003b0: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
+000003c0: 6474 696c 6573 2e65 6469 745f 6261 723c  dtiles.edit_bar<
+000003d0: 2f65 6c65 6d65 6e74 3e0a 2020 2020 2020  /element>.      
+000003e0: 3c65 6c65 6d65 6e74 3e70 6c6f 6e65 2e61  <element>plone.a
+000003f0: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
+00000400: 2e65 6d62 6564 3c2f 656c 656d 656e 743e  .embed</element>
+00000410: 0a20 2020 2020 203c 656c 656d 656e 743e  .      <element>
+00000420: 706c 6f6e 652e 6170 702e 7374 616e 6461  plone.app.standa
+00000430: 7264 7469 6c65 732e 7261 7765 6d62 6564  rdtiles.rawembed
+00000440: 3c2f 656c 656d 656e 743e 0a20 2020 2020  </element>.     
+00000450: 203c 656c 656d 656e 743e 706c 6f6e 652e   <element>plone.
+00000460: 6170 702e 7374 616e 6461 7264 7469 6c65  app.standardtile
+00000470: 732e 6578 6973 7469 6e67 636f 6e74 656e  s.existingconten
+00000480: 743c 2f65 6c65 6d65 6e74 3e0a 2020 2020  t</element>.    
+00000490: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
+000004a0: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
+000004b0: 6573 2e66 6176 6963 6f6e 6c69 6e6b 3c2f  es.faviconlink</
+000004c0: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
+000004d0: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
+000004e0: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
+000004f0: 6669 656c 643c 2f65 6c65 6d65 6e74 3e0a  field</element>.
+00000500: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
+00000510: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
+00000520: 6474 696c 6573 2e66 6f6f 7465 723c 2f65  dtiles.footer</e
+00000530: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
+00000540: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+00000550: 2e73 7461 6e64 6172 6474 696c 6573 2e67  .standardtiles.g
+00000560: 6c6f 6261 6c5f 7365 6374 696f 6e73 3c2f  lobal_sections</
+00000570: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
+00000580: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
+00000590: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
+000005a0: 6865 6164 7469 746c 653c 2f65 6c65 6d65  headtitle</eleme
+000005b0: 6e74 3e0a 2020 2020 2020 3c65 6c65 6d65  nt>.      <eleme
+000005c0: 6e74 3e70 6c6f 6e65 2e61 7070 2e73 7461  nt>plone.app.sta
+000005d0: 6e64 6172 6474 696c 6573 2e68 6973 746f  ndardtiles.histo
+000005e0: 7279 3c2f 656c 656d 656e 743e 0a20 2020  ry</element>.   
+000005f0: 2020 203c 656c 656d 656e 743e 706c 6f6e     <element>plon
+00000600: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
+00000610: 6c65 732e 6a61 7661 7363 7269 7074 733c  les.javascripts<
+00000620: 2f65 6c65 6d65 6e74 3e0a 2020 2020 2020  /element>.      
+00000630: 3c65 6c65 6d65 6e74 3e70 6c6f 6e65 2e61  <element>plone.a
+00000640: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
+00000650: 2e6b 6579 776f 7264 733c 2f65 6c65 6d65  .keywords</eleme
+00000660: 6e74 3e0a 2020 2020 2020 3c65 6c65 6d65  nt>.      <eleme
+00000670: 6e74 3e70 6c6f 6e65 2e61 7070 2e73 7461  nt>plone.app.sta
+00000680: 6e64 6172 6474 696c 6573 2e6c 616e 6775  ndardtiles.langu
+00000690: 6167 6573 656c 6563 746f 723c 2f65 6c65  ageselector</ele
+000006a0: 6d65 6e74 3e0a 2020 2020 2020 3c65 6c65  ment>.      <ele
+000006b0: 6d65 6e74 3e70 6c6f 6e65 2e61 7070 2e73  ment>plone.app.s
+000006c0: 7461 6e64 6172 6474 696c 6573 2e6c 6f63  tandardtiles.loc
+000006d0: 6b69 6e66 6f3c 2f65 6c65 6d65 6e74 3e0a  kinfo</element>.
+000006e0: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
+000006f0: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
+00000700: 6474 696c 6573 2e6c 6f67 696e 3c2f 656c  dtiles.login</el
+00000710: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
+00000720: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
+00000730: 7374 616e 6461 7264 7469 6c65 732e 6c6f  standardtiles.lo
+00000740: 676f 3c2f 656c 656d 656e 743e 0a20 2020  go</element>.   
+00000750: 2020 203c 656c 656d 656e 743e 706c 6f6e     <element>plon
+00000760: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
+00000770: 6c65 732e 6e61 7669 6761 7469 6f6e 3c2f  les.navigation</
+00000780: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
+00000790: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
+000007a0: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
+000007b0: 6e61 7669 6761 7469 6f6e 6c69 6e6b 3c2f  navigationlink</
+000007c0: 656c 656d 656e 743e 0a20 2020 2020 203c  element>.      <
+000007d0: 656c 656d 656e 743e 706c 6f6e 652e 6170  element>plone.ap
+000007e0: 702e 7374 616e 6461 7264 7469 6c65 732e  p.standardtiles.
+000007f0: 6e65 7874 7072 6576 696f 7573 3c2f 656c  nextprevious</el
+00000800: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
+00000810: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
+00000820: 7374 616e 6461 7264 7469 6c65 732e 7061  standardtiles.pa
+00000830: 7468 5f62 6172 3c2f 656c 656d 656e 743e  th_bar</element>
+00000840: 0a20 2020 2020 203c 656c 656d 656e 743e  .      <element>
+00000850: 706c 6f6e 652e 6170 702e 7374 616e 6461  plone.app.standa
+00000860: 7264 7469 6c65 732e 7065 7273 6f6e 616c  rdtiles.personal
+00000870: 5f62 6172 3c2f 656c 656d 656e 743e 0a20  _bar</element>. 
+00000880: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
+00000890: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
+000008a0: 7469 6c65 732e 706f 7274 6c65 743c 2f65  tiles.portlet</e
+000008b0: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
+000008c0: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+000008d0: 2e73 7461 6e64 6172 6474 696c 6573 2e70  .standardtiles.p
+000008e0: 6f72 746c 6574 6d61 6e61 6765 723c 2f65  ortletmanager</e
+000008f0: 6c65 6d65 6e74 3e0a 2020 2020 2020 3c65  lement>.      <e
+00000900: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+00000910: 2e73 7461 6e64 6172 6474 696c 6573 2e72  .standardtiles.r
+00000920: 656c 6174 6564 5f69 7465 6d73 3c2f 656c  elated_items</el
+00000930: 656d 656e 743e 0a20 2020 2020 203c 656c  ement>.      <el
+00000940: 656d 656e 743e 706c 6f6e 652e 6170 702e  ement>plone.app.
+00000950: 7374 616e 6461 7264 7469 6c65 732e 7273  standardtiles.rs
+00000960: 733c 2f65 6c65 6d65 6e74 3e0a 2020 2020  s</element>.    
+00000970: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
+00000980: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
+00000990: 6573 2e72 7373 6c69 6e6b 3c2f 656c 656d  es.rsslink</elem
+000009a0: 656e 743e 0a20 2020 2020 203c 656c 656d  ent>.      <elem
+000009b0: 656e 743e 706c 6f6e 652e 6170 702e 7374  ent>plone.app.st
+000009c0: 616e 6461 7264 7469 6c65 732e 7365 6172  andardtiles.sear
+000009d0: 6368 626f 783c 2f65 6c65 6d65 6e74 3e0a  chbox</element>.
+000009e0: 2020 2020 2020 3c65 6c65 6d65 6e74 3e70        <element>p
+000009f0: 6c6f 6e65 2e61 7070 2e73 7461 6e64 6172  lone.app.standar
+00000a00: 6474 696c 6573 2e73 6561 7263 686c 696e  dtiles.searchlin
+00000a10: 6b3c 2f65 6c65 6d65 6e74 3e0a 2020 2020  k</element>.    
+00000a20: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
+00000a30: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
+00000a40: 6573 2e73 6974 655f 6163 7469 6f6e 733c  es.site_actions<
+00000a50: 2f65 6c65 6d65 6e74 3e0a 2020 2020 2020  /element>.      
+00000a60: 3c65 6c65 6d65 6e74 3e70 6c6f 6e65 2e61  <element>plone.a
+00000a70: 7070 2e73 7461 6e64 6172 6474 696c 6573  pp.standardtiles
+00000a80: 2e73 6974 656d 6170 3c2f 656c 656d 656e  .sitemap</elemen
+00000a90: 743e 0a20 2020 2020 203c 656c 656d 656e  t>.      <elemen
+00000aa0: 743e 706c 6f6e 652e 6170 702e 7374 616e  t>plone.app.stan
+00000ab0: 6461 7264 7469 6c65 732e 736b 6970 5f6c  dardtiles.skip_l
+00000ac0: 696e 6b73 3c2f 656c 656d 656e 743e 0a20  inks</element>. 
+00000ad0: 2020 2020 203c 656c 656d 656e 743e 706c       <element>pl
+00000ae0: 6f6e 652e 6170 702e 7374 616e 6461 7264  one.app.standard
+00000af0: 7469 6c65 732e 7374 796c 6573 6865 6574  tiles.stylesheet
+00000b00: 733c 2f65 6c65 6d65 6e74 3e0a 2020 2020  s</element>.    
+00000b10: 2020 3c65 6c65 6d65 6e74 3e70 6c6f 6e65    <element>plone
+00000b20: 2e61 7070 2e73 7461 6e64 6172 6474 696c  .app.standardtil
+00000b30: 6573 2e74 6162 6c65 6f66 636f 6e74 656e  es.tableofconten
+00000b40: 7473 3c2f 656c 656d 656e 743e 0a20 2020  ts</element>.   
+00000b50: 2020 203c 656c 656d 656e 743e 706c 6f6e     <element>plon
+00000b60: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
+00000b70: 6c65 732e 7469 746c 653c 2f65 6c65 6d65  les.title</eleme
+00000b80: 6e74 3e0a 2020 2020 2020 3c65 6c65 6d65  nt>.      <eleme
+00000b90: 6e74 3e70 6c6f 6e65 2e61 7070 2e73 7461  nt>plone.app.sta
+00000ba0: 6e64 6172 6474 696c 6573 2e74 6f6f 6c62  ndardtiles.toolb
+00000bb0: 6172 3c2f 656c 656d 656e 743e 0a20 2020  ar</element>.   
+00000bc0: 2020 203c 656c 656d 656e 743e 706c 6f6e     <element>plon
+00000bd0: 652e 6170 702e 7374 616e 6461 7264 7469  e.app.standardti
+00000be0: 6c65 732e 7669 6577 6c65 746d 616e 6167  les.viewletmanag
+00000bf0: 6572 3c2f 656c 656d 656e 743e 0a20 2020  er</element>.   
+00000c00: 203c 2f76 616c 7565 3e0a 2020 3c2f 7265   </value>.  </re
+00000c10: 636f 7264 3e0a 0a20 203c 7265 636f 7264  cord>..  <record
+00000c20: 206e 616d 653d 2270 6c6f 6e65 2e61 7070   name="plone.app
+00000c30: 2e73 7461 6e64 6172 6474 696c 6573 2e6c  .standardtiles.l
+00000c40: 6973 7469 6e67 5f76 6965 7773 223e 0a20  isting_views">. 
+00000c50: 2020 203c 6669 656c 6420 7479 7065 3d22     <field type="
+00000c60: 706c 6f6e 652e 7265 6769 7374 7279 2e66  plone.registry.f
+00000c70: 6965 6c64 2e44 6963 7422 3e0a 2020 2020  ield.Dict">.    
+00000c80: 2020 3c74 6974 6c65 3e4c 6973 7469 6e67    <title>Listing
+00000c90: 2056 6965 7773 3c2f 7469 746c 653e 0a20   Views</title>. 
+00000ca0: 2020 2020 203c 6b65 795f 7479 7065 2074       <key_type t
+00000cb0: 7970 653d 2270 6c6f 6e65 2e72 6567 6973  ype="plone.regis
+00000cc0: 7472 792e 6669 656c 642e 5465 7874 4c69  try.field.TextLi
+00000cd0: 6e65 2220 2f3e 0a20 2020 2020 203c 7661  ne" />.      <va
+00000ce0: 6c75 655f 7479 7065 2074 7970 653d 2270  lue_type type="p
+00000cf0: 6c6f 6e65 2e72 6567 6973 7472 792e 6669  lone.registry.fi
+00000d00: 656c 642e 5465 7874 4c69 6e65 2220 2f3e  eld.TextLine" />
+00000d10: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
+00000d20: 2020 3c76 616c 7565 2070 7572 6765 3d22    <value purge="
+00000d30: 6661 6c73 6522 3e0a 2020 2020 2020 3c65  false">.      <e
+00000d40: 6c65 6d65 6e74 206b 6579 3d22 6c69 7374  lement key="list
+00000d50: 696e 675f 7669 6577 223e 4c69 7374 696e  ing_view">Listin
+00000d60: 6720 7669 6577 3c2f 656c 656d 656e 743e  g view</element>
+00000d70: 0a20 2020 2020 203c 656c 656d 656e 7420  .      <element 
+00000d80: 6b65 793d 2273 756d 6d61 7279 5f76 6965  key="summary_vie
+00000d90: 7722 3e53 756d 6d61 7279 2076 6965 773c  w">Summary view<
+00000da0: 2f65 6c65 6d65 6e74 3e0a 2020 2020 2020  /element>.      
+00000db0: 3c65 6c65 6d65 6e74 206b 6579 3d22 7461  <element key="ta
+00000dc0: 6275 6c61 725f 7669 6577 223e 5461 6275  bular_view">Tabu
+00000dd0: 6c61 7220 7669 6577 3c2f 656c 656d 656e  lar view</elemen
+00000de0: 743e 0a20 2020 203c 2f76 616c 7565 3e0a  t>.    </value>.
+00000df0: 2020 3c2f 7265 636f 7264 3e0a 0a20 203c    </record>..  <
+00000e00: 7265 636f 7264 206e 616d 653d 2270 6c6f  record name="plo
+00000e10: 6e65 2e61 7070 2e73 7461 6e64 6172 6474  ne.app.standardt
+00000e20: 696c 6573 2e63 6f6e 7465 6e74 5f76 6965  iles.content_vie
+00000e30: 7773 223e 0a20 2020 203c 6669 656c 6420  ws">.    <field 
+00000e40: 7479 7065 3d22 706c 6f6e 652e 7265 6769  type="plone.regi
+00000e50: 7374 7279 2e66 6965 6c64 2e44 6963 7422  stry.field.Dict"
+00000e60: 3e0a 2020 2020 2020 3c74 6974 6c65 3e43  >.      <title>C
+00000e70: 6f6e 7465 6e74 2056 6965 7773 3c2f 7469  ontent Views</ti
+00000e80: 746c 653e 0a20 2020 2020 203c 7265 7175  tle>.      <requ
+00000e90: 6972 6564 3e46 616c 7365 3c2f 7265 7175  ired>False</requ
+00000ea0: 6972 6564 3e0a 2020 2020 2020 3c6b 6579  ired>.      <key
+00000eb0: 5f74 7970 6520 7479 7065 3d22 706c 6f6e  _type type="plon
+00000ec0: 652e 7265 6769 7374 7279 2e66 6965 6c64  e.registry.field
+00000ed0: 2e54 6578 744c 696e 6522 202f 3e0a 2020  .TextLine" />.  
+00000ee0: 2020 2020 3c76 616c 7565 5f74 7970 6520      <value_type 
+00000ef0: 7479 7065 3d22 706c 6f6e 652e 7265 6769  type="plone.regi
+00000f00: 7374 7279 2e66 6965 6c64 2e54 6578 744c  stry.field.TextL
+00000f10: 696e 6522 202f 3e0a 2020 2020 3c2f 6669  ine" />.    </fi
+00000f20: 656c 643e 0a20 203c 2f72 6563 6f72 643e  eld>.  </record>
+00000f30: 0a0a 2020 3c72 6563 6f72 6473 2069 6e74  ..  <records int
+00000f40: 6572 6661 6365 3d22 706c 6f6e 652e 6170  erface="plone.ap
+00000f50: 702e 7175 6572 7973 7472 696e 672e 696e  p.querystring.in
+00000f60: 7465 7266 6163 6573 2e49 5175 6572 7946  terfaces.IQueryF
+00000f70: 6965 6c64 220a 2020 2020 2020 2020 2020  ield".          
+00000f80: 2070 7265 6669 783d 2270 6c6f 6e65 2e61   prefix="plone.a
+00000f90: 7070 2e71 7565 7279 7374 7269 6e67 2e66  pp.querystring.f
+00000fa0: 6965 6c64 2e67 6574 4f62 6a50 6f73 6974  ield.getObjPosit
+00000fb0: 696f 6e49 6e50 6172 656e 7422 0a20 203e  ionInParent".  >
+00000fc0: 0a20 2020 203c 7661 6c75 6520 6b65 793d  .    <value key=
+00000fd0: 2273 6f72 7461 626c 6522 3e54 7275 653c  "sortable">True<
+00000fe0: 2f76 616c 7565 3e0a 2020 3c2f 7265 636f  /value>.  </reco
+00000ff0: 7264 733e 0a0a 2020 3c72 6563 6f72 6420  rds>..  <record 
+00001000: 6e61 6d65 3d22 706c 6f6e 652e 6170 702e  name="plone.app.
+00001010: 706f 7274 6c65 7473 2e50 6f72 746c 6574  portlets.Portlet
+00001020: 4d61 6e61 6765 7242 6c61 636b 6c69 7374  ManagerBlacklist
+00001030: 223e 0a20 2020 203c 6669 656c 6420 7479  ">.    <field ty
+00001040: 7065 3d22 706c 6f6e 652e 7265 6769 7374  pe="plone.regist
+00001050: 7279 2e66 6965 6c64 2e4c 6973 7422 3e0a  ry.field.List">.
+00001060: 2020 2020 2020 3c74 6974 6c65 3e54 6f6f        <title>Too
+00001070: 6c62 6172 2050 6f72 746c 6574 204d 616e  lbar Portlet Man
+00001080: 6167 6572 2042 6c61 636b 6c69 7374 3c2f  ager Blacklist</
+00001090: 7469 746c 653e 0a20 2020 2020 203c 6465  title>.      <de
+000010a0: 7363 7269 7074 696f 6e3e 4120 6c69 7374  scription>A list
+000010b0: 206f 6620 706f 7274 6c65 7420 6d61 6e61   of portlet mana
+000010c0: 6765 7220 6e61 6d65 7320 7468 6174 2077  ger names that w
+000010d0: 696c 6c20 6e6f 7420 6265 2073 686f 776e  ill not be shown
+000010e0: 2069 6e20 7468 6520 746f 6f6c 6261 7220   in the toolbar 
+000010f0: 6472 6f70 646f 776e 3c2f 6465 7363 7269  dropdown</descri
+00001100: 7074 696f 6e3e 0a20 2020 2020 203c 7661  ption>.      <va
+00001110: 6c75 655f 7479 7065 2074 7970 653d 2270  lue_type type="p
+00001120: 6c6f 6e65 2e72 6567 6973 7472 792e 6669  lone.registry.fi
+00001130: 656c 642e 5465 7874 4c69 6e65 2220 2f3e  eld.TextLine" />
+00001140: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
+00001150: 2020 3c76 616c 7565 2070 7572 6765 3d22    <value purge="
+00001160: 6661 6c73 6522 3e0a 2020 2020 2020 3c65  false">.      <e
+00001170: 6c65 6d65 6e74 3e70 6c6f 6e65 2e61 7070  lement>plone.app
+00001180: 2e73 7461 6e64 6172 6474 696c 6573 2e70  .standardtiles.p
+00001190: 6f72 746c 6574 4d61 6e61 6765 723c 2f65  ortletManager</e
+000011a0: 6c65 6d65 6e74 3e0a 2020 2020 3c2f 7661  lement>.    </va
+000011b0: 6c75 653e 0a20 203c 2f72 6563 6f72 643e  lue>.  </record>
+000011c0: 0a3c 2f72 6567 6973 7472 793e 0a         .</registry>.
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/rawembed.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rawembed.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/rss.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/setuphandlers.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/sitemap.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/attachment_listing.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/attachment_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/configlets.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/configlets.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/contentlisting_view.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/contentlisting_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/existingcontent_view.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/existingcontent_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/image.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/image.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/listing_view.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/listing_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/login.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/login.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/namedimage.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/namedimage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/navigation.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/navigation_recurse.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigation_recurse.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/navigationlink.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/navigationlink.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/rawembed.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rawembed.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/rss.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/rss.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/summary_view.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/summary_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/templates/tabular_view.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/templates/tabular_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/testing.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/testing.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/RSS.xml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/RSS.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,183 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 7574  .0" encoding="ut
-00000020: 662d 3822 203f 3e0a 3c72 6466 3a52 4446  f-8" ?>.<rdf:RDF
-00000030: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f70   xmlns="http://p
-00000040: 7572 6c2e 6f72 672f 7273 732f 312e 302f  url.org/rss/1.0/
-00000050: 220a 2020 2020 2020 2020 2078 6d6c 6e73  ".         xmlns
-00000060: 3a64 633d 2268 7474 703a 2f2f 7075 726c  :dc="http://purl
-00000070: 2e6f 7267 2f64 632f 656c 656d 656e 7473  .org/dc/elements
-00000080: 2f31 2e31 2f22 0a20 2020 2020 2020 2020  /1.1/".         
-00000090: 786d 6c6e 733a 7264 663d 2268 7474 703a  xmlns:rdf="http:
-000000a0: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
-000000b0: 392f 3032 2f32 322d 7264 662d 7379 6e74  9/02/22-rdf-synt
-000000c0: 6178 2d6e 7323 220a 2020 2020 2020 2020  ax-ns#".        
-000000d0: 2078 6d6c 6e73 3a73 796e 3d22 6874 7470   xmlns:syn="http
-000000e0: 3a2f 2f70 7572 6c2e 6f72 672f 7273 732f  ://purl.org/rss/
-000000f0: 312e 302f 6d6f 6475 6c65 732f 7379 6e64  1.0/modules/synd
-00000100: 6963 6174 696f 6e2f 220a 3e0a 0a0a 0a0a  ication/".>.....
-00000110: 0a0a 0a0a 2020 3c63 6861 6e6e 656c 2072  ....  <channel r
-00000120: 6466 3a61 626f 7574 3d22 6874 7470 3a2f  df:about="http:/
-00000130: 2f6c 6f63 616c 686f 7374 3a35 3534 3430  /localhost:55440
-00000140: 2f70 6c6f 6e65 2f63 6f6c 6c65 6374 696f  /plone/collectio
-00000150: 6e2f 5253 5322 3e0a 2020 2020 3c74 6974  n/RSS">.    <tit
-00000160: 6c65 3e43 6f6c 6c65 6374 696f 6e20 666f  le>Collection fo
-00000170: 7220 5253 533c 2f74 6974 6c65 3e0a 2020  r RSS</title>.  
-00000180: 2020 3c6c 696e 6b3e 6874 7470 3a2f 2f6c    <link>http://l
-00000190: 6f63 616c 686f 7374 3a35 3534 3430 2f70  ocalhost:55440/p
-000001a0: 6c6f 6e65 3c2f 6c69 6e6b 3e0a 0a20 2020  lone</link>..   
-000001b0: 203c 6465 7363 7269 7074 696f 6e3e 0a0a   <description>..
-000001c0: 0a0a 2020 2020 3c2f 6465 7363 7269 7074  ..    </descript
-000001d0: 696f 6e3e 0a0a 0a0a 0a20 2020 203c 7379  ion>.....    <sy
-000001e0: 6e3a 7570 6461 7465 5065 7269 6f64 3e64  n:updatePeriod>d
-000001f0: 6169 6c79 3c2f 7379 6e3a 7570 6461 7465  aily</syn:update
-00000200: 5065 7269 6f64 3e0a 2020 2020 3c73 796e  Period>.    <syn
-00000210: 3a75 7064 6174 6546 7265 7175 656e 6379  :updateFrequency
-00000220: 3e31 3c2f 7379 6e3a 7570 6461 7465 4672  >1</syn:updateFr
-00000230: 6571 7565 6e63 793e 0a20 2020 203c 7379  equency>.    <sy
-00000240: 6e3a 7570 6461 7465 4261 7365 3e32 3031  n:updateBase>201
-00000250: 312d 3039 2d32 3254 3130 3a32 333a 3537  1-09-22T10:23:57
-00000260: 5a3c 2f73 796e 3a75 7064 6174 6542 6173  Z</syn:updateBas
-00000270: 653e 0a0a 0a20 2020 203c 696d 6167 6520  e>...    <image 
-00000280: 7264 663a 7265 736f 7572 6365 3d22 6874  rdf:resource="ht
-00000290: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a35  tp://localhost:5
-000002a0: 3534 3430 2f70 6c6f 6e65 2f6c 6f67 6f2e  5440/plone/logo.
-000002b0: 706e 6722 202f 3e0a 0a20 2020 203c 6974  png" />..    <it
-000002c0: 656d 733e 0a20 2020 2020 203c 7264 663a  ems>.      <rdf:
-000002d0: 5365 713e 0a0a 2020 2020 2020 2020 3c72  Seq>..        <r
-000002e0: 6466 3a6c 6920 7264 663a 7265 736f 7572  df:li rdf:resour
-000002f0: 6365 3d22 6874 7470 3a2f 2f6c 6f63 616c  ce="http://local
-00000300: 686f 7374 3a35 3534 3430 2f70 6c6f 6e65  host:55440/plone
-00000310: 2f64 6f63 2d6f 6e65 2220 2f3e 0a0a 0a20  /doc-one" />... 
-00000320: 2020 2020 2020 203c 7264 663a 6c69 2072         <rdf:li r
-00000330: 6466 3a72 6573 6f75 7263 653d 2268 7474  df:resource="htt
-00000340: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3535  p://localhost:55
-00000350: 3434 302f 706c 6f6e 652f 646f 632d 7477  440/plone/doc-tw
-00000360: 6f22 202f 3e0a 0a0a 2020 2020 2020 2020  o" />...        
-00000370: 3c72 6466 3a6c 6920 7264 663a 7265 736f  <rdf:li rdf:reso
-00000380: 7572 6365 3d22 6874 7470 3a2f 2f6c 6f63  urce="http://loc
-00000390: 616c 686f 7374 3a35 3534 3430 2f70 6c6f  alhost:55440/plo
-000003a0: 6e65 2f64 6f63 2d74 6872 6565 2220 2f3e  ne/doc-three" />
-000003b0: 0a0a 0a20 2020 2020 2020 203c 7264 663a  ...        <rdf:
-000003c0: 6c69 2072 6466 3a72 6573 6f75 7263 653d  li rdf:resource=
-000003d0: 2268 7474 703a 2f2f 6c6f 6361 6c68 6f73  "http://localhos
-000003e0: 743a 3535 3434 302f 706c 6f6e 652f 612d  t:55440/plone/a-
-000003f0: 7369 6d70 6c65 2d70 6167 6522 202f 3e0a  simple-page" />.
-00000400: 0a20 2020 2020 203c 2f72 6466 3a53 6571  .      </rdf:Seq
-00000410: 3e0a 2020 2020 3c2f 6974 656d 733e 0a0a  >.    </items>..
-00000420: 2020 3c2f 6368 616e 6e65 6c3e 0a0a 0a20    </channel>... 
-00000430: 203c 6974 656d 2072 6466 3a61 626f 7574   <item rdf:about
-00000440: 3d22 6874 7470 3a2f 2f6c 6f63 616c 686f  ="http://localho
-00000450: 7374 3a35 3534 3430 2f70 6c6f 6e65 2f64  st:55440/plone/d
-00000460: 6f63 2d6f 6e65 223e 0a20 2020 203c 7469  oc-one">.    <ti
-00000470: 746c 653e 446f 6320 6f6e 653c 2f74 6974  tle>Doc one</tit
-00000480: 6c65 3e0a 2020 2020 3c6c 696e 6b3e 6874  le>.    <link>ht
-00000490: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a35  tp://localhost:5
-000004a0: 3534 3430 2f70 6c6f 6e65 2f64 6f63 2d6f  5440/plone/doc-o
-000004b0: 6e65 3c2f 6c69 6e6b 3e0a 2020 2020 3c64  ne</link>.    <d
-000004c0: 6573 6372 6970 7469 6f6e 202f 3e0a 2020  escription />.  
-000004d0: 2020 3c63 6f6e 7465 6e74 3a65 6e63 6f64    <content:encod
-000004e0: 6564 2078 6d6c 6e73 3a63 6f6e 7465 6e74  ed xmlns:content
-000004f0: 3d22 6874 7470 3a2f 2f70 7572 6c2e 6f72  ="http://purl.or
-00000500: 672f 7273 732f 312e 302f 6d6f 6475 6c65  g/rss/1.0/module
-00000510: 732f 636f 6e74 656e 742f 223e 0a20 2020  s/content/">.   
-00000520: 203c 2f63 6f6e 7465 6e74 3a65 6e63 6f64   </content:encod
-00000530: 6564 3e0a 2020 2020 3c64 633a 7075 626c  ed>.    <dc:publ
-00000540: 6973 6865 723e 4e6f 2070 7562 6c69 7368  isher>No publish
-00000550: 6572 3c2f 6463 3a70 7562 6c69 7368 6572  er</dc:publisher
-00000560: 3e0a 2020 2020 3c64 633a 6372 6561 746f  >.    <dc:creato
-00000570: 723e 7465 7374 5f75 7365 725f 315f 3c2f  r>test_user_1_</
-00000580: 6463 3a63 7265 6174 6f72 3e0a 2020 2020  dc:creator>.    
-00000590: 3c64 633a 7269 6768 7473 202f 3e0a 2020  <dc:rights />.  
-000005a0: 2020 3c64 633a 6461 7465 3e32 3031 312d    <dc:date>2011-
-000005b0: 3039 2d32 3254 3130 3a32 343a 3230 5a3c  09-22T10:24:20Z<
-000005c0: 2f64 633a 6461 7465 3e0a 2020 2020 3c64  /dc:date>.    <d
-000005d0: 633a 7479 7065 3e50 6167 653c 2f64 633a  c:type>Page</dc:
-000005e0: 7479 7065 3e0a 2020 3c2f 6974 656d 3e0a  type>.  </item>.
-000005f0: 0a0a 2020 3c69 7465 6d20 7264 663a 6162  ..  <item rdf:ab
-00000600: 6f75 743d 2268 7474 703a 2f2f 6c6f 6361  out="http://loca
-00000610: 6c68 6f73 743a 3535 3434 302f 706c 6f6e  lhost:55440/plon
-00000620: 652f 646f 632d 7477 6f22 3e0a 2020 2020  e/doc-two">.    
-00000630: 3c74 6974 6c65 3e44 6f63 2074 776f 3c2f  <title>Doc two</
-00000640: 7469 746c 653e 0a20 2020 203c 6c69 6e6b  title>.    <link
-00000650: 3e68 7474 703a 2f2f 6c6f 6361 6c68 6f73  >http://localhos
-00000660: 743a 3535 3434 302f 706c 6f6e 652f 646f  t:55440/plone/do
-00000670: 632d 7477 6f3c 2f6c 696e 6b3e 0a20 2020  c-two</link>.   
-00000680: 203c 6465 7363 7269 7074 696f 6e20 2f3e   <description />
-00000690: 0a20 2020 203c 636f 6e74 656e 743a 656e  .    <content:en
-000006a0: 636f 6465 6420 786d 6c6e 733a 636f 6e74  coded xmlns:cont
-000006b0: 656e 743d 2268 7474 703a 2f2f 7075 726c  ent="http://purl
-000006c0: 2e6f 7267 2f72 7373 2f31 2e30 2f6d 6f64  .org/rss/1.0/mod
-000006d0: 756c 6573 2f63 6f6e 7465 6e74 2f22 3e0a  ules/content/">.
-000006e0: 2020 2020 3c2f 636f 6e74 656e 743a 656e      </content:en
-000006f0: 636f 6465 643e 0a20 2020 203c 6463 3a70  coded>.    <dc:p
-00000700: 7562 6c69 7368 6572 3e4e 6f20 7075 626c  ublisher>No publ
-00000710: 6973 6865 723c 2f64 633a 7075 626c 6973  isher</dc:publis
-00000720: 6865 723e 0a20 2020 203c 6463 3a63 7265  her>.    <dc:cre
-00000730: 6174 6f72 3e74 6573 745f 7573 6572 5f31  ator>test_user_1
-00000740: 5f3c 2f64 633a 6372 6561 746f 723e 0a20  _</dc:creator>. 
-00000750: 2020 203c 6463 3a72 6967 6874 7320 2f3e     <dc:rights />
-00000760: 0a20 2020 203c 6463 3a64 6174 653e 3230  .    <dc:date>20
-00000770: 3131 2d30 392d 3232 5431 303a 3234 3a32  11-09-22T10:24:2
-00000780: 305a 3c2f 6463 3a64 6174 653e 0a20 2020  0Z</dc:date>.   
-00000790: 203c 6463 3a74 7970 653e 5061 6765 3c2f   <dc:type>Page</
-000007a0: 6463 3a74 7970 653e 0a20 203c 2f69 7465  dc:type>.  </ite
-000007b0: 6d3e 0a0a 0a20 203c 6974 656d 2072 6466  m>...  <item rdf
-000007c0: 3a61 626f 7574 3d22 6874 7470 3a2f 2f6c  :about="http://l
-000007d0: 6f63 616c 686f 7374 3a35 3534 3430 2f70  ocalhost:55440/p
-000007e0: 6c6f 6e65 2f64 6f63 2d74 6872 6565 223e  lone/doc-three">
-000007f0: 0a20 2020 203c 7469 746c 653e 446f 6320  .    <title>Doc 
-00000800: 7468 7265 653c 2f74 6974 6c65 3e0a 2020  three</title>.  
-00000810: 2020 3c6c 696e 6b3e 6874 7470 3a2f 2f6c    <link>http://l
-00000820: 6f63 616c 686f 7374 3a35 3534 3430 2f70  ocalhost:55440/p
-00000830: 6c6f 6e65 2f64 6f63 2d74 6872 6565 3c2f  lone/doc-three</
-00000840: 6c69 6e6b 3e0a 2020 2020 3c64 6573 6372  link>.    <descr
-00000850: 6970 7469 6f6e 202f 3e0a 2020 2020 3c63  iption />.    <c
-00000860: 6f6e 7465 6e74 3a65 6e63 6f64 6564 2078  ontent:encoded x
-00000870: 6d6c 6e73 3a63 6f6e 7465 6e74 3d22 6874  mlns:content="ht
-00000880: 7470 3a2f 2f70 7572 6c2e 6f72 672f 7273  tp://purl.org/rs
-00000890: 732f 312e 302f 6d6f 6475 6c65 732f 636f  s/1.0/modules/co
-000008a0: 6e74 656e 742f 223e 0a20 2020 203c 2f63  ntent/">.    </c
-000008b0: 6f6e 7465 6e74 3a65 6e63 6f64 6564 3e0a  ontent:encoded>.
-000008c0: 2020 2020 3c64 633a 7075 626c 6973 6865      <dc:publishe
-000008d0: 723e 4e6f 2070 7562 6c69 7368 6572 3c2f  r>No publisher</
-000008e0: 6463 3a70 7562 6c69 7368 6572 3e0a 2020  dc:publisher>.  
-000008f0: 2020 3c64 633a 6372 6561 746f 723e 7465    <dc:creator>te
-00000900: 7374 5f75 7365 725f 315f 3c2f 6463 3a63  st_user_1_</dc:c
-00000910: 7265 6174 6f72 3e0a 2020 2020 3c64 633a  reator>.    <dc:
-00000920: 7269 6768 7473 202f 3e0a 2020 2020 3c64  rights />.    <d
-00000930: 633a 6461 7465 3e32 3031 312d 3039 2d32  c:date>2011-09-2
-00000940: 3254 3130 3a32 343a 3230 5a3c 2f64 633a  2T10:24:20Z</dc:
-00000950: 6461 7465 3e0a 2020 2020 3c64 633a 7479  date>.    <dc:ty
-00000960: 7065 3e50 6167 653c 2f64 633a 7479 7065  pe>Page</dc:type
-00000970: 3e0a 2020 3c2f 6974 656d 3e0a 0a0a 2020  >.  </item>...  
-00000980: 3c69 7465 6d20 7264 663a 6162 6f75 743d  <item rdf:about=
-00000990: 2268 7474 703a 2f2f 6c6f 6361 6c68 6f73  "http://localhos
-000009a0: 743a 3535 3434 302f 706c 6f6e 652f 612d  t:55440/plone/a-
-000009b0: 7369 6d70 6c65 2d70 6167 6522 3e0a 2020  simple-page">.  
-000009c0: 2020 3c74 6974 6c65 3e41 2073 696d 706c    <title>A simpl
-000009d0: 6520 7061 6765 3c2f 7469 746c 653e 0a20  e page</title>. 
-000009e0: 2020 203c 6c69 6e6b 3e68 7474 703a 2f2f     <link>http://
-000009f0: 6c6f 6361 6c68 6f73 743a 3535 3434 302f  localhost:55440/
-00000a00: 706c 6f6e 652f 612d 7369 6d70 6c65 2d70  plone/a-simple-p
-00000a10: 6167 653c 2f6c 696e 6b3e 0a20 2020 203c  age</link>.    <
-00000a20: 6465 7363 7269 7074 696f 6e3e 4120 6465  description>A de
-00000a30: 7363 7269 7074 696f 6e3c 2f64 6573 6372  scription</descr
-00000a40: 6970 7469 6f6e 3e0a 2020 2020 3c63 6f6e  iption>.    <con
-00000a50: 7465 6e74 3a65 6e63 6f64 6564 2078 6d6c  tent:encoded xml
-00000a60: 6e73 3a63 6f6e 7465 6e74 3d22 6874 7470  ns:content="http
-00000a70: 3a2f 2f70 7572 6c2e 6f72 672f 7273 732f  ://purl.org/rss/
-00000a80: 312e 302f 6d6f 6475 6c65 732f 636f 6e74  1.0/modules/cont
-00000a90: 656e 742f 223e 0a20 2020 203c 2f63 6f6e  ent/">.    </con
-00000aa0: 7465 6e74 3a65 6e63 6f64 6564 3e0a 2020  tent:encoded>.  
-00000ab0: 2020 3c64 633a 7075 626c 6973 6865 723e    <dc:publisher>
-00000ac0: 4e6f 2070 7562 6c69 7368 6572 3c2f 6463  No publisher</dc
-00000ad0: 3a70 7562 6c69 7368 6572 3e0a 2020 2020  :publisher>.    
-00000ae0: 3c64 633a 6372 6561 746f 723e 7465 7374  <dc:creator>test
-00000af0: 5f75 7365 725f 315f 3c2f 6463 3a63 7265  _user_1_</dc:cre
-00000b00: 6174 6f72 3e0a 2020 2020 3c64 633a 7269  ator>.    <dc:ri
-00000b10: 6768 7473 202f 3e0a 2020 2020 3c64 633a  ghts />.    <dc:
-00000b20: 6461 7465 3e32 3031 312d 3039 2d32 3254  date>2011-09-22T
-00000b30: 3130 3a32 343a 3137 5a3c 2f64 633a 6461  10:24:17Z</dc:da
-00000b40: 7465 3e0a 2020 2020 3c64 633a 7479 7065  te>.    <dc:type
-00000b50: 3e50 6167 653c 2f64 633a 7479 7065 3e0a  >Page</dc:type>.
-00000b60: 2020 3c2f 6974 656d 3e0a 0a0a 0a0a 0a3c    </item>......<
-00000b70: 2f72 6466 3a52 4446 3e0a                 /rdf:RDF>.
+00000020: 662d 3822 3f3e 0a3c 7264 663a 5244 4620  f-8"?>.<rdf:RDF 
+00000030: 786d 6c6e 733d 2268 7474 703a 2f2f 7075  xmlns="http://pu
+00000040: 726c 2e6f 7267 2f72 7373 2f31 2e30 2f22  rl.org/rss/1.0/"
+00000050: 0a20 2020 2020 2020 2020 786d 6c6e 733a  .         xmlns:
+00000060: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
+00000070: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
+00000080: 312e 312f 220a 2020 2020 2020 2020 2078  1.1/".         x
+00000090: 6d6c 6e73 3a72 6466 3d22 6874 7470 3a2f  mlns:rdf="http:/
+000000a0: 2f77 7777 2e77 332e 6f72 672f 3139 3939  /www.w3.org/1999
+000000b0: 2f30 322f 3232 2d72 6466 2d73 796e 7461  /02/22-rdf-synta
+000000c0: 782d 6e73 2322 0a20 2020 2020 2020 2020  x-ns#".         
+000000d0: 786d 6c6e 733a 7379 6e3d 2268 7474 703a  xmlns:syn="http:
+000000e0: 2f2f 7075 726c 2e6f 7267 2f72 7373 2f31  //purl.org/rss/1
+000000f0: 2e30 2f6d 6f64 756c 6573 2f73 796e 6469  .0/modules/syndi
+00000100: 6361 7469 6f6e 2f22 0a3e 0a0a 0a0a 0a0a  cation/".>......
+00000110: 0a0a 0a20 203c 6368 616e 6e65 6c20 7264  ...  <channel rd
+00000120: 663a 6162 6f75 743d 2268 7474 703a 2f2f  f:about="http://
+00000130: 6c6f 6361 6c68 6f73 743a 3535 3434 302f  localhost:55440/
+00000140: 706c 6f6e 652f 636f 6c6c 6563 7469 6f6e  plone/collection
+00000150: 2f52 5353 223e 0a20 2020 203c 7469 746c  /RSS">.    <titl
+00000160: 653e 436f 6c6c 6563 7469 6f6e 2066 6f72  e>Collection for
+00000170: 2052 5353 3c2f 7469 746c 653e 0a20 2020   RSS</title>.   
+00000180: 203c 6c69 6e6b 3e68 7474 703a 2f2f 6c6f   <link>http://lo
+00000190: 6361 6c68 6f73 743a 3535 3434 302f 706c  calhost:55440/pl
+000001a0: 6f6e 653c 2f6c 696e 6b3e 0a0a 2020 2020  one</link>..    
+000001b0: 3c64 6573 6372 6970 7469 6f6e 3e0a 0a0a  <description>...
+000001c0: 0a20 2020 203c 2f64 6573 6372 6970 7469  .    </descripti
+000001d0: 6f6e 3e0a 0a0a 0a0a 2020 2020 3c73 796e  on>.....    <syn
+000001e0: 3a75 7064 6174 6550 6572 696f 643e 6461  :updatePeriod>da
+000001f0: 696c 793c 2f73 796e 3a75 7064 6174 6550  ily</syn:updateP
+00000200: 6572 696f 643e 0a20 2020 203c 7379 6e3a  eriod>.    <syn:
+00000210: 7570 6461 7465 4672 6571 7565 6e63 793e  updateFrequency>
+00000220: 313c 2f73 796e 3a75 7064 6174 6546 7265  1</syn:updateFre
+00000230: 7175 656e 6379 3e0a 2020 2020 3c73 796e  quency>.    <syn
+00000240: 3a75 7064 6174 6542 6173 653e 3230 3131  :updateBase>2011
+00000250: 2d30 392d 3232 5431 303a 3233 3a35 375a  -09-22T10:23:57Z
+00000260: 3c2f 7379 6e3a 7570 6461 7465 4261 7365  </syn:updateBase
+00000270: 3e0a 0a0a 2020 2020 3c69 6d61 6765 2072  >...    <image r
+00000280: 6466 3a72 6573 6f75 7263 653d 2268 7474  df:resource="htt
+00000290: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3535  p://localhost:55
+000002a0: 3434 302f 706c 6f6e 652f 6c6f 676f 2e70  440/plone/logo.p
+000002b0: 6e67 2220 2f3e 0a0a 2020 2020 3c69 7465  ng" />..    <ite
+000002c0: 6d73 3e0a 2020 2020 2020 3c72 6466 3a53  ms>.      <rdf:S
+000002d0: 6571 3e0a 0a20 2020 2020 2020 203c 7264  eq>..        <rd
+000002e0: 663a 6c69 2072 6466 3a72 6573 6f75 7263  f:li rdf:resourc
+000002f0: 653d 2268 7474 703a 2f2f 6c6f 6361 6c68  e="http://localh
+00000300: 6f73 743a 3535 3434 302f 706c 6f6e 652f  ost:55440/plone/
+00000310: 646f 632d 6f6e 6522 202f 3e0a 0a0a 2020  doc-one" />...  
+00000320: 2020 2020 2020 3c72 6466 3a6c 6920 7264        <rdf:li rd
+00000330: 663a 7265 736f 7572 6365 3d22 6874 7470  f:resource="http
+00000340: 3a2f 2f6c 6f63 616c 686f 7374 3a35 3534  ://localhost:554
+00000350: 3430 2f70 6c6f 6e65 2f64 6f63 2d74 776f  40/plone/doc-two
+00000360: 2220 2f3e 0a0a 0a20 2020 2020 2020 203c  " />...        <
+00000370: 7264 663a 6c69 2072 6466 3a72 6573 6f75  rdf:li rdf:resou
+00000380: 7263 653d 2268 7474 703a 2f2f 6c6f 6361  rce="http://loca
+00000390: 6c68 6f73 743a 3535 3434 302f 706c 6f6e  lhost:55440/plon
+000003a0: 652f 646f 632d 7468 7265 6522 202f 3e0a  e/doc-three" />.
+000003b0: 0a0a 2020 2020 2020 2020 3c72 6466 3a6c  ..        <rdf:l
+000003c0: 6920 7264 663a 7265 736f 7572 6365 3d22  i rdf:resource="
+000003d0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+000003e0: 3a35 3534 3430 2f70 6c6f 6e65 2f61 2d73  :55440/plone/a-s
+000003f0: 696d 706c 652d 7061 6765 2220 2f3e 0a0a  imple-page" />..
+00000400: 2020 2020 2020 3c2f 7264 663a 5365 713e        </rdf:Seq>
+00000410: 0a20 2020 203c 2f69 7465 6d73 3e0a 0a20  .    </items>.. 
+00000420: 203c 2f63 6861 6e6e 656c 3e0a 0a0a 2020   </channel>...  
+00000430: 3c69 7465 6d20 7264 663a 6162 6f75 743d  <item rdf:about=
+00000440: 2268 7474 703a 2f2f 6c6f 6361 6c68 6f73  "http://localhos
+00000450: 743a 3535 3434 302f 706c 6f6e 652f 646f  t:55440/plone/do
+00000460: 632d 6f6e 6522 3e0a 2020 2020 3c74 6974  c-one">.    <tit
+00000470: 6c65 3e44 6f63 206f 6e65 3c2f 7469 746c  le>Doc one</titl
+00000480: 653e 0a20 2020 203c 6c69 6e6b 3e68 7474  e>.    <link>htt
+00000490: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3535  p://localhost:55
+000004a0: 3434 302f 706c 6f6e 652f 646f 632d 6f6e  440/plone/doc-on
+000004b0: 653c 2f6c 696e 6b3e 0a20 2020 203c 6465  e</link>.    <de
+000004c0: 7363 7269 7074 696f 6e20 2f3e 0a20 2020  scription />.   
+000004d0: 203c 636f 6e74 656e 743a 656e 636f 6465   <content:encode
+000004e0: 6420 786d 6c6e 733a 636f 6e74 656e 743d  d xmlns:content=
+000004f0: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
+00000500: 2f72 7373 2f31 2e30 2f6d 6f64 756c 6573  /rss/1.0/modules
+00000510: 2f63 6f6e 7465 6e74 2f22 3e0a 3c2f 636f  /content/">.</co
+00000520: 6e74 656e 743a 656e 636f 6465 643e 0a20  ntent:encoded>. 
+00000530: 2020 203c 6463 3a70 7562 6c69 7368 6572     <dc:publisher
+00000540: 3e4e 6f20 7075 626c 6973 6865 723c 2f64  >No publisher</d
+00000550: 633a 7075 626c 6973 6865 723e 0a20 2020  c:publisher>.   
+00000560: 203c 6463 3a63 7265 6174 6f72 3e74 6573   <dc:creator>tes
+00000570: 745f 7573 6572 5f31 5f3c 2f64 633a 6372  t_user_1_</dc:cr
+00000580: 6561 746f 723e 0a20 2020 203c 6463 3a72  eator>.    <dc:r
+00000590: 6967 6874 7320 2f3e 0a20 2020 203c 6463  ights />.    <dc
+000005a0: 3a64 6174 653e 3230 3131 2d30 392d 3232  :date>2011-09-22
+000005b0: 5431 303a 3234 3a32 305a 3c2f 6463 3a64  T10:24:20Z</dc:d
+000005c0: 6174 653e 0a20 2020 203c 6463 3a74 7970  ate>.    <dc:typ
+000005d0: 653e 5061 6765 3c2f 6463 3a74 7970 653e  e>Page</dc:type>
+000005e0: 0a20 203c 2f69 7465 6d3e 0a0a 0a20 203c  .  </item>...  <
+000005f0: 6974 656d 2072 6466 3a61 626f 7574 3d22  item rdf:about="
+00000600: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00000610: 3a35 3534 3430 2f70 6c6f 6e65 2f64 6f63  :55440/plone/doc
+00000620: 2d74 776f 223e 0a20 2020 203c 7469 746c  -two">.    <titl
+00000630: 653e 446f 6320 7477 6f3c 2f74 6974 6c65  e>Doc two</title
+00000640: 3e0a 2020 2020 3c6c 696e 6b3e 6874 7470  >.    <link>http
+00000650: 3a2f 2f6c 6f63 616c 686f 7374 3a35 3534  ://localhost:554
+00000660: 3430 2f70 6c6f 6e65 2f64 6f63 2d74 776f  40/plone/doc-two
+00000670: 3c2f 6c69 6e6b 3e0a 2020 2020 3c64 6573  </link>.    <des
+00000680: 6372 6970 7469 6f6e 202f 3e0a 2020 2020  cription />.    
+00000690: 3c63 6f6e 7465 6e74 3a65 6e63 6f64 6564  <content:encoded
+000006a0: 2078 6d6c 6e73 3a63 6f6e 7465 6e74 3d22   xmlns:content="
+000006b0: 6874 7470 3a2f 2f70 7572 6c2e 6f72 672f  http://purl.org/
+000006c0: 7273 732f 312e 302f 6d6f 6475 6c65 732f  rss/1.0/modules/
+000006d0: 636f 6e74 656e 742f 223e 0a3c 2f63 6f6e  content/">.</con
+000006e0: 7465 6e74 3a65 6e63 6f64 6564 3e0a 2020  tent:encoded>.  
+000006f0: 2020 3c64 633a 7075 626c 6973 6865 723e    <dc:publisher>
+00000700: 4e6f 2070 7562 6c69 7368 6572 3c2f 6463  No publisher</dc
+00000710: 3a70 7562 6c69 7368 6572 3e0a 2020 2020  :publisher>.    
+00000720: 3c64 633a 6372 6561 746f 723e 7465 7374  <dc:creator>test
+00000730: 5f75 7365 725f 315f 3c2f 6463 3a63 7265  _user_1_</dc:cre
+00000740: 6174 6f72 3e0a 2020 2020 3c64 633a 7269  ator>.    <dc:ri
+00000750: 6768 7473 202f 3e0a 2020 2020 3c64 633a  ghts />.    <dc:
+00000760: 6461 7465 3e32 3031 312d 3039 2d32 3254  date>2011-09-22T
+00000770: 3130 3a32 343a 3230 5a3c 2f64 633a 6461  10:24:20Z</dc:da
+00000780: 7465 3e0a 2020 2020 3c64 633a 7479 7065  te>.    <dc:type
+00000790: 3e50 6167 653c 2f64 633a 7479 7065 3e0a  >Page</dc:type>.
+000007a0: 2020 3c2f 6974 656d 3e0a 0a0a 2020 3c69    </item>...  <i
+000007b0: 7465 6d20 7264 663a 6162 6f75 743d 2268  tem rdf:about="h
+000007c0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+000007d0: 3535 3434 302f 706c 6f6e 652f 646f 632d  55440/plone/doc-
+000007e0: 7468 7265 6522 3e0a 2020 2020 3c74 6974  three">.    <tit
+000007f0: 6c65 3e44 6f63 2074 6872 6565 3c2f 7469  le>Doc three</ti
+00000800: 746c 653e 0a20 2020 203c 6c69 6e6b 3e68  tle>.    <link>h
+00000810: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00000820: 3535 3434 302f 706c 6f6e 652f 646f 632d  55440/plone/doc-
+00000830: 7468 7265 653c 2f6c 696e 6b3e 0a20 2020  three</link>.   
+00000840: 203c 6465 7363 7269 7074 696f 6e20 2f3e   <description />
+00000850: 0a20 2020 203c 636f 6e74 656e 743a 656e  .    <content:en
+00000860: 636f 6465 6420 786d 6c6e 733a 636f 6e74  coded xmlns:cont
+00000870: 656e 743d 2268 7474 703a 2f2f 7075 726c  ent="http://purl
+00000880: 2e6f 7267 2f72 7373 2f31 2e30 2f6d 6f64  .org/rss/1.0/mod
+00000890: 756c 6573 2f63 6f6e 7465 6e74 2f22 3e0a  ules/content/">.
+000008a0: 3c2f 636f 6e74 656e 743a 656e 636f 6465  </content:encode
+000008b0: 643e 0a20 2020 203c 6463 3a70 7562 6c69  d>.    <dc:publi
+000008c0: 7368 6572 3e4e 6f20 7075 626c 6973 6865  sher>No publishe
+000008d0: 723c 2f64 633a 7075 626c 6973 6865 723e  r</dc:publisher>
+000008e0: 0a20 2020 203c 6463 3a63 7265 6174 6f72  .    <dc:creator
+000008f0: 3e74 6573 745f 7573 6572 5f31 5f3c 2f64  >test_user_1_</d
+00000900: 633a 6372 6561 746f 723e 0a20 2020 203c  c:creator>.    <
+00000910: 6463 3a72 6967 6874 7320 2f3e 0a20 2020  dc:rights />.   
+00000920: 203c 6463 3a64 6174 653e 3230 3131 2d30   <dc:date>2011-0
+00000930: 392d 3232 5431 303a 3234 3a32 305a 3c2f  9-22T10:24:20Z</
+00000940: 6463 3a64 6174 653e 0a20 2020 203c 6463  dc:date>.    <dc
+00000950: 3a74 7970 653e 5061 6765 3c2f 6463 3a74  :type>Page</dc:t
+00000960: 7970 653e 0a20 203c 2f69 7465 6d3e 0a0a  ype>.  </item>..
+00000970: 0a20 203c 6974 656d 2072 6466 3a61 626f  .  <item rdf:abo
+00000980: 7574 3d22 6874 7470 3a2f 2f6c 6f63 616c  ut="http://local
+00000990: 686f 7374 3a35 3534 3430 2f70 6c6f 6e65  host:55440/plone
+000009a0: 2f61 2d73 696d 706c 652d 7061 6765 223e  /a-simple-page">
+000009b0: 0a20 2020 203c 7469 746c 653e 4120 7369  .    <title>A si
+000009c0: 6d70 6c65 2070 6167 653c 2f74 6974 6c65  mple page</title
+000009d0: 3e0a 2020 2020 3c6c 696e 6b3e 6874 7470  >.    <link>http
+000009e0: 3a2f 2f6c 6f63 616c 686f 7374 3a35 3534  ://localhost:554
+000009f0: 3430 2f70 6c6f 6e65 2f61 2d73 696d 706c  40/plone/a-simpl
+00000a00: 652d 7061 6765 3c2f 6c69 6e6b 3e0a 2020  e-page</link>.  
+00000a10: 2020 3c64 6573 6372 6970 7469 6f6e 3e41    <description>A
+00000a20: 2064 6573 6372 6970 7469 6f6e 3c2f 6465   description</de
+00000a30: 7363 7269 7074 696f 6e3e 0a20 2020 203c  scription>.    <
+00000a40: 636f 6e74 656e 743a 656e 636f 6465 6420  content:encoded 
+00000a50: 786d 6c6e 733a 636f 6e74 656e 743d 2268  xmlns:content="h
+00000a60: 7474 703a 2f2f 7075 726c 2e6f 7267 2f72  ttp://purl.org/r
+00000a70: 7373 2f31 2e30 2f6d 6f64 756c 6573 2f63  ss/1.0/modules/c
+00000a80: 6f6e 7465 6e74 2f22 3e0a 3c2f 636f 6e74  ontent/">.</cont
+00000a90: 656e 743a 656e 636f 6465 643e 0a20 2020  ent:encoded>.   
+00000aa0: 203c 6463 3a70 7562 6c69 7368 6572 3e4e   <dc:publisher>N
+00000ab0: 6f20 7075 626c 6973 6865 723c 2f64 633a  o publisher</dc:
+00000ac0: 7075 626c 6973 6865 723e 0a20 2020 203c  publisher>.    <
+00000ad0: 6463 3a63 7265 6174 6f72 3e74 6573 745f  dc:creator>test_
+00000ae0: 7573 6572 5f31 5f3c 2f64 633a 6372 6561  user_1_</dc:crea
+00000af0: 746f 723e 0a20 2020 203c 6463 3a72 6967  tor>.    <dc:rig
+00000b00: 6874 7320 2f3e 0a20 2020 203c 6463 3a64  hts />.    <dc:d
+00000b10: 6174 653e 3230 3131 2d30 392d 3232 5431  ate>2011-09-22T1
+00000b20: 303a 3234 3a31 375a 3c2f 6463 3a64 6174  0:24:17Z</dc:dat
+00000b30: 653e 0a20 2020 203c 6463 3a74 7970 653e  e>.    <dc:type>
+00000b40: 5061 6765 3c2f 6463 3a74 7970 653e 0a20  Page</dc:type>. 
+00000b50: 203c 2f69 7465 6d3e 0a0a 0a0a 0a0a 3c2f   </item>......</
+00000b60: 7264 663a 5244 463e 0a                   rdf:RDF>.
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/custom_existingcontent_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/funky_display.pt` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/funky_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_content.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_existing_content.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_existing_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_field.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_head.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_head.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_layout.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_media.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/tests/test_setup.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/upgrades.zcml` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/utils.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone/app/standardtiles/viewletmanager.py` & `plone.app.standardtiles-3.0.1/src/plone/app/standardtiles/viewletmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/PKG-INFO` & `plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: plone.app.standardtiles
-Version: 3.0.0b1
+Version: 3.0.1
 Summary: Tiles for plone.app.blocks page composition
 Home-page: https://github.com/plone/plone.app.standardtiles
 Author: Rob Gietema
 Author-email: rob@fourdigits.nl
 License: GPL
 Keywords: tiles content plone
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: attachment
 License-File: LICENSE.GPL
 License-File: LICENSE.txt
 
 Plone Standard Tiles
 ====================
@@ -57,14 +58,33 @@
 -------
 
 The project is licensed under the GPLv2.
 
 Changelog
 =========
 
+3.0.1 (2023-04-22)
+------------------
+
+- Fix broken CMFDynamicViewFTI import.
+  [thet]
+
+- Fix byline viewlet name
+  [frapell]
+
+
+3.0.0 (2022-12-05)
+------------------
+
+- Added linkintegrity for html and existingcontent tile.
+  Code is ported form version 2.5.0, and is only active when
+  plone.app.blocks version 6.0.2 or higher is used.
+  [petschki]
+
+
 3.0.0b1 (2022-06-24)
 --------------------
 
 - Fix ``isDefaultPage`` import which was moved to ``plone.base.defaultpage``
   [petschki]
 
 - Cleanup and fix ExistingContentTile in 5.2
@@ -493,9 +513,7 @@
   smaller than width columns
   [datakurre]
 
 1.0a1 (2015-05-25)
 ------------------
 
 - First alpha release.
-
-
```

### Comparing `plone.app.standardtiles-3.0.0b1/src/plone.app.standardtiles.egg-info/SOURCES.txt` & `plone.app.standardtiles-3.0.1/src/plone.app.standardtiles.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/plone/app/standardtiles/existingcontent.py
 src/plone/app/standardtiles/field.py
 src/plone/app/standardtiles/head.py
 src/plone/app/standardtiles/head.zcml
 src/plone/app/standardtiles/html.py
 src/plone/app/standardtiles/interfaces.py
 src/plone/app/standardtiles/layout.zcml
+src/plone/app/standardtiles/linkintegrity.py
 src/plone/app/standardtiles/media.zcml
 src/plone/app/standardtiles/metadata.py
 src/plone/app/standardtiles/navigation.py
 src/plone/app/standardtiles/rawembed.py
 src/plone/app/standardtiles/rss.py
 src/plone/app/standardtiles/setuphandlers.py
 src/plone/app/standardtiles/sitemap.py
```

