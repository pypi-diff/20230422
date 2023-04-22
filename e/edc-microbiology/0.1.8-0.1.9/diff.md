# Comparing `tmp/edc-microbiology-0.1.8.tar.gz` & `tmp/edc-microbiology-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-microbiology-0.1.8.tar", last modified: Sun Sep 25 18:46:11 2022, max compression
+gzip compressed data, was "edc-microbiology-0.1.9.tar", last modified: Wed Oct  5 19:11:56 2022, max compression
```

## Comparing `edc-microbiology-0.1.8.tar` & `edc-microbiology-0.1.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.047987 edc-microbiology-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      108 2022-02-16 18:04:06.000000 edc-microbiology-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-02-16 18:04:06.000000 edc-microbiology-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.035735 edc-microbiology-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.039055 edc-microbiology-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 18:42:08.000000 edc-microbiology-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-02-16 14:40:34.000000 edc-microbiology-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-09-25 18:46:11.048096 edc-microbiology-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      734 2022-09-25 18:46:02.000000 edc-microbiology-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 18:46:01.000000 edc-microbiology-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.041522 edc-microbiology-0.1.8/edc_microbiology/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:04:06.000000 edc-microbiology-0.1.8/edc_microbiology/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      536 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-06-01 18:29:20.000000 edc-microbiology-0.1.8/edc_microbiology/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      195 2022-02-28 17:41:48.000000 edc-microbiology-0.1.8/edc_microbiology/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      607 2022-06-01 18:29:26.000000 edc-microbiology-0.1.8/edc_microbiology/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      378 2022-02-16 18:04:06.000000 edc-microbiology-0.1.8/edc_microbiology/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1851 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-06-01 18:29:42.000000 edc-microbiology-0.1.8/edc_microbiology/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6981 2022-09-25 18:42:08.000000 edc-microbiology-0.1.8/edc_microbiology/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      420 2022-06-01 18:29:51.000000 edc-microbiology-0.1.8/edc_microbiology/forms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.043869 edc-microbiology-0.1.8/edc_microbiology/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    41348 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      936 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0002_auto_20220223_2236.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3477 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0003_auto_20220223_2256.py
--rw-r--r--   0 erikvw     (501) staff       (20)      589 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0004_auto_20220223_2258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1961 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0005_auto_20220224_1509.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4651 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0006_auto_20220224_1826.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2621 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0007_auto_20220224_1910.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6341 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0008_auto_20220224_1926.py
--rw-r--r--   0 erikvw     (501) staff       (20)      803 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/0009_auto_20220711_1230.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.045097 edc-microbiology-0.1.8/edc_microbiology/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      401 2022-02-28 17:41:48.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1838 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/blood_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      944 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/csf_genexpert.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1709 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/histopathology.py
--rw-r--r--   0 erikvw     (501) staff       (20)      891 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/sputum_afb.py
--rw-r--r--   0 erikvw     (501) staff       (20)      878 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/sputum_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      960 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/sputum_genexpert.py
--rw-r--r--   0 erikvw     (501) staff       (20)      998 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/urinary_lam.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1237 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/model_mixins/urine_culture.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.045954 edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-02-28 17:41:48.000000 edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      495 2022-02-28 17:41:48.000000 edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/blood_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)      449 2022-02-28 17:41:48.000000 edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/histopathology.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1029 2022-06-01 18:28:40.000000 edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/microbiology.py
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/urine_culture.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.046155 edc-microbiology-0.1.8/edc_microbiology/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.047547 edc-microbiology-0.1.8/edc_microbiology/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2022-02-17 01:44:12.000000 edc-microbiology-0.1.8/edc_microbiology/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.047873 edc-microbiology-0.1.8/edc_microbiology/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/edc_microbiology/tests/tests/test_auth.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15363 2022-06-01 18:59:45.000000 edc-microbiology-0.1.8/edc_microbiology/tests/tests/test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      307 2022-02-16 18:20:26.000000 edc-microbiology-0.1.8/edc_microbiology/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 18:46:11.042268 edc-microbiology-0.1.8/edc_microbiology.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-09-25 18:46:11.000000 edc-microbiology-0.1.8/edc_microbiology.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2583 2022-09-25 18:46:11.000000 edc-microbiology-0.1.8/edc_microbiology.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 18:46:11.000000 edc-microbiology-0.1.8/edc_microbiology.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-02-16 17:07:31.000000 edc-microbiology-0.1.8/edc_microbiology.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       17 2022-09-25 18:46:11.000000 edc-microbiology-0.1.8/edc_microbiology.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1724 2022-08-26 02:09:03.000000 edc-microbiology-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-09-25 18:46:11.048397 edc-microbiology-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.872375 edc-microbiology-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      108 2022-02-16 18:04:06.000000 edc-microbiology-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-02-16 18:04:06.000000 edc-microbiology-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.859449 edc-microbiology-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.862432 edc-microbiology-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1660 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 18:42:08.000000 edc-microbiology-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-02-16 14:40:34.000000 edc-microbiology-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-10-05 19:11:56.872476 edc-microbiology-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      734 2022-09-25 18:46:02.000000 edc-microbiology-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-05 19:11:49.000000 edc-microbiology-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.865078 edc-microbiology-0.1.9/edc_microbiology/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:04:06.000000 edc-microbiology-0.1.9/edc_microbiology/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      536 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      177 2022-06-01 18:29:20.000000 edc-microbiology-0.1.9/edc_microbiology/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      195 2022-02-28 17:41:48.000000 edc-microbiology-0.1.9/edc_microbiology/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      607 2022-06-01 18:29:26.000000 edc-microbiology-0.1.9/edc_microbiology/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      378 2022-02-16 18:04:06.000000 edc-microbiology-0.1.9/edc_microbiology/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1851 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2638 2022-06-01 18:29:42.000000 edc-microbiology-0.1.9/edc_microbiology/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7469 2022-10-05 19:11:49.000000 edc-microbiology-0.1.9/edc_microbiology/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      420 2022-06-01 18:29:51.000000 edc-microbiology-0.1.9/edc_microbiology/forms.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.867419 edc-microbiology-0.1.9/edc_microbiology/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    41348 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      936 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0002_auto_20220223_2236.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3477 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0003_auto_20220223_2256.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      589 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0004_auto_20220223_2258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1961 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0005_auto_20220224_1509.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4651 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0006_auto_20220224_1826.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2621 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0007_auto_20220224_1910.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6341 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0008_auto_20220224_1926.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      803 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/0009_auto_20220711_1230.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.869061 edc-microbiology-0.1.9/edc_microbiology/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      401 2022-02-28 17:41:48.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1838 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/blood_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      944 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/csf_genexpert.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1709 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/histopathology.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      891 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/sputum_afb.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      878 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/sputum_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      960 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/sputum_genexpert.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      998 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/urinary_lam.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1237 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/model_mixins/urine_culture.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.870224 edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-02-28 17:41:48.000000 edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      495 2022-02-28 17:41:48.000000 edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/blood_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      449 2022-02-28 17:41:48.000000 edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/histopathology.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1029 2022-06-01 18:28:40.000000 edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/microbiology.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-06-01 18:59:45.000000 edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/urine_culture.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1196 2022-10-05 19:11:49.000000 edc-microbiology-0.1.9/edc_microbiology/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.870449 edc-microbiology-0.1.9/edc_microbiology/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.871878 edc-microbiology-0.1.9/edc_microbiology/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      818 2022-10-05 19:11:49.000000 edc-microbiology-0.1.9/edc_microbiology/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.872257 edc-microbiology-0.1.9/edc_microbiology/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/edc_microbiology/tests/tests/test_auth.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15821 2022-10-05 19:11:49.000000 edc-microbiology-0.1.9/edc_microbiology/tests/tests/test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      307 2022-02-16 18:20:26.000000 edc-microbiology-0.1.9/edc_microbiology/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-05 19:11:56.865832 edc-microbiology-0.1.9/edc_microbiology.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-10-05 19:11:56.000000 edc-microbiology-0.1.9/edc_microbiology.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2583 2022-10-05 19:11:56.000000 edc-microbiology-0.1.9/edc_microbiology.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-05 19:11:56.000000 edc-microbiology-0.1.9/edc_microbiology.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-02-16 17:07:31.000000 edc-microbiology-0.1.9/edc_microbiology.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       17 2022-10-05 19:11:56.000000 edc-microbiology-0.1.9/edc_microbiology.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1734 2022-08-26 02:09:03.000000 edc-microbiology-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1764 2022-10-05 19:11:49.000000 edc-microbiology-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1269 2022-10-05 19:11:56.872820 edc-microbiology-0.1.9/setup.cfg
```

### Comparing `edc-microbiology-0.1.8/.github/workflows/build.yml` & `edc-microbiology-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/.gitignore` & `edc-microbiology-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/.pre-commit-config.yaml` & `edc-microbiology-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/LICENSE` & `edc-microbiology-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/PKG-INFO` & `edc-microbiology-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-microbiology
-Version: 0.1.8
+Version: 0.1.9
 Summary: Microbiology model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microbiology
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microbiology,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-microbiology-0.1.8/README.rst` & `edc-microbiology-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/admin.py` & `edc-microbiology-0.1.9/edc_microbiology/admin.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/auth_objects.py` & `edc-microbiology-0.1.9/edc_microbiology/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/choices.py` & `edc-microbiology-0.1.9/edc_microbiology/choices.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/fieldsets.py` & `edc-microbiology-0.1.9/edc_microbiology/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/form_validators.py` & `edc-microbiology-0.1.9/edc_microbiology/form_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from edc_consent.form_validators import ConsentFormValidatorMixin
 from edc_constants.constants import OTHER, POS, YES
 from edc_crf.crf_form_validator import CrfFormValidator
