# Comparing `tmp/allianceauth_afat-2.9.6.tar.gz` & `tmp/allianceauth_afat-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_afat-2.9.6.tar", last modified: Fri Jul 29 20:09:51 2022, max compression
+gzip compressed data, was "allianceauth_afat-2.9.7.tar", last modified: Wed Aug 10 23:25:57 2022, max compression
```

## Comparing `allianceauth_afat-2.9.6.tar` & `allianceauth_afat-2.9.7.tar`

### file list

```diff
@@ -1,217 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9790 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8380 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.868670 allianceauth_afat-2.9.6/afat/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    72644 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/docs/images/add-fatlink.png
--rw-r--r--   0 runner    (1001) docker     (121)   133006 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/docs/images/afat-dashboard.png
--rw-r--r--   0 runner    (1001) docker     (121)    92809 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/docs/images/fatlink-list.png
--rw-r--r--   0 runner    (1001) docker     (121)    78316 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/docs/images/manually-close-esi-links.png
--rw-r--r--   0 runner    (1001) docker     (121)    96508 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/docs/images/ship-type-overview.png
--rw-r--r--   0 runner    (1001) docker     (121)    49911 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/docs/images/statistics-dashboard.png
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/helper/
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/helper/fatlinks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/helper/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     9078 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/helper/views_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    19878 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    33749 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    25462 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    25462 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    25415 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    25415 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    25455 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    25415 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    25088 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    38925 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    25455 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/management/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.872671 allianceauth_afat-2.9.6/afat/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/management/commands/afat_import_from_allianceauth_fat.py
--rw-r--r--   0 runner    (1001) docker     (121)    14351 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/management/commands/afat_import_from_imicusfat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/management/commands/afat_migrate_manual_fat_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0002_manualfat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0003_auto_20180911_0831.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0004_clickfatduration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0005_auto_20200816_2042.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0006_auto_20200820_2013.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0007_auto_20200826_1537.py
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0008_auto_20200912_1116.py
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0009_auto_20200925_2206.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0010_permissoins_update_20201002_1909.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0011_change_meta_options_on_manualafat_20201003_2222.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0012_manualafat_created_at.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0013_basic_module_access_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0014_auto_20201224_0930.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0015_afatlink_character.py
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0016_permissions_overhaul.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0017_remove_soft_deletion.py
--rw-r--r--   0 runner    (1001) docker     (121)     6395 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0018_auto_20210420_2016.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0019_add_several_indices.py
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0020_auto_20210617_1037.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/0021_alter_afatlink_fleet.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8975 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/static/afat/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/static/afat/css/
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/css/allianceauth-afat.css
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/css/allianceauth-afat.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/static/afat/javascript/
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-dashboard.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlink-details.js
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlink-details.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlist.js
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlist.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-logs.js
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-logs.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/allianceauth-afat.js
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/javascript/allianceauth-afat.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/static/afat/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/static/afat/libs/chartjs/
--rw-r--r--   0 runner    (1001) docker     (121)   159639 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/libs/chartjs/chart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/static/afat/libs/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/static/afat/libs/datatables/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/libs/datatables/plugins/datetime.js
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/static/afat/libs/datatables/plugins/datetime.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.864670 allianceauth_afat-2.9.6/afat/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/templates/afat/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/templates/afat/bundles/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/bundles/chartjs-js.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.876670 allianceauth_afat-2.9.6/afat/templates/afat/modals/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/modals/general.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/tabs/fatlinks.html
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/tabs/fats.html
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/tabs_navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/add/
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/add/clickable_link.html
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/add/esi_link.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/
--rw-r--r--   0 runner    (1001) docker     (121)     5019 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/fatlink_info.html
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/tabs/fats.html
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/tabs_navigation.html
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/fatlink_list_legend.html
--rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/open_esi_fleets.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/form/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/form/required_field_hint.html
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/menu.html
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/month_navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.868670 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html
--rw-r--r--   0 runner    (1001) docker     (121)     5703 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/tabs_navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/tabs/graphs.html
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/tabs/raw_data.html
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/tabs_navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/tabs/member.html
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/tabs_navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/tabs/
--rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/tabs/corps.html
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/tabs/mine.html
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/tabs_navigation.html
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/partials/year_navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.868670 allianceauth_afat-2.9.6/afat/templates/afat/view/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/view/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/dashboard/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/view/fatlinks/
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/fatlinks/fatlinks_overview.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/view/logs/
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/logs/logs_overview.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.880671 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_alliance.html
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_alliance_year_overview.html
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_character.html
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_corporation.html
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_corporation_year_overview.html
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_overview.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/afat/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templatetags/afat_versioned_static.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/templatetags/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/afat/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/afat/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/fixtures/allianceauth.json
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/fixtures/generate_fat_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/fixtures/load_allianceauth.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (121)    15157 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_views_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    11036 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_views_fatlinks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_views_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/tests/test_views_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5438 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/afat/views/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/views/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    32837 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/views/fatlinks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/views/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19351 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/afat/views/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9790 2022-07-29 20:09:51.000000 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6463 2022-07-29 20:09:51.000000 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 20:09:51.000000 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 20:09:51.000000 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-29 20:09:51.000000 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-29 20:09:51.000000 allianceauth_afat-2.9.6/allianceauth_afat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-29 20:09:35.000000 allianceauth_afat-2.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-07-29 20:09:51.884671 allianceauth_afat-2.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10611 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9298 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    72644 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/docs/images/add-fatlink.png
+-rw-r--r--   0 runner    (1001) docker     (121)   133006 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/docs/images/afat-dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (121)    92809 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/docs/images/fatlink-list.png
+-rw-r--r--   0 runner    (1001) docker     (121)    78316 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/docs/images/manually-close-esi-links.png
+-rw-r--r--   0 runner    (1001) docker     (121)    96508 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/docs/images/ship-type-overview.png
+-rw-r--r--   0 runner    (1001) docker     (121)    49911 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/docs/images/statistics-dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/helper/
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/helper/fatlinks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/helper/time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9078 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/helper/views_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/de/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)    19878 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    33749 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/en/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    25462 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/es/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    25462 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/fr_FR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)    25415 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/it_IT/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)    25415 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ja/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)    25455 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ko_KR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)    25415 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.490828 allianceauth_afat-2.9.7/afat/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ru/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)    25088 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    38925 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/zh_Hans/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    25455 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/management/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/management/commands/afat_import_from_allianceauth_fat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14351 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/management/commands/afat_import_from_imicusfat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/management/commands/afat_migrate_manual_fat_log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     2740 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0002_manualfat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0003_auto_20180911_0831.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0004_clickfatduration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0005_auto_20200816_2042.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0006_auto_20200820_2013.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0007_auto_20200826_1537.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0008_auto_20200912_1116.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0009_auto_20200925_2206.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0010_permissoins_update_20201002_1909.py
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0011_change_meta_options_on_manualafat_20201003_2222.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0012_manualafat_created_at.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0013_basic_module_access_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0014_auto_20201224_0930.py
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0015_afatlink_character.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0016_permissions_overhaul.py
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0017_remove_soft_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6395 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0018_auto_20210420_2016.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0019_add_several_indices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0020_auto_20210617_1037.py
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/0021_alter_afatlink_fleet.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8975 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/static/afat/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/static/afat/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/css/afat.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/css/afat.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/static/afat/javascript/
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-dashboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4995 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlink-details.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlink-details.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlist.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlist.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-logs.js
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-logs.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/javascript/afat.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/static/afat/libs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/static/afat/libs/Chart.js/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/static/afat/libs/Chart.js/2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (121)   159639 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/static/afat/libs/Chart.js/2.7.2/chart.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.494828 allianceauth_afat-2.9.7/afat/templates/afat/
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/bundles/
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/afat-css.html
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/afat-dashboard-js.html
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/afat-fatlink-details-js.html
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/afat-fatlist-js.html
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/afat-js.html
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/afat-logs-js.html
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/bundles/chartjs-js.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/modals/
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/modals/general.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/tabs/fatlinks.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/tabs/fats.html
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/tabs_navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/add/
+-rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/add/clickable_link.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/add/esi_link.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/
+-rw-r--r--   0 runner    (1001) docker     (121)     5019 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/fatlink_info.html
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/tabs/fats.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html
+-rw-r--r--   0 runner    (1001) docker     (121)      422 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/tabs_navigation.html
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/fatlink_list_legend.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2883 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/open_esi_fleets.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/form/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/form/required_field_hint.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/menu.html
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/month_navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/tabs_navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/tabs/graphs.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/tabs/raw_data.html
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/tabs_navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/tabs/member.html
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/tabs_navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/tabs/
+-rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/tabs/corps.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/tabs/mine.html
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/tabs_navigation.html
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/partials/year_navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.486828 allianceauth_afat-2.9.7/afat/templates/afat/view/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/view/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/dashboard/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/view/fatlinks/
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3406 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/fatlinks/fatlinks_overview.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/view/logs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/logs/logs_overview.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_alliance.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_alliance_year_overview.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_character.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_corporation.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_corporation_year_overview.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_overview.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.498828 allianceauth_afat-2.9.7/afat/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templatetags/afat_versioned_static.py
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/templatetags/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/afat/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/afat/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/fixtures/allianceauth.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/fixtures/generate_fat_links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/fixtures/load_allianceauth.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15157 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_views_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11036 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_views_fatlinks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_views_logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/tests/test_views_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5438 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/afat/views/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/views/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32837 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/views/fatlinks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/views/logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19351 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/afat/views/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10611 2022-08-10 23:25:57.000000 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6965 2022-08-10 23:25:57.000000 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 23:25:57.000000 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 23:25:57.000000 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-10 23:25:57.000000 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-10 23:25:57.000000 allianceauth_afat-2.9.7/allianceauth_afat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-10 23:25:41.000000 allianceauth_afat-2.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-08-10 23:25:57.502828 allianceauth_afat-2.9.7/setup.cfg
```

### Comparing `allianceauth_afat-2.9.6/LICENSE` & `allianceauth_afat-2.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/PKG-INFO` & `allianceauth_afat-2.9.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: allianceauth_afat
-Version: 2.9.6
+Version: 2.9.7
 Summary: Another Fleet Activity Tracking tool for Alliance Auth
 Home-page: https://github.com/ppfeufer/allianceauth-afat
 Author: Peter Pfeufer
