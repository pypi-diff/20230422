# Comparing `tmp/lnhub_rest-0.8.1.tar.gz` & `tmp/lnhub_rest-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.8.1.tar", last modified: Tue Apr 18 16:22:44 2023, max compression
+gzip compressed data, was "lnhub_rest-0.8.2.tar", last modified: Sat Apr 22 05:00:47 2023, max compression
```

## Comparing `lnhub_rest-0.8.1.tar` & `lnhub_rest-0.8.2.tar`

### file list

```diff
@@ -1,224 +1,198 @@
--rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.8.1/.dockerignore
--rw-r--r--   0        0        0     3217 2023-04-18 16:21:04.417331 lnhub_rest-0.8.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     5087 2023-04-18 16:02:04.937394 lnhub_rest-0.8.1/.github/workflows/google-cloudrun-docker.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.8.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.8.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.8.1/.gitignore
--rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.8.1/.gitmodules
--rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.8.1/Dockerfile
--rw-r--r--   0        0        0     1149 2023-04-18 16:21:04.417682 lnhub_rest-0.8.1/README.md
--rw-r--r--   0        0        0    12677 2023-04-18 16:21:04.417854 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-2efe1dee9baf.svg
--rw-r--r--   0        0        0    16617 2023-04-18 16:21:04.418149 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-a88f5298b8f7.svg
--rw-r--r--   0        0        0    13696 2023-04-18 16:21:04.418591 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-c13c9dd0f3ae.svg
--rw-r--r--   0        0        0    12677 2023-04-18 16:21:04.418734 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-e7151581f790.svg
--rw-r--r--   0        0        0    15062 2023-04-18 16:21:04.419104 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-e7eef9775586.svg
--rw-r--r--   0        0        0    14594 2023-04-18 16:21:04.419540 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-f2cb77148a6e.svg
--rw-r--r--   0        0        0    12677 2023-04-18 16:21:04.419648 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-f7ba9352c706.svg
--rw-r--r--   0        0        0    14594 2023-04-18 16:21:04.419768 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-fe962c9a0ae7.svg
--rw-r--r--   0        0        0     5302 2023-04-18 16:02:04.940153 lnhub_rest-0.8.1/docs/account/01-signup-signin.ipynb
--rw-r--r--   0        0        0     4559 2023-04-18 16:02:04.940245 lnhub_rest-0.8.1/docs/account/02-create-account.ipynb
--rw-r--r--   0        0        0     5606 2023-04-18 16:02:04.940348 lnhub_rest-0.8.1/docs/account/03-update-account.ipynb
--rw-r--r--   0        0        0     6182 2023-04-18 16:02:04.940428 lnhub_rest-0.8.1/docs/account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9084 2023-04-18 16:02:04.940536 lnhub_rest-0.8.1/docs/account/05-rls.ipynb
--rw-r--r--   0        0        0    21465 2023-04-18 16:22:13.686823 lnhub_rest-0.8.1/docs/changelog.md
--rw-r--r--   0        0        0     1299 2023-04-18 16:02:04.941369 lnhub_rest-0.8.1/docs/checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0       69 2023-04-18 16:21:04.419847 lnhub_rest-0.8.1/docs/content.md
--rw-r--r--   0        0        0    11226 2023-04-18 16:02:04.941781 lnhub_rest-0.8.1/docs/instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5286 2023-04-18 16:02:04.942110 lnhub_rest-0.8.1/docs/instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6191 2023-04-18 16:02:04.942208 lnhub_rest-0.8.1/docs/instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8663 2023-04-18 16:02:04.942323 lnhub_rest-0.8.1/docs/instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     6993 2023-04-18 16:02:04.942408 lnhub_rest-0.8.1/docs/instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19485 2023-04-18 16:02:04.942491 lnhub_rest-0.8.1/docs/instance/06-rls.ipynb
--rw-r--r--   0        0        0     2065 2023-04-18 16:21:04.420117 lnhub_rest-0.8.1/docs/migration/01-migration.ipynb
--rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.8.1/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.8.1/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.8.1/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0     3875 2023-04-18 16:02:04.943815 lnhub_rest-0.8.1/docs/organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     3999 2023-04-18 16:02:04.943880 lnhub_rest-0.8.1/docs/organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5888 2023-04-18 16:02:04.944098 lnhub_rest-0.8.1/docs/organization/03-rls.ipynb
--rw-r--r--   0        0        0     3866 2023-04-18 16:02:04.944372 lnhub_rest-0.8.1/docs/storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9833 2023-04-18 16:02:04.944483 lnhub_rest-0.8.1/docs/storage/02-rls.ipynb
--rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.8.1/lamin-project.yaml
--rw-r--r--   0        0        0     3832 2023-04-18 13:35:36.828846 lnhub_rest-0.8.1/lndb/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.8.1/lndb/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.8.1/lndb/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.8.1/lndb/.gitignore
--rw-r--r--   0        0        0     1772 2023-03-14 19:46:06.422493 lnhub_rest-0.8.1/lndb/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.8.1/lndb/LICENSE
--rw-r--r--   0        0        0      173 2023-03-30 17:54:41.276204 lnhub_rest-0.8.1/lndb/README.md
--rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.8.1/lndb/docs/api.md
--rw-r--r--   0        0        0    45851 2023-04-18 13:35:36.829219 lnhub_rest-0.8.1/lndb/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.8.1/lndb/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.8.1/lndb/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-30 17:54:41.276594 lnhub_rest-0.8.1/lndb/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-30 17:54:41.276682 lnhub_rest-0.8.1/lndb/docs/faq/index.md
--rw-r--r--   0        0        0     1180 2023-04-18 13:35:36.829371 lnhub_rest-0.8.1/lndb/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.8.1/lndb/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-18 13:35:36.829492 lnhub_rest-0.8.1/lndb/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-18 13:35:36.829617 lnhub_rest-0.8.1/lndb/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-03-30 17:54:41.277018 lnhub_rest-0.8.1/lndb/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10679 2023-04-18 13:35:36.829735 lnhub_rest-0.8.1/lndb/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5573 2023-03-30 17:54:41.277206 lnhub_rest-0.8.1/lndb/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5290 2023-03-14 19:46:06.424075 lnhub_rest-0.8.1/lndb/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-03-30 17:54:41.277308 lnhub_rest-0.8.1/lndb/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-30 17:54:41.277655 lnhub_rest-0.8.1/lndb/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     3282 2023-03-30 17:54:41.277763 lnhub_rest-0.8.1/lndb/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.8.1/lndb/docs/guide/index.md
--rw-r--r--   0        0        0     3152 2023-03-30 17:54:41.277866 lnhub_rest-0.8.1/lndb/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.8.1/lndb/docs/index.md
--rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.8.1/lndb/lamin-project.yaml
--rw-r--r--   0        0        0     1932 2023-04-18 13:35:36.829834 lnhub_rest-0.8.1/lndb/lndb/__init__.py
--rw-r--r--   0        0        0     4242 2023-03-14 19:46:06.424708 lnhub_rest-0.8.1/lndb/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.8.1/lndb/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-18 13:35:36.829911 lnhub_rest-0.8.1/lndb/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      216 2023-04-18 13:35:36.830020 lnhub_rest-0.8.1/lndb/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-18 13:35:36.830147 lnhub_rest-0.8.1/lndb/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-18 13:35:36.830259 lnhub_rest-0.8.1/lndb/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-03-14 19:46:06.425064 lnhub_rest-0.8.1/lndb/lndb/_info.py
--rw-r--r--   0        0        0     5710 2023-04-18 13:35:36.830369 lnhub_rest-0.8.1/lndb/lndb/_init_instance.py
--rw-r--r--   0        0        0     3980 2023-04-18 13:35:36.830476 lnhub_rest-0.8.1/lndb/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-18 13:35:36.830566 lnhub_rest-0.8.1/lndb/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-18 13:35:36.830658 lnhub_rest-0.8.1/lndb/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3469 2023-04-18 13:35:36.830722 lnhub_rest-0.8.1/lndb/lndb/_migrate/core.py
--rw-r--r--   0        0        0     6303 2023-04-18 13:35:36.830802 lnhub_rest-0.8.1/lndb/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.8.1/lndb/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-03-14 19:46:06.425679 lnhub_rest-0.8.1/lndb/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-18 13:35:36.830883 lnhub_rest-0.8.1/lndb/lndb/_migrate/utils.py
--rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.8.1/lndb/lndb/_schema.py
--rw-r--r--   0        0        0     1493 2023-04-18 13:35:36.830975 lnhub_rest-0.8.1/lndb/lndb/_set.py
--rw-r--r--   0        0        0     2181 2023-04-18 13:35:36.831075 lnhub_rest-0.8.1/lndb/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.8.1/lndb/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.8.1/lndb/lndb/_settings_store.py
--rw-r--r--   0        0        0     4927 2023-04-18 13:35:36.831210 lnhub_rest-0.8.1/lndb/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-18 13:35:36.831323 lnhub_rest-0.8.1/lndb/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-30 17:54:41.279075 lnhub_rest-0.8.1/lndb/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-18 13:35:36.831429 lnhub_rest-0.8.1/lndb/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.8.1/lndb/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.8.1/lndb/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-18 13:35:36.831581 lnhub_rest-0.8.1/lndb/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8429 2023-04-18 13:35:36.831706 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-30 17:54:41.279257 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-18 13:35:36.831800 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-30 17:54:41.279348 lnhub_rest-0.8.1/lndb/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     6997 2023-04-18 13:35:36.831921 lnhub_rest-0.8.1/lndb/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-18 13:35:36.832173 lnhub_rest-0.8.1/lndb/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.8.1/lndb/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-18 13:35:36.832243 lnhub_rest-0.8.1/lndb/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-18 13:35:36.832350 lnhub_rest-0.8.1/lndb/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.8.1/lndb/lndb/test/_env.py
--rw-r--r--   0        0        0     3856 2023-03-30 17:54:41.279631 lnhub_rest-0.8.1/lndb/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-18 13:35:36.832454 lnhub_rest-0.8.1/lndb/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.8.1/lndb/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.8.1/lndb/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-18 13:35:36.832538 lnhub_rest-0.8.1/lndb/noxfile.py
--rw-r--r--   0        0        0     1378 2023-04-18 13:35:36.832791 lnhub_rest-0.8.1/lndb/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-18 13:35:36.832925 lnhub_rest-0.8.1/lndb/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.8.1/lndb/tests/test_init_instance.py
--rw-r--r--   0        0        0      385 2023-03-14 19:46:06.428715 lnhub_rest-0.8.1/lndb/tests/test_notebooks.py
--rw-r--r--   0        0        0      225 2023-04-18 16:02:04.945178 lnhub_rest-0.8.1/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     8251 2023-04-18 16:21:04.420589 lnhub_rest-0.8.1/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       59 2023-04-18 16:02:04.945972 lnhub_rest-0.8.1/lnhub_rest/_add_storage.py
--rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.8.1/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0     1026 2023-01-15 12:17:52.330665 lnhub_rest-0.8.1/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1094 2023-02-07 14:01:34.054166 lnhub_rest-0.8.1/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.8.1/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0      998 2023-04-18 16:02:04.946668 lnhub_rest-0.8.1/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5718 2023-04-18 16:02:04.946827 lnhub_rest-0.8.1/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0       64 2023-04-18 16:02:04.946919 lnhub_rest-0.8.1/lnhub_rest/_delete_instance.py
--rw-r--r--   0        0        0       45 2023-04-18 16:02:04.947004 lnhub_rest-0.8.1/lnhub_rest/_engine.py
--rw-r--r--   0        0        0       62 2023-04-18 16:02:04.947118 lnhub_rest-0.8.1/lnhub_rest/_init_instance.py
--rw-r--r--   0        0        0       62 2023-04-18 16:02:04.947229 lnhub_rest-0.8.1/lnhub_rest/_load_instance.py
--rw-r--r--   0        0        0       90 2023-01-15 12:17:52.330955 lnhub_rest-0.8.1/lnhub_rest/_models.py
--rw-r--r--   0        0        0       47 2023-04-18 16:02:04.947314 lnhub_rest-0.8.1/lnhub_rest/_sbclient.py
--rw-r--r--   0        0        0       61 2023-04-18 16:02:04.947399 lnhub_rest-0.8.1/lnhub_rest/_signup_signin.py
--rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.8.1/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.8.1/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-18 16:02:04.947726 lnhub_rest-0.8.1/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.8.1/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      735 2023-04-18 16:02:04.948122 lnhub_rest-0.8.1/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3314 2023-04-18 16:02:04.948225 lnhub_rest-0.8.1/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1419 2023-04-18 16:02:04.948320 lnhub_rest-0.8.1/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.8.1/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     2735 2023-04-18 16:02:04.948532 lnhub_rest-0.8.1/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.8.1/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.8.1/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1280 2023-04-18 16:02:04.949021 lnhub_rest-0.8.1/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6471 2023-04-18 16:02:04.949102 lnhub_rest-0.8.1/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1528 2023-04-18 16:02:04.949405 lnhub_rest-0.8.1/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1063 2023-04-18 16:02:04.949739 lnhub_rest-0.8.1/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.8.1/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.8.1/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.8.1/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     2850 2023-04-18 16:02:04.950032 lnhub_rest-0.8.1/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.8.1/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      796 2023-04-18 16:02:04.950233 lnhub_rest-0.8.1/lnhub_rest/main.py
--rw-r--r--   0        0        0       11 2023-04-18 16:02:04.950293 lnhub_rest-0.8.1/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      224 2023-04-18 16:02:04.950361 lnhub_rest-0.8.1/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     2543 2023-04-18 16:02:04.950590 lnhub_rest-0.8.1/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      198 2023-04-18 16:02:04.950703 lnhub_rest-0.8.1/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4121 2023-04-18 16:02:04.950818 lnhub_rest-0.8.1/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.8.1/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.8.1/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     4243 2023-04-18 16:02:04.951226 lnhub_rest-0.8.1/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.8.1/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1061 2023-04-18 16:02:04.951701 lnhub_rest-0.8.1/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.8.1/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.8.1/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.8.1/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.8.1/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.8.1/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.8.1/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.8.1/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       50 2023-04-18 16:02:04.953110 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     2979 2023-04-18 16:02:04.953601 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0      757 2023-04-18 16:02:04.955360 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/settings.py
--rw-r--r--   0        0        0     5549 2023-04-18 16:02:04.955713 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     1816 2023-04-18 16:21:04.420695 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-13-53709f2a2043-v0_0_1a.py
--rw-r--r--   0        0        0      935 2023-04-18 16:21:04.420776 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-13-c555c87a640c-v0_0_1.py
--rw-r--r--   0        0        0     5052 2023-04-18 16:21:04.421051 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-14-f7ba9352c706-v0_0_2.py
--rw-r--r--   0        0        0     1401 2023-04-18 16:21:04.421410 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-23-c13c9dd0f3ae-v0_1_4a.py
--rw-r--r--   0        0        0      536 2023-04-18 16:21:04.421665 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-24-e7151581f790-v0_1_4b.py
--rw-r--r--   0        0        0      512 2023-04-18 16:21:04.421743 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-30-2efe1dee9baf-v0_1_4c.py
--rw-r--r--   0        0        0      667 2023-04-18 16:21:04.421817 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-95073282294e-v0_1_4e.py
--rw-r--r--   0        0        0      869 2023-04-18 16:21:04.422041 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-9c02109e4faa-v0_2_0.py
--rw-r--r--   0        0        0     2190 2023-04-18 16:21:04.422119 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-f2cb77148a6e-v0_1_4d.py
--rw-r--r--   0        0        0      458 2023-04-18 16:21:04.422361 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-08-e7eef9775586-0_2_1.py
--rw-r--r--   0        0        0     1220 2023-04-18 16:21:04.422588 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-15-641d1508baab-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-18 16:21:04.422993 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.8.1/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.8.1/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.8.1/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.8.1/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.8.1/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3816 2023-04-18 16:02:04.957124 lnhub_rest-0.8.1/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1758 2023-04-18 16:02:04.957587 lnhub_rest-0.8.1/noxfile.py
--rw-r--r--   0        0        0     1253 2023-04-18 16:02:04.957709 lnhub_rest-0.8.1/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.8.1/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.8.1/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.8.1/supabase/config.toml
--rw-r--r--   0        0        0      866 2023-04-18 16:21:04.423121 lnhub_rest-0.8.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     2068 1970-01-01 00:00:00.000000 lnhub_rest-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.8.2/.dockerignore
+-rw-r--r--   0        0        0     3315 2023-04-22 04:03:15.788282 lnhub_rest-0.8.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5113 2023-04-19 15:57:22.483317 lnhub_rest-0.8.2/.github/workflows/google-cloudrun-docker.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.8.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.8.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.8.2/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.8.2/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.8.2/Dockerfile
+-rw-r--r--   0        0        0     1140 2023-04-19 18:12:02.220748 lnhub_rest-0.8.2/README.md
+-rw-r--r--   0        0        0     1754 2023-04-19 18:12:02.221232 lnhub_rest-0.8.2/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-04-19 15:57:22.509145 lnhub_rest-0.8.2/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     5218 2023-04-19 15:57:22.508991 lnhub_rest-0.8.2/docs/02-account/01-signup-signin.ipynb
+-rw-r--r--   0        0        0     4487 2023-04-19 15:57:22.508836 lnhub_rest-0.8.2/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-04-19 15:57:22.508666 lnhub_rest-0.8.2/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6146 2023-04-19 15:57:22.508504 lnhub_rest-0.8.2/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-04-19 15:57:22.508334 lnhub_rest-0.8.2/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11211 2023-04-21 10:12:34.724112 lnhub_rest-0.8.2/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5290 2023-04-19 15:57:22.507982 lnhub_rest-0.8.2/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6195 2023-04-19 15:57:22.507801 lnhub_rest-0.8.2/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-04-19 15:57:22.507620 lnhub_rest-0.8.2/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-04-19 15:57:22.507431 lnhub_rest-0.8.2/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-04-19 15:57:22.507215 lnhub_rest-0.8.2/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3870 2023-04-21 10:12:34.724397 lnhub_rest-0.8.2/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-04-19 15:57:22.506877 lnhub_rest-0.8.2/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-04-19 15:57:22.506712 lnhub_rest-0.8.2/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4003 2023-04-19 15:57:22.506559 lnhub_rest-0.8.2/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-04-19 15:57:22.506399 lnhub_rest-0.8.2/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.8.2/docs/README.md
+-rw-r--r--   0        0        0    22591 2023-04-22 05:00:27.269158 lnhub_rest-0.8.2/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.8.2/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.8.2/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.8.2/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.8.2/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.8.2/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.8.2/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.8.2/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.8.2/lndb/.gitignore
+-rw-r--r--   0        0        0     1772 2023-03-14 19:46:06.422493 lnhub_rest-0.8.2/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.8.2/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.8.2/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.8.2/lndb/docs/api.md
+-rw-r--r--   0        0        0    46285 2023-04-18 21:59:42.219504 lnhub_rest-0.8.2/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.8.2/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.8.2/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.8.2/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.8.2/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1180 2023-04-18 16:53:14.551280 lnhub_rest-0.8.2/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.8.2/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.8.2/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10679 2023-04-18 16:53:14.551748 lnhub_rest-0.8.2/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5573 2023-04-18 16:53:14.551912 lnhub_rest-0.8.2/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5290 2023-03-14 19:46:06.424075 lnhub_rest-0.8.2/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-04-18 16:53:14.552033 lnhub_rest-0.8.2/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.8.2/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     3282 2023-04-18 16:53:14.552254 lnhub_rest-0.8.2/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.8.2/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3152 2023-04-18 16:53:14.552393 lnhub_rest-0.8.2/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.8.2/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.8.2/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1932 2023-04-18 16:53:14.552609 lnhub_rest-0.8.2/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4242 2023-03-14 19:46:06.424708 lnhub_rest-0.8.2/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.8.2/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.8.2/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      216 2023-04-18 16:53:14.553485 lnhub_rest-0.8.2/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.8.2/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.8.2/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-03-14 19:46:06.425064 lnhub_rest-0.8.2/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     5751 2023-04-18 21:59:42.219684 lnhub_rest-0.8.2/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-18 21:59:42.219815 lnhub_rest-0.8.2/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.8.2/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.8.2/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3469 2023-04-18 16:53:14.554644 lnhub_rest-0.8.2/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     6303 2023-04-18 16:53:14.554756 lnhub_rest-0.8.2/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.8.2/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-03-14 19:46:06.425679 lnhub_rest-0.8.2/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.8.2/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.8.2/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1506 2023-04-18 21:59:42.219950 lnhub_rest-0.8.2/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.8.2/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.8.2/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.8.2/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     4940 2023-04-18 21:59:42.220094 lnhub_rest-0.8.2/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.8.2/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.8.2/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.8.2/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.8.2/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.8.2/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.8.2/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8429 2023-04-18 16:53:14.556252 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.8.2/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     6997 2023-04-18 16:53:14.556779 lnhub_rest-0.8.2/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4917 2023-04-18 16:53:14.556926 lnhub_rest-0.8.2/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.8.2/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.8.2/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.8.2/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.8.2/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-18 21:59:42.220234 lnhub_rest-0.8.2/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.8.2/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.8.2/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.8.2/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.8.2/lndb/noxfile.py
+-rw-r--r--   0        0        0     1395 2023-04-18 16:53:14.557716 lnhub_rest-0.8.2/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.8.2/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.8.2/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.8.2/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      158 2023-04-22 05:00:02.722421 lnhub_rest-0.8.2/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     8011 2023-04-19 18:12:02.222219 lnhub_rest-0.8.2/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.8.2/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0     1026 2023-01-15 12:17:52.330665 lnhub_rest-0.8.2/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1094 2023-04-22 04:59:42.149916 lnhub_rest-0.8.2/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.8.2/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0      998 2023-04-19 18:12:02.222640 lnhub_rest-0.8.2/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.8.2/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.8.2/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.8.2/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.8.2/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.8.2/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.8.2/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.8.2/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.8.2/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.8.2/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     2735 2023-04-18 16:02:04.948532 lnhub_rest-0.8.2/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.8.2/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.8.2/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.8.2/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6751 2023-04-22 04:02:09.361507 lnhub_rest-0.8.2/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.8.2/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.8.2/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.8.2/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.8.2/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.8.2/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     2861 2023-04-19 15:57:22.493317 lnhub_rest-0.8.2/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.8.2/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      796 2023-04-19 18:12:02.223356 lnhub_rest-0.8.2/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.8.2/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-19 18:12:02.224109 lnhub_rest-0.8.2/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     2543 2023-04-19 18:12:02.224813 lnhub_rest-0.8.2/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      198 2023-04-18 16:02:04.950703 lnhub_rest-0.8.2/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4121 2023-04-18 16:02:04.950818 lnhub_rest-0.8.2/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.8.2/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.8.2/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     4317 2023-04-19 15:57:22.493965 lnhub_rest-0.8.2/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.8.2/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.8.2/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.8.2/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.8.2/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.8.2/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.8.2/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.8.2/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.8.2/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.8.2/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       50 2023-04-18 16:02:04.953110 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     2979 2023-04-19 18:12:02.225453 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0      757 2023-04-19 18:12:02.225538 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/settings.py
+-rw-r--r--   0        0        0     5549 2023-04-19 18:12:02.226092 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.8.2/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.8.2/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.8.2/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.8.2/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.8.2/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.8.2/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1782 2023-04-19 15:57:22.494980 lnhub_rest-0.8.2/noxfile.py
+-rw-r--r--   0        0        0     1253 2023-04-18 16:02:04.957709 lnhub_rest-0.8.2/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.8.2/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.8.2/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.8.2/supabase/config.toml
+-rw-r--r--   0        0        0      864 2023-04-19 15:57:22.495574 lnhub_rest-0.8.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 lnhub_rest-0.8.2/PKG-INFO
```

### Comparing `lnhub_rest-0.8.1/.dockerignore` & `lnhub_rest-0.8.2/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/.github/workflows/build.yml` & `lnhub_rest-0.8.2/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
         package:
           - "lnhub-rest"
           - "lndb"