+from edc_crf.crf_form_validator_mixins import BaseFormValidatorMixin
+from edc_form_validators import FormValidator
 from edc_form_validators.extra_mixins import StudyDayFormValidatorMixin
 
 from .constants import BACTERIA
 
 
 class BloodCultureFormValidatorMixin:
     def validate_blood_culture(self: CrfFormValidator):
@@ -185,24 +188,23 @@
         self.applicable_if(
             POS,
             field="urinary_lam_result",
             field_applicable="urinary_lam_result_grade",
         )
 
 
-class MicrobiologyFormValidator(
+class MicrobiologyFormValidatorMixin(
     StudyDayFormValidatorMixin,
     UrinaryLamFormValidatorMixin,
     SputumGenexpertFormValidatorMixin,
     SputumCultureFormValidatorMixin,
     SputumAfbFormValidatorMixin,
     BloodCultureFormValidatorMixin,
     HistopathologyFormValidatorMixin,
     UrineCultureFormValidatorMixin,
-    CrfFormValidator,
 ):
     def clean(self):
         self.validate_study_day_with_datetime(
             subject_identifier=self.subject_identifier,
             study_day=self.cleaned_data.get("day_blood_taken"),
             compare_date=self.cleaned_data.get("blood_taken_date"),
             study_day_field="day_blood_taken",
@@ -224,7 +226,24 @@
         self.validate_sputum_genexpert()
 
         self.validate_blood_culture()
 
         self.validate_histopathology()
 
         self.validate_urine_culture()
+
+
+class MicrobiologyFormValidator(MicrobiologyFormValidatorMixin, CrfFormValidator):
+    """Assumes this is a CRF"""
+
+    pass
+
+
+class MicrobiologyPrnFormValidator(
+    MicrobiologyFormValidatorMixin,
+    ConsentFormValidatorMixin,
+    BaseFormValidatorMixin,
+    FormValidator,
+):
+    """Assumes this is a PRN"""
+
+    pass
```

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0001_initial.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0002_auto_20220223_2236.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0002_auto_20220223_2236.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0003_auto_20220223_2256.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0003_auto_20220223_2256.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0004_auto_20220223_2258.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0004_auto_20220223_2258.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0005_auto_20220224_1509.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0005_auto_20220224_1509.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0006_auto_20220224_1826.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0006_auto_20220224_1826.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0007_auto_20220224_1910.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0007_auto_20220224_1910.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0008_auto_20220224_1926.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0008_auto_20220224_1926.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/migrations/0009_auto_20220711_1230.py` & `edc-microbiology-0.1.9/edc_microbiology/migrations/0009_auto_20220711_1230.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/blood_culture.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/blood_culture.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/csf_genexpert.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/csf_genexpert.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/histopathology.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/histopathology.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/sputum_afb.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/sputum_afb.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/sputum_culture.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/sputum_culture.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/sputum_genexpert.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/sputum_genexpert.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/urinary_lam.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/urinary_lam.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/model_mixins/urine_culture.py` & `edc-microbiology-0.1.9/edc_microbiology/model_mixins/urine_culture.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/modeladmin_mixins/microbiology.py` & `edc-microbiology-0.1.9/edc_microbiology/modeladmin_mixins/microbiology.py`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/models.py` & `edc-microbiology-0.1.9/edc_microbiology/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,23 +11,31 @@
     SputumCultureModelMixin,
     SputumGenexpertModelMixin,
     UrinaryLamModelMixin,
     UrineCultureModelMixin,
 )
 
 
-class Microbiology(
-    UniqueSubjectIdentifierFieldMixin,
-    UrinaryLamModelMixin,
-    SputumGenexpertModelMixin,
-    SputumCultureModelMixin,
-    SputumAfbModelMixin,
-    UrineCultureModelMixin,
+class MicrobiologyModelMixin(
     BloodCultureModelMixin,
     HistopathologyModelMixin,
+    SputumAfbModelMixin,
+    SputumCultureModelMixin,
+    SputumGenexpertModelMixin,
+    UrinaryLamModelMixin,
+    UrineCultureModelMixin,
+    models.Model,
+):
+    class Meta:
+        abstract = True
+
+
+class Microbiology(
+    UniqueSubjectIdentifierFieldMixin,
+    MicrobiologyModelMixin,
     SiteModelMixin,
     BaseUuidModel,
 ):
 
     report_datetime = models.DateTimeField(default=get_utcnow)
 
     on_site = CurrentSiteManager()
```

### Comparing `edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-rsa-local-private.pem` & `edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/tests/etc/user-rsa-restricted-private.pem` & `edc-microbiology-0.1.9/edc_microbiology/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/edc_microbiology/tests/tests/test_form.py` & `edc-microbiology-0.1.9/edc_microbiology/tests/tests/test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+from decimal import Decimal
+
 from django import forms
 from django.core.exceptions import ValidationError
-from django.test import TestCase
+from django.test import TestCase, tag
 from edc_constants.constants import NO, NOT_APPLICABLE, OTHER, POS, YES
+from edc_crf.crf_form_validator_mixins import BaseFormValidatorMixin
+from edc_form_validators import FormValidator
 from edc_registration.models import RegisteredSubject
 from edc_utils import get_utcnow
 from edc_visit_schedule.constants import DAY1
 
 from edc_microbiology.constants import (
     BACTERIA,
     CRYPTOCOCCUS_NEOFORMANS,
     KLEBSIELLA_SPP,
     NO_GROWTH,
 )
-from edc_microbiology.form_validators import MicrobiologyFormValidator
+from edc_microbiology.form_validators import MicrobiologyFormValidatorMixin
 
 from ..models import Appointment, SubjectVisit
 
 
+class MicrobiologyFormValidator(
+    MicrobiologyFormValidatorMixin,
+    BaseFormValidatorMixin,
+    FormValidator,
+):
+    """Assumes this is a PRN"""
+
+    pass
+
+
 class TestMicrobiologyFormValidator(TestCase):
     def setUp(self):
         self.subject_identifier = "1234"
         RegisteredSubject.objects.create(
             subject_identifier=self.subject_identifier,
             randomization_datetime=get_utcnow(),
         )
         appointment = Appointment.objects.create(
             subject_identifier=self.subject_identifier,
             appt_datetime=get_utcnow(),
             visit_code=DAY1,
+            visit_schedule_name="visit_schedule",
+            schedule_name="schedule",
+            timepoint=Decimal("0.0"),
         )
         self.subject_visit = SubjectVisit.objects.create(
             appointment=appointment, subject_identifier=self.subject_identifier
         )
 
     def test_urine_culture_performed_yes_require_urine_culture_result(self):
         cleaned_data = {
@@ -199,14 +216,15 @@
             "blood_culture_organism": BACTERIA,
             "blood_culture_bacteria": NOT_APPLICABLE,
         }
         form_validator = MicrobiologyFormValidator(cleaned_data=cleaned_data)
         self.assertRaises(ValidationError, form_validator.validate)
         self.assertIn("blood_culture_bacteria", form_validator._errors)
 
+    @tag("1'")
     def test_blood_organism_is_bacteria_na_bacteria_identified(self):
         cleaned_data = {
             "subject_visit": self.subject_visit,
             "blood_culture_organism": NOT_APPLICABLE,
             "blood_culture_bacteria": KLEBSIELLA_SPP,
         }
         form_validator = MicrobiologyFormValidator(cleaned_data=cleaned_data)
```

### Comparing `edc-microbiology-0.1.8/edc_microbiology.egg-info/PKG-INFO` & `edc-microbiology-0.1.9/edc_microbiology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-microbiology
-Version: 0.1.8
+Version: 0.1.9
 Summary: Microbiology model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microbiology
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microbiology,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-microbiology-0.1.8/edc_microbiology.egg-info/SOURCES.txt` & `edc-microbiology-0.1.9/edc_microbiology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/pyproject.toml` & `edc-microbiology-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-microbiology-0.1.8/runtests.py` & `edc-microbiology-0.1.9/runtests.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         "multisite",
         "django_crypto_fields.apps.AppConfig",
         "edc_auth.apps.AppConfig",
         "edc_appointment.apps.AppConfig",
         "edc_notification.apps.AppConfig",
         "edc_export.apps.AppConfig",
         "edc_crf.apps.AppConfig",
+        "edc_timepoint.apps.AppConfig",
         "edc_registration.apps.AppConfig",
         "edc_metadata.apps.AppConfig",
         "edc_sites.apps.AppConfig",
         "edc_microbiology.apps.AppConfig",
     ],
     add_dashboard_middleware=True,
 ).settings
```

### Comparing `edc-microbiology-0.1.8/setup.cfg` & `edc-microbiology-0.1.9/setup.cfg`

 * *Files identical despite different names*