-Author-email: development@ppfeufer.de
+Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
-Maintainer-email: development@ppfeufer.de
+Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/allianceauth-afat/issues
 Project-URL: Changelog, https://github.com/ppfeufer/allianceauth-afat/blob/master/CHANGELOG.md
 Keywords: allianceauth,eveonline,theme,template
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Alliance Auth AFAT - Another Fleet Activity Tracker
 
 [![Version](https://img.shields.io/pypi/v/allianceauth-afat?label=release)](https://pypi.org/project/allianceauth-afat/)
 [![License](https://img.shields.io/badge/license-GPLv3-green)](https://pypi.org/project/allianceauth-afat/)
@@ -56,14 +54,15 @@
 - [Features and highlights](#features-and-highlights)
 - [Screenshots](#screenshots)
 - [Installation](#installation)
 - [Updating](#updating)
 - [Data Migration](#data-migration)
     - [From Alliance Auth native FAT](#import-from-native-fat)
     - [From ImicusFAT](#import-from-imicusfat)
+        - [Uninstall ImicusFAT](#uninstall-imicusfat)
 - [Settings](#settings)
 - [Permissions](#permissions)
 - [Changelog](#changelog)
 - [Credits](#credits)
 - [Contributing](#contributing)
 
 
@@ -196,14 +195,44 @@
 
 To import from the ImicusFAT module, simply run the following command:
 
 ```shell
 python myauth/manage.py afat_import_from_imicusfat
 ```
 
+#### Uninstall ImicusFAT
+
+Now that you've migrated, you can uninstal `ImicusFAT`.
+
+First, remove all Django migrations for `ImicusFAT` with:
+
+```shell
+python manage.py migrate imicusfat zero
+```
+
+This will remove all migrations for `ImicusFAT` including its DB tables.
+
+Should this command throw an error, a bit of manual labor is needed, but nothing you
+can't handle, I'm sure.
+
+```shell
+python manage.py migrate imicusfat zero --fake
+```
+
+And remove all DB tables beginning with `imicusfat_` from your DB manually afterwards.
+
+Now that the DB is cleaned up, time to remove te app.
+
+```shell
+pip uninstall allianceauth-imicusfat
+```
+
+Now remove `imicusfat` from your `INSTALLED_APPS` in your `local.py`, restart
+supervisor and ... Done!
+
 
 ## Settings
 
 To customize the module, the following settings are available.
 
 | Name                             | Description                                                     | Default Value           |
 |:---------------------------------|:----------------------------------------------------------------|:------------------------|
@@ -238,11 +267,14 @@
 
 Please make sure to read the [contribution guidelines](https://github.com/ppfeufer/allianceauth-afat/blob/master/CONTRIBUTING.md)
 (I promise, it's not much, just some basics)
 
 
 ## Credits
 
-AFAT is maintained by @ppfeufer is based on
-[ImicusFAT](https://gitlab.com/evictus.iou/allianceauth-imicusfat) maintained
-by @exiom with @Aproia and @ppfeufer (no longer) which is based on
+AFAT is maintained by @ppfeufer and is based on
+[ImicusFAT](https://gitlab.com/evictus.iou/allianceauth-imicusfat)
+by @exiom with @Aproia and @ppfeufer which is based on
 [allianceauth-bfat](https://gitlab.com/colcrunch/allianceauth-bfat) by @colcrunch
+
+Both of these modules are no longer maintained and are deprecated. Both modules will
+not run with the latest stable releases of Alliance Auth.
```

### Comparing `allianceauth_afat-2.9.6/README.md` & `allianceauth_afat-2.9.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 - [Features and highlights](#features-and-highlights)
 - [Screenshots](#screenshots)
 - [Installation](#installation)
 - [Updating](#updating)
 - [Data Migration](#data-migration)
     - [From Alliance Auth native FAT](#import-from-native-fat)
     - [From ImicusFAT](#import-from-imicusfat)
+        - [Uninstall ImicusFAT](#uninstall-imicusfat)
 - [Settings](#settings)
 - [Permissions](#permissions)
 - [Changelog](#changelog)
 - [Credits](#credits)
 - [Contributing](#contributing)
 
 
@@ -163,14 +164,44 @@
 
 To import from the ImicusFAT module, simply run the following command:
 
 ```shell
 python myauth/manage.py afat_import_from_imicusfat
 ```
 
+#### Uninstall ImicusFAT
+
+Now that you've migrated, you can uninstal `ImicusFAT`.
+
+First, remove all Django migrations for `ImicusFAT` with:
+
+```shell
+python manage.py migrate imicusfat zero
+```
+
+This will remove all migrations for `ImicusFAT` including its DB tables.
+
+Should this command throw an error, a bit of manual labor is needed, but nothing you
+can't handle, I'm sure.
+
+```shell
+python manage.py migrate imicusfat zero --fake
+```
+
+And remove all DB tables beginning with `imicusfat_` from your DB manually afterwards.
+
+Now that the DB is cleaned up, time to remove te app.
+
+```shell
+pip uninstall allianceauth-imicusfat
+```
+
+Now remove `imicusfat` from your `INSTALLED_APPS` in your `local.py`, restart
+supervisor and ... Done!
+
 
 ## Settings
 
 To customize the module, the following settings are available.
 
 | Name                             | Description                                                     | Default Value           |
 |:---------------------------------|:----------------------------------------------------------------|:------------------------|
@@ -205,11 +236,14 @@
 
 Please make sure to read the [contribution guidelines](https://github.com/ppfeufer/allianceauth-afat/blob/master/CONTRIBUTING.md)
 (I promise, it's not much, just some basics)
 
 
 ## Credits
 
-AFAT is maintained by @ppfeufer is based on
-[ImicusFAT](https://gitlab.com/evictus.iou/allianceauth-imicusfat) maintained
-by @exiom with @Aproia and @ppfeufer (no longer) which is based on
+AFAT is maintained by @ppfeufer and is based on
+[ImicusFAT](https://gitlab.com/evictus.iou/allianceauth-imicusfat)
+by @exiom with @Aproia and @ppfeufer which is based on
 [allianceauth-bfat](https://gitlab.com/colcrunch/allianceauth-bfat) by @colcrunch
+
+Both of these modules are no longer maintained and are deprecated. Both modules will
+not run with the latest stable releases of Alliance Auth.
```

### Comparing `allianceauth_afat-2.9.6/afat/admin.py` & `allianceauth_afat-2.9.7/afat/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/app_settings.py` & `allianceauth_afat-2.9.7/afat/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/auth_hooks.py` & `allianceauth_afat-2.9.7/afat/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/docs/images/add-fatlink.png` & `allianceauth_afat-2.9.7/afat/docs/images/add-fatlink.png`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/docs/images/afat-dashboard.png` & `allianceauth_afat-2.9.7/afat/docs/images/afat-dashboard.png`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/docs/images/fatlink-list.png` & `allianceauth_afat-2.9.7/afat/docs/images/fatlink-list.png`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/docs/images/manually-close-esi-links.png` & `allianceauth_afat-2.9.7/afat/docs/images/manually-close-esi-links.png`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/docs/images/ship-type-overview.png` & `allianceauth_afat-2.9.7/afat/docs/images/ship-type-overview.png`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/docs/images/statistics-dashboard.png` & `allianceauth_afat-2.9.7/afat/docs/images/statistics-dashboard.png`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/forms.py` & `allianceauth_afat-2.9.7/afat/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/helper/fatlinks.py` & `allianceauth_afat-2.9.7/afat/helper/fatlinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/helper/time.py` & `allianceauth_afat-2.9.7/afat/helper/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/helper/views_helper.py` & `allianceauth_afat-2.9.7/afat/helper/views_helper.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/de/LC_MESSAGES/django.mo` & `allianceauth_afat-2.9.7/afat/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/de/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/en/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/es/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/fr_FR/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/it_IT/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/ja/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/ko_KR/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/ru/LC_MESSAGES/django.mo` & `allianceauth_afat-2.9.7/afat/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/ru/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/locale/zh_Hans/LC_MESSAGES/django.po` & `allianceauth_afat-2.9.7/afat/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/management/commands/afat_import_from_allianceauth_fat.py` & `allianceauth_afat-2.9.7/afat/management/commands/afat_import_from_allianceauth_fat.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/management/commands/afat_import_from_imicusfat.py` & `allianceauth_afat-2.9.7/afat/management/commands/afat_import_from_imicusfat.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/management/commands/afat_migrate_manual_fat_log.py` & `allianceauth_afat-2.9.7/afat/management/commands/afat_migrate_manual_fat_log.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/managers.py` & `allianceauth_afat-2.9.7/afat/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0001_initial.py` & `allianceauth_afat-2.9.7/afat/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0002_manualfat.py` & `allianceauth_afat-2.9.7/afat/migrations/0002_manualfat.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0003_auto_20180911_0831.py` & `allianceauth_afat-2.9.7/afat/migrations/0003_auto_20180911_0831.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0004_clickfatduration.py` & `allianceauth_afat-2.9.7/afat/migrations/0004_clickfatduration.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0005_auto_20200816_2042.py` & `allianceauth_afat-2.9.7/afat/migrations/0005_auto_20200816_2042.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0006_auto_20200820_2013.py` & `allianceauth_afat-2.9.7/afat/migrations/0006_auto_20200820_2013.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0008_auto_20200912_1116.py` & `allianceauth_afat-2.9.7/afat/migrations/0008_auto_20200912_1116.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0009_auto_20200925_2206.py` & `allianceauth_afat-2.9.7/afat/migrations/0009_auto_20200925_2206.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0010_permissoins_update_20201002_1909.py` & `allianceauth_afat-2.9.7/afat/migrations/0010_permissoins_update_20201002_1909.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0012_manualafat_created_at.py` & `allianceauth_afat-2.9.7/afat/migrations/0012_manualafat_created_at.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0013_basic_module_access_permissions.py` & `allianceauth_afat-2.9.7/afat/migrations/0013_basic_module_access_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0014_auto_20201224_0930.py` & `allianceauth_afat-2.9.7/afat/migrations/0014_auto_20201224_0930.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0015_afatlink_character.py` & `allianceauth_afat-2.9.7/afat/migrations/0015_afatlink_character.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0016_permissions_overhaul.py` & `allianceauth_afat-2.9.7/afat/migrations/0016_permissions_overhaul.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0017_remove_soft_deletion.py` & `allianceauth_afat-2.9.7/afat/migrations/0017_remove_soft_deletion.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0018_auto_20210420_2016.py` & `allianceauth_afat-2.9.7/afat/migrations/0018_auto_20210420_2016.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0019_add_several_indices.py` & `allianceauth_afat-2.9.7/afat/migrations/0019_add_several_indices.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/migrations/0020_auto_20210617_1037.py` & `allianceauth_afat-2.9.7/afat/migrations/0020_auto_20210617_1037.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/models.py` & `allianceauth_afat-2.9.7/afat/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/css/allianceauth-afat.css` & `allianceauth_afat-2.9.7/afat/static/afat/css/afat.css`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,21 @@
     .btn-afat-action {
         margin: 0 0.25rem;
         height: 35px;
         width: 35px;
     }
 
     .fatlink-list-legend {
-        border-top: 1px solid rgb(236, 240, 241);
+        border-top: 1px solid rgb(236 240 241);
         margin-top: 1rem;
         padding-top: 1rem;
     }
 
     .template-dark-mode .fatlink-list-legend {
-        border-top: 1px solid rgb(70, 69, 69);
+        border-top: 1px solid rgb(70 69 69);
     }
 }
 
 /* esi fleet list (add fatlink view)
 ------------------------------------------------------------------------------------- */
 @media all {
     .allianceauth-afat .esi-fleet-list {
@@ -25,23 +25,22 @@
         padding: 0;
     }
 
     .allianceauth-afat .esi-fleet-list-item {
         align-content: space-between;
         align-items: center;
         display: flex;
-        flex-direction: row;
-        flex-wrap: nowrap;
+        flex-flow: row nowrap;
         justify-content: space-between;
         list-style: none;
         padding: 0.5rem 1rem;
     }
 
     .allianceauth-afat .esi-fleet-list-item:hover {
-        background-color: rgba(0, 0, 0, 0.1);
+        background-color: rgb(0 0 0 / 10%);
     }
 
     .allianceauth-afat .esi-fleet-list-item .eve-image-with-text {
         display: flex;
     }
 
     .allianceauth-afat .esi-fleet-list-item .eve-image-with-text .eve-image {
@@ -65,21 +64,21 @@
     }
 }
 
 /* labels
 ------------------------------------------------------------------------------------- */
 @media all {
     .afat-label-via-esi {
-        background-color: rgb(192, 192, 192);
-        color: rgb(54, 54, 54);
+        background-color: rgb(192 192 192);
+        color: rgb(54 54 54);
         margin-left: 1rem;
     }
 
     .afat-label-active-esi-fleet {
-        background-color: rgb(98, 196, 98);
+        background-color: rgb(98 196 98);
     }
 
     .afat-label-statistics {
         margin-left: 1rem;
         margin-right: 1rem;
         position: relative;
         top: 0.2rem;
```

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/css/allianceauth-afat.min.css` & `allianceauth_afat-2.9.7/afat/static/afat/css/afat.min.css`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-@media all{.btn-afat-action{margin:0 .25rem;height:35px;width:35px}.fatlink-list-legend{border-top:1px solid #ecf0f1;margin-top:1rem;padding-top:1rem}.template-dark-mode .fatlink-list-legend{border-top:1px solid #464545}.allianceauth-afat .esi-fleet-list{margin-bottom:1rem;margin-top:1rem;padding:0}.allianceauth-afat .esi-fleet-list-item{align-content:space-between;align-items:center;display:flex;flex-direction:row;flex-wrap:nowrap;justify-content:space-between;list-style:none;padding:.5rem 1rem}.allianceauth-afat .esi-fleet-list-item:hover{background-color:rgba(0,0,0,.1)}.allianceauth-afat .esi-fleet-list-item .eve-image-with-text{display:flex}.allianceauth-afat .esi-fleet-list-item .eve-image-with-text .eve-image{margin:auto}.allianceauth-afat .esi-fleet-list-item .eve-character-portrait{margin-right:.5rem}.allianceauth-afat .table>tbody>tr>td,.allianceauth-afat .table>tbody>tr>th,.allianceauth-afat .table>tfoot>tr>td,.allianceauth-afat .table>tfoot>tr>th,.allianceauth-afat .table>thead>tr>td{vertical-align:middle}.afat-label-via-esi{background-color:silver;color:#363636;margin-left:1rem}.afat-label-active-esi-fleet{background-color:#62c462}.afat-label-statistics{margin-left:1rem;margin-right:1rem;position:relative;top:.2rem}.afat-select-time-period{font-size:19px;font-weight:400;line-height:1.1;margin-top:10.5px;margin-bottom:10.5px}.dataTables_wrapper>.form-inline{margin-bottom:1rem}.dataTables_wrapper>.form-inline select{margin-bottom:1rem;margin-right:1rem}.dataTables_wrapper>.form-inline select:last-child{margin-right:0}.dataTables_length select{margin:0 1rem}}@media (min-width:768px){.dataTables_wrapper>.form-inline select:first-child{margin-left:1rem}}
+@media all{.btn-afat-action{margin:0 .25rem;height:35px;width:35px}.fatlink-list-legend{border-top:1px solid rgb(236 240 241);margin-top:1rem;padding-top:1rem}.template-dark-mode .fatlink-list-legend{border-top:1px solid rgb(70 69 69)}.allianceauth-afat .esi-fleet-list{margin-bottom:1rem;margin-top:1rem;padding:0}.allianceauth-afat .esi-fleet-list-item{align-content:space-between;align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;list-style:none;padding:.5rem 1rem}.allianceauth-afat .esi-fleet-list-item:hover{background-color:rgb(0 0 0/10%)}.allianceauth-afat .esi-fleet-list-item .eve-image-with-text{display:flex}.allianceauth-afat .esi-fleet-list-item .eve-image-with-text .eve-image{margin:auto}.allianceauth-afat .esi-fleet-list-item .eve-character-portrait{margin-right:.5rem}.allianceauth-afat .table>tbody>tr>td,.allianceauth-afat .table>tbody>tr>th,.allianceauth-afat .table>tfoot>tr>td,.allianceauth-afat .table>tfoot>tr>th,.allianceauth-afat .table>thead>tr>td{vertical-align:middle}.afat-label-via-esi{background-color:rgb(192 192 192);color:rgb(54 54 54);margin-left:1rem}.afat-label-active-esi-fleet{background-color:rgb(98 196 98)}.afat-label-statistics{margin-left:1rem;margin-right:1rem;position:relative;top:.2rem}.afat-select-time-period{font-size:19px;font-weight:400;line-height:1.1;margin-top:10.5px;margin-bottom:10.5px}.dataTables_wrapper>.form-inline{margin-bottom:1rem}.dataTables_wrapper>.form-inline select{margin-bottom:1rem;margin-right:1rem}.dataTables_wrapper>.form-inline select:last-child{margin-right:0}.dataTables_length select{margin:0 1rem}}@media (min-width:768px){.dataTables_wrapper>.form-inline select:first-child{margin-left:1rem}}
```

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-dashboard.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-dashboard.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-dashboard.min.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlink-details.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlink-details.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlink-details.min.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlink-details.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlist.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlist.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-fatlist.min.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-fatlist.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-logs.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-logs.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/afat-logs.min.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat-logs.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/allianceauth-afat.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/javascript/allianceauth-afat.min.js` & `allianceauth_afat-2.9.7/afat/static/afat/javascript/afat.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/static/afat/libs/chartjs/chart.min.js` & `allianceauth_afat-2.9.7/afat/static/afat/libs/Chart.js/2.7.2/chart.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tasks.py` & `allianceauth_afat-2.9.7/afat/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/modals/general.html` & `allianceauth_afat-2.9.7/afat/templates/afat/modals/general.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/tabs/fatlinks.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/tabs/fatlinks.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/dashboard/tabs/fats.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/dashboard/tabs/fats.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% load evelinks %}
 {% load i18n %}
 
-<script type="application/javascript">
+<script>
     let characters = [];
 </script>
 
 <div id="fats" class="tab-pane fade in active panel panel-default">
     <div class="panel-body">
         <h4>{% translate "Your Most Recent FATs" %}</h4>
 
         <p>{% translate "Only characters that have recent FATs are shown. <small>(latest 10 FATs per character)</small>" %}</p>
 
         {% if characters %}
             <ul class="nav nav-pills">
                 {% for character in characters %}
                     <li class="afat-character-tab{% if forloop.first %} active{% endif %}">
-                        <script type="application/javascript">
+                        <script>
                             characters.push({
                                 charId: {{ character.character_id }},
                                 charName: '{{ character.character_name }}'
                             })
                         </script>
 
                         <a data-toggle="tab" href="#{{ character.character_id }}">
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/add/clickable_link.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/add/clickable_link.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/add/esi_link.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/add/esi_link.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/fatlink_info.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/fatlink_info.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/tabs/fats.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/tabs/fats.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/fatlinks/open_esi_fleets.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/fatlinks/open_esi_fleets.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/menu.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/menu.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-{% load static %}
 {% load i18n %}
 {% load navactive %}
 
 <nav class="navbar navbar-default">
     <div class="container-fluid">
         <div class="navbar-header">
             <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% load static %} {% load i18n %} {% load navactive %}
+{% load i18n %} {% load navactive %}
  {% translate "Toggle navigation" %}     {%_translate_"Fleet_Activity_Tracking"
 %}
     * {%_translate_"Statistics"_%}
     * {%_translate_"FAT_Links"_%}
     * {% if perms.afat.add_fatlink or perms.afat.manage_afat %}
     * {%_translate_"Add_FAT_Link"_%}
     * {% endif %} {% if perms.afat.log_view %}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/month_navigation.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/month_navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                 <div class="panel-body">
                     <h3>
                         {% translate "FATs by Ship Type" %}
                     </h3>
 
                     <canvas id="ship-pie" width="800" height="500"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let shipPieChart = new Chart(document.getElementById("ship-pie"), {
                             type: "pie",
                             data: {
                                 datasets: [{
                                     data: {{ data_ship_type.1| safe }},
                                     backgroundColor: {{ data_ship_type.2| safe }}
                                 }],
@@ -40,15 +40,15 @@
                 <div class="panel-body">
                     <h3>
                         {% translate "FATs by Time" %}
                     </h3>
 
                     <canvas id="time-line" width="800" height="500"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let timeLineChart = new Chart(document.getElementById("time-line"), {
                             type: 'line',
                             data: {
                                 datasets: [{
                                     label: '# of FATs',
                                     backgroundColor: {{ data_time.2|safe }},
                                     data: {{ data_time.1 }}
@@ -67,15 +67,15 @@
                 <div class="panel-body">
                     <h3>
                         {% translate "FATs by Weekday" %}
                     </h3>
 
                     <canvas id="weekday-line" width="800" height="500"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let weekdayLineChart = new Chart(document.getElementById('weekday-line'), {
                             type: 'line',
                             data:{
                                 datasets: [{
                                     label: '# of FATs',
                                     backgroundColor: {{ data_weekday.2|safe }},
                                     data: {{ data_weekday.1 }}
@@ -94,15 +94,15 @@
                 <div class="panel-body">
                     <h3>
                         {% translate "Average FATs by Corporation" %}
                     </h3>
 
                     <canvas id="avgs" width="1000" height="700"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let averagesHorizontalBarChart = new Chart(document.getElementById('avgs'), {
                             type: 'horizontalBar',
                             data:{
                                 datasets: [{
                                     label: 'Average # of FATs',
                                     backgroundColor: '{{ data_avgs.2|safe }}',
                                     data: {{ data_avgs.1 }}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/tabs/graphs.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/tabs/graphs.html`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <div id="graphs" class="tab-pane fade in active panel panel-default">
     <div class="panel-body">
         <div class="col-md-4">
             <h4>{% translate "FATs by Ship Type" %}</h4>
 
             <canvas style="width: 400px; max-width: 100%; height: 400px;" id="pie-ship"></canvas>
 
-            <script type="application/javascript">
+            <script>
                 let shipPieChart = new Chart(document.getElementById("pie-ship"), {
                     type: "pie",
                     data: {
                         datasets: [{
                             data: {{ data_ship_type.1|safe }},
                             backgroundColor: {{ data_ship_type.2|safe }}
                         }],
@@ -25,15 +25,15 @@
         </div>
 
         <div class="col-md-8">
             <h4>{% translate "FATs by Time of Day" %}</h4>
 
             <canvas style="width: 100%; height: 400px;" id="line-time"></canvas>
 
-            <script type="application/javascript">
+            <script>
                 let FATLineChart = new Chart(document.getElementById("line-time"),{
                     type: "line",
                     data: {
                         datasets: [{
                             label: '{% translate "# of FATs" %}',
                             data: {{ data_time.1|safe }},
                             backgroundColor: {{ data_time.2|safe }}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/character/tabs/raw_data.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/character/tabs/raw_data.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         <div class="tab-content">
             <div class="tab-pane fade in active panel-default" id="fatsbyship">
                 <div class="panel-body">
                     <h3>{% translate "FATs by Ship Type" %}</h3>
 
                     <canvas id="ship-bar-stacked" width="800" height="500"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let corpShipTypeBarChart = new Chart(document.getElementById('ship-bar-stacked'), {
                             type: "bar",
                             data: {
                                 datasets: [{% for set in data_stacked.1 %}
                                     {
                                         label: '{{ set.0|escapejs }}',
                                         backgroundColor: '{{ set.1|safe }}',
@@ -49,15 +49,15 @@
 
             <div id="fatsbytime" class="tab-pane fade in panel-default">
                 <div class="panel-body">
                     <h3>{% translate "FATs By Time" %}</h3>
 
                     <canvas id="time-line" width="800" height="500"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let timeLineChart = new Chart(document.getElementById("time-line"), {
                             type: 'line',
                             data: {
                                 datasets: [{
                                     label: '# of FATs',
                                     backgroundColor: {{ data_time.2|safe }},
                                     data: {{ data_time.1 }}
@@ -74,15 +74,15 @@
 
             <div class="tab-pane fade in panel-default" id="fatsbyweek">
                 <div class="panel-body">
                     <h3>{% translate "FATs By Weekday" %}</h3>
 
                     <canvas id="weekday-line" width="800" height="500"></canvas>
 
-                    <script type="application/javascript">
+                    <script>
                         let weekdayLineChart = new Chart(document.getElementById('weekday-line'), {
                             type: 'line',
                             data:{
                                 datasets: [{
                                     label: '# of FATs',
                                     backgroundColor: {{ data_weekday.2|safe }},
                                     data: {{ data_weekday.1 }}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/corporation/tabs/member.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/corporation/tabs/member.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/tabs/corps.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/tabs/corps.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/statistics/overview/tabs/mine.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/statistics/overview/tabs/mine.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/partials/year_navigation.html` & `allianceauth_afat-2.9.7/afat/templates/afat/partials/year_navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% extends 'afat/base.html' %}
 
-{% load afat_versioned_static %}
 {% load i18n %}
 
 {% block page_title %}{% translate 'Fleet Activity' %}{% endblock %}
 
 {% block afat_header %}
     <br>
     {% include "afat/partials/menu.html" %}
@@ -30,26 +29,23 @@
 
     {% translate "Delete FAT" as translated_title %}
     {% include "afat/modals/general.html" with modal_name='deleteFat' modal_title=translated_title confirm_button_class='btn-danger' %}
 {% endblock %}
 
 {% block extra_css %}
     {% include 'bundles/datatables-css.html' %}
-
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/allianceauth-afat.min.css' %}">
+    {% include "afat/bundles/afat-css.html" %}
 {% endblock %}
 
 {% block extra_javascript %}
-    <script type="application/javascript" src="{% afat_static 'afat/javascript/allianceauth-afat.min.js' %}"></script>
-
+    {% include "afat/bundles/afat-js.html" %}
     {% include 'bundles/datatables-js.html' %}
     {% include 'bundles/clipboard-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         let afatSettings = {
             url: '{% url "afat:fatlinks_ajax_get_fats_by_fatlink" 0 %}'.replace(
                     '0',
                     '{{ link.hash }}'
                 ),
             modal: {
                 deleteFatModal: {
@@ -61,9 +57,10 @@
                 cancelEsiFleetModal: {
                     element: '#cancelEsiFleetModal',
                 }
             },
             reloadDatatable: {{ link_ongoing|yesno:"true,false" }}
         }
     </script>
-    <script type="application/javascript" src="{% afat_static 'afat/javascript/afat-fatlink-details.min.js' %}"></script>
+
+    {% include "afat/bundles/afat-fatlink-details-js.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-{% extends 'afat/base.html' %} {% load afat_versioned_static %} {% load i18n %}
-{% block page_title %}{% translate 'Fleet Activity' %}{% endblock %} {% block
-afat_header %}
+{% extends 'afat/base.html' %} {% load i18n %} {% block page_title %}{%
+translate 'Fleet Activity' %}{% endblock %} {% block afat_header %}
 {% include "afat/partials/menu.html" %}
 ***** {% translate "FAT Link Details" %} *****
 {% endblock %} {% block afat_body %} {% if perms.afat.manage_afat %} {% include
 "afat/partials/fatlinks/details/fatlink_name_form.html" %} {% endif %} {%
 include "afat/partials/fatlinks/details/fatlink_info.html" %}
  
 {% include "afat/partials/fatlinks/details/tabs_navigation.html" %}
 {% include "afat/partials/fatlinks/details/tabs/fats.html" %} {% include "afat/
 partials/fatlinks/details/tabs/manualfat.html" %}
 {% translate "Delete FAT" as translated_title %} {% include "afat/modals/
 general.html" with modal_name='deleteFat' modal_title=translated_title
 confirm_button_class='btn-danger' %} {% endblock %} {% block extra_css %} {%
-include 'bundles/datatables-css.html' %}
-
- {% endblock %} {% block extra_javascript %}
- {% include 'bundles/datatables-js.html' %} {% include 'bundles/clipboard-
-js.html' %}
- {% endblock %}
+include 'bundles/datatables-css.html' %} {% include "afat/bundles/afat-
+css.html" %} {% endblock %} {% block extra_javascript %} {% include "afat/
+bundles/afat-js.html" %} {% include 'bundles/datatables-js.html' %} {% include
+'bundles/clipboard-js.html' %}
+ {% include "afat/bundles/afat-fatlink-details-js.html" %} {% endblock %}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_alliance.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_alliance.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 {% extends 'afat/base.html' %}
 
 {% load evelinks %}
-{% load static %}
-{% load afat_versioned_static %}
 {% load i18n %}
 
 {% block page_title %}{{ alliance }} {% translate "Statistics" %}{% endblock %}
 
 {% block afat_header %}
     <br>
     {% include 'afat/partials/menu.html' %}
@@ -38,24 +36,22 @@
         {% include 'afat/partials/statistics/alliance/tabs/graphs.html' %}
         {% include 'afat/partials/statistics/alliance/tabs/corporations.html' %}
     </div>
 {% endblock %}
 
 {% block extra_css %}
     {% include 'bundles/datatables-css.html' %}
-
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/allianceauth-afat.min.css' %}">
+    {% include "afat/bundles/afat-css.html" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
     {% include 'bundles/moment-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         /**
          * datetime formatting
          *
          * @param format
          * @param locale
          */
         $.fn.dataTable.moment = function(format, locale) {
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_alliance_year_overview.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_alliance_year_overview.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% extends 'afat/base.html' %}
 
-{% load afat_versioned_static %}
 {% load i18n %}
 {% load filters %}
 
 {% block page_title %}{{ alliance }} {% translate "Fleet Activity" %}{% endblock %}
 
 {% block afat_header %}
     <br>
@@ -57,10 +56,9 @@
                 </tbody>
             </table>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/allianceauth-afat.min.css' %}">
+    {% include "afat/bundles/afat-css.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-{% extends 'afat/base.html' %} {% load afat_versioned_static %} {% load i18n %}
-{% load filters %} {% block page_title %}{{ alliance }} {% translate "Fleet
-Activity" %}{% endblock %} {% block afat_header %}
+{% extends 'afat/base.html' %} {% load i18n %} {% load filters %} {% block
+page_title %}{{ alliance }} {% translate "Fleet Activity" %}{% endblock %} {%
+block afat_header %}
 {% include "afat/partials/menu.html" %}
 ***** {{ alliance }} {% translate "Fleet Activity" %} *****
 {% endblock %} {% block afat_body %} {% url 'afat:statistics_alliance'
 allianceid year_prev as url_previous_year %} {% url 'afat:statistics_alliance'
 allianceid year_next as url_next_year %} {% url 'afat:statistics_alliance'
 allianceid year_current as url_current_year %} {% include "afat/partials/
 year_navigation.html" with url_previous_year=url_previous_year
 url_next_year=url_next_year url_current_year=url_current_year %}
 {% translate "Month" {% translate "FATs" {% translate "Avg
 %}                   %}                  FATs" %}
 {                                                          {% if alliance !=
 { month.0|month_name {{ month.1 }}       {{ month.2 }}     'No Alliance' %}  {%
 }}                                                         endif %}
-{% endblock %} {% block extra_css %}
-
- {% endblock %}
+{% endblock %} {% block extra_css %} {% include "afat/bundles/afat-css.html" %}
+{% endblock %}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_character.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_corporation.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,56 @@
-{% extends "afat/base.html" %}
+{% extends 'afat/base.html' %}
 
-{% load static %}
-{% load afat_versioned_static %}
 {% load i18n %}
 
-{% block page_title %}{{ character.character_name }} {% translate "FAT Statistics" %}{% endblock %}
+{% block page_title %}{{ corporation }} {% translate "Statistics" %}{% endblock %}
 
 {% block afat_header %}
     <br>
     {% include 'afat/partials/menu.html' %}
 
-    <h2>{{ character.character_name }} {% translate "Statistics" %}</h2>
+    <h2>{{ corporation }} {% translate "Statistics" %}</h2>
 {% endblock %}
 
 {% block afat_body %}
     {% include 'afat/bundles/chartjs-js.html' %}
 
     {% if month == '1' %}
-        {% url 'afat:statistics_character' character.character_id year_prev 12 as url_previous_month %}
+        {% url 'afat:statistics_corporation' corp.corporation_id year_prev 12 as url_previous_month %}
     {% else %}
-        {% url 'afat:statistics_character' character.character_id year month_prev as url_previous_month %}
+        {% url 'afat:statistics_corporation' corp.corporation_id year month_prev as url_previous_month %}
     {% endif %}
 
     {% if month == '12' %}
-        {% url 'afat:statistics_character' character.character_id year_next 1 as url_next_month %}
-        {% url 'afat:statistics_character' character.character_id year_current month_current as url_current_month %}
+        {% url 'afat:statistics_corporation' corp.corporation_id year_next 1 as url_next_month %}
+        {% url 'afat:statistics_corporation' corp.corporation_id year_current month_current as url_current_month %}
     {% else %}
-        {% url 'afat:statistics_character' character.character_id year month_next as url_next_month %}
-        {% url 'afat:statistics_character' character.character_id year_current month_current as url_current_month %}
+        {% url 'afat:statistics_corporation' corp.corporation_id year month_next as url_next_month %}
+        {% url 'afat:statistics_corporation' corp.corporation_id year_current month_current as url_current_month %}
     {% endif %}
     {% include "afat/partials/month_navigation.html" with url_previous_month=url_previous_month url_next_month=url_next_month url_current_month=url_current_month %}
 
-    {% include 'afat/partials/statistics/character/tabs_navigation.html' %}
+    {% include 'afat/partials/statistics/corporation/tabs_navigation.html' %}
 
     <div class="tab-content">
-        {% include 'afat/partials/statistics/character/tabs/graphs.html' %}
-        {% include 'afat/partials/statistics/character/tabs/raw_data.html' %}
+        {% include 'afat/partials/statistics/corporation/tabs/graphs.html' %}
+        {% include 'afat/partials/statistics/corporation/tabs/member.html' %}
     </div>
 {% endblock %}
 
 {% block extra_css %}
     {% include 'bundles/datatables-css.html' %}
-
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/allianceauth-afat.min.css' %}">
+    {% include "afat/bundles/afat-css.html" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
     {% include 'bundles/moment-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         /**
          * datetime formatting
          *
          * @param format
          * @param locale
          */
         $.fn.dataTable.moment = function(format, locale) {
@@ -70,15 +66,16 @@
                 return moment(d, format, locale, true).unix();
             };
         };
 
         $(document).ready(function() {
             $.fn.dataTable.moment('YYYY-MMM-DD, HH:mm');
 
-            $('#raw-data').DataTable({
-                "order": [
-                    [4, "desc"]
-                ]
+            $('#corp-members').DataTable({
+                order: [
+                    [1, 'desc'],
+                    [0, 'asc']
+                ],
             });
         });
     </script>
 {% endblock %}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_corporation.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/fatlinks/fatlinks_overview.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,190 +1,213 @@
 00000000: 7b25 2065 7874 656e 6473 2027 6166 6174  {% extends 'afat
 00000010: 2f62 6173 652e 6874 6d6c 2720 257d 0a0a  /base.html' %}..
-00000020: 7b25 206c 6f61 6420 7374 6174 6963 2025  {% load static %
-00000030: 7d0a 7b25 206c 6f61 6420 6166 6174 5f76  }.{% load afat_v
-00000040: 6572 7369 6f6e 6564 5f73 7461 7469 6320  ersioned_static 
-00000050: 257d 0a7b 2520 6c6f 6164 2069 3138 6e20  %}.{% load i18n 
-00000060: 257d 0a0a 7b25 2062 6c6f 636b 2070 6167  %}..{% block pag
-00000070: 655f 7469 746c 6520 257d 7b7b 2063 6f72  e_title %}{{ cor
-00000080: 706f 7261 7469 6f6e 207d 7d20 7b25 2074  poration }} {% t
-00000090: 7261 6e73 6c61 7465 2022 5374 6174 6973  ranslate "Statis
-000000a0: 7469 6373 2220 257d 7b25 2065 6e64 626c  tics" %}{% endbl
-000000b0: 6f63 6b20 257d 0a0a 7b25 2062 6c6f 636b  ock %}..{% block
-000000c0: 2061 6661 745f 6865 6164 6572 2025 7d0a   afat_header %}.
-000000d0: 2020 2020 3c62 723e 0a20 2020 207b 2520      <br>.    {% 
-000000e0: 696e 636c 7564 6520 2761 6661 742f 7061  include 'afat/pa
-000000f0: 7274 6961 6c73 2f6d 656e 752e 6874 6d6c  rtials/menu.html
-00000100: 2720 257d 0a0a 2020 2020 3c68 323e 7b7b  ' %}..    <h2>{{
-00000110: 2063 6f72 706f 7261 7469 6f6e 207d 7d20   corporation }} 
-00000120: 7b25 2074 7261 6e73 6c61 7465 2022 5374  {% translate "St
-00000130: 6174 6973 7469 6373 2220 257d 3c2f 6832  atistics" %}</h2
-00000140: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
-00000150: 0a0a 7b25 2062 6c6f 636b 2061 6661 745f  ..{% block afat_
-00000160: 626f 6479 2025 7d0a 2020 2020 7b25 2069  body %}.    {% i
-00000170: 6e63 6c75 6465 2027 6166 6174 2f62 756e  nclude 'afat/bun
-00000180: 646c 6573 2f63 6861 7274 6a73 2d6a 732e  dles/chartjs-js.
-00000190: 6874 6d6c 2720 257d 0a0a 2020 2020 7b25  html' %}..    {%
-000001a0: 2069 6620 6d6f 6e74 6820 3d3d 2027 3127   if month == '1'
-000001b0: 2025 7d0a 2020 2020 2020 2020 7b25 2075   %}.        {% u
-000001c0: 726c 2027 6166 6174 3a73 7461 7469 7374  rl 'afat:statist
-000001d0: 6963 735f 636f 7270 6f72 6174 696f 6e27  ics_corporation'
-000001e0: 2063 6f72 702e 636f 7270 6f72 6174 696f   corp.corporatio
-000001f0: 6e5f 6964 2079 6561 725f 7072 6576 2031  n_id year_prev 1
-00000200: 3220 6173 2075 726c 5f70 7265 7669 6f75  2 as url_previou
-00000210: 735f 6d6f 6e74 6820 257d 0a20 2020 207b  s_month %}.    {
-00000220: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-00000230: 2020 7b25 2075 726c 2027 6166 6174 3a73    {% url 'afat:s
-00000240: 7461 7469 7374 6963 735f 636f 7270 6f72  tatistics_corpor
-00000250: 6174 696f 6e27 2063 6f72 702e 636f 7270  ation' corp.corp
-00000260: 6f72 6174 696f 6e5f 6964 2079 6561 7220  oration_id year 
-00000270: 6d6f 6e74 685f 7072 6576 2061 7320 7572  month_prev as ur
-00000280: 6c5f 7072 6576 696f 7573 5f6d 6f6e 7468  l_previous_month
-00000290: 2025 7d0a 2020 2020 7b25 2065 6e64 6966   %}.    {% endif
-000002a0: 2025 7d0a 0a20 2020 207b 2520 6966 206d   %}..    {% if m
-000002b0: 6f6e 7468 203d 3d20 2731 3227 2025 7d0a  onth == '12' %}.
-000002c0: 2020 2020 2020 2020 7b25 2075 726c 2027          {% url '
-000002d0: 6166 6174 3a73 7461 7469 7374 6963 735f  afat:statistics_
-000002e0: 636f 7270 6f72 6174 696f 6e27 2063 6f72  corporation' cor
-000002f0: 702e 636f 7270 6f72 6174 696f 6e5f 6964  p.corporation_id
-00000300: 2079 6561 725f 6e65 7874 2031 2061 7320   year_next 1 as 
-00000310: 7572 6c5f 6e65 7874 5f6d 6f6e 7468 2025  url_next_month %
-00000320: 7d0a 2020 2020 2020 2020 7b25 2075 726c  }.        {% url
-00000330: 2027 6166 6174 3a73 7461 7469 7374 6963   'afat:statistic
-00000340: 735f 636f 7270 6f72 6174 696f 6e27 2063  s_corporation' c
-00000350: 6f72 702e 636f 7270 6f72 6174 696f 6e5f  orp.corporation_
-00000360: 6964 2079 6561 725f 6375 7272 656e 7420  id year_current 
-00000370: 6d6f 6e74 685f 6375 7272 656e 7420 6173  month_current as
-00000380: 2075 726c 5f63 7572 7265 6e74 5f6d 6f6e   url_current_mon
-00000390: 7468 2025 7d0a 2020 2020 7b25 2065 6c73  th %}.    {% els
-000003a0: 6520 257d 0a20 2020 2020 2020 207b 2520  e %}.        {% 
-000003b0: 7572 6c20 2761 6661 743a 7374 6174 6973  url 'afat:statis
-000003c0: 7469 6373 5f63 6f72 706f 7261 7469 6f6e  tics_corporation
-000003d0: 2720 636f 7270 2e63 6f72 706f 7261 7469  ' corp.corporati
-000003e0: 6f6e 5f69 6420 7965 6172 206d 6f6e 7468  on_id year month
-000003f0: 5f6e 6578 7420 6173 2075 726c 5f6e 6578  _next as url_nex
-00000400: 745f 6d6f 6e74 6820 257d 0a20 2020 2020  t_month %}.     
-00000410: 2020 207b 2520 7572 6c20 2761 6661 743a     {% url 'afat:
-00000420: 7374 6174 6973 7469 6373 5f63 6f72 706f  statistics_corpo
-00000430: 7261 7469 6f6e 2720 636f 7270 2e63 6f72  ration' corp.cor
-00000440: 706f 7261 7469 6f6e 5f69 6420 7965 6172  poration_id year
-00000450: 5f63 7572 7265 6e74 206d 6f6e 7468 5f63  _current month_c
-00000460: 7572 7265 6e74 2061 7320 7572 6c5f 6375  urrent as url_cu
-00000470: 7272 656e 745f 6d6f 6e74 6820 257d 0a20  rrent_month %}. 
-00000480: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00000490: 2020 207b 2520 696e 636c 7564 6520 2261     {% include "a
-000004a0: 6661 742f 7061 7274 6961 6c73 2f6d 6f6e  fat/partials/mon
-000004b0: 7468 5f6e 6176 6967 6174 696f 6e2e 6874  th_navigation.ht
-000004c0: 6d6c 2220 7769 7468 2075 726c 5f70 7265  ml" with url_pre
-000004d0: 7669 6f75 735f 6d6f 6e74 683d 7572 6c5f  vious_month=url_
-000004e0: 7072 6576 696f 7573 5f6d 6f6e 7468 2075  previous_month u
-000004f0: 726c 5f6e 6578 745f 6d6f 6e74 683d 7572  rl_next_month=ur
-00000500: 6c5f 6e65 7874 5f6d 6f6e 7468 2075 726c  l_next_month url
-00000510: 5f63 7572 7265 6e74 5f6d 6f6e 7468 3d75  _current_month=u
-00000520: 726c 5f63 7572 7265 6e74 5f6d 6f6e 7468  rl_current_month
-00000530: 2025 7d0a 0a20 2020 207b 2520 696e 636c   %}..    {% incl
-00000540: 7564 6520 2761 6661 742f 7061 7274 6961  ude 'afat/partia
-00000550: 6c73 2f73 7461 7469 7374 6963 732f 636f  ls/statistics/co
-00000560: 7270 6f72 6174 696f 6e2f 7461 6273 5f6e  rporation/tabs_n
-00000570: 6176 6967 6174 696f 6e2e 6874 6d6c 2720  avigation.html' 
-00000580: 257d 0a0a 2020 2020 3c64 6976 2063 6c61  %}..    <div cla
-00000590: 7373 3d22 7461 622d 636f 6e74 656e 7422  ss="tab-content"
-000005a0: 3e0a 2020 2020 2020 2020 7b25 2069 6e63  >.        {% inc
-000005b0: 6c75 6465 2027 6166 6174 2f70 6172 7469  lude 'afat/parti
-000005c0: 616c 732f 7374 6174 6973 7469 6373 2f63  als/statistics/c
-000005d0: 6f72 706f 7261 7469 6f6e 2f74 6162 732f  orporation/tabs/
-000005e0: 6772 6170 6873 2e68 746d 6c27 2025 7d0a  graphs.html' %}.
-000005f0: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
-00000600: 6465 2027 6166 6174 2f70 6172 7469 616c  de 'afat/partial
-00000610: 732f 7374 6174 6973 7469 6373 2f63 6f72  s/statistics/cor
-00000620: 706f 7261 7469 6f6e 2f74 6162 732f 6d65  poration/tabs/me
-00000630: 6d62 6572 2e68 746d 6c27 2025 7d0a 2020  mber.html' %}.  
-00000640: 2020 3c2f 6469 763e 0a7b 2520 656e 6462    </div>.{% endb
-00000650: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
-00000660: 6b20 6578 7472 615f 6373 7320 257d 0a20  k extra_css %}. 
-00000670: 2020 207b 2520 696e 636c 7564 6520 2762     {% include 'b
-00000680: 756e 646c 6573 2f64 6174 6174 6162 6c65  undles/datatable
-00000690: 732d 6373 732e 6874 6d6c 2720 257d 0a0a  s-css.html' %}..
-000006a0: 2020 2020 3c6c 696e 6b20 7265 6c3d 2273      <link rel="s
-000006b0: 7479 6c65 7368 6565 7422 2074 7970 653d  tylesheet" type=
-000006c0: 2274 6578 742f 6373 7322 2068 7265 663d  "text/css" href=
-000006d0: 227b 2520 6166 6174 5f73 7461 7469 6320  "{% afat_static 
-000006e0: 2761 6661 742f 6373 732f 6161 2d62 6f6f  'afat/css/aa-boo
-000006f0: 7473 7472 6170 2d66 6978 2e6d 696e 2e63  tstrap-fix.min.c
-00000700: 7373 2720 257d 223e 0a20 2020 203c 6c69  ss' %}">.    <li
-00000710: 6e6b 2072 656c 3d22 7374 796c 6573 6865  nk rel="styleshe
-00000720: 6574 2220 7479 7065 3d22 7465 7874 2f63  et" type="text/c
-00000730: 7373 2220 6872 6566 3d22 7b25 2061 6661  ss" href="{% afa
-00000740: 745f 7374 6174 6963 2027 6166 6174 2f63  t_static 'afat/c
-00000750: 7373 2f61 6c6c 6961 6e63 6561 7574 682d  ss/allianceauth-
-00000760: 6166 6174 2e6d 696e 2e63 7373 2720 257d  afat.min.css' %}
-00000770: 223e 0a7b 2520 656e 6462 6c6f 636b 2025  ">.{% endblock %
-00000780: 7d0a 0a7b 2520 626c 6f63 6b20 6578 7472  }..{% block extr
-00000790: 615f 6a61 7661 7363 7269 7074 2025 7d0a  a_javascript %}.
-000007a0: 2020 2020 7b25 2069 6e63 6c75 6465 2027      {% include '
-000007b0: 6275 6e64 6c65 732f 6461 7461 7461 626c  bundles/datatabl
-000007c0: 6573 2d6a 732e 6874 6d6c 2720 257d 0a20  es-js.html' %}. 
-000007d0: 2020 207b 2520 696e 636c 7564 6520 2762     {% include 'b
-000007e0: 756e 646c 6573 2f6d 6f6d 656e 742d 6a73  undles/moment-js
-000007f0: 2e68 746d 6c27 2025 7d0a 0a20 2020 203c  .html' %}..    <
-00000800: 7363 7269 7074 2074 7970 653d 2261 7070  script type="app
-00000810: 6c69 6361 7469 6f6e 2f6a 6176 6173 6372  lication/javascr
-00000820: 6970 7422 3e0a 2020 2020 2020 2020 2f2a  ipt">.        /*
-00000830: 2a0a 2020 2020 2020 2020 202a 2064 6174  *.         * dat
-00000840: 6574 696d 6520 666f 726d 6174 7469 6e67  etime formatting
-00000850: 0a20 2020 2020 2020 2020 2a0a 2020 2020  .         *.    
-00000860: 2020 2020 202a 2040 7061 7261 6d20 666f       * @param fo
-00000870: 726d 6174 0a20 2020 2020 2020 2020 2a20  rmat.         * 
-00000880: 4070 6172 616d 206c 6f63 616c 650a 2020  @param locale.  
-00000890: 2020 2020 2020 202a 2f0a 2020 2020 2020         */.      
-000008a0: 2020 242e 666e 2e64 6174 6154 6162 6c65    $.fn.dataTable
-000008b0: 2e6d 6f6d 656e 7420 3d20 6675 6e63 7469  .moment = functi
-000008c0: 6f6e 2866 6f72 6d61 742c 206c 6f63 616c  on(format, local
-000008d0: 6529 207b 0a20 2020 2020 2020 2020 2020  e) {.           
-000008e0: 206c 6574 2074 7970 6573 203d 2024 2e66   let types = $.f
-000008f0: 6e2e 6461 7461 5461 626c 652e 6578 742e  n.dataTable.ext.
-00000900: 7479 7065 3b0a 0a20 2020 2020 2020 2020  type;..         
-00000910: 2020 202f 2f20 4164 6420 7479 7065 2064     // Add type d
-00000920: 6574 6563 7469 6f6e 0a20 2020 2020 2020  etection.       
-00000930: 2020 2020 2074 7970 6573 2e64 6574 6563       types.detec
-00000940: 742e 756e 7368 6966 7428 6675 6e63 7469  t.unshift(functi
-00000950: 6f6e 2864 2920 7b0a 2020 2020 2020 2020  on(d) {.        
-00000960: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-00000970: 6f6d 656e 7428 642c 2066 6f72 6d61 742c  oment(d, format,
-00000980: 206c 6f63 616c 652c 2074 7275 6529 2e69   locale, true).i
-00000990: 7356 616c 6964 2829 203f 2027 6d6f 6d65  sValid() ? 'mome
-000009a0: 6e74 2d27 202b 2066 6f72 6d61 7420 3a20  nt-' + format : 
-000009b0: 6e75 6c6c 3b0a 2020 2020 2020 2020 2020  null;.          
-000009c0: 2020 7d29 3b0a 0a20 2020 2020 2020 2020    });..         
-000009d0: 2020 202f 2f20 4164 6420 736f 7274 696e     // Add sortin
-000009e0: 6720 6d65 7468 6f64 202d 2075 7365 2061  g method - use a
-000009f0: 6e20 696e 7465 6765 7220 666f 7220 7468  n integer for th
-00000a00: 6520 736f 7274 696e 670a 2020 2020 2020  e sorting.      
-00000a10: 2020 2020 2020 7479 7065 732e 6f72 6465        types.orde
-00000a20: 725b 276d 6f6d 656e 742d 2720 2b20 666f  r['moment-' + fo
-00000a30: 726d 6174 202b 2027 2d70 7265 275d 203d  rmat + '-pre'] =
-00000a40: 2066 756e 6374 696f 6e28 6429 207b 0a20   function(d) {. 
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000a60: 6574 7572 6e20 6d6f 6d65 6e74 2864 2c20  eturn moment(d, 
-00000a70: 666f 726d 6174 2c20 6c6f 6361 6c65 2c20  format, locale, 
-00000a80: 7472 7565 292e 756e 6978 2829 3b0a 2020  true).unix();.  
-00000a90: 2020 2020 2020 2020 2020 7d3b 0a20 2020            };.   
-00000aa0: 2020 2020 207d 3b0a 0a20 2020 2020 2020       };..       
-00000ab0: 2024 2864 6f63 756d 656e 7429 2e72 6561   $(document).rea
-00000ac0: 6479 2866 756e 6374 696f 6e28 2920 7b0a  dy(function() {.
-00000ad0: 2020 2020 2020 2020 2020 2020 242e 666e              $.fn
-00000ae0: 2e64 6174 6154 6162 6c65 2e6d 6f6d 656e  .dataTable.momen
-00000af0: 7428 2759 5959 592d 4d4d 4d2d 4444 2c20  t('YYYY-MMM-DD, 
-00000b00: 4848 3a6d 6d27 293b 0a0a 2020 2020 2020  HH:mm');..      
-00000b10: 2020 2020 2020 2428 2723 636f 7270 2d6d        $('#corp-m
-00000b20: 656d 6265 7273 2729 2e44 6174 6154 6162  embers').DataTab
-00000b30: 6c65 287b 0a20 2020 2020 2020 2020 2020  le({.           
-00000b40: 2020 2020 206f 7264 6572 3a20 5b0a 2020       order: [.  
+00000020: 7b25 206c 6f61 6420 6931 386e 2025 7d0a  {% load i18n %}.
+00000030: 0a7b 2520 626c 6f63 6b20 7061 6765 5f74  .{% block page_t
+00000040: 6974 6c65 2025 7d7b 2520 7472 616e 736c  itle %}{% transl
+00000050: 6174 6520 2746 6c65 6574 2041 6374 6976  ate 'Fleet Activ
+00000060: 6974 7927 2025 7d7b 2520 656e 6462 6c6f  ity' %}{% endblo
+00000070: 636b 2025 7d0a 0a7b 2520 626c 6f63 6b20  ck %}..{% block 
+00000080: 6166 6174 5f68 6561 6465 7220 257d 0a20  afat_header %}. 
+00000090: 2020 203c 6272 3e0a 2020 2020 7b25 2069     <br>.    {% i
+000000a0: 6e63 6c75 6465 2022 6166 6174 2f70 6172  nclude "afat/par
+000000b0: 7469 616c 732f 6d65 6e75 2e68 746d 6c22  tials/menu.html"
+000000c0: 2025 7d0a 0a20 2020 203c 6832 3e7b 2520   %}..    <h2>{% 
+000000d0: 7472 616e 736c 6174 6520 2241 6c6c 2046  translate "All F
+000000e0: 4154 204c 696e 6b73 2220 257d 3c2f 6832  AT Links" %}</h2
+000000f0: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
+00000100: 0a0a 7b25 2062 6c6f 636b 2061 6661 745f  ..{% block afat_
+00000110: 626f 6479 2025 7d0a 2020 2020 7b25 2075  body %}.    {% u
+00000120: 726c 2027 6166 6174 3a66 6174 6c69 6e6b  rl 'afat:fatlink
+00000130: 735f 6f76 6572 7669 6577 2720 7965 6172  s_overview' year
+00000140: 5f70 7265 7620 6173 2075 726c 5f70 7265  _prev as url_pre
+00000150: 7669 6f75 735f 7965 6172 2025 7d0a 2020  vious_year %}.  
+00000160: 2020 7b25 2075 726c 2027 6166 6174 3a66    {% url 'afat:f
+00000170: 6174 6c69 6e6b 735f 6f76 6572 7669 6577  atlinks_overview
+00000180: 2720 7965 6172 5f6e 6578 7420 6173 2075  ' year_next as u
+00000190: 726c 5f6e 6578 745f 7965 6172 2025 7d0a  rl_next_year %}.
+000001a0: 2020 2020 7b25 2075 726c 2027 6166 6174      {% url 'afat
+000001b0: 3a66 6174 6c69 6e6b 735f 6f76 6572 7669  :fatlinks_overvi
+000001c0: 6577 2720 7965 6172 5f63 7572 7265 6e74  ew' year_current
+000001d0: 2061 7320 7572 6c5f 6375 7272 656e 745f   as url_current_
+000001e0: 7965 6172 2025 7d0a 2020 2020 7b25 2069  year %}.    {% i
+000001f0: 6e63 6c75 6465 2022 6166 6174 2f70 6172  nclude "afat/par
+00000200: 7469 616c 732f 7965 6172 5f6e 6176 6967  tials/year_navig
+00000210: 6174 696f 6e2e 6874 6d6c 2220 7769 7468  ation.html" with
+00000220: 2075 726c 5f70 7265 7669 6f75 735f 7965   url_previous_ye
+00000230: 6172 3d75 726c 5f70 7265 7669 6f75 735f  ar=url_previous_
+00000240: 7965 6172 2075 726c 5f6e 6578 745f 7965  year url_next_ye
+00000250: 6172 3d75 726c 5f6e 6578 745f 7965 6172  ar=url_next_year
+00000260: 2075 726c 5f63 7572 7265 6e74 5f79 6561   url_current_yea
+00000270: 723d 7572 6c5f 6375 7272 656e 745f 7965  r=url_current_ye
+00000280: 6172 2025 7d0a 0a20 2020 203c 6469 7620  ar %}..    <div 
+00000290: 636c 6173 733d 2270 616e 656c 2070 616e  class="panel pan
+000002a0: 656c 2d64 6566 6175 6c74 223e 0a20 2020  el-default">.   
+000002b0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000002c0: 2270 616e 656c 2d62 6f64 7922 3e0a 2020  "panel-body">.  
+000002d0: 2020 2020 2020 2020 2020 3c74 6162 6c65            <table
+000002e0: 2063 6c61 7373 3d22 7461 626c 6520 7461   class="table ta
+000002f0: 626c 652d 7374 7269 7065 6420 7461 626c  ble-striped tabl
+00000300: 652d 686f 7665 7222 2069 643d 226c 696e  e-hover" id="lin
+00000310: 6b2d 6c69 7374 2220 7374 796c 653d 2277  k-list" style="w
+00000320: 6964 7468 3a20 3130 3025 3b22 3e0a 2020  idth: 100%;">.  
+00000330: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00000340: 6865 6164 3e0a 2020 2020 2020 2020 2020  head>.          
+00000350: 2020 2020 2020 2020 2020 3c74 723e 0a20            <tr>. 
+00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000370: 2020 2020 2020 203c 7468 3e7b 2520 7472         <th>{% tr
+00000380: 616e 736c 6174 6520 2246 6c65 6574 204e  anslate "Fleet N
+00000390: 616d 6522 2025 7d3c 2f74 683e 0a20 2020  ame" %}</th>.   
+000003a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003b0: 2020 2020 203c 7468 3e7b 2520 7472 616e       <th>{% tran
+000003c0: 736c 6174 6520 2246 6c65 6574 2054 7970  slate "Fleet Typ
+000003d0: 6522 2025 7d3c 2f74 683e 0a20 2020 2020  e" %}</th>.     
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 2020 203c 7468 3e7b 2520 7472 616e 736c     <th>{% transl
+00000400: 6174 6520 2243 7265 6174 6f72 2220 257d  ate "Creator" %}
+00000410: 3c2f 7468 3e0a 2020 2020 2020 2020 2020  </th>.          
+00000420: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00000430: 683e 7b25 2074 7261 6e73 6c61 7465 2022  h>{% translate "
+00000440: 4556 4520 5469 6d65 2220 257d 3c2f 7468  EVE Time" %}</th
+00000450: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000460: 2020 2020 2020 2020 2020 3c74 683e 7b25            <th>{%
+00000470: 2074 7261 6e73 6c61 7465 2022 2320 6f66   translate "# of
+00000480: 2046 4154 7322 2025 7d3c 2f74 683e 0a20   FATs" %}</th>. 
+00000490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004a0: 2020 2020 2020 203c 7468 3e3c 212d 2d20         <th><!-- 
+000004b0: 7b25 2074 7261 6e73 6c61 7465 2022 4163  {% translate "Ac
+000004c0: 7469 6f6e 7322 2025 7d20 2d2d 3e3c 2f74  tions" %} --></t
+000004d0: 683e 0a20 2020 2020 2020 2020 2020 2020  h>.             
+000004e0: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
+000004f0: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+00000500: 6865 6164 3e0a 0a20 2020 2020 2020 2020  head>..         
+00000510: 2020 2020 2020 203c 7462 6f64 793e 3c2f         <tbody></
+00000520: 7462 6f64 793e 0a0a 2020 2020 2020 2020  tbody>..        
+00000530: 2020 2020 2020 2020 3c74 666f 6f74 3e0a          <tfoot>.
+00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000550: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000570: 203c 7464 2063 6f6c 7370 616e 3d22 7b25   <td colspan="{%
+00000580: 2069 6620 7065 726d 732e 6166 6174 2e6d   if perms.afat.m
+00000590: 616e 6167 655f 6166 6174 2025 7d36 7b25  anage_afat %}6{%
+000005a0: 2065 6c73 6520 257d 357b 2520 656e 6469   else %}5{% endi
+000005b0: 6620 257d 223e 0a20 2020 2020 2020 2020  f %}">.         
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2020 207b 2520 696e 636c 7564 6520 2261     {% include "a
+000005e0: 6661 742f 7061 7274 6961 6c73 2f66 6174  fat/partials/fat
+000005f0: 6c69 6e6b 732f 6661 746c 696e 6b5f 6c69  links/fatlink_li
+00000600: 7374 5f6c 6567 656e 642e 6874 6d6c 2220  st_legend.html" 
+00000610: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00000620: 2020 2020 2020 2020 2020 203c 2f74 643e             </td>
+00000630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000640: 2020 2020 203c 2f74 723e 0a20 2020 2020       </tr>.     
+00000650: 2020 2020 2020 2020 2020 203c 2f74 666f             </tfo
+00000660: 6f74 3e0a 2020 2020 2020 2020 2020 2020  ot>.            
+00000670: 3c2f 7461 626c 653e 0a20 2020 2020 2020  </table>.       
+00000680: 203c 2f64 6976 3e0a 2020 2020 3c2f 6469   </div>.    </di
+00000690: 763e 0a0a 2020 2020 7b25 2074 7261 6e73  v>..    {% trans
+000006a0: 6c61 7465 2022 4465 6c65 7465 2046 4154  late "Delete FAT
+000006b0: 204c 696e 6b22 2061 7320 7472 616e 736c   Link" as transl
+000006c0: 6174 6564 5f74 6974 6c65 2025 7d0a 2020  ated_title %}.  
+000006d0: 2020 7b25 2069 6e63 6c75 6465 2022 6166    {% include "af
+000006e0: 6174 2f6d 6f64 616c 732f 6765 6e65 7261  at/modals/genera
+000006f0: 6c2e 6874 6d6c 2220 7769 7468 206d 6f64  l.html" with mod
+00000700: 616c 5f6e 616d 653d 2764 656c 6574 6546  al_name='deleteF
+00000710: 6174 4c69 6e6b 2720 6d6f 6461 6c5f 7469  atLink' modal_ti
+00000720: 746c 653d 7472 616e 736c 6174 6564 5f74  tle=translated_t
+00000730: 6974 6c65 2063 6f6e 6669 726d 5f62 7574  itle confirm_but
+00000740: 746f 6e5f 636c 6173 733d 2762 746e 2d64  ton_class='btn-d
+00000750: 616e 6765 7227 2025 7d0a 0a20 2020 207b  anger' %}..    {
+00000760: 2520 7472 616e 736c 6174 6520 2243 6c6f  % translate "Clo
+00000770: 7365 2045 5349 2046 6c65 6574 2054 7261  se ESI Fleet Tra
+00000780: 636b 696e 6722 2061 7320 7472 616e 736c  cking" as transl
+00000790: 6174 6564 5f74 6974 6c65 2025 7d0a 2020  ated_title %}.  
+000007a0: 2020 7b25 2069 6e63 6c75 6465 2027 6166    {% include 'af
+000007b0: 6174 2f6d 6f64 616c 732f 6765 6e65 7261  at/modals/genera
+000007c0: 6c2e 6874 6d6c 2720 7769 7468 206d 6f64  l.html' with mod
+000007d0: 616c 5f6e 616d 653d 2763 616e 6365 6c45  al_name='cancelE
+000007e0: 7369 466c 6565 7427 206d 6f64 616c 5f74  siFleet' modal_t
+000007f0: 6974 6c65 3d74 7261 6e73 6c61 7465 645f  itle=translated_
+00000800: 7469 746c 6520 636f 6e66 6972 6d5f 6275  title confirm_bu
+00000810: 7474 6f6e 5f63 6c61 7373 3d27 6274 6e2d  tton_class='btn-
+00000820: 6461 6e67 6572 2720 257d 0a7b 2520 656e  danger' %}.{% en
+00000830: 6462 6c6f 636b 2025 7d0a 0a7b 2520 626c  dblock %}..{% bl
+00000840: 6f63 6b20 6578 7472 615f 6373 7320 257d  ock extra_css %}
+00000850: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
+00000860: 2762 756e 646c 6573 2f64 6174 6174 6162  'bundles/datatab
+00000870: 6c65 732d 6373 732e 6874 6d6c 2720 257d  les-css.html' %}
+00000880: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
+00000890: 2261 6661 742f 6275 6e64 6c65 732f 6166  "afat/bundles/af
+000008a0: 6174 2d63 7373 2e68 746d 6c22 2025 7d0a  at-css.html" %}.
+000008b0: 7b25 2065 6e64 626c 6f63 6b20 257d 0a0a  {% endblock %}..
+000008c0: 7b25 2062 6c6f 636b 2065 7874 7261 5f6a  {% block extra_j
+000008d0: 6176 6173 6372 6970 7420 257d 0a20 2020  avascript %}.   
+000008e0: 207b 2520 696e 636c 7564 6520 2762 756e   {% include 'bun
+000008f0: 646c 6573 2f64 6174 6174 6162 6c65 732d  dles/datatables-
+00000900: 6a73 2e68 746d 6c27 2025 7d0a 2020 2020  js.html' %}.    
+00000910: 7b25 2069 6e63 6c75 6465 2027 6275 6e64  {% include 'bund
+00000920: 6c65 732f 6d6f 6d65 6e74 2d6a 732e 6874  les/moment-js.ht
+00000930: 6d6c 2720 7769 7468 206c 6f63 616c 653d  ml' with locale=
+00000940: 5472 7565 2025 7d0a 2020 2020 7b25 2069  True %}.    {% i
+00000950: 6e63 6c75 6465 2022 6166 6174 2f62 756e  nclude "afat/bun
+00000960: 646c 6573 2f61 6661 742d 6a73 2e68 746d  dles/afat-js.htm
+00000970: 6c22 2025 7d0a 0a20 2020 203c 7363 7269  l" %}..    <scri
+00000980: 7074 3e0a 2020 2020 2020 2020 6c65 7420  pt>.        let 
+00000990: 6166 6174 5365 7474 696e 6773 203d 207b  afatSettings = {
+000009a0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+000009b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000009c0: 2020 2020 6c69 6e6b 4c69 7374 3a20 277b      linkList: '{
+000009d0: 2520 7572 6c20 2761 6661 743a 6661 746c  % url 'afat:fatl
+000009e0: 696e 6b73 5f61 6a61 785f 6765 745f 6661  inks_ajax_get_fa
+000009f0: 746c 696e 6b73 5f62 795f 7965 6172 2720  tlinks_by_year' 
+00000a00: 7965 6172 2025 7d27 0a20 2020 2020 2020  year %}'.       
+00000a10: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000a20: 2020 2020 7065 726d 6973 7369 6f6e 733a      permissions:
+00000a30: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000a40: 2020 2061 6464 4661 744c 696e 6b3a 207b     addFatLink: {
+00000a50: 2520 6966 2070 6572 6d73 2e61 6661 742e  % if perms.afat.
+00000a60: 6164 645f 6661 746c 696e 6b20 257d 7472  add_fatlink %}tr
+00000a70: 7565 7b25 2065 6c73 6520 257d 6661 6c73  ue{% else %}fals
+00000a80: 657b 2520 656e 6469 6620 257d 2c0a 2020  e{% endif %},.  
+00000a90: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00000aa0: 6e61 6765 4166 6174 3a20 7b25 2069 6620  nageAfat: {% if 
+00000ab0: 7065 726d 732e 6166 6174 2e6d 616e 6167  perms.afat.manag
+00000ac0: 655f 6166 6174 2025 7d74 7275 657b 2520  e_afat %}true{% 
+00000ad0: 656c 7365 2025 7d66 616c 7365 7b25 2065  else %}false{% e
+00000ae0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00000af0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000b00: 2020 2074 7261 6e73 6c61 7469 6f6e 3a20     translation: 
+00000b10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000b20: 2020 6461 7461 5461 626c 653a 207b 0a20    dataTable: {. 
+00000b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b40: 2020 2066 696c 7465 723a 207b 0a20 2020     filter: {.   
 00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 5b31 2c20 2764 6573 6327 5d2c 0a20    [1, 'desc'],. 
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 2020 205b 302c 2027 6173 6327 5d0a 2020     [0, 'asc'].  
-00000b90: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000ba0: 0a20 2020 2020 2020 2020 2020 207d 293b  .            });
-00000bb0: 0a20 2020 2020 2020 207d 293b 0a20 2020  .        });.   
-00000bc0: 203c 2f73 6372 6970 743e 0a7b 2520 656e   </script>.{% en
-00000bd0: 6462 6c6f 636b 2025 7d0a                 dblock %}.
+00000b60: 2020 2020 2076 6961 4573 693a 2027 7b25       viaEsi: '{%
+00000b70: 2074 7261 6e73 6c61 7465 2027 7669 6120   translate 'via 
+00000b80: 4553 4927 2025 7d27 0a20 2020 2020 2020  ESI' %}'.       
+00000b90: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00000bb0: 2c0a 2020 2020 2020 2020 2020 2020 7d2c  ,.            },
+00000bc0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+00000bd0: 616c 3a20 7b0a 2020 2020 2020 2020 2020  al: {.          
+00000be0: 2020 2020 2020 6465 6c65 7465 4661 744c        deleteFatL
+00000bf0: 696e 6b4d 6f64 616c 3a20 7b0a 2020 2020  inkModal: {.    
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c10: 656c 656d 656e 743a 2027 2364 656c 6574  element: '#delet
+00000c20: 6546 6174 4c69 6e6b 4d6f 6461 6c27 0a20  eFatLinkModal'. 
+00000c30: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00000c40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000c50: 2020 6361 6e63 656c 4573 6946 6c65 6574    cancelEsiFleet
+00000c60: 4d6f 6461 6c3a 207b 0a20 2020 2020 2020  Modal: {.       
+00000c70: 2020 2020 2020 2020 2020 2020 2065 6c65               ele
+00000c80: 6d65 6e74 3a20 2723 6361 6e63 656c 4573  ment: '#cancelEs
+00000c90: 6946 6c65 6574 4d6f 6461 6c27 0a20 2020  iFleetModal'.   
+00000ca0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00000cb0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000cc0: 2020 2020 207d 0a20 2020 203c 2f73 6372       }.    </scr
+00000cd0: 6970 743e 0a0a 2020 2020 7b25 2069 6e63  ipt>..    {% inc
+00000ce0: 6c75 6465 2022 6166 6174 2f62 756e 646c  lude "afat/bundl
+00000cf0: 6573 2f61 6661 742d 6661 746c 6973 742d  es/afat-fatlist-
+00000d00: 6a73 2e68 746d 6c22 2025 7d0a 2020 2020  js.html" %}.    
+00000d10: 7b25 2069 6e63 6c75 6465 2027 6275 6e64  {% include 'bund
+00000d20: 6c65 732f 6669 6c74 6572 6472 6f70 646f  les/filterdropdo
+00000d30: 776e 2d6a 732e 6874 6d6c 2720 257d 0a7b  wn-js.html' %}.{
+00000d40: 2520 656e 6462 6c6f 636b 2025 7d0a       % endblock %}.
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_corporation_year_overview.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_corporation_year_overview.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% extends 'afat/base.html' %}
 
-{% load afat_versioned_static %}
 {% load i18n %}
 {% load filters %}
 
 {% block page_title %}{{ corporation }} {% translate "Fleet Activity" %}{% endblock %}
 
 {% block afat_header %}
     <br>
@@ -57,10 +56,9 @@
                 </tbody>
             </table>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/allianceauth-afat.min.css' %}">
+    {% include "afat/bundles/afat-css.html" %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-{% extends 'afat/base.html' %} {% load afat_versioned_static %} {% load i18n %}
-{% load filters %} {% block page_title %}{{ corporation }} {% translate "Fleet
-Activity" %}{% endblock %} {% block afat_header %}
+{% extends 'afat/base.html' %} {% load i18n %} {% load filters %} {% block
+page_title %}{{ corporation }} {% translate "Fleet Activity" %}{% endblock %}
+{% block afat_header %}
 {% include "afat/partials/menu.html" %}
 ***** {{ corporation }} {% translate "Fleet Activity" %} *****
 {% endblock %} {% block afat_body %} {% url 'afat:statistics_corporation'
 corpid year_prev as url_previous_year %} {% url 'afat:statistics_corporation'
 corpid year_next as url_next_year %} {% url 'afat:statistics_corporation'
 corpid year_current as url_current_year %} {% include "afat/partials/
 year_navigation.html" with url_previous_year=url_previous_year
 url_next_year=url_next_year url_current_year=url_current_year %}
 {% translate "Month" {% translate "FATs" {% translate "Avg
 %}                   %}                  FATs" %}
 {                                                          {% if corporation !=
 { month.0|month_name {{ month.1 }}       {{ month.2 }}     'No Alliance' %}  {%
 }}                                                         endif %}
-{% endblock %} {% block extra_css %}
-
- {% endblock %}
+{% endblock %} {% block extra_css %} {% include "afat/bundles/afat-css.html" %}
+{% endblock %}
```

### Comparing `allianceauth_afat-2.9.6/afat/templates/afat/view/statistics/statistics_overview.html` & `allianceauth_afat-2.9.7/afat/templates/afat/view/statistics/statistics_overview.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% extends 'afat/base.html' %}
 
-{% load afat_versioned_static %}
 {% load i18n %}
 {% load evelinks %}
 {% load filters %}
 
 {% block page_title %}{% translate 'Fleet Activity' %}{% endblock %}
 
 {% block afat_header %}
@@ -28,10 +27,9 @@
         {% if perms.afat.stats_corporation_own or perms.afat.stats_corporation_other or perms.afat.manage_afat %}
             {% include "afat/partials/statistics/overview/tabs/corps.html" %}
         {% endif %}
     </div>
 {% endblock %}
 
 {% block extra_css %}
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/aa-bootstrap-fix.min.css' %}">
-    <link rel="stylesheet" type="text/css" href="{% afat_static 'afat/css/allianceauth-afat.min.css' %}">
+    {% include "afat/bundles/afat-css.html" %}
 {% endblock %}
```

### Comparing `allianceauth_afat-2.9.6/afat/templatetags/filters.py` & `allianceauth_afat-2.9.7/afat/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/fixtures/allianceauth.json` & `allianceauth_afat-2.9.7/afat/tests/fixtures/allianceauth.json`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/fixtures/generate_fat_links.py` & `allianceauth_afat-2.9.7/afat/tests/fixtures/generate_fat_links.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/fixtures/load_allianceauth.py` & `allianceauth_afat-2.9.7/afat/tests/fixtures/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_access.py` & `allianceauth_afat-2.9.7/afat/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_helpers.py` & `allianceauth_afat-2.9.7/afat/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_templatetags.py` & `allianceauth_afat-2.9.7/afat/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_views_dashboard.py` & `allianceauth_afat-2.9.7/afat/tests/test_views_dashboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_views_fatlinks.py` & `allianceauth_afat-2.9.7/afat/tests/test_views_fatlinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_views_logs.py` & `allianceauth_afat-2.9.7/afat/tests/test_views_logs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/tests/test_views_statistics.py` & `allianceauth_afat-2.9.7/afat/tests/test_views_statistics.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/urls.py` & `allianceauth_afat-2.9.7/afat/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/utils.py` & `allianceauth_afat-2.9.7/afat/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/views/dashboard.py` & `allianceauth_afat-2.9.7/afat/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/views/fatlinks.py` & `allianceauth_afat-2.9.7/afat/views/fatlinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/views/logs.py` & `allianceauth_afat-2.9.7/afat/views/logs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/afat/views/statistics.py` & `allianceauth_afat-2.9.7/afat/views/statistics.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-2.9.6/allianceauth_afat.egg-info/PKG-INFO` & `allianceauth_afat-2.9.7/allianceauth_afat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: allianceauth-afat
-Version: 2.9.6
+Version: 2.9.7
 Summary: Another Fleet Activity Tracking tool for Alliance Auth
 Home-page: https://github.com/ppfeufer/allianceauth-afat
 Author: Peter Pfeufer
-Author-email: development@ppfeufer.de
+Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
-Maintainer-email: development@ppfeufer.de
+Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/allianceauth-afat/issues
 Project-URL: Changelog, https://github.com/ppfeufer/allianceauth-afat/blob/master/CHANGELOG.md
 Keywords: allianceauth,eveonline,theme,template
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Alliance Auth AFAT - Another Fleet Activity Tracker
 
 [![Version](https://img.shields.io/pypi/v/allianceauth-afat?label=release)](https://pypi.org/project/allianceauth-afat/)
 [![License](https://img.shields.io/badge/license-GPLv3-green)](https://pypi.org/project/allianceauth-afat/)
@@ -56,14 +54,15 @@
 - [Features and highlights](#features-and-highlights)
 - [Screenshots](#screenshots)
 - [Installation](#installation)
 - [Updating](#updating)
 - [Data Migration](#data-migration)
     - [From Alliance Auth native FAT](#import-from-native-fat)
     - [From ImicusFAT](#import-from-imicusfat)
+        - [Uninstall ImicusFAT](#uninstall-imicusfat)
 - [Settings](#settings)
 - [Permissions](#permissions)
 - [Changelog](#changelog)
 - [Credits](#credits)
 - [Contributing](#contributing)
 
 
@@ -196,14 +195,44 @@
 
 To import from the ImicusFAT module, simply run the following command:
 
 ```shell
 python myauth/manage.py afat_import_from_imicusfat
 ```
 
+#### Uninstall ImicusFAT
+
+Now that you've migrated, you can uninstal `ImicusFAT`.
+
+First, remove all Django migrations for `ImicusFAT` with:
+
+```shell
+python manage.py migrate imicusfat zero
+```
+
+This will remove all migrations for `ImicusFAT` including its DB tables.
+
+Should this command throw an error, a bit of manual labor is needed, but nothing you
+can't handle, I'm sure.
+
+```shell
+python manage.py migrate imicusfat zero --fake
+```
+
+And remove all DB tables beginning with `imicusfat_` from your DB manually afterwards.
+
+Now that the DB is cleaned up, time to remove te app.
+
+```shell
+pip uninstall allianceauth-imicusfat
+```
+
+Now remove `imicusfat` from your `INSTALLED_APPS` in your `local.py`, restart
+supervisor and ... Done!
+
 
 ## Settings
 
 To customize the module, the following settings are available.
 
 | Name                             | Description                                                     | Default Value           |
 |:---------------------------------|:----------------------------------------------------------------|:------------------------|
@@ -238,11 +267,14 @@
 
 Please make sure to read the [contribution guidelines](https://github.com/ppfeufer/allianceauth-afat/blob/master/CONTRIBUTING.md)
 (I promise, it's not much, just some basics)
 
 
 ## Credits
 
-AFAT is maintained by @ppfeufer is based on
-[ImicusFAT](https://gitlab.com/evictus.iou/allianceauth-imicusfat) maintained
-by @exiom with @Aproia and @ppfeufer (no longer) which is based on
+AFAT is maintained by @ppfeufer and is based on
+[ImicusFAT](https://gitlab.com/evictus.iou/allianceauth-imicusfat)
+by @exiom with @Aproia and @ppfeufer which is based on
 [allianceauth-bfat](https://gitlab.com/colcrunch/allianceauth-bfat) by @colcrunch
+
+Both of these modules are no longer maintained and are deprecated. Both modules will
+not run with the latest stable releases of Alliance Auth.
```

### Comparing `allianceauth_afat-2.9.6/allianceauth_afat.egg-info/SOURCES.txt` & `allianceauth_afat-2.9.7/allianceauth_afat.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 afat/__init__.py
 afat/admin.py
 afat/app_settings.py
 afat/apps.py
@@ -20,26 +21,36 @@
 afat/docs/images/fatlink-list.png
 afat/docs/images/manually-close-esi-links.png
 afat/docs/images/ship-type-overview.png
 afat/docs/images/statistics-dashboard.png
 afat/helper/fatlinks.py
 afat/helper/time.py
 afat/helper/views_helper.py
+afat/locale/.gitkeep
+afat/locale/de/LC_MESSAGES/.gitkeep
 afat/locale/de/LC_MESSAGES/django.mo
 afat/locale/de/LC_MESSAGES/django.po
+afat/locale/en/LC_MESSAGES/.gitkeep
 afat/locale/en/LC_MESSAGES/django.mo
 afat/locale/en/LC_MESSAGES/django.po
+afat/locale/es/LC_MESSAGES/.gitkeep
 afat/locale/es/LC_MESSAGES/django.mo
 afat/locale/es/LC_MESSAGES/django.po
+afat/locale/fr_FR/LC_MESSAGES/.gitkeep
 afat/locale/fr_FR/LC_MESSAGES/django.po
+afat/locale/it_IT/LC_MESSAGES/.gitkeep
 afat/locale/it_IT/LC_MESSAGES/django.po
+afat/locale/ja/LC_MESSAGES/.gitkeep
 afat/locale/ja/LC_MESSAGES/django.po
+afat/locale/ko_KR/LC_MESSAGES/.gitkeep
 afat/locale/ko_KR/LC_MESSAGES/django.po
+afat/locale/ru/LC_MESSAGES/.gitkeep
 afat/locale/ru/LC_MESSAGES/django.mo
 afat/locale/ru/LC_MESSAGES/django.po
+afat/locale/zh_Hans/LC_MESSAGES/.gitkeep
 afat/locale/zh_Hans/LC_MESSAGES/django.mo
 afat/locale/zh_Hans/LC_MESSAGES/django.po
 afat/management/commands/afat_import_from_allianceauth_fat.py
 afat/management/commands/afat_import_from_imicusfat.py
 afat/management/commands/afat_migrate_manual_fat_log.py
 afat/migrations/0001_initial.py
 afat/migrations/0002_manualfat.py
@@ -61,30 +72,34 @@
 afat/migrations/0018_auto_20210420_2016.py
 afat/migrations/0019_add_several_indices.py
 afat/migrations/0020_auto_20210617_1037.py
 afat/migrations/0021_alter_afatlink_fleet.py
 afat/migrations/__init__.py
 afat/static/afat/css/aa-bootstrap-fix.css
 afat/static/afat/css/aa-bootstrap-fix.min.css
-afat/static/afat/css/allianceauth-afat.css
-afat/static/afat/css/allianceauth-afat.min.css
+afat/static/afat/css/afat.css
+afat/static/afat/css/afat.min.css
 afat/static/afat/javascript/afat-dashboard.js
 afat/static/afat/javascript/afat-dashboard.min.js
 afat/static/afat/javascript/afat-fatlink-details.js
 afat/static/afat/javascript/afat-fatlink-details.min.js
 afat/static/afat/javascript/afat-fatlist.js
 afat/static/afat/javascript/afat-fatlist.min.js
 afat/static/afat/javascript/afat-logs.js
 afat/static/afat/javascript/afat-logs.min.js
-afat/static/afat/javascript/allianceauth-afat.js
-afat/static/afat/javascript/allianceauth-afat.min.js
-afat/static/afat/libs/chartjs/chart.min.js
-afat/static/afat/libs/datatables/plugins/datetime.js
-afat/static/afat/libs/datatables/plugins/datetime.min.js
+afat/static/afat/javascript/afat.js
+afat/static/afat/javascript/afat.min.js
+afat/static/afat/libs/Chart.js/2.7.2/chart.min.js
 afat/templates/afat/base.html
+afat/templates/afat/bundles/afat-css.html
+afat/templates/afat/bundles/afat-dashboard-js.html
+afat/templates/afat/bundles/afat-fatlink-details-js.html
+afat/templates/afat/bundles/afat-fatlist-js.html
+afat/templates/afat/bundles/afat-js.html
+afat/templates/afat/bundles/afat-logs-js.html
 afat/templates/afat/bundles/chartjs-js.html
 afat/templates/afat/modals/general.html
 afat/templates/afat/partials/menu.html
 afat/templates/afat/partials/month_navigation.html
 afat/templates/afat/partials/year_navigation.html
 afat/templates/afat/partials/dashboard/tabs_navigation.html
 afat/templates/afat/partials/dashboard/tabs/fatlinks.html
```

### Comparing `allianceauth_afat-2.9.6/setup.cfg` & `allianceauth_afat-2.9.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [metadata]
 name = allianceauth_afat
 version = attr: afat.__version__
 description = Another Fleet Activity Tracking tool for Alliance Auth
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Peter Pfeufer
-author_email = development@ppfeufer.de
+author_email = develop@ppfeufer.de
 maintainer = Peter Pfeufer
-maintainer_email = development@ppfeufer.de
+maintainer_email = develop@ppfeufer.de
 license = GPL-3.0
 license_file = LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 home_page = https://github.com/ppfeufer/allianceauth-afat
@@ -36,18 +34,18 @@
 project_urls = 
 	Issue / Bug Reports = https://github.com/ppfeufer/allianceauth-afat/issues
 	Changelog = https://github.com/ppfeufer/allianceauth-afat/blob/master/CHANGELOG.md
 
 [options]
 packages = find_namespace:
 install_requires = 
-	allianceauth>=2.14.0
-	allianceauth-app-utils>=1.12.0
-	unidecode>=1.3.3
-python_requires = ~=3.7
+	allianceauth>=2.15.1
+	allianceauth-app-utils>=1.14.1
+	unidecode>=1.3.4
+python_requires = ~=3.8
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = afat*
 
 [options.package_data]
```