+        lamin_env:
+          - "local"
+          - "staging"
     timeout-minutes: 25
 
     steps:
       - name: Checkout main
         uses: actions/checkout@v3
         with:
           submodules: recursive
@@ -83,13 +86,13 @@
       - name: Configure Google Cloud
         id: "auth"
         uses: "google-github-actions/auth@v0"
         with:
           credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
       - name: Build
         run: |
-          nox -s "build(package='${{ matrix.package }}')"
+          nox -s "build(lamin_env='${{ matrix.lamin_env }}', package='${{ matrix.package }}')"
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `lnhub_rest-0.8.1/.github/workflows/google-cloudrun-docker.yml` & `lnhub_rest-0.8.2/.github/workflows/google-cloudrun-docker.yml`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 #   Container Registry vs Artifact Registry   - https://cloud.google.com/blog/products/application-development/understanding-artifact-registry-vs-container-registry
 #   Principle of least privilege              - https://cloud.google.com/blog/products/identity-security/dont-get-pwned-practicing-the-principle-of-least-privilege
 
 name: Build and Deploy to Cloud Run
 
 on:
   push:
-    branches: ["main", "staging"]
+    branches: ["staging"]
+  release:
+    types: [published]
 
 env:
   PROJECT_ID: ${{ secrets.GCP_PROJECT_ID }} # TODO: update Google Cloud project id
   GAR_LOCATION: us-central1 # TODO: update Artifact Registry location
   SERVICE: lnhub-rest-cloud-run-$GITHUB_REF_NAME # TODO: update Cloud Run service name
   REGION: us-central1 # TODO: update Cloud Run service region
   REPO_NAME: ${{ github.event.repository.name }}
