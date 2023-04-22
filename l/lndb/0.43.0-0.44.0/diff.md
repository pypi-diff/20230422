# Comparing `tmp/lndb-0.43.0.tar.gz` & `tmp/lndb-0.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.43.0.tar", last modified: Fri Apr 21 00:22:24 2023, max compression
+gzip compressed data, was "lndb-0.44.0.tar", last modified: Sat Apr 22 05:24:18 2023, max compression
```

## Comparing `lndb-0.43.0.tar` & `lndb-0.44.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.43.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.43.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.43.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.43.0/.gitignore
--rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.43.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.43.0/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.43.0/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.43.0/docs/api.md
--rw-r--r--   0        0        0    46932 2023-04-21 00:21:53.441957 lndb-0.43.0/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.43.0/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.43.0/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.43.0/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.43.0/docs/faq/index.md
--rw-r--r--   0        0        0     1180 2023-04-05 05:10:26.112382 lndb-0.43.0/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.43.0/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.43.0/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.43.0/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.43.0/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.43.0/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.43.0/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5418 2023-04-20 08:37:12.609361 lndb-0.43.0/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.43.0/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.43.0/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.43.0/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.43.0/docs/guide/index.md
--rw-r--r--   0        0        0     3152 2023-03-25 20:23:06.444401 lndb-0.43.0/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.43.0/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.43.0/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-21 00:21:42.236801 lndb-0.43.0/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.43.0/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.43.0/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.43.0/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      216 2023-04-18 16:33:57.539501 lndb-0.43.0/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.43.0/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.43.0/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.43.0/lndb/_info.py
--rw-r--r--   0        0        0     6042 2023-04-21 00:21:08.924753 lndb-0.43.0/lndb/_init_instance.py
--rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.43.0/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.43.0/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.43.0/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3469 2023-04-05 12:41:02.533096 lndb-0.43.0/lndb/_migrate/core.py
--rw-r--r--   0        0        0     6303 2023-04-05 05:10:26.114561 lndb-0.43.0/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.43.0/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.43.0/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.43.0/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.43.0/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.43.0/lndb/_schema.py
--rw-r--r--   0        0        0     1313 2023-04-20 08:37:12.610024 lndb-0.43.0/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.43.0/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.43.0/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.43.0/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.43.0/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.43.0/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.43.0/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.43.0/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.43.0/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.43.0/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.43.0/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8649 2023-04-21 00:21:08.925542 lndb-0.43.0/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.43.0/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.43.0/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.43.0/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.43.0/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.43.0/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     6997 2023-04-17 13:30:19.225702 lndb-0.43.0/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.43.0/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.43.0/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.43.0/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.43.0/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.43.0/lndb/test/_env.py
--rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.43.0/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.43.0/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.43.0/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.43.0/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.43.0/noxfile.py
--rw-r--r--   0        0        0     1395 2023-04-18 16:33:57.539648 lndb-0.43.0/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.43.0/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.43.0/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.43.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.43.0/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.44.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.44.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.44.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.44.0/.gitignore
+-rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.44.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.44.0/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.44.0/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.44.0/docs/api.md
+-rw-r--r--   0        0        0    47427 2023-04-22 05:23:40.755846 lndb-0.44.0/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.44.0/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.44.0/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.44.0/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.44.0/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.44.0/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.44.0/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.44.0/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.44.0/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.44.0/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.44.0/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.44.0/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5418 2023-04-20 08:37:12.609361 lndb-0.44.0/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.44.0/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.44.0/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.44.0/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.44.0/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-21 17:24:54.958979 lndb-0.44.0/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.44.0/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.44.0/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-22 05:23:11.724584 lndb-0.44.0/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.44.0/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.44.0/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.44.0/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-22 05:22:50.971625 lndb-0.44.0/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.44.0/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.44.0/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.44.0/lndb/_info.py
+-rw-r--r--   0        0        0     6051 2023-04-21 12:45:57.904490 lndb-0.44.0/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.44.0/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.44.0/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.44.0/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-21 17:30:25.327407 lndb-0.44.0/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7525 2023-04-21 17:14:41.542726 lndb-0.44.0/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.44.0/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.44.0/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.44.0/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.44.0/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.44.0/lndb/_schema.py
+-rw-r--r--   0        0        0     1313 2023-04-20 08:37:12.610024 lndb-0.44.0/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.44.0/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.44.0/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.44.0/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.44.0/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.44.0/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.44.0/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.44.0/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.44.0/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.44.0/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.44.0/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8764 2023-04-21 12:45:57.904794 lndb-0.44.0/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.44.0/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.44.0/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.44.0/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.44.0/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.44.0/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     6997 2023-04-17 13:30:19.225702 lndb-0.44.0/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.44.0/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.44.0/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.44.0/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.44.0/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.44.0/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.44.0/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.44.0/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.44.0/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.44.0/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.44.0/noxfile.py
+-rw-r--r--   0        0        0     1395 2023-04-22 05:22:50.971891 lndb-0.44.0/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.44.0/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.44.0/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.44.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.44.0/PKG-INFO
```

### Comparing `lndb-0.43.0/.github/workflows/build.yml` & `lndb-0.44.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/.github/workflows/latest-changes.yml` & `lndb-0.44.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/.gitignore` & `lndb-0.44.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/.pre-commit-config.yaml` & `lndb-0.44.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/LICENSE` & `lndb-0.44.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/changelog.md` & `lndb-0.44.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.0
+🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
+🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
 🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 👷 Remove lnhub-rest CI calls | [360](https://github.com/laminlabs/lndb/pull/360) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Enable non-owner to set storage | [358](https://github.com/laminlabs/lndb/pull/358) | [falexwolf](https://github.com/falexwolf) | 2023-04-19 |
 ♻️ Restructure hub imports | [357](https://github.com/laminlabs/lndb/pull/357) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 ⬆️ Upgrade to lnhub_rest 0.8.1 | [356](https://github.com/laminlabs/lndb/pull/356) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.42.0
 ✅ Use nbproject-test directly | [355](https://github.com/laminlabs/lndb/pull/355) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 |
```

### Comparing `lndb-0.43.0/docs/faq/check-synchronization.ipynb` & `lndb-0.44.0/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/faq/clone.ipynb` & `lndb-0.44.0/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.44.0/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/faq/manage-migrations.ipynb` & `lndb-0.44.0/docs/faq/manage-migrations.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'cells'": '{3: {\'source\': [\'# lndb.migrate.generate(package_name="lnschema_core")\']}}'}*

```diff
@@ -29,15 +29,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lndb.migrate.generate(package_name=\"lnschema_core\")"
+                "# lndb.migrate.generate(package_name=\"lnschema_core\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lndb-0.43.0/docs/faq/switch-environment.ipynb` & `lndb-0.44.0/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.44.0/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/faq/test-migrations-unit.ipynb` & `lndb-0.44.0/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/01-setup-user.ipynb` & `lndb-0.44.0/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/02-init-instance.ipynb` & `lndb-0.44.0/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/03-load-instance.ipynb` & `lndb-0.44.0/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/04-set-storage.ipynb` & `lndb-0.44.0/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/05-schema-modules.ipynb` & `lndb-0.44.0/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/06-info.ipynb` & `lndb-0.44.0/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/07-delete.ipynb` & `lndb-0.44.0/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/docs/guide/migrate.md` & `lndb-0.44.0/docs/guide/migrate.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 ```
 
 This page documents how to create a tested migration using the CI-guided workflow for postgres-based instances.
 
 1. Create a new branch (e.g. `migr`) in your repository: Update an ORM, e.g., by renaming a column.
 
    :::{dropdown} Example: Rename a column.
-   Let's try to rename the `v` column to `version` in `Notebook` table of `lnschema_core`.
+   Let's try to rename the `version` column to `v` in the `Transform` ORM of `lnschema_core`.
 
-   In the `lnschema_core/_core.py` `Notebook` class, modify line:
+   In the `lnschema_core/_core.py` `Transform` ORM, modify line:
 
    ```{code-block} python
    ---
    emphasize-lines: 1, 3
    ---
-   v: str = Field(default="1", primary_key=True)
-   to:
    version: str = Field(default="1", primary_key=True)
+   to:
+   v: str = Field(default="1", primary_key=True)
    ```
 
    :::
 
-2. On the command line (at the root of the repository), run `lamin migrate generate` to generate an empty script file under `{package_name}/migrations/versions/`.
+2. On the command line (at the root of the repository), run `lamin migrate generate` to generate a migration script under `{package_name}/migrations/versions/`.
 
    :::{dropdown} Example
 
    Migration script location: The script will be named `{date}-{revision}-vx_x_x.py`.
 
    ```{code-block} yaml
    ---
@@ -42,15 +42,15 @@
    |-- migrations
    |   |-- versions
    |       |-- 2023-02-16-dd2b4a9499f2-vx_x_x.py
    |-- __init__.py
    |-- _core.py
    ```
 
-   Content of migration script.
+   Example of an empty migration script.
 
    ```{code-block} python
    ---
    emphasize-lines: 10
    ---
    """vX.X.X."""
    from alembic import op
@@ -73,25 +73,25 @@
 
    ```{code-block} python
    _migration = "dd2b4a9499f2"
    ```
 
    :::
 
-3. Commit all changes, create a pull request from the `migr` branch, and inspect the output of the failing CI step `Build`.
+3. Commit all changes, create a pull request from the `migr` branch, and inspect the CI step `Build`.
 
    :::{dropdown} Example: Bottom of failed CI output.
 
    ```{code-block} python
    op.alter_column("notebook", column_name="v", new_column_name="version", schema="core")
    ```
 
    :::
 
-4. Copy the suggested changes into the `update()` function in the `{date}-{revision}-vx_x_x.py` file.
+4. In case CI failed, copy the suggested changes into the `update()` function in the `{date}-{revision}-vx_x_x.py` file.
    Commit & push changes: Now CI should pass! 🎉
 
    :::{dropdown} Example: Modified migration script.
 
    ```{code-block} python
    def upgrade() -> None:
        op.alter_column("notebook", column_name="v", new_column_name="version", schema="core")
```

### Comparing `lndb-0.43.0/lndb/__init__.py` & `lndb-0.44.0/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.43.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.43.0/lndb/__main__.py` & `lndb-0.44.0/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_check_instance_setup.py` & `lndb-0.44.0/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_close.py` & `lndb-0.44.0/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_delete.py` & `lndb-0.44.0/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_init_instance.py` & `lndb-0.44.0/lndb/_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             "Not registering instance on hub, if you want, call `lamin register`"
         )
 
     # this does not yet setup a setup for a new database
     persist_settings_load_schema(isettings)
 
     message = None
-    if not isettings._is_db_setup()[0]:
+    if not isettings._is_db_setup(mute=True)[0]:
         setup_schema(isettings, settings.user)
         register(isettings, settings.user)
         write_bionty_versions(isettings)
         # now ensure that everything worked
         check, msg = isettings._is_db_setup()
         if not check:
             raise RuntimeError(msg)
```

### Comparing `lndb-0.43.0/lndb/_load_instance.py` & `lndb-0.44.0/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_migrate/alembic.ini` & `lndb-0.44.0/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_migrate/core.py` & `lndb-0.44.0/lndb/_migrate/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,31 +48,39 @@
         """
         if package_name is None:
             package_name = get_package_name()
         package_dir, migrations_dir, schema_id = get_schema_package_info(package_name)
         generate_module_files(package_name)
         testdb_path = package_dir.parent / "testdb/testdb.lndb"  # type: ignore # noqa
         if testdb_path.exists():
-            # runs dev mode to write migration scripts
             rm = False
             set_alembic_logging_level(migrations_dir, level="INFO")
             logger.info(f"Generating based on {testdb_path}")
         else:
-            # runs CI-guided mode to generate empty migration scripts
             rm = True
             from lndb._settings import settings
 
+            if settings._instance_exists:
+                response = input(
+                    "Will generate migration for instance"
+                    " f{settings.instance.identifier}. Continue? (y/n)"
+                )
+                if response != "y":
+                    return None
+            else:
+                logger.error("Please load the instance you'd like to migrate!")
+                return None
+
             modify_alembic_ini(
                 filepath=package_dir / "alembic.ini",
                 isettings=settings.instance,
                 package_name=package_name,
                 move_sl=False,
             )
             set_alembic_logging_level(migrations_dir, level="WARN")
-            logger.info("Generate empty migration script.")
         command = (
             f"alembic --config {str(package_dir)}/alembic.ini --name"
             f" {schema_id} revision --autogenerate -m '{version}'"
         )
         process = run(command, shell=True)
 
         modify_migration_id_in__init__(package_name)
```

### Comparing `lndb-0.43.0/lndb/_migrate/deploy.py` & `lndb-0.44.0/lndb/dev/_setup_schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,167 @@
-"""Check and auto-deploy migrations."""
-
 import importlib
-import os
-from pathlib import Path
-from subprocess import run
-from typing import Any, Optional
+from types import ModuleType
 
+import sqlalchemy as sa
 import sqlmodel as sqm
+from importlib_metadata import requires as importlib_requires
+from importlib_metadata import version as get_pip_version
 from lamin_logger import logger
-from natsort import natsorted
-from packaging.version import parse as vparse
+from lnhub_rest._assets._schemas import get_schema_lookup_name, get_schema_module_name
+from packaging.requirements import Requirement
 
-from lndb._migrate.utils import generate_module_files, modify_alembic_ini
-from lndb.dev._db import insert
-from lndb.dev._settings_instance import InstanceSettings
-from lndb.dev._settings_user import UserSettings
-from lndb.dev._setup_schema import create_schema_if_not_exists, get_schema_module_name
-
-
-def check_deploy_migration(
-    *,
-    usettings: UserSettings,
-    isettings: InstanceSettings,
-    attempt_deploy: Optional[bool] = None,
-):
-    if "LAMIN_SKIP_MIGRATION" in os.environ:
-        if os.environ["LAMIN_SKIP_MIGRATION"] == "true":
-            return "migrate-skipped"
-
-    # lock the whole migration
-    locker = isettings._cloud_sqlite_locker
-    locker.lock()
-    # synchronize the sqlite file before proceeding
-    isettings._update_local_sqlite_file()
+from ._db import insert
+from ._settings_instance import InstanceSettings
+from ._settings_user import UserSettings
+
+
+def create_schema_if_not_exists(schema_name: str, isettings: InstanceSettings):
+    # create the SQL-level schema module in case it doesn't exist
+    schema_lookup_name = get_schema_lookup_name(schema_name)
+    if isettings.dialect != "sqlite":
+        with isettings.engine.connect() as conn:
+            if not conn.dialect.has_schema(conn, schema_lookup_name):
+                conn.execute(sa.schema.CreateSchema(schema_lookup_name))
+            conn.commit()
+
+
+def reload_orms(schema_name, module, isettings):
+    # root-level ORMs
+    orms = [cls for cls in module.__dict__.values() if hasattr(cls, "__table__")]
+    # dev-level ORMs
+    if hasattr(module, "dev"):
+        orms += [
+            cls
+            for cls in module.dev.__dict__.values()
+            if hasattr(cls, "__table__")
+            # exclude the version_* and migration_* tables in the root namespace
+            and not cls.__name__.startswith("version_")
+            and not cls.__name__.startswith("migration_")
+        ]
+    # link tables
+    if hasattr(module, "link"):
+        orms += [
+            cls for cls in module.link.__dict__.values() if hasattr(cls, "__table__")
+        ]
+    if isettings.dialect == "sqlite":
+        # only those orms that are actually in a schema
+        orms = [
+            orm
+            for orm in orms
+            if hasattr(orm.__table__, "schema") and orm.__table__.schema is not None
+        ]
+        for orm in orms:
+            orm.__table__.schema = None
+            # I don't know why the following is needed... it shouldn't
+            if not orm.__table__.name.startswith(f"{schema_name}."):
+                orm.__table__.name = f"{schema_name}.{orm.__table__.name}"
+    else:  # postgres
+        orms = [
+            orm
+            for orm in orms
+            if (hasattr(orm.__table__, "schema") and orm.__table__.schema is None)
+        ]
+        for orm in orms:
+            orm.__table__.schema = schema_name
+            orm.__table__.name = orm.__table__.name.replace(f"{schema_name}.", "")
 
-    status = []
-    schema_names = ["core"] + list(isettings.schema)
-    # enforce order (if bionty is part of schema_names, it needs to come 2nd)
-    if "bionty" in schema_names:
-        schema_names.remove("bionty")
-        schema_names.insert(1, "bionty")
 
-    for schema_name in schema_names:
-        create_schema_if_not_exists(schema_name, isettings)
+def check_schema_version_and_import(schema_name) -> ModuleType:
+    def check_version(module_version):
         schema_module_name = get_schema_module_name(schema_name)
-        schema_module = importlib.import_module(schema_module_name)
-        # if _migration is None, there hasn't yet been any
-        if schema_module._migration is None:
-            status.append("migrate-unnecessary")
-            continue
+        lamindb_version = get_pip_version("lamindb")
+        for req in importlib_requires("lamindb"):
+            req = Requirement(req)
+            if schema_module_name == req.name:
+                if not req.specifier.contains(module_version):
+                    # it's currently important that we only import lamindb in
+                    # case of an error being raised
+                    import lamindb
+
+                    if lamindb.__version__ != lamindb_version:
+                        warning = (
+                            "\nWARNING: importlib_metadata.version('lamindb') gives"
+                            f" v{lamindb_version}, whereas `import lamindb` gives"
+                            f" v{lamindb.__version__}"
+                            f"\nConsider `pip install lamindb=={lamindb_version}`"
+                        )
+                    else:
+                        warning = ""
+                    raise RuntimeError(
+                        f"lamindb v{lamindb_version} needs"
+                        f" lnschema_{schema_name}{req.specifier}, you have"
+                        f" {module_version} {warning}"
+                    )
 
-        schema_id = schema_module._schema_id
+    try:
+        # use live version if we can import
+        module = importlib.import_module(get_schema_module_name(schema_name))
+        module_version = module.__version__
+    except Exception as import_error:
+        # use pypi version instead
+        module_version = get_pip_version(get_schema_module_name(schema_name))
+        check_version(module_version)
+        raise import_error
 
-        with sqm.Session(isettings.engine) as session:
-            table_loc = (
-                schema_module.dev if hasattr(schema_module, "dev") else schema_module
-            )
-            version_table = getattr(table_loc, f"version_{schema_id}")
-            versions = session.exec(sqm.select(version_table.v)).all()
-            versions = natsorted(versions)  # latest version is last
-
-        current_version = schema_module.__version__
-
-        # attempt deploy as we want to test migrating the database
-        if attempt_deploy:
-            deploy_migration = True
-        # check whether we need to deploy based on version comparison
-        elif current_version not in versions and len(versions) > 0:
-            if vparse(current_version) < vparse(versions[-1]):  # type: ignore
-                raise RuntimeError(
-                    f"You are trying to connect to a DB ({isettings.identifier}) that"
-                    f" runs v{versions[-1]} of {schema_module_name} but you only have"
-                    f" v{current_version} installed.\nPlease run `pip install"
-                    f" {schema_module_name}=={versions[-1]}`, or install the latest"
-                    " schema module version from GitHub."
-                )
-            logger.warning(
-                f"Schema {schema_name} v{versions[-1]} is not up to date"
-                f" with {current_version}"
-            )
-            # if migration is confirmed, continue
-            if "PYTEST_CURRENT_TEST" not in os.environ:
-                logger.warning(
-                    "Run the command in the shell to respond to the following dialogue"
-                )
-
-                response = input(
-                    f"Do you want to migrate {schema_name} from {versions[-1]} to"
-                    f" {current_version} (y/n)?"
-                )
-
-                if response != "y":
-                    logger.warning(
-                        f"Instance {isettings.identifier} does not match the latest version of schema {schema_name}.\n"  # noqa
-                        "For production use, either install"
-                        f" {schema_module_name} {versions[-1]} "
-                        f"or migrate the database to {current_version}."
-                    )
-                    return None
-            else:
-                logger.warning(
-                    f"Migrate instance {isettings.name} outside a test (CI) run. "
-                    "Unexpected errors might happen."
-                )
-                return "migrate-failed"
-
-            deploy_migration = True
-
-        else:
-            deploy_migration = False
-            status.append("migrate-unnecessary")
-
-        if deploy_migration:
-            generate_module_files(
-                package_name=schema_module_name,
-                migrations_path=Path(schema_module.__file__).parent / "migrations",  # type: ignore  # noqa
-                schema_id=schema_id,
-            )
-            migrate_status = deploy(
-                version=current_version,
-                usettings=usettings,
-                isettings=isettings,
-                schema_name=schema_name,
-                schema_id=schema_id,
-                schema_module=schema_module,
-            )
-            status.append(migrate_status)
+    check_version(module_version)
+    return module
 
-    locker.unlock()
 
-    if "migrate-failed" in status:
-        return "migrate-failed"
-    elif "migrate-success" in status:
-        return "migrate-success"
-    else:
-        return "migrate-unnecessary"
-
-
-def deploy(
-    *,
-    version: str,
-    usettings: UserSettings,
-    isettings: InstanceSettings,
-    schema_name: str,
-    schema_id: str,
-    schema_module: Any,
-):
-    """Migrate database to latest version."""
-    schema_root = Path(schema_module.__file__).parent
-    filepath = schema_root / "alembic.ini"
-
-    modify_alembic_ini(filepath, isettings, schema_name)
-
-    process = run(
-        f"python -m alembic --name {schema_id} upgrade head",
-        cwd=f"{schema_root}",
-        shell=True,
+def load_schema(isettings: InstanceSettings):
+    reload = False  # see comments below
+    schema_names = ["core"] + list(isettings.schema)
+    msg = "Loading schema modules: "
+    for schema_name in schema_names:
+        create_schema_if_not_exists(schema_name, isettings)
+        module = check_schema_version_and_import(schema_name)
+        if schema_name == "core":
+            # here, we determine whether we have to reload the ORMs
+            # it's necessary if switching from or to sqlite
+            user_table = module.User.__table__
+            if isettings.dialect != "sqlite" and user_table.schema is None:
+                reload = True
+            if isettings.dialect == "sqlite" and user_table.schema is not None:
+                reload = True
+        if reload:  # importlib.reload doesn't do the job! hence, manual below
+            reload_orms(schema_name, module, isettings)
+        msg += f"{schema_name}=={module.__version__} "
+    return msg, schema_names
+
+
+def setup_schema(isettings: InstanceSettings, usettings: UserSettings):
+    msg, schema_names = load_schema(isettings)
+    logger.info(f"{msg}")
+
+    sqm.SQLModel.metadata.create_all(isettings.engine)
+
+    # we could try to also retrieve the user name here at some point
+    insert.user(
+        email=usettings.email,
+        user_id=usettings.id,
+        handle=usettings.handle,
+        name=usettings.name,
     )
 
-    if process.returncode == 0:
-        logger.success(f"Migrated schema {schema_name} to v{version}")
-        # The following call will also update the sqlite file in the cloud.
+    for schema_name in schema_names:
+        schema_module = importlib.import_module(get_schema_module_name(schema_name))
         insert.version(
             schema_module=schema_module,
             user_id=usettings.id,  # type: ignore
+            cloud_sqlite=False,
         )
-    else:
-        logger.error("Automatic migration failed.")
-
-    modify_alembic_ini(filepath, isettings, schema_name, revert=True)
-
-    if process.returncode == 0:
-        return "migrate-success"
-    else:
-        return "migrate-failed"
+        # this is the only time we need manipulate the migration table
+        # in all other cases alembic is going to to do this for us
+        schema_id, migration = schema_module._schema_id, schema_module._migration
+        if migration is not None:
+            table_loc = (
+                schema_module.dev if hasattr(schema_module, "dev") else schema_module
+            )
+            migration_table = getattr(table_loc, f"migration_{schema_id}")
+            # we purposefully do not use isettings.session(), here, as we do *not*
+            # want to update the local sqlite file from the cloud while looping over
+            # schema modules
+            # in fact, a synchronization issue led to loss of version information,
+            # because the old cloud sqlite file overwrote the newer local file
+            with sqm.Session(isettings.engine) as session:
+                session.add(migration_table(version_num=migration))
+                session.commit()
+    isettings._update_cloud_sqlite_file()
```

### Comparing `lndb-0.43.0/lndb/_migrate/env.py` & `lndb-0.44.0/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_migrate/utils.py` & `lndb-0.44.0/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_register_instance.py` & `lndb-0.44.0/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_schema.py` & `lndb-0.44.0/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_set.py` & `lndb-0.44.0/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_settings.py` & `lndb-0.44.0/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/_setup_user.py` & `lndb-0.44.0/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/__init__.py` & `lndb-0.44.0/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_clone.py` & `lndb-0.44.0/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_db.py` & `lndb-0.44.0/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_deprecated.py` & `lndb-0.44.0/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_exclusion.py` & `lndb-0.44.0/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_settings_instance.py` & `lndb-0.44.0/lndb/dev/_settings_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,17 +210,17 @@
         shutil.copy2(filepath, current_instance_settings_file())
         # persist under settings class for same session reference
         # need to import here to avoid circular import
         from .._settings import settings
 
         settings._instance_settings = self
 
-    def _is_db_setup(self) -> Tuple[bool, str]:
+    def _is_db_setup(self, mute: bool = False) -> Tuple[bool, str]:
         """Is the database available and initialized as LaminDB?"""
-        if not self._is_db_reachable():
+        if not self._is_db_reachable(mute=mute):
             if self.dialect == "sqlite":
                 return False, f"SQLite file {self._sqlite_file} does not exist"
             else:
                 return False, f"Connection {self.db} not reachable"
         # cannot import lnschema_core here, yet!
 
         with self.engine.connect() as conn:
@@ -228,20 +228,22 @@
                 result = conn.execute(sa.text("select * from version_yvzi")).first()
             except Exception as e:
                 return False, f"Your DB is not initialized: {e}"
             if result is None:
                 return False, "Your DB is not initialized: version_yvzi has no row"
         return True, ""
 
-    def _is_db_reachable(self) -> bool:
+    def _is_db_reachable(self, mute: bool = False) -> bool:
         if self.dialect == "sqlite":
             if not self._sqlite_file.exists():
-                logger.warning(f"SQLite file {self._sqlite_file} does not exist")
+                if not mute:
+                    logger.warning(f"SQLite file {self._sqlite_file} does not exist")
                 return False
         else:
             engine = sa.create_engine(self.db)
             try:
                 engine.connect()
             except Exception:
-                logger.warning(f"Connection {self.db} not reachable")
+                if not mute:
+                    logger.warning(f"Connection {self.db} not reachable")
                 return False
         return True
```

### Comparing `lndb-0.43.0/lndb/dev/_settings_load.py` & `lndb-0.44.0/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_settings_save.py` & `lndb-0.44.0/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_settings_store.py` & `lndb-0.44.0/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_settings_user.py` & `lndb-0.44.0/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_setup_knowledge.py` & `lndb-0.44.0/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/_storage.py` & `lndb-0.44.0/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/dev/upath.py` & `lndb-0.44.0/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/test/_migrations_e2e.py` & `lndb-0.44.0/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/lndb/test/_migrations_unit.py` & `lndb-0.44.0/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/noxfile.py` & `lndb-0.44.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/pyproject.toml` & `lndb-0.44.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.8.1",
+    "lnhub_rest==0.8.2",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
```

### Comparing `lndb-0.43.0/tests/test_bionty.py` & `lndb-0.44.0/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/tests/test_init_instance.py` & `lndb-0.44.0/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.43.0/PKG-INFO` & `lndb-0.44.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.43.0
+Version: 0.44.0
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.8.1
+Requires-Dist: lnhub_rest==0.8.2
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: cloudpathlib
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
```

