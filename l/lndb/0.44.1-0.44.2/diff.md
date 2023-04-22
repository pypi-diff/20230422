# Comparing `tmp/lndb-0.44.1.tar.gz` & `tmp/lndb-0.44.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.44.1.tar", last modified: Sat Apr 22 12:01:36 2023, max compression
+gzip compressed data, was "lndb-0.44.2.tar", last modified: Sat Apr 22 19:12:42 2023, max compression
```

## Comparing `lndb-0.44.1.tar` & `lndb-0.44.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.44.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.44.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.44.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.44.1/.gitignore
--rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.44.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.44.1/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.44.1/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.44.1/docs/api.md
--rw-r--r--   0        0        0    47427 2023-04-22 12:01:22.085003 lndb-0.44.1/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.44.1/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.44.1/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.44.1/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.44.1/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.44.1/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.44.1/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.44.1/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.44.1/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.44.1/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.44.1/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.44.1/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5418 2023-04-20 08:37:12.609361 lndb-0.44.1/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.44.1/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.44.1/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.44.1/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.44.1/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-21 17:24:54.958979 lndb-0.44.1/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.44.1/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.44.1/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-22 12:01:08.955968 lndb-0.44.1/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.44.1/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.44.1/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.44.1/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-22 05:22:50.971625 lndb-0.44.1/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.44.1/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.44.1/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.44.1/lndb/_info.py
--rw-r--r--   0        0        0     6051 2023-04-21 12:45:57.904490 lndb-0.44.1/lndb/_init_instance.py
--rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.44.1/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.44.1/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.44.1/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-21 17:30:25.327407 lndb-0.44.1/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-22 12:00:39.395914 lndb-0.44.1/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.44.1/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.44.1/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.44.1/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.44.1/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.44.1/lndb/_schema.py
--rw-r--r--   0        0        0     1313 2023-04-20 08:37:12.610024 lndb-0.44.1/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.44.1/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.44.1/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.44.1/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.44.1/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.44.1/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.44.1/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.44.1/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.44.1/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.44.1/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.44.1/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8764 2023-04-21 12:45:57.904794 lndb-0.44.1/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.44.1/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.44.1/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.44.1/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.44.1/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.44.1/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     6997 2023-04-17 13:30:19.225702 lndb-0.44.1/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.44.1/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.44.1/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.44.1/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.44.1/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.44.1/lndb/test/_env.py
--rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.44.1/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.44.1/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.44.1/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.44.1/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.44.1/noxfile.py
--rw-r--r--   0        0        0     1395 2023-04-22 05:22:50.971891 lndb-0.44.1/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.44.1/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.44.1/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.44.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.44.1/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.44.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.44.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.44.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.44.2/.gitignore
+-rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.44.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.44.2/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.44.2/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.44.2/docs/api.md
+-rw-r--r--   0        0        0    47427 2023-04-22 19:12:27.272250 lndb-0.44.2/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.44.2/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.44.2/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.44.2/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.44.2/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.44.2/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.44.2/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.44.2/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.44.2/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.44.2/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.44.2/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.44.2/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5418 2023-04-20 08:37:12.609361 lndb-0.44.2/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.44.2/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.44.2/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.44.2/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.44.2/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-21 17:24:54.958979 lndb-0.44.2/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.44.2/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.44.2/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-22 19:12:22.465207 lndb-0.44.2/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.44.2/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.44.2/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.44.2/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-22 05:22:50.971625 lndb-0.44.2/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.44.2/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.44.2/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.44.2/lndb/_info.py
+-rw-r--r--   0        0        0     6051 2023-04-21 12:45:57.904490 lndb-0.44.2/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.44.2/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.44.2/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.44.2/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-21 17:30:25.327407 lndb-0.44.2/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-22 12:00:39.395914 lndb-0.44.2/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.44.2/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.44.2/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.44.2/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.44.2/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.44.2/lndb/_schema.py
+-rw-r--r--   0        0        0     1313 2023-04-20 08:37:12.610024 lndb-0.44.2/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.44.2/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.44.2/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.44.2/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.44.2/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.44.2/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.44.2/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.44.2/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.44.2/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.44.2/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.44.2/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8764 2023-04-21 12:45:57.904794 lndb-0.44.2/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.44.2/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.44.2/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.44.2/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.44.2/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.44.2/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-22 19:12:00.877065 lndb-0.44.2/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.44.2/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.44.2/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.44.2/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.44.2/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.44.2/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.44.2/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.44.2/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.44.2/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.44.2/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.44.2/noxfile.py
+-rw-r--r--   0        0        0     1395 2023-04-22 05:22:50.971891 lndb-0.44.2/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.44.2/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.44.2/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.44.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.44.2/PKG-INFO
```

### Comparing `lndb-0.44.1/.github/workflows/build.yml` & `lndb-0.44.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/.github/workflows/latest-changes.yml` & `lndb-0.44.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/.gitignore` & `lndb-0.44.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/.pre-commit-config.yaml` & `lndb-0.44.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/LICENSE` & `lndb-0.44.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/changelog.md` & `lndb-0.44.2/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.1
+⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
 🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 👷 Remove lnhub-rest CI calls | [360](https://github.com/laminlabs/lndb/pull/360) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Enable non-owner to set storage | [358](https://github.com/laminlabs/lndb/pull/358) | [falexwolf](https://github.com/falexwolf) | 2023-04-19 |
 ♻️ Restructure hub imports | [357](https://github.com/laminlabs/lndb/pull/357) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
```

### Comparing `lndb-0.44.1/docs/faq/check-synchronization.ipynb` & `lndb-0.44.2/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/faq/clone.ipynb` & `lndb-0.44.2/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.44.2/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/faq/manage-migrations.ipynb` & `lndb-0.44.2/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/faq/switch-environment.ipynb` & `lndb-0.44.2/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.44.2/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/faq/test-migrations-unit.ipynb` & `lndb-0.44.2/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/01-setup-user.ipynb` & `lndb-0.44.2/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/02-init-instance.ipynb` & `lndb-0.44.2/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/03-load-instance.ipynb` & `lndb-0.44.2/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/04-set-storage.ipynb` & `lndb-0.44.2/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/05-schema-modules.ipynb` & `lndb-0.44.2/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/06-info.ipynb` & `lndb-0.44.2/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/07-delete.ipynb` & `lndb-0.44.2/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/docs/guide/migrate.md` & `lndb-0.44.2/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/__init__.py` & `lndb-0.44.2/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.1"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.2"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.44.1/lndb/__main__.py` & `lndb-0.44.2/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_check_instance_setup.py` & `lndb-0.44.2/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_close.py` & `lndb-0.44.2/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_delete.py` & `lndb-0.44.2/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_init_instance.py` & `lndb-0.44.2/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_load_instance.py` & `lndb-0.44.2/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_migrate/alembic.ini` & `lndb-0.44.2/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_migrate/core.py` & `lndb-0.44.2/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_migrate/deploy.py` & `lndb-0.44.2/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_migrate/env.py` & `lndb-0.44.2/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_migrate/utils.py` & `lndb-0.44.2/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_register_instance.py` & `lndb-0.44.2/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_schema.py` & `lndb-0.44.2/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_set.py` & `lndb-0.44.2/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_settings.py` & `lndb-0.44.2/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/_setup_user.py` & `lndb-0.44.2/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/__init__.py` & `lndb-0.44.2/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_clone.py` & `lndb-0.44.2/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_db.py` & `lndb-0.44.2/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_deprecated.py` & `lndb-0.44.2/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_exclusion.py` & `lndb-0.44.2/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_settings_instance.py` & `lndb-0.44.2/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_settings_load.py` & `lndb-0.44.2/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_settings_save.py` & `lndb-0.44.2/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_settings_store.py` & `lndb-0.44.2/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_settings_user.py` & `lndb-0.44.2/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_setup_knowledge.py` & `lndb-0.44.2/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/_setup_schema.py` & `lndb-0.44.2/lndb/dev/_setup_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,29 +71,31 @@
         lamindb_version = get_pip_version("lamindb")
         for req in importlib_requires("lamindb"):
             req = Requirement(req)
             if schema_module_name == req.name:
                 if not req.specifier.contains(module_version):
                     # it's currently important that we only import lamindb in
                     # case of an error being raised
-                    import lamindb
-
-                    if lamindb.__version__ != lamindb_version:
-                        warning = (
-                            "\nWARNING: importlib_metadata.version('lamindb') gives"
-                            f" v{lamindb_version}, whereas `import lamindb` gives"
-                            f" v{lamindb.__version__}"
-                            f"\nConsider `pip install lamindb=={lamindb_version}`"
-                        )
-                    else:
-                        warning = ""
+                    # the following might mask the actual error because this is
+                    # raised during instance creation time where lamindb
+                    # cannot yet be imported
+                    # import lamindb
+                    # if lamindb.__version__ != lamindb_version:
+                    #     warning = (
+                    #         "\nWARNING: importlib_metadata.version('lamindb') gives"
+                    #         f" v{lamindb_version}, whereas `import lamindb` gives"
+                    #         f" v{lamindb.__version__}"
+                    #         f"\nConsider `pip install lamindb=={lamindb_version}`"
+                    #     )
+                    # else:
+                    #     warning = ""
                     raise RuntimeError(
                         f"lamindb v{lamindb_version} needs"
                         f" lnschema_{schema_name}{req.specifier}, you have"
-                        f" {module_version} {warning}"
+                        f" {module_version}"
                     )
 
     try:
         # use live version if we can import
         module = importlib.import_module(get_schema_module_name(schema_name))
         module_version = module.__version__
     except Exception as import_error:
```

### Comparing `lndb-0.44.1/lndb/dev/_storage.py` & `lndb-0.44.2/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/dev/upath.py` & `lndb-0.44.2/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/test/_migrations_e2e.py` & `lndb-0.44.2/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/lndb/test/_migrations_unit.py` & `lndb-0.44.2/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/noxfile.py` & `lndb-0.44.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/pyproject.toml` & `lndb-0.44.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/tests/test_bionty.py` & `lndb-0.44.2/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/tests/test_init_instance.py` & `lndb-0.44.2/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.1/PKG-INFO` & `lndb-0.44.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.44.1
+Version: 0.44.2
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.8.2
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
```