```

### Comparing `lnhub_rest-0.8.1/.github/workflows/latest-changes.yml` & `lnhub_rest-0.8.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/.gitignore` & `lnhub_rest-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/.pre-commit-config.yaml` & `lnhub_rest-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/README.md` & `lnhub_rest-0.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # lnhub-rest: Cross-instance management
 
-Note: For more extensive documentation, see [docs/content](docs/content.md).
+Note: For more extensive documentation & testing, see [docs](docs).
 
 ## Summary
 
 1. Installation
 2. CLI
    1. Run server
    2. Run tests
```

### Comparing `lnhub_rest-0.8.1/docs/account/01-signup-signin.ipynb` & `lnhub_rest-0.8.2/docs/02-account/01-signup-signin.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923611111111111%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from lnhub_rest.orm._sbclient import connect_hub\\n'), "*

 * *            "(2, 'from lnhub_rest.core.account._signup_signin import sign_up_hub\\n'), (3, 'from "*

 * *            "lnhub_rest.core.account._signup_signin import sign_in_hub\\n')], delete: [3, 2, 0]}}, "*

 * *            'delete: [20]}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -9,18 +9,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lnhub_rest._sbclient import connect_hub\n",
+                "from lnhub_rest.orm._sbclient import connect_hub\n",
                 "from lnhub_rest._clean_ci import delete_ci_accounts\n",
-                "from lnhub_rest._signup_signin import sign_up_hub\n",
-                "from lnhub_rest._signup_signin import sign_in_hub\n",
+                "from lnhub_rest.core.account._signup_signin import sign_up_hub\n",
+                "from lnhub_rest.core.account._signup_signin import sign_in_hub\n",
                 "import jwt\n",
                 "import string, secrets\n",
                 "import os\n",
                 "\n",
                 "# Ensure using production or staging environment to perform this test\n",
                 "# as we need autoconfirm supabase parameter to be off\n",
                 "# and testuser1 to exists\n",
@@ -196,21 +196,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Switch back to local environment\n",
                 "if lamin_env == \"local\":\n",
                 "    os.environ[\"LAMIN_ENV\"] = lamin_env"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -221,15 +214,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/account/02-create-account.ipynb` & `lnhub_rest-0.8.2/docs/02-account/02-create-account.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9890873015873016%*

 * *Differences: {"'cells'": "{2: {delete: ['attachments']}, 5: {delete: ['attachments']}, 12: {delete: "*

 * *            "['attachments']}, 18: {delete: ['attachments']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'version': '3.9.15'}}"}*

```diff
@@ -18,15 +18,14 @@
                 "from lnhub_rest.core.account import create_user_account, delete_account\n",
                 "from lnhub_rest.utils._test import create_test_auth\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parameterize"
             ]
         },
         {
@@ -48,15 +47,14 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Create a new account"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Call `create_user_account`"
             ]
         },
         {
@@ -116,15 +114,14 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Create a new account using an existing handle"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Call `create_user_account` on existing account"
             ]
         },
         {
@@ -177,15 +174,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert response.json() == \"handle-exists-already\""
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Clean up"
             ]
         },
         {
@@ -206,29 +202,29 @@
             "source": [
                 "clean_ci()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "base",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/account/03-update-account.ipynb` & `lnhub_rest-0.8.2/docs/02-account/03-update-account.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995673740510697%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from lnhub_rest.orm._sbclient import connect_hub\\n')], "*

 * *            "delete: [3]}}, 2: {delete: ['attachments']}, 20: {delete: ['attachments']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -12,23 +12,22 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import update_account, delete_account\n",
                 "from lnhub_rest.core.account._crud import sb_select_account_by_handle\n",
                 "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
-                "from lnhub_rest._sbclient import connect_hub\n",
+                "from lnhub_rest.orm._sbclient import connect_hub\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci\n",
                 "\n",
                 "hub = connect_hub()"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parameterize"
             ]
         },
         {
@@ -209,15 +208,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert response.json() == \"account-not-exists\""
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Clean up"
             ]
         },
         {
@@ -251,15 +249,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/account/04-fetch-account.ipynb` & `lnhub_rest-0.8.2/docs/02-account/04-fetch-account.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956909937888199%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'from lnhub_rest.orm._sbclient import "*

 * *            "get_access_token\\n'), (8, 'from lnhub_rest.orm._sbclient import connect_hub\\n')], "*

 * *            "delete: [8, 1]}}, 2: {delete: ['attachments']}, 20: {delete: ['attachments']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -10,36 +10,35 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from deepdiff import DeepDiff\n",
-                "from lnhub_rest._sbclient import get_access_token\n",
+                "from lnhub_rest.orm._sbclient import get_access_token\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest.routers.account import (\n",
                 "    get_account_by_handle,\n",
                 "    get_account_by_id,\n",
                 "    get_account_instances,\n",
                 ")\n",
-                "from lnhub_rest._sbclient import connect_hub\n",
+                "from lnhub_rest.orm._sbclient import connect_hub\n",
                 "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    create_test_storage,\n",
                 "    create_test_instance,\n",
                 "    add_test_collaborator,\n",
                 ")\n",
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.instance import delete_instance\n",
                 "from lnhub_rest._clean_ci import clean_ci"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parameterize "
             ]
         },
         {
@@ -215,15 +214,14 @@
                 "    f\"/account/resources/instances/{account_handle}\",\n",
                 "    headers={\"authentication\": f\"Bearer {access_token}\"},\n",
                 ")\n",
                 "assert str(response.json()) == str(account_instances_expected)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Clean up"
             ]
         },
         {
@@ -258,15 +256,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/account/05-rls.ipynb` & `lnhub_rest-0.8.2/docs/02-account/05-rls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983928571428571%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(1, 'from lnhub_rest.orm._sbclient import connect_hub, "*

 * *            "connect_hub_with_auth\\n'), (2, 'from lnhub_rest.utils._test import create_test_auth, "*

 * *            "create_test_account\\n')], delete: [1, 0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -22,17 +22,17 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
-                "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
                 "import pytest\n",
+                "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
+                "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
                 "from lnhub_rest.core.account._crud import (\n",
                 "    sb_insert_account,\n",
                 "    sb_update_account,\n",
                 "    sb_select_account_by_handle,\n",
                 "    sb_delete_account,\n",
                 ")\n",
                 "import string, secrets\n",
@@ -374,15 +374,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/changelog.md` & `lnhub_rest-0.8.2/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🍱  Add schema module `lamin1` | [187](https://github.com/laminlabs/lnhub-rest/pull/187) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.8.2
+:children_crossing: Ask for postgresql instead of postgres | [186](https://github.com/laminlabs/lnhub-rest/pull/186) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 |
+👷 Run tests on staging | [179](https://github.com/laminlabs/lnhub-rest/pull/179) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
+✅ Decouple tests from lndb-related objects | [184](https://github.com/laminlabs/lnhub-rest/pull/184) | [bpenteado](https://github.com/bpenteado) | 2023-04-20 |
+💚 Fix tests | [178](https://github.com/laminlabs/lnhub-rest/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
+🚚 Rename folders in docs | [177](https://github.com/laminlabs/lnhub-rest/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
+🏗️ Clean up historical migrations & remove cloning from production for migrations testing | [175](https://github.com/laminlabs/lnhub-rest/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 🏗️ Fix local development setup | [174](https://github.com/laminlabs/lnhub-rest/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.8.1
 🗃️ Fix RLS for storage table | [173](https://github.com/laminlabs/lnhub-rest/pull/173) | [fredericenard](https://github.com/fredericenard) | 2023-04-18 |
 ✨ Create organization endpoints | [165](https://github.com/laminlabs/lnhub-rest/pull/165) | [bpenteado](https://github.com/bpenteado) | 2023-04-17 |
 👷 Run tests against `lndb` | [143](https://github.com/laminlabs/lnhub-rest/pull/143) | [falexwolf](https://github.com/falexwolf) | 2023-04-13 |
 ♻️ Simplify migrations testing | [168](https://github.com/laminlabs/lnhub-rest/pull/168) | [falexwolf](https://github.com/falexwolf) | 2023-04-12 |
 🗃️ Create organization membership table | [163](https://github.com/laminlabs/lnhub-rest/pull/163) | [bpenteado](https://github.com/bpenteado) | 2023-04-11 |
 🗃️ Reset RLS policies | [161](https://github.com/laminlabs/lnhub-rest/pull/161) | [bpenteado](https://github.com/bpenteado) | 2023-04-05 |
```

### Comparing `lnhub_rest-0.8.1/docs/checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.8.2/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9651785714285714%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'from lnhub_rest.orm._sbclient import connect_hub')], "*

 * *            'delete: [1]}}, delete: [3]}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -10,35 +10,28 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest._check_breaks_lndb import check_breaks_lndb\n",
-                "from lnhub_rest._sbclient import connect_hub"
+                "from lnhub_rest.orm._sbclient import connect_hub"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "hub = connect_hub()\n",
                 "breaks_lndb = check_breaks_lndb(hub)\n",
                 "print(breaks_lndb)\n",
                 "assert isinstance(breaks_lndb, bool)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -49,15 +42,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/instance/01-init-instance.ipynb` & `lnhub_rest-0.8.2/docs/03-instance/01-init-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997465156794425%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(6, 'from lnhub_rest.orm._sbclient import connect_hub, "*

 * *            "connect_hub_with_auth\\n')], delete: [6]}}, 5: {'source': {insert: [(9, '    "*

 * *            '"s3://lnhub-rest-ci"\\n\')], delete: [9]}}, 21: {\'source\': {insert: [(1, \'assert '*

 * *            'storage.region == "eu-central-1"\')], delete: [1]}}, 38: {delete: [\'attachments\']}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -24,15 +24,15 @@
             "source": [
                 "from lnhub_rest.core.storage._add_storage import validate_root_arg\n",
                 "from lnhub_rest.core.instance._init_instance import (\n",
                 "    validate_db_arg,\n",
                 "    validate_schema_arg,\n",
                 "    validate_storage_arg,\n",
                 ")\n",
-                "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
                 "from lnhub_rest.core.instance import init_instance, delete_instance\n",
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest._clean_ci import delete_ci_instances\n",
                 "import sqlmodel as sqm\n",
                 "from lnhub_rest.schema import Instance, Account, Storage\n",
                 "from lnhub_rest.main import client\n",
                 "import string, secrets\n",
@@ -72,15 +72,15 @@
                 "auth_1 = create_test_auth()\n",
                 "access_token_1 = auth_1[\"access_token\"]\n",
                 "account_1 = create_test_account(handle=auth_1[\"handle\"], access_token=access_token_1)\n",
                 "account_id_1 = account_1[\"id\"]\n",
                 "account_handle_1 = account_1[\"handle\"]\n",
                 "\n",
                 "existing_storage_root = (  # need to test setting the region parameter\n",
-                "    \"s3://lndb-setup-ci\"\n",
+                "    \"s3://lnhub-rest-ci\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -215,15 +215,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert storage.root == existing_storage_root\n",
-                "assert storage.region == \"us-east-1\""
+                "assert storage.region == \"eu-central-1\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Post method on `/instance` route"
@@ -412,15 +412,14 @@
                 "validate_db_arg(postgresdsn)\n",
                 "mysqldsn = \"mssql://postgres:pwd@0.0.0.0:5432/pgtest\"\n",
                 "with pytest.raises(ValueError):\n",
                 "    validate_db_arg(mysqldsn)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Clean up test assets"
             ]
         },
         {
@@ -460,15 +459,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/instance/02-load-instance.ipynb` & `lnhub_rest-0.8.2/docs/03-instance/02-load-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984130905326558%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, 'from lnhub_rest.orm._sbclient import connect_hub\\n')], "*

 * *            'delete: [6]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -15,15 +15,15 @@
             "source": [
                 "from lnhub_rest.core.instance import init_instance, load_instance, delete_instance\n",
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest._clean_ci import delete_ci_instances\n",
                 "import sqlmodel as sqm\n",
                 "from lnhub_rest.schema import Instance, Account\n",
                 "import string, secrets\n",
-                "from lnhub_rest._sbclient import connect_hub\n",
+                "from lnhub_rest.orm._sbclient import connect_hub\n",
                 "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
                 "from lnhub_rest.orm._engine import engine\n",
                 "from lnhub_rest._clean_ci import clean_ci"
             ]
         },
         {
             "cell_type": "code",
@@ -236,15 +236,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/instance/03-update-instance.ipynb` & `lnhub_rest-0.8.2/docs/03-instance/03-update-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375000000001%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(10, 'from lnhub_rest.orm._sbclient import "*

 * *            "connect_hub_with_auth\\n')], delete: [10]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -19,15 +19,15 @@
                 "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    create_test_instance,\n",
                 "    create_test_storage,\n",
                 "    add_test_collaborator,\n",
                 ")\n",
-                "from lnhub_rest._sbclient import connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub_with_auth\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -262,15 +262,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/instance/04-delete-instance.ipynb` & `lnhub_rest-0.8.2/docs/03-instance/04-delete-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984684265010352%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(14, 'from lnhub_rest.orm._sbclient import connect_hub, "*

 * *            "connect_hub_with_auth\\n')], delete: [14]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -23,15 +23,15 @@
                 "from lnhub_rest.core.collaborator._crud import sb_select_collaborators\n",
                 "from lnhub_rest.routers.instance import get_instance_accounts\n",
                 "from lnhub_rest._clean_ci import delete_ci_instances\n",
                 "import sqlmodel as sqm\n",
                 "from lnhub_rest.schema import Instance\n",
                 "from lnhub_rest.main import client\n",
                 "import string, secrets\n",
-                "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
                 "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    add_test_collaborator,\n",
                 ")\n",
                 "from lnhub_rest.orm._engine import engine\n",
                 "from lnhub_rest._clean_ci import clean_ci"
@@ -330,15 +330,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/instance/05-fetch-instance.ipynb` & `lnhub_rest-0.8.2/docs/03-instance/05-fetch-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983803258145363%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from lnhub_rest.orm._sbclient import "*

 * *            "get_access_token\\n'), (9, 'from lnhub_rest.orm._sbclient import connect_hub\\n')], "*

 * *            'delete: [9, 3]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -12,21 +12,21 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from deepdiff import DeepDiff\n",
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.instance import delete_instance\n",
-                "from lnhub_rest._sbclient import get_access_token\n",
+                "from lnhub_rest.orm._sbclient import get_access_token\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest.routers.instance import (\n",
                 "    get_instance_accounts,\n",
                 "    get_instance_by_name,\n",
                 ")\n",
-                "from lnhub_rest._sbclient import connect_hub\n",
+                "from lnhub_rest.orm._sbclient import connect_hub\n",
                 "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    create_test_storage,\n",
                 "    create_test_instance,\n",
                 "    add_test_collaborator,\n",
                 ")\n",
@@ -260,15 +260,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/instance/06-rls.ipynb` & `lnhub_rest-0.8.2/docs/03-instance/06-rls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966905290222599%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from lnhub_rest.orm._sbclient import connect_hub, "*

 * *            "connect_hub_with_auth\\n')], delete: [2]}}, 14: {delete: ['attachments']}, 16: "*

 * *            "{delete: ['attachments']}, 23: {delete: ['attachments']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -13,15 +13,15 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.instance import delete_instance\n",
-                "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
                 "import pytest\n",
                 "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    create_test_storage,\n",
                 ")\n",
                 "from lnhub_rest.core.instance._crud import (\n",
@@ -222,15 +222,14 @@
                 "        supabase_client=account_hub_1,\n",
                 "    )\n",
                 "    is not None\n",
                 ")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A admin can add a collaborator with a read role."
             ]
         },
         {
@@ -257,15 +256,14 @@
                 "        supabase_client=account_hub_2,\n",
                 "    )\n",
                 "    is not None\n",
                 ")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A collaborator with a read role can't add a collaborator."
             ]
         },
         {
@@ -347,15 +345,14 @@
                 "        supabase_client=account_hub_2,\n",
                 "    )[\"role\"]\n",
                 "    == \"write\"\n",
                 ")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A member with a non admin role can't update a collaborator."
             ]
         },
         {
@@ -754,15 +751,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/migration/01-migration.ipynb` & `lnhub_rest-0.8.2/docs/00-migrate.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9770833333333333%*

 * *Differences: {"'cells'": "{1: {'source': ['from lnhub_rest._ci import start_local_supabase\\n', 'from "*

 * *            "lnhub_rest.schema.migrations.testing import (\\n', '    "*

 * *            "migration_id_is_consistent,\\n', '    model_definitions_match_ddl,\\n', ')']}, 2: "*

 * *            "{'metadata': {replace: OrderedDict()}, 'source': ['migration_id_is_consistent()  # "*

 * *            'checks consistency of the migration id in scripts with the one in '*

 * *            "schema/__init__.py']}, 3: {'source': ['!export LN_SERVER_DEPL […]*

```diff
@@ -13,61 +13,55 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "import os\n",
-                "\n",
-                "os.chdir(\"../../\")"
+                "from lnhub_rest._ci import start_local_supabase\n",
+                "from lnhub_rest.schema.migrations.testing import (\n",
+                "    migration_id_is_consistent,\n",
+                "    model_definitions_match_ddl,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from lnhub_rest.schema.migrations.testing import (\n",
-                "    migration_id_is_consistent,\n",
-                "    model_definitions_match_ddl,\n",
-                ")"
+                "migration_id_is_consistent()  # checks consistency of the migration id in scripts with the one in schema/__init__.py"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "migration_id_is_consistent()  # checks consistency of the migration id in scripts with the one in schema/__init__.py"
+                "!export LN_SERVER_DEPLOY=1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "model_definitions_match_ddl(clone=True)"
+                "pgurl = start_local_supabase()"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Alternative workflow:\n",
-                "\n",
-                "1. Install lnhub_rest version 0.4.0.\n",
-                "2. Create an empty Supabase postgres and create the schema with version 0.4.0. This creates a test DB that replaces the cloning-based test DB.\n",
-                "3. Install the current lnhub-rest version to run tests.\n",
-                "3. Pass the connection string to the database to `execute_model_definitions_match_ddl` as an arg."
+                "model_definitions_match_ddl(test_db=pgurl)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lnhub_rest-0.8.1/docs/migrations.md` & `lnhub_rest-0.8.2/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.8.2/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/docs/organization/01-create-organization.ipynb` & `lnhub_rest-0.8.2/docs/05-organization/01-create-organization.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968063186813187%*

 * *Differences: {"'cells'": "{1: {'metadata': {replace: OrderedDict([('tags', [])])}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -6,15 +6,17 @@
             "source": [
                 "# Test create organization"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import sqlmodel as sqm\n",
                 "\n",
                 "# Test subjects\n",
                 "from lnhub_rest.core.account import create_organization_account\n",
                 "\n",
@@ -153,13 +155,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lnhub_rest-0.8.1/docs/organization/02-manage-members.ipynb` & `lnhub_rest-0.8.2/docs/05-organization/02-manage-members.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975942460317461%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(7, 'from lnhub_rest.orm._sbclient import "*

 * *            "connect_hub_with_auth\\n')], delete: [7]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -16,15 +16,15 @@
                 "import sqlmodel as sqm\n",
                 "\n",
                 "# Test assets\n",
                 "from lnhub_rest.core.account import create_organization_account\n",
                 "\n",
                 "# Test utils\n",
                 "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
-                "from lnhub_rest._sbclient import connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub_with_auth\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci\n",
                 "from lnhub_rest.utils._id import base62"
             ]
         },
         {
             "cell_type": "markdown",
@@ -154,13 +154,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lnhub_rest-0.8.1/docs/organization/03-rls.ipynb` & `lnhub_rest-0.8.2/docs/05-organization/03-rls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976717032967033%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(8, 'from lnhub_rest.orm._sbclient import "*

 * *            "connect_hub_with_auth\\n')], delete: [8]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -17,15 +17,15 @@
                 "import pytest\n",
                 "\n",
                 "# Test assets\n",
                 "from lnhub_rest.core.account import create_organization_account\n",
                 "\n",
                 "# Test utils\n",
                 "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
-                "from lnhub_rest._sbclient import connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub_with_auth\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci\n",
                 "from lnhub_rest.utils._id import base62"
             ]
         },
         {
             "cell_type": "markdown",
@@ -227,13 +227,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lnhub_rest-0.8.1/docs/storage/01-add-storage.ipynb` & `lnhub_rest-0.8.2/docs/04-storage/01-add-storage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981398809523809%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, 'from lnhub_rest.orm._sbclient import connect_hub, "*

 * *            "connect_hub_with_auth\\n')], delete: [4]}}, 3: {'source': {insert: [(6, "*

 * *            '\'existing_storage_root = "s3://lnhub-rest-ci"\')], delete: [6]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -13,15 +13,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.storage import add_storage\n",
                 "import sqlmodel as sqm\n",
                 "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
-                "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
                 "from lnhub_rest._clean_ci import clean_ci"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -36,15 +36,15 @@
             "source": [
                 "hub = connect_hub()\n",
                 "\n",
                 "auth = create_test_auth()\n",
                 "access_token = auth[\"access_token\"]\n",
                 "account = create_test_account(handle=auth[\"handle\"], access_token=access_token)\n",
                 "\n",
-                "existing_storage_root = \"s3://lndb-setup-ci\""
+                "existing_storage_root = \"s3://lnhub-rest-ci\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Add a storage"
@@ -178,15 +178,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/docs/storage/02-rls.ipynb` & `lnhub_rest-0.8.2/docs/04-storage/02-rls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984698172198172%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'from lnhub_rest.orm._sbclient import connect_hub, "*

 * *            "connect_hub_with_auth\\n')], delete: [1]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.15'}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import delete_account\n",
-                "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
+                "from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth\n",
                 "import pytest\n",
                 "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    create_test_storage,\n",
                 ")\n",
                 "from lnhub_rest.core.storage._crud import (\n",
@@ -396,15 +396,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.1/lndb/.github/workflows/build.yml` & `lnhub_rest-0.8.2/lndb/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/.github/workflows/latest-changes.yml` & `lnhub_rest-0.8.2/lndb/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/.gitignore` & `lnhub_rest-0.8.2/lndb/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/.pre-commit-config.yaml` & `lnhub_rest-0.8.2/lndb/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/LICENSE` & `lnhub_rest-0.8.2/lndb/LICENSE`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/changelog.md` & `lnhub_rest-0.8.2/lndb/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Restructure hub imports | [357](https://github.com/laminlabs/lndb/pull/357) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
+⬆️ Upgrade to lnhub_rest 0.8.1 | [356](https://github.com/laminlabs/lndb/pull/356) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.42.0
+✅ Use nbproject-test directly | [355](https://github.com/laminlabs/lndb/pull/355) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 |
 🔊 Clarify access based on locally cached instance metadata | [354](https://github.com/laminlabs/lndb/pull/354) | [falexwolf](https://github.com/falexwolf) | 2023-04-11 | 0.41.0
 🎨 Move setup checks from lamindb here | [352](https://github.com/laminlabs/lndb/pull/352) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 | 0.41rc1
 🔧 Increase configure-aws-credentials version from v1 to v2 | [344](https://github.com/laminlabs/lndb/pull/344) | [Zethson](https://github.com/Zethson) | 2023-04-07 |
 🚸 Expose `id` in `StorageSettings` | [351](https://github.com/laminlabs/lndb/pull/351) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.2
 ➕ Add cloudpathlib back | [350](https://github.com/laminlabs/lndb/pull/350) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.1
 🚸 Rename settings directory to `.lamin` | [349](https://github.com/laminlabs/lndb/pull/349) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.0
 🚸 Expose storage in settings | [348](https://github.com/laminlabs/lndb/pull/348) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 |
```

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/check-synchronization.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/clone.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/edge-cases-login-init.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/manage-migrations.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/switch-environment.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/test-migrations-e2e.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/faq/test-migrations-unit.ipynb` & `lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/01-setup-user.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/02-init-instance.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/03-load-instance.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/04-set-storage.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/05-schema-modules.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/06-info.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/07-delete.ipynb` & `lnhub_rest-0.8.2/lndb/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/docs/guide/migrate.md` & `lnhub_rest-0.8.2/lndb/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/__init__.py` & `lnhub_rest-0.8.2/lndb/lndb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.41.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.42.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/__main__.py` & `lnhub_rest-0.8.2/lndb/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_check_instance_setup.py` & `lnhub_rest-0.8.2/lndb/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_close.py` & `lnhub_rest-0.8.2/lndb/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_delete.py` & `lnhub_rest-0.8.2/lndb/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_init_instance.py` & `lnhub_rest-0.8.2/lndb/lndb/_init_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import importlib
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
-from lnhub_rest._add_storage import get_storage_region
-from lnhub_rest._init_instance import init_instance as init_instance_hub
-from lnhub_rest._init_instance import (
+from lnhub_rest.core.instance._init_instance import init_instance as init_instance_hub
+from lnhub_rest.core.instance._init_instance import (
     validate_db_arg,
     validate_schema_arg,
     validate_storage_arg,
 )
+from lnhub_rest.core.storage._add_storage import get_storage_region
 from pydantic import PostgresDsn
 
 from lndb.dev.upath import UPath
 
 from ._load_instance import load, load_from_isettings
 from ._settings import settings
 from .dev import InstanceSettings
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_load_instance.py` & `lnhub_rest-0.8.2/lndb/lndb/_load_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from typing import Optional
 
 from lamin_logger import logger
-from lnhub_rest._load_instance import load_instance as load_instance_from_hub
+from lnhub_rest.core.instance._load_instance import (
+    load_instance as load_instance_from_hub,
+)
 
 from ._settings import InstanceSettings, settings
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 
 
 def load(
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_migrate/alembic.ini` & `lnhub_rest-0.8.2/lndb/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_migrate/core.py` & `lnhub_rest-0.8.2/lndb/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_migrate/deploy.py` & `lnhub_rest-0.8.2/lndb/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_migrate/env.py` & `lnhub_rest-0.8.2/lndb/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_migrate/utils.py` & `lnhub_rest-0.8.2/lndb/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_schema.py` & `lnhub_rest-0.8.2/lndb/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_set.py` & `lnhub_rest-0.8.2/lndb/lndb/_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import Union
 
 from lamin_logger import logger
-from lnhub_rest._add_storage import add_storage as add_storage_hub
+from lnhub_rest.core.storage._add_storage import add_storage as add_storage_hub
 
 from lndb.dev.upath import UPath
 
 from ._init_instance import register
 from ._settings import settings
 from .dev import deprecated
 from .dev._settings_instance import InstanceSettings
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_settings.py` & `lnhub_rest-0.8.2/lndb/lndb/_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return self.fget(owner_cls)
 
 
 class settings:
     """Settings access.
 
     - :class:`~lndb.dev.InstanceSettings`
-    - :class:`~lndb.dev.Storage`
+    - :class:`~lndb.dev.StorageSettings`
     - :class:`~lndb.dev.UserSettings`
     """
 
     _user_settings: Union[UserSettings, None] = None
     _instance_settings: Union[InstanceSettings, None] = None
 
     _user_settings_env: Union[str, None] = None
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/_setup_user.py` & `lnhub_rest-0.8.2/lndb/lndb/_setup_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union
 
 from lamin_logger import logger
-from lnhub_rest._signup_signin import sign_in_hub, sign_up_hub
+from lnhub_rest.core.account._signup_signin import sign_in_hub, sign_up_hub
 from sqlalchemy import create_engine
 
 from ._settings import settings
 from .dev._db import upsert
 from .dev._settings_load import load_or_create_user_settings, load_user_settings
 from .dev._settings_save import save_user_settings
 from .dev._settings_store import user_settings_file_email, user_settings_file_handle
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/__init__.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_clone.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_db.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_deprecated.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_exclusion.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_settings_instance.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_settings_load.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_settings_save.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_settings_store.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_settings_user.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_setup_knowledge.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_setup_schema.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/_storage.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/dev/upath.py` & `lnhub_rest-0.8.2/lndb/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/lndb/test/_migrations_e2e.py` & `lnhub_rest-0.8.2/lndb/lndb/test/_migrations_e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from subprocess import run
 from typing import Optional
 
 from lamin_logger import logger
 from lnhub_rest._assets import instances as test_instances
-from lnhub_rest._init_instance import (
+from lnhub_rest.core.instance._init_instance import (
     validate_db_arg,
     validate_schema_arg,
     validate_storage_arg,
 )
 
 from lndb._init_instance import infer_instance_name, init
 from lndb._settings import settings
```

### Comparing `lnhub_rest-0.8.1/lndb/lndb/test/_migrations_unit.py` & `lnhub_rest-0.8.2/lndb/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/noxfile.py` & `lnhub_rest-0.8.2/lndb/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/pyproject.toml` & `lnhub_rest-0.8.2/lndb/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.7.2",
+    "lnhub_rest==0.8.1",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
@@ -39,14 +39,15 @@
     "nox",
 ]
 test = [
     "lamindb[bionty,wetlab]>=0.35.6",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
+    "nbproject",
 ]
 
 [project.scripts]
 lndb = "lndb.__main__:main"
 
 [tool.black]
 preview = true
```

### Comparing `lnhub_rest-0.8.1/lndb/tests/test_bionty.py` & `lnhub_rest-0.8.2/lndb/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lndb/tests/test_init_instance.py` & `lnhub_rest-0.8.2/lndb/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/__main__.py` & `lnhub_rest-0.8.2/lnhub_rest/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,74 +42,74 @@
 # Helpers to check environment variables
 
 
 def check_lamin_env():
     response = input("Choose an environment (local/staging/prod): ")
 
     if response not in ["local", "staging", "prod"]:
-        raise SystemExit(
+        raise RuntimeError(
             f"Error: '{response}' is not a valid choice, choose local, staging or prod."
         )
 
     if "LAMIN_ENV" in os.environ:
         lamin_env = os.environ["LAMIN_ENV"]
     else:
-        raise SystemExit(
+        raise RuntimeError(
             "Error: Current LAMIN_ENV is not set"
             f", run 'export LAMIN_ENV={response}' and try again."
         )
 
     if lamin_env != response:
-        raise SystemExit(
+        raise RuntimeError(
             f"Error: Current LAMIN_ENV is set on {lamin_env}"
             f", run 'export LAMIN_ENV={response}' and try again."
         )
 
     return lamin_env
 
 
 def check_env_ln_server_deploy():
     if "LN_SERVER_DEPLOY" not in os.environ:
-        raise SystemExit(
+        raise RuntimeError(
             "Current LN_SERVER_DEPLOY is not set"
             ", run 'export LN_SERVER_DEPLOY=1' and try again."
         )
 
 
 def check_env_lnhub_pg_password(lamin_env: Literal["local", "staging", "prod"]):
     if lamin_env == "staging":
         if "LNHUB_STAGING_PG_PASSWORD" not in os.environ:
-            raise SystemExit("Current LNHUB_STAGING_PG_PASSWORD is not set.")
+            raise RuntimeError("Current LNHUB_STAGING_PG_PASSWORD is not set.")
     elif lamin_env == "prod":
         if "LNHUB_PROD_PG_PASSWORD" not in os.environ:
-            raise SystemExit("Current LNHUB_PROD_PG_PASSWORD is not set.")
+            raise RuntimeError("Current LNHUB_PROD_PG_PASSWORD is not set.")
 
 
 def check_env_supabase_url(lamin_env: Literal["local", "staging", "prod"]):
     if lamin_env == "staging":
         if "SUPABASE_STAGING_URL" not in os.environ:
-            raise SystemExit("Current SUPABASE_STAGING_URL is not set.")
+            raise RuntimeError("Current SUPABASE_STAGING_URL is not set.")
     elif lamin_env == "prod":
         if "SUPABASE_PROD_URL" not in os.environ:
-            raise SystemExit("Current SUPABASE_PROD_URL is not set.")
+            raise RuntimeError("Current SUPABASE_PROD_URL is not set.")
 
 
 def check_env_supabase_anon_key(lamin_env: Literal["local", "staging", "prod"]):
     if lamin_env == "staging":
         if "SUPABASE_STAGING_ANON_KEY" not in os.environ:
-            raise SystemExit("Current SUPABASE_STAGING_ANON_KEY is not set.")
+            raise RuntimeError("Current SUPABASE_STAGING_ANON_KEY is not set.")
 
 
 def check_env_supabase_service_role_key(lamin_env: Literal["local", "staging", "prod"]):
     if lamin_env == "staging":
         if "SUPABASE_STAGING_SERVICE_ROLE_KEY" not in os.environ:
-            raise SystemExit("Current SUPABASE_STAGING_SERVICE_ROLE_KEY is not set.")
+            raise RuntimeError("Current SUPABASE_STAGING_SERVICE_ROLE_KEY is not set.")
     elif lamin_env == "prod":
         if "SUPABASE_PROD_SERVICE_ROLE_KEY" not in os.environ:
-            raise SystemExit("Current SUPABASE_PROD_SERVICE_ROLE_KEY is not set.")
+            raise RuntimeError("Current SUPABASE_PROD_SERVICE_ROLE_KEY is not set.")
 
 
 # CLI
 
 
 def generate():
     run(
@@ -126,50 +126,50 @@
     from lnhub_rest.schema import __version__, _migration
     from lnhub_rest.schema.versions import version_cbwk
 
     if len(__version__.split(".")) != 3:
         raise RuntimeError("Your __version__ string is not of form X.X.X")
 
     if breaks_lndb is None:
-        raise SystemExit("Error: Pass --breaks-lndb y or --breaks-lndb n")
+        raise RuntimeError("Error: Pass --breaks-lndb y or --breaks-lndb n")
 
     lamin_env = check_lamin_env()
     if lamin_env == "local":
-        raise SystemExit(
+        raise RuntimeError(
             "Execute ./docs/migration/01-migration.ipynb to perform migration on local"
             " supabase."
         )
     check_env_ln_server_deploy()
     check_env_lnhub_pg_password(lamin_env)
 
     if breaks_lndb:
         response = input(
             "Have you ensured that lndb and lamindb have releases on PyPI that users"
             " can pull?"
         )
         if response == "y":
             pass
         else:
-            raise SystemExit(
+            raise RuntimeError(
                 "Please test thoroughly and prepare releases for lndb and lamindb.\n"
                 "Pin lnhub_rest in lamindb, set a lower bound in lndb."
             )
 
     if settings.user.handle.startswith(("test", "static-test")):
-        raise SystemExit("Error: Log in with your developer handle, e.g., falexwolf")
+        raise RuntimeError("Error: Log in with your developer handle, e.g., falexwolf")
 
     # check that a release was made
     with sqm.Session(engine) as ss:
         deployed_v = ss.exec(
             sqm.select(version_cbwk.v)
             .order_by(version_cbwk.v.desc())  # type: ignore
             .limit(1)
         ).one()
     if deployed_v == __version__:
-        raise SystemExit("Error: Make a new release before deploying the migration!")
+        raise RuntimeError("Error: Make a new release before deploying the migration!")
     if vparse(deployed_v) > vparse(__version__):
         raise RuntimeError(
             "The new version has to be greater than the deployed version."
         )
 
     process = run(
         "alembic --config lnhub_rest/schema/alembic.ini --name cbwk upgrade head",
@@ -203,24 +203,21 @@
     )
 
 
 def test():
     lamin_env = check_lamin_env()
     check_env_ln_server_deploy()
     if lamin_env == "local":
-        # Needed to mirror the production schema
-        # to apply local migration
-        check_env_lnhub_pg_password("prod")
+        start_local_supabase()
         # Needed to enable sign in and signup tests
         # to be performed on staging environment
         check_env_supabase_url("staging")
         check_env_supabase_anon_key("staging")
         check_env_supabase_service_role_key("staging")
     else:
-        check_env_lnhub_pg_password(lamin_env)
         check_env_supabase_url(lamin_env)
         check_env_supabase_anon_key(lamin_env)
         check_env_supabase_service_role_key(lamin_env)
 
     run(
         "python3 -m nox",
         shell=True,
@@ -230,17 +227,14 @@
 def jupyter():
     lamin_env = check_lamin_env()
 
     if lamin_env == "local":
         # Needed to run the local migration
         # through migration notebook
         check_env_ln_server_deploy()
-        # Needed to mirror the production schema
-        # to apply local migration
-        check_env_lnhub_pg_password("prod")
         # Needed to enable sign in and signup tests
         # to be performed on staging environment
         check_env_supabase_url("staging")
         check_env_supabase_anon_key("staging")
         check_env_supabase_service_role_key("staging")
     else:
         check_env_supabase_url(lamin_env)
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/_assets/_instances.py` & `lnhub_rest-0.8.2/lnhub_rest/_assets/_instances.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.8.2/lnhub_rest/_assets/_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 # we might loosen the uniqueness requirement
 # currently, these handles are usually called "name"
 # this is confusing as there are also module names and lookup names
 schema_handles = [
     "hub",
     "bionty",
     "wetlab",
-    "drylab",
+    "lamin1",
     "hedera",
     "retro",
     "swarm",
     "harmonic-docking",
 ]
 schemas = schema_handles
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.8.2/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/_ci.py` & `lnhub_rest-0.8.2/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.8.2/lnhub_rest/_clean_ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, timedelta
 
 from lamin_logger import logger
 from sqlalchemy import text
 
-from lnhub_rest import engine
-from lnhub_rest._sbclient import connect_hub_with_auth
+from lnhub_rest.orm import engine
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 
 
 def delete_ci_instances() -> None:
     hub = connect_hub_with_auth()
     try:
         # Delete instances created by the CI more than one hour ago
         instance_to_delete = (
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.8.2/lnhub_rest/core/account/_create_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 from uuid import uuid4
 
 from postgrest.exceptions import APIError
 
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_insert_account
 from lnhub_rest.core.member._crud import sb_insert_member
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 from lnhub_rest.utils._access_token import extract_id
 from lnhub_rest.utils._id import base62
 
 
 def create_user_account(
     _access_token: str,
     handle: str,
@@ -28,18 +28,19 @@
             },
             hub,
         )
         assert account is not None
 
         return None
     except APIError as api_error:
-        usermeta_pkey_error = (
-            'duplicate key value violates unique constraint "usermeta_pkey"'
-        )
-        if api_error.message == usermeta_pkey_error:
+        # allowed errors
+        message = api_error.message
+        error1 = 'duplicate key value violates unique constraint "pk_account"'
+        error2 = 'duplicate key value violates unique constraint "usermeta_pkey"'
+        if message == error1 or message == error2:
             return "handle-exists-already"
         raise api_error
     except Exception as e:
         raise e
     finally:
         hub.auth.sign_out()
 
@@ -69,17 +70,18 @@
             },
             hub,
         )
         assert member is not None
 
         return None
     except APIError as api_error:
-        usermeta_pkey_error = (
-            'duplicate key value violates unique constraint "usermeta_pkey"'
-        )
-        if api_error.message == usermeta_pkey_error:
+        # allowed errors
+        message = api_error.message
+        error1 = 'duplicate key value violates unique constraint "pk_account"'
+        error2 = 'duplicate key value violates unique constraint "usermeta_pkey"'
+        if message == error1 or message == error2:
             return "handle-exists-already"
         raise api_error
     except Exception as e:
         raise e
     finally:
         hub.auth.sign_out()
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.8.2/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.8.2/lnhub_rest/core/account/_delete_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union
 
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_delete_account, sb_select_account_by_handle
 from lnhub_rest.core.collaborator._crud import sb_delete_collaborator_from_all_instances
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 
 
 def delete_account(
     handle: str,  # owner handle
     _access_token: Optional[str] = None,
 ) -> Union[None, str]:
     hub = connect_hub_with_auth(access_token=_access_token)
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.8.2/lnhub_rest/core/account/_signup_signin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from lamin_logger import logger
 
 from lnhub_rest import check_breaks_lndb_and_error
+from lnhub_rest.orm._sbclient import connect_hub, get_lamin_site_base_url
 from lnhub_rest.utils._id import secret
 
-from ..._sbclient import connect_hub, get_lamin_site_base_url
-
 
 def sign_up_hub(email) -> str:
     from lndb._settings_store import settings_dir
 
     hub = connect_hub()
     check_breaks_lndb_and_error(hub)
     password = secret()  # generate new password
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.8.2/lnhub_rest/core/account/_update_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Union
 
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_update_account
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 from lnhub_rest.utils._access_token import extract_id
 from lnhub_rest.utils._query import filter_null_from_dict
 
 
 def update_account(
     _access_token: str,
     handle: Optional[str] = None,
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.8.2/lnhub_rest/core/collaborator/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.8.2/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.8.2/lnhub_rest/core/instance/_delete_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional, Union
 
 from lnhub_rest import check_breaks_lndb_and_error
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_select_account_by_handle
 from lnhub_rest.core.instance._crud import (
     sb_delete_instance,
     sb_select_instance_by_name,
 )
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 
 
 def delete_instance(
     *,
     owner: str,  # owner handle
     name: str,  # instance name
     _email: Optional[str] = None,
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.8.2/lnhub_rest/core/instance/_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from typing import Mapping, Optional
 from uuid import UUID, uuid4
 
 from postgrest.exceptions import APIError
 
 from lnhub_rest import check_breaks_lndb_and_error
 from lnhub_rest._assets import schemas as known_schema_names
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_select_account_by_handle
 from lnhub_rest.core.collaborator._crud import sb_insert_collaborator
 from lnhub_rest.core.instance._crud import (
     sb_insert_instance,
     sb_select_instance_by_name,
 )
 from lnhub_rest.core.storage import add_storage
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 
 
 def init_instance(
     *,
     owner: str,  # owner handle
     name: str,  # instance name
     storage: str,  # storage location on cloud
@@ -142,14 +142,19 @@
             raise ValueError(
                 "`storage` is neither a valid local, a Google Cloud nor an S3 path."
             )
 
 
 def validate_db_arg(db: Optional[str]) -> None:
     if db is not None:
+        if db.startswith("postgres") and not db.startswith("postgresql"):
+            raise ValueError(
+                "Please follow the SQLAlchemy convention of prefixing the connection"
+                " string with 'postgresql://' instead of 'postgres://'"
+            )
         if not db.startswith("postgresql"):
             raise ValueError("Only postgres connection strings are allowed.")
         if not len(db.split("://")) == 2:
             raise ValueError("Your postgres URI does not contain '://'")
         remainder = db.split("://")[1]
         if not len(remainder.split("/")) == 2:
             raise ValueError("Your postgres URI does not end with a database '/dbname'")
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.8.2/lnhub_rest/core/instance/_load_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Tuple, Union
 
 from lnhub_rest import check_breaks_lndb_and_error
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_select_account_by_handle
 from lnhub_rest.core.instance._crud import sb_select_instance_by_name
 from lnhub_rest.core.storage._crud import sb_select_storage
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 from lnhub_rest.schema import Instance, Storage
 
 
 def load_instance(
     *,
     owner: str,  # owner handle
     name: str,  # instance name
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.8.2/lnhub_rest/core/instance/_update_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Union
 
-from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.instance._crud import sb_update_instance
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 from lnhub_rest.utils._query import filter_null_from_dict
 
 
 def update_instance(
     instance_id: str,
     account_id: Union[str, None] = None,
     public: Optional[bool] = False,
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.8.2/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.8.2/lnhub_rest/core/storage/_add_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from typing import Optional, Tuple
 from uuid import UUID, uuid4
 
 from lnhub_rest import check_breaks_lndb_and_error
 from lnhub_rest.core.storage._crud import sb_insert_storage, sb_select_storage_by_root
+from lnhub_rest.orm._sbclient import connect_hub_with_auth
 from lnhub_rest.utils._id import base62
 
-from ..._sbclient import connect_hub_with_auth
-
 
 def add_storage(
     root: str, account_handle: str, _access_token: Optional[str] = None
 ) -> Tuple[Optional[UUID], Optional[str]]:
     from botocore.exceptions import ClientError
 
     from lnhub_rest.core.account._crud import sb_select_account_by_handle
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.8.2/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/main.py` & `lnhub_rest-0.8.2/lnhub_rest/main.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.8.2/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/routers/account.py` & `lnhub_rest-0.8.2/lnhub_rest/routers/account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/routers/ci.py` & `lnhub_rest-0.8.2/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/routers/instance.py` & `lnhub_rest-0.8.2/lnhub_rest/routers/instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import Union
 
 from fastapi import APIRouter, Header
 
-from .._delete_instance import delete_instance as delete_instance_base
-from .._init_instance import init_instance as init_instance_base
-from ..core.instance._update_instance import update_instance as update_instance_base
+from lnhub_rest.core.instance._delete_instance import (
+    delete_instance as delete_instance_base,
+)
+from lnhub_rest.core.instance._init_instance import init_instance as init_instance_base
+from lnhub_rest.core.instance._update_instance import (
+    update_instance as update_instance_base,
+)
+
 from .account import get_account_by_handle
 from .utils import (
     extract_access_token,
     get_account_role_for_instance,
     get_supabase_client,
 )
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/routers/organization.py` & `lnhub_rest-0.8.2/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/routers/utils.py` & `lnhub_rest-0.8.2/lnhub_rest/routers/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
 import jwt
 from fastapi import Header
 
-from .._sbclient import connect_hub, connect_hub_with_auth
+from lnhub_rest.orm._sbclient import connect_hub, connect_hub_with_auth
 
 supabase_client = connect_hub()
 
 
 def get_account_role_for_instance(instance_id: str, access_token: str):
     supabase_client = connect_hub_with_auth(access_token=access_token)
     session_payload = jwt.decode(
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/_core.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.8.2/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/settings.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/settings.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-30-2efe1dee9baf-v0_1_4c.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""v0.1.4c.
+"""v0.6.1.
 
-Revision ID: 2efe1dee9baf
-Revises: e7151581f790
-Create Date: 2023-01-30 15:03:43.834723
+Revision ID: 0c4d4fe5f2c6
+Revises: a88f5298b8f7
+Create Date: 2023-03-09 09:37:32.028048
 
 """
 import sqlalchemy as sa  # noqa
 import sqlmodel  # noqa
 from alembic import op
 
+from lnhub_rest.schema.migrations.rls._2023_03_09_0c4d4fe5f2c6_v0_6_1 import (
+    sql_rls_migration,
+    sql_rls_version,
+)
+
 # revision identifiers, used by Alembic.
-revision = "2efe1dee9baf"
-down_revision = "e7151581f790"
+revision = "0c4d4fe5f2c6"
+down_revision = "a88f5298b8f7"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
-    op.add_column(
-        "account",
-        sa.Column("avatar_url", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
-    )
+    op.execute(sql_rls_migration)
+    op.execute(sql_rls_version)
 
 
 def downgrade() -> None:
     pass
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-9c02109e4faa-v0_2_0.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,52 @@
-"""v0.2.0.
+"""v0.8.dev1.
 
-Revision ID: 9c02109e4faa
-Revises: 95073282294e
-Create Date: 2023-02-06 15:54:02.292777
+Revision ID: b5907be59c45
+Revises: 333fd693eac8
+Create Date: 2023-03-30 17:35:52.404091
 
 """
 import sqlalchemy as sa  # noqa
 import sqlmodel  # noqa
 from alembic import op
 
+from lnhub_rest.schema.migrations.rls._2023_03_30_b5907be59c45_v0_8_dev1 import (
+    sql_rls_instance_2,
+)
+
 # revision identifiers, used by Alembic.
-revision = "9c02109e4faa"
-down_revision = "95073282294e"
+revision = "b5907be59c45"
+down_revision = "333fd693eac8"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
+    op.drop_constraint(
+        "fk_account_instance_account_id_account", "account_instance", type_="foreignkey"
+    )
+    op.drop_constraint(
+        "fk_account_instance_instance_id_instance",
+        "account_instance",
+        type_="foreignkey",
+    )
+    op.create_foreign_key(
+        op.f("fk_account_instance_account_id_account"),
+        "account_instance",
+        "account",
+        ["account_id"],
+        ["id"],
+        ondelete="CASCADE",
+    )
     op.create_foreign_key(
         op.f("fk_account_instance_instance_id_instance"),
         "account_instance",
         "instance",
         ["instance_id"],
         ["id"],
+        ondelete="CASCADE",
     )
-    op.alter_column("instance", "public", existing_type=sa.BOOLEAN(), nullable=True)
+    op.execute(sql_rls_instance_2)
 
 
 def downgrade() -> None:
-    op.alter_column("instance", "public", existing_type=sa.BOOLEAN(), nullable=False)
-    op.drop_constraint(
-        op.f("fk_account_instance_instance_id_instance"),
-        "account_instance",
-        type_="foreignkey",
-    )
+    pass
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-"""v0.6.1.
+"""v0.8.dev2.
 
-Revision ID: 0c4d4fe5f2c6
-Revises: a88f5298b8f7
-Create Date: 2023-03-09 09:37:32.028048
+Revision ID: 6e7d7a97c233
+Revises: b5907be59c45
+Create Date: 2023-04-04 17:20:25.264729
 
 """
 import sqlalchemy as sa  # noqa
 import sqlmodel  # noqa
 from alembic import op
 
-from lnhub_rest.schema.migrations.rls._2023_03_09_0c4d4fe5f2c6_v0_6_1 import (
-    sql_rls_migration,
-    sql_rls_version,
+from lnhub_rest.schema.migrations.function._2023_04_04_6e7d7a97c233_v0_8_dev2 import (
+    sql_reset_functions,
+)
+from lnhub_rest.schema.migrations.rls._2023_04_04_6e7d7a97c233_v0_8_dev2 import (
+    sql_drop_rls_all,
+    sql_reset_rls_all,
 )
 
 # revision identifiers, used by Alembic.
-revision = "0c4d4fe5f2c6"
-down_revision = "a88f5298b8f7"
+revision = "6e7d7a97c233"
+down_revision = "b5907be59c45"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
-    op.execute(sql_rls_migration)
-    op.execute(sql_rls_version)
+    op.execute(sql_drop_rls_all)
+    op.execute(sql_reset_functions)
+    op.execute(sql_reset_rls_all)
 
 
 def downgrade() -> None:
     pass
```

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/lnhub_rest/utils/_test.py` & `lnhub_rest-0.8.2/lnhub_rest/utils/_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import uuid
 from typing import Union
 
 import requests  # type: ignore
 
-from lnhub_rest._sbclient import (
+from lnhub_rest.core.account._crud import sb_insert_account
+from lnhub_rest.core.collaborator._crud import sb_insert_collaborator
+from lnhub_rest.core.instance._crud import sb_insert_instance
+from lnhub_rest.core.storage._crud import sb_insert_storage
+from lnhub_rest.orm._sbclient import (
     connect_hub,
     connect_hub_with_auth,
     connect_hub_with_service_role,
     get_lamin_site_base_url,
 )
-from lnhub_rest.core.account._crud import sb_insert_account
-from lnhub_rest.core.collaborator._crud import sb_insert_collaborator
-from lnhub_rest.core.instance._crud import sb_insert_instance
-from lnhub_rest.core.storage._crud import sb_insert_storage
 from lnhub_rest.utils._access_token import extract_id
 from lnhub_rest.utils._id import base62
 
 
 def create_test_auth():
     handle = f"lamin.ci.user.{base62(6)}"
     email = f"{handle}@gmail.com"
```

### Comparing `lnhub_rest-0.8.1/noxfile.py` & `lnhub_rest-0.8.2/noxfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 if "BRANCH_NAME" in os.environ:
     branch_name = os.environ["BRANCH_NAME"]
     logger.info(f"Using BRANCH_NAME {branch_name}")
 else:
     logger.info("Env variable BRANCH_NAME not found")
 
 
-lamin_env = "local"
-if branch_name is not None:
-    if branch_name == "main":
-        lamin_env = "prod"
-    elif branch_name == "staging":
-        lamin_env = "staging"
-    else:
-        lamin_env = "local"
-elif "LAMIN_ENV" in os.environ:
-    lamin_env = os.environ["LAMIN_ENV"]
+# lamin_env = "local"
+# if branch_name is not None:
+#     if branch_name == "main":
+#         lamin_env = "prod"
+#     elif branch_name == "staging":
+#         lamin_env = "staging"
+#     else:
+#         lamin_env = "local"
+# elif "LAMIN_ENV" in os.environ:
+#     lamin_env = os.environ["LAMIN_ENV"]
 
-logger.info(f"Setting LAMIN_ENV to {lamin_env}")
+# logger.info(f"Setting LAMIN_ENV to {lamin_env}")
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
     session.install("pre-commit")
     session.run("pre-commit", "install")
     session.run("pre-commit", "run", "--all-files")
 
 
 @nox.session
 @nox.parametrize("package", ["lnhub-rest", "lndb"])
-def build(session: nox.Session, package: str):
+@nox.parametrize("lamin_env", ["local", "staging"])
+def build(session: nox.Session, package: str, lamin_env: str):
     session.install("./lndb[dev,test]")
     session.install(".[dev,test]")
     session.run(
         "pytest",
         "-s",
         "--cov=lnhub_rest",
         "--cov-append",
@@ -52,16 +53,14 @@
         login_testuser1(session)
         login_testuser2(session)
         os.chdir(f"./{package}")
         session.run(
             "pytest",
             "-s",
             "./tests",
-            "--ignore",
-            "./tests/test_migrations.py",
             env={"LAMIN_ENV": lamin_env},
         )
 
 
 @nox.session
 def supabase_stop(session: nox.Session) -> None:
     session.run("supabase", "db", "reset", external=True)
```

### Comparing `lnhub_rest-0.8.1/pyproject.toml` & `lnhub_rest-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/supabase/config.toml` & `lnhub_rest-0.8.2/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.1/tests/test_notebooks.py` & `lnhub_rest-0.8.2/tests/test_notebooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 
 def test_notebooks():
     # assuming this is in the tests folder
     docs_folder = Path(__file__).parents[1] / "docs/"
 
     if os.environ["LAMIN_ENV"] == "local":
-        logger.debug("\nmigration")
-        test.execute_notebooks(docs_folder / "migration/", write=True)
+        logger.debug("\nmigrate")
+        test.execute_notebooks(docs_folder, write=True)
 
     logger.debug("\nchecks")
-    test.execute_notebooks(docs_folder / "checks/", write=True)
+    test.execute_notebooks(docs_folder / "01-checks/", write=True)
 
     logger.debug("\naccount")
-    test.execute_notebooks(docs_folder / "account/", write=True)
+    test.execute_notebooks(docs_folder / "02-account/", write=True)
 
     logger.debug("\ninstance")
-    test.execute_notebooks(docs_folder / "instance/", write=True)
+    test.execute_notebooks(docs_folder / "03-instance/", write=True)
 
     logger.debug("\nstorage")
-    test.execute_notebooks(docs_folder / "storage/", write=True)
+    test.execute_notebooks(docs_folder / "04-storage/", write=True)
 
     logger.debug("\norganization")
-    test.execute_notebooks(docs_folder / "organization/", write=True)
+    test.execute_notebooks(docs_folder / "05-organization/", write=True)
```

### Comparing `lnhub_rest-0.8.1/PKG-INFO` & `lnhub_rest-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.8.1
+Version: 0.8.2
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: supabase==1.0.2
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
@@ -27,15 +27,15 @@
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnhub-rest
 Provides-Extra: dev
 Provides-Extra: test
 
 # lnhub-rest: Cross-instance management
 
-Note: For more extensive documentation, see [docs/content](docs/content.md).
+Note: For more extensive documentation & testing, see [docs](docs).
 
 ## Summary
 
 1. Installation
 2. CLI
    1. Run server
    2. Run tests
```

