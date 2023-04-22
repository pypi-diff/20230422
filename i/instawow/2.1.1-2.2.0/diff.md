# Comparing `tmp/instawow-2.1.1.tar.gz` & `tmp/instawow-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instawow-2.1.1.tar", max compression
+gzip compressed data, was "instawow-2.2.0.tar", max compression
```

## Comparing `instawow-2.1.1.tar` & `instawow-2.2.0.tar`

### file list

```diff
@@ -1,122 +1,121 @@
--rw-r--r--   0        0        0    35147 2019-12-02 23:23:41.000000 instawow-2.1.1/COPYING
--rw-r--r--   0        0        0     7232 2022-09-11 11:09:45.272521 instawow-2.1.1/README.rst
--rw-r--r--   0        0        0        0 2021-09-26 23:03:02.610144 instawow-2.1.1/gui-webview/src/instawow_gui/__init__.py
--rw-r--r--   0        0        0     3339 2022-12-15 05:55:39.664388 instawow-2.1.1/gui-webview/src/instawow_gui/app.py
--rw-r--r--   0        0        0       27 2021-06-12 09:49:57.192616 instawow-2.1.1/gui-webview/src/instawow_gui/frontend/.gitignore
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.192724 instawow-2.1.1/gui-webview/src/instawow_gui/frontend/__init__.py
--rw-r--r--   0        0        0      415 2022-12-15 06:12:05.112268 instawow-2.1.1/gui-webview/src/instawow_gui/frontend/index.html
--rw-r--r--   0        0        0    19459 2022-12-15 06:12:13.379115 instawow-2.1.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.css
--rw-r--r--   0        0        0   911741 2022-12-15 06:12:13.385877 instawow-2.1.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.js
--rw-r--r--   0        0        0    29999 2022-12-15 05:55:39.665238 instawow-2.1.1/gui-webview/src/instawow_gui/json_rpc_server.py
--rw-r--r--   0        0        0        0 2021-09-18 16:01:49.335972 instawow-2.1.1/gui-webview/src/instawow_gui/py.typed
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.193550 instawow-2.1.1/gui-webview/src/instawow_gui/resources/__init__.py
--rw-r--r--   0        0        0   133998 2021-06-12 09:49:57.194686 instawow-2.1.1/gui-webview/src/instawow_gui/resources/instawow_gui.icns
--rw-r--r--   0        0        0     8736 2021-06-12 09:49:57.195656 instawow-2.1.1/gui-webview/src/instawow_gui/resources/instawow_gui.ico
--rw-r--r--   0        0        0    60410 2021-06-12 09:49:57.197567 instawow-2.1.1/gui-webview/src/instawow_gui/resources/instawow_gui.png
--rw-r--r--   0        0        0     3152 2022-12-15 06:14:05.101227 instawow-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      176 2022-12-15 06:11:21.614197 instawow-2.1.1/src/instawow/__init__.py
--rw-r--r--   0        0        0      444 2022-12-03 13:43:31.061801 instawow-2.1.1/src/instawow/__main__.py
--rw-r--r--   0        0        0     2775 2022-12-15 05:55:39.666760 instawow-2.1.1/src/instawow/_addon_hashing.py
--rw-r--r--   0        0        0     9893 2022-12-15 06:04:40.466163 instawow-2.1.1/src/instawow/_cli_prompts.py
--rw-r--r--   0        0        0     7766 2022-12-15 05:52:01.512766 instawow-2.1.1/src/instawow/_custom_slpp.py
--rw-r--r--   0        0        0      175 2022-12-15 06:04:40.467223 instawow-2.1.1/src/instawow/_deferred_types.py
--rw-r--r--   0        0        0     3426 2022-12-15 05:55:39.667266 instawow-2.1.1/src/instawow/_http_cache_db.py
--rw-r--r--   0        0        0      838 2022-12-15 05:44:18.229462 instawow-2.1.1/src/instawow/_import_wrapper.py
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.208218 instawow-2.1.1/src/instawow/_migrations/__init__.py
--rw-r--r--   0        0        0     1623 2021-06-12 09:49:57.208876 instawow-2.1.1/src/instawow/_migrations/alembic.ini
--rw-r--r--   0        0        0     1225 2022-11-13 23:27:31.145353 instawow-2.1.1/src/instawow/_migrations/env.py
--rw-r--r--   0        0        0      494 2021-06-12 09:49:57.209309 instawow-2.1.1/src/instawow/_migrations/script.py.mako
--rw-r--r--   0        0        0      531 2021-09-18 16:01:49.339737 instawow-2.1.1/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py
--rw-r--r--   0        0        0      579 2022-12-15 05:44:18.230591 instawow-2.1.1/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py
--rw-r--r--   0        0        0      735 2022-08-12 11:35:28.364230 instawow-2.1.1/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py
--rw-r--r--   0        0        0     1294 2022-08-12 11:35:28.364597 instawow-2.1.1/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py
--rw-r--r--   0        0        0      716 2022-12-15 05:52:01.513882 instawow-2.1.1/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py
--rw-r--r--   0        0        0      733 2022-12-15 05:52:01.514371 instawow-2.1.1/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py
--rw-r--r--   0        0        0      822 2022-12-15 05:52:01.514842 instawow-2.1.1/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py
--rw-r--r--   0        0        0     3206 2022-12-15 05:44:18.234937 instawow-2.1.1/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py
--rw-r--r--   0        0        0     2565 2022-12-15 05:52:01.515440 instawow-2.1.1/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py
--rw-r--r--   0        0        0      778 2022-12-15 05:44:18.236981 instawow-2.1.1/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.211018 instawow-2.1.1/src/instawow/_migrations/versions/__init__.py
--rw-r--r--   0        0        0      748 2022-12-15 05:52:01.516033 instawow-2.1.1/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py
--rw-r--r--   0        0        0     3811 2022-12-15 05:52:01.516577 instawow-2.1.1/src/instawow/_migrations/versions/e13430219249_add_cascade.py
--rw-r--r--   0        0        0     1230 2022-12-15 05:52:01.517072 instawow-2.1.1/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py
--rw-r--r--   0        0        0     1195 2021-09-18 16:01:49.342935 instawow-2.1.1/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py
--rw-r--r--   0        0        0      520 2022-12-15 05:52:01.517611 instawow-2.1.1/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py
--rw-r--r--   0        0        0        0 2022-08-14 14:15:56.303799 instawow-2.1.1/src/instawow/_sources/__init__.py
--rw-r--r--   0        0        0    14371 2022-12-15 05:52:01.518530 instawow-2.1.1/src/instawow/_sources/cfcore.py
--rw-r--r--   0        0        0    16433 2022-12-15 05:55:39.667911 instawow-2.1.1/src/instawow/_sources/github.py
--rw-r--r--   0        0        0     2349 2022-12-15 05:52:01.519729 instawow-2.1.1/src/instawow/_sources/instawow.py
--rw-r--r--   0        0        0     7814 2022-12-15 05:52:01.520377 instawow-2.1.1/src/instawow/_sources/tukui.py
--rw-r--r--   0        0        0     6824 2022-12-15 05:52:01.521132 instawow-2.1.1/src/instawow/_sources/wago.py
--rw-r--r--   0        0        0     8740 2022-12-15 05:55:39.668487 instawow-2.1.1/src/instawow/_sources/wowi.py
--rw-r--r--   0        0        0       22 2022-12-15 06:14:05.105822 instawow-2.1.1/src/instawow/_version.py
--rw-r--r--   0        0        0      115 2022-12-15 06:04:29.918392 instawow-2.1.1/src/instawow/_wa_templates/CHANGELOG.md
--rw-r--r--   0        0        0    18046 2021-06-12 09:49:57.216042 instawow-2.1.1/src/instawow/_wa_templates/COPYING.WeakAuras-Companion
--rw-r--r--   0        0        0      223 2021-12-05 22:28:54.088794 instawow-2.1.1/src/instawow/_wa_templates/README
--rw-r--r--   0        0        0      360 2022-12-15 06:04:29.919814 instawow-2.1.1/src/instawow/_wa_templates/WeakAurasCompanion.toc
--rw-r--r--   0        0        0        0 2021-06-12 09:49:57.216549 instawow-2.1.1/src/instawow/_wa_templates/__init__.py
--rw-r--r--   0        0        0      418 2022-12-15 06:04:29.919169 instawow-2.1.1/src/instawow/_wa_templates/data.lua
--rw-r--r--   0        0        0     1059 2022-12-15 05:55:39.670209 instawow-2.1.1/src/instawow/_wa_templates/init.lua
--rw-r--r--   0        0        0     3760 2022-10-23 20:30:20.239285 instawow-2.1.1/src/instawow/cataloguer.py
--rw-r--r--   0        0        0    39352 2022-12-15 06:10:29.811622 instawow-2.1.1/src/instawow/cli.py
--rw-r--r--   0        0        0     3406 2022-12-15 05:55:39.671690 instawow-2.1.1/src/instawow/common.py
--rw-r--r--   0        0        0    11795 2022-12-15 05:55:39.672892 instawow-2.1.1/src/instawow/config.py
--rw-r--r--   0        0        0     5395 2022-12-15 05:55:39.673557 instawow-2.1.1/src/instawow/db.py
--rw-r--r--   0        0        0     1698 2022-09-02 09:43:18.977398 instawow-2.1.1/src/instawow/github_auth.py
--rw-r--r--   0        0        0     3101 2022-12-15 06:04:40.469711 instawow-2.1.1/src/instawow/http.py
--rw-r--r--   0        0        0    29901 2022-12-15 06:10:03.071840 instawow-2.1.1/src/instawow/manager.py
--rw-r--r--   0        0        0     6552 2022-12-15 05:52:01.528013 instawow-2.1.1/src/instawow/matchers.py
--rw-r--r--   0        0        0     4176 2022-12-15 06:09:19.699891 instawow-2.1.1/src/instawow/models.py
--rw-r--r--   0        0        0     1190 2022-12-15 05:52:01.529660 instawow-2.1.1/src/instawow/plugins.py
--rw-r--r--   0        0        0        0 2021-09-18 22:38:54.214209 instawow-2.1.1/src/instawow/py.typed
--rw-r--r--   0        0        0     5807 2022-12-15 06:09:56.791601 instawow-2.1.1/src/instawow/resolvers.py
--rw-r--r--   0        0        0     4016 2022-10-23 20:29:50.421695 instawow-2.1.1/src/instawow/results.py
--rw-r--r--   0        0        0     8874 2022-12-15 05:55:39.675785 instawow-2.1.1/src/instawow/utils.py
--rw-r--r--   0        0        0    12396 2022-12-15 06:04:29.920787 instawow-2.1.1/src/instawow/wa_updater.py
--rw-r--r--   0        0        0        0 2022-10-01 14:46:03.853827 instawow-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3950 2022-12-15 05:52:01.533193 instawow-2.1.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2019-09-13 12:49:54.000000 instawow-2.1.1/tests/fixtures/FakeAddon/FakeAddon.lua
--rw-r--r--   0        0        0      116 2019-09-13 12:49:54.000000 instawow-2.1.1/tests/fixtures/FakeAddon/FakeAddon.toc
--rw-r--r--   0        0        0     8799 2022-12-15 05:52:01.534031 instawow-2.1.1/tests/fixtures/http/__init__.py
--rw-r--r--   0        0        0  4816882 2022-08-31 22:25:56.442109 instawow-2.1.1/tests/fixtures/http/base-catalogue-v7.compact.json
--rw-r--r--   0        0        0   210360 2022-08-31 20:23:48.857256 instawow-2.1.1/tests/fixtures/http/curse-addon--all.json
--rw-r--r--   0        0        0      113 2022-08-31 20:23:50.334581 instawow-2.1.1/tests/fixtures/http/curse-addon-changelog.json
--rw-r--r--   0        0        0    71851 2022-08-31 20:23:49.676910 instawow-2.1.1/tests/fixtures/http/curse-addon-files.json
--rw-r--r--   0        0        0      115 2022-08-31 20:24:16.713339 instawow-2.1.1/tests/fixtures/http/github-oauth-login-access-token.json
--rw-r--r--   0        0        0      187 2022-08-31 20:24:16.643118 instawow-2.1.1/tests/fixtures/http/github-oauth-login-device-code.json
--rw-r--r--   0        0        0      376 2022-08-31 20:24:09.661693 instawow-2.1.1/tests/fixtures/http/github-release-molinari-release-json.json
--rw-r--r--   0        0        0     6036 2022-08-31 20:24:08.368219 instawow-2.1.1/tests/fixtures/http/github-release-molinari.json
--rw-r--r--   0        0        0     1895 2022-08-31 20:24:14.230192 instawow-2.1.1/tests/fixtures/http/github-release-no-assets.json
--rw-r--r--   0        0        0     8518 2022-08-31 20:24:11.947838 instawow-2.1.1/tests/fixtures/http/github-release-no-release-json.json
--rw-r--r--   0        0        0      398 2022-08-31 20:24:06.271014 instawow-2.1.1/tests/fixtures/http/github-release-release-json-release-json.json
--rw-r--r--   0        0        0     8128 2022-08-31 20:24:04.451313 instawow-2.1.1/tests/fixtures/http/github-release-release-json.json
--rw-r--r--   0        0        0     6715 2022-08-31 20:24:07.258377 instawow-2.1.1/tests/fixtures/http/github-repo-molinari.json
--rw-r--r--   0        0        0     6813 2022-08-31 20:24:10.657644 instawow-2.1.1/tests/fixtures/http/github-repo-no-release-json.json
--rw-r--r--   0        0        0     6740 2022-08-31 20:24:13.112037 instawow-2.1.1/tests/fixtures/http/github-repo-no-releases.json
--rw-r--r--   0        0        0     5508 2022-08-31 20:24:02.620371 instawow-2.1.1/tests/fixtures/http/github-repo-release-json.json
--rwxr-xr-x   0        0        0     4643 2022-10-04 08:31:31.924694 instawow-2.1.1/tests/fixtures/http/regen.sh
--rw-r--r--   0        0        0      742 2022-09-12 20:30:46.898294 instawow-2.1.1/tests/fixtures/http/tukui-classic-addons.json
--rw-r--r--   0        0        0      754 2022-09-12 20:30:49.198297 instawow-2.1.1/tests/fixtures/http/tukui-classic-wotlk-addons.json
--rw-r--r--   0        0        0      738 2022-09-12 20:30:45.511712 instawow-2.1.1/tests/fixtures/http/tukui-retail-addons.json
--rw-r--r--   0        0        0      790 2022-09-12 20:30:43.625964 instawow-2.1.1/tests/fixtures/http/tukui-ui--elvui.json
--rw-r--r--   0        0        0      716 2022-09-12 20:30:41.827769 instawow-2.1.1/tests/fixtures/http/tukui-ui--tukui.json
--rw-r--r--   0        0        0      938 2022-10-04 08:31:13.687772 instawow-2.1.1/tests/fixtures/http/wago-match-addons.json
--rw-r--r--   0        0        0     2126 2022-08-31 20:23:52.860250 instawow-2.1.1/tests/fixtures/http/wowi-filedetails.json
--rw-r--r--   0        0        0      924 2022-08-31 20:23:51.724107 instawow-2.1.1/tests/fixtures/http/wowi-filelist.json
--rw-r--r--   0        0        0     1268 2022-12-15 05:52:01.534861 instawow-2.1.1/tests/plugin/instawow_test_plugin.py
--rw-r--r--   0        0        0       92 2022-06-02 10:31:06.427153 instawow-2.1.1/tests/plugin/pyproject.toml
--rw-r--r--   0        0        0      201 2022-08-12 11:35:28.378652 instawow-2.1.1/tests/plugin/setup.py
--rw-r--r--   0        0        0     5196 2022-12-15 05:44:18.265903 instawow-2.1.1/tests/test__slpp.py
--rw-r--r--   0        0        0     9828 2022-12-15 05:52:01.535678 instawow-2.1.1/tests/test__sources.py
--rw-r--r--   0        0        0    16833 2022-12-15 05:52:01.536573 instawow-2.1.1/tests/test_cli.py
--rw-r--r--   0        0        0     2192 2022-12-15 05:55:39.677042 instawow-2.1.1/tests/test_common.py
--rw-r--r--   0        0        0     3676 2022-12-15 05:52:01.537348 instawow-2.1.1/tests/test_config.py
--rw-r--r--   0        0        0      422 2022-12-15 05:44:18.270434 instawow-2.1.1/tests/test_github_oauth_flow.py
--rw-r--r--   0        0        0     3163 2022-12-15 05:52:01.538095 instawow-2.1.1/tests/test_github_zip_parsing.py
--rw-r--r--   0        0        0     4390 2022-12-15 05:52:01.538824 instawow-2.1.1/tests/test_json_rpc_api.py
--rw-r--r--   0        0        0    13756 2022-12-15 05:52:01.539668 instawow-2.1.1/tests/test_manager.py
--rw-r--r--   0        0        0     3842 2022-12-15 05:44:18.274112 instawow-2.1.1/tests/test_matchers.py
--rw-r--r--   0        0        0     4490 2022-12-15 05:52:01.540448 instawow-2.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     3467 2022-12-15 05:55:39.677621 instawow-2.1.1/tests/test_wa_updater.py
--rw-r--r--   0        0        0     9222 1970-01-01 00:00:00.000000 instawow-2.1.1/setup.py
--rw-r--r--   0        0        0     8909 1970-01-01 00:00:00.000000 instawow-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2019-12-02 23:23:41.000000 instawow-2.2.0/COPYING
+-rw-r--r--   0        0        0     7232 2022-09-11 11:09:45.272521 instawow-2.2.0/README.rst
+-rw-r--r--   0        0        0        0 2021-09-26 23:03:02.610144 instawow-2.2.0/gui-webview/src/instawow_gui/__init__.py
+-rw-r--r--   0        0        0     4374 2023-04-15 10:43:33.025204 instawow-2.2.0/gui-webview/src/instawow_gui/app.py
+-rw-r--r--   0        0        0       27 2021-06-12 09:49:57.192616 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/.gitignore
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.192724 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-22 10:09:21.216534 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/index.html
+-rw-r--r--   0        0        0    19643 2023-04-22 10:09:31.184620 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css
+-rw-r--r--   0        0        0   494619 2023-04-22 10:09:31.185238 instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.js
+-rw-r--r--   0        0        0    27256 2023-04-19 21:34:51.388261 instawow-2.2.0/gui-webview/src/instawow_gui/json_rpc_server.py
+-rw-r--r--   0        0        0        0 2021-09-18 16:01:49.335972 instawow-2.2.0/gui-webview/src/instawow_gui/py.typed
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.193550 instawow-2.2.0/gui-webview/src/instawow_gui/resources/__init__.py
+-rw-r--r--   0        0        0   133998 2021-06-12 09:49:57.194686 instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns
+-rw-r--r--   0        0        0     8736 2021-06-12 09:49:57.195656 instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico
+-rw-r--r--   0        0        0    60410 2021-06-12 09:49:57.197567 instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.png
+-rw-r--r--   0        0        0     3775 2023-04-22 10:10:13.919108 instawow-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      213 2023-04-13 13:01:04.746899 instawow-2.2.0/src/instawow/__init__.py
+-rw-r--r--   0        0        0      480 2023-02-10 14:46:48.188526 instawow-2.2.0/src/instawow/__main__.py
+-rw-r--r--   0        0        0     2775 2022-12-15 05:55:39.666760 instawow-2.2.0/src/instawow/_addon_hashing.py
+-rw-r--r--   0        0        0     9904 2023-04-19 15:05:25.729293 instawow-2.2.0/src/instawow/_cli_prompts.py
+-rw-r--r--   0        0        0     7760 2023-02-01 10:07:51.063301 instawow-2.2.0/src/instawow/_custom_slpp.py
+-rw-r--r--   0        0        0     3427 2023-04-16 14:08:11.800604 instawow-2.2.0/src/instawow/_http_cache_db.py
+-rw-r--r--   0        0        0      842 2023-04-17 17:43:24.869397 instawow-2.2.0/src/instawow/_import_wrapper.py
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.208218 instawow-2.2.0/src/instawow/_migrations/__init__.py
+-rw-r--r--   0        0        0     1623 2021-06-12 09:49:57.208876 instawow-2.2.0/src/instawow/_migrations/alembic.ini
+-rw-r--r--   0        0        0     1261 2023-02-10 14:46:48.159866 instawow-2.2.0/src/instawow/_migrations/env.py
+-rw-r--r--   0        0        0      494 2021-06-12 09:49:57.209309 instawow-2.2.0/src/instawow/_migrations/script.py.mako
+-rw-r--r--   0        0        0      567 2023-02-10 14:46:48.144898 instawow-2.2.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py
+-rw-r--r--   0        0        0      615 2023-02-10 14:46:48.148613 instawow-2.2.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py
+-rw-r--r--   0        0        0      771 2023-02-10 14:46:48.142255 instawow-2.2.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py
+-rw-r--r--   0        0        0     1330 2023-02-10 14:46:48.148806 instawow-2.2.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py
+-rw-r--r--   0        0        0      752 2023-02-10 14:46:48.137514 instawow-2.2.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py
+-rw-r--r--   0        0        0      769 2023-02-10 14:46:48.139872 instawow-2.2.0/src/instawow/_migrations/versions/75f69831f74f_replace_curse_strategies.py
+-rw-r--r--   0        0        0      858 2023-02-10 14:46:48.133648 instawow-2.2.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py
+-rw-r--r--   0        0        0     3242 2023-02-10 14:46:48.157600 instawow-2.2.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py
+-rw-r--r--   0        0        0     2601 2023-02-10 14:46:48.153141 instawow-2.2.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py
+-rw-r--r--   0        0        0      814 2023-02-10 14:46:48.145012 instawow-2.2.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.211018 instawow-2.2.0/src/instawow/_migrations/versions/__init__.py
+-rw-r--r--   0        0        0      784 2023-02-10 14:46:48.139232 instawow-2.2.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py
+-rw-r--r--   0        0        0     3847 2023-02-10 14:46:48.143020 instawow-2.2.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py
+-rw-r--r--   0        0        0     1266 2023-02-10 14:46:48.135782 instawow-2.2.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py
+-rw-r--r--   0        0        0     1231 2023-02-10 14:46:48.147304 instawow-2.2.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py
+-rw-r--r--   0        0        0      556 2023-02-10 14:46:48.146303 instawow-2.2.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py
+-rw-r--r--   0        0        0        0 2022-08-14 14:15:56.303799 instawow-2.2.0/src/instawow/_sources/__init__.py
+-rw-r--r--   0        0        0    14338 2023-04-10 23:13:29.001702 instawow-2.2.0/src/instawow/_sources/cfcore.py
+-rw-r--r--   0        0        0    16388 2023-04-19 22:34:59.730527 instawow-2.2.0/src/instawow/_sources/github.py
+-rw-r--r--   0        0        0     2335 2023-04-10 23:13:27.566255 instawow-2.2.0/src/instawow/_sources/instawow.py
+-rw-r--r--   0        0        0     7782 2023-04-10 23:13:28.412152 instawow-2.2.0/src/instawow/_sources/tukui.py
+-rw-r--r--   0        0        0     6824 2022-12-18 21:54:41.548677 instawow-2.2.0/src/instawow/_sources/wago.py
+-rw-r--r--   0        0        0     8708 2023-04-10 23:13:28.429759 instawow-2.2.0/src/instawow/_sources/wowi.py
+-rw-r--r--   0        0        0     1317 2023-04-22 10:10:13.924559 instawow-2.2.0/src/instawow/_version.py
+-rw-r--r--   0        0        0      120 2022-12-15 17:34:52.403485 instawow-2.2.0/src/instawow/_wa_templates/CHANGELOG.md
+-rw-r--r--   0        0        0    18046 2021-06-12 09:49:57.216042 instawow-2.2.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion
+-rw-r--r--   0        0        0      223 2021-12-05 22:28:54.088794 instawow-2.2.0/src/instawow/_wa_templates/README
+-rw-r--r--   0        0        0      360 2022-12-15 06:04:29.919814 instawow-2.2.0/src/instawow/_wa_templates/WeakAurasCompanion.toc
+-rw-r--r--   0        0        0        0 2021-06-12 09:49:57.216549 instawow-2.2.0/src/instawow/_wa_templates/__init__.py
+-rw-r--r--   0        0        0      418 2022-12-15 06:04:29.919169 instawow-2.2.0/src/instawow/_wa_templates/data.lua
+-rw-r--r--   0        0        0     1059 2023-04-22 08:30:05.257712 instawow-2.2.0/src/instawow/_wa_templates/init.lua
+-rw-r--r--   0        0        0     3733 2023-04-17 22:51:34.488709 instawow-2.2.0/src/instawow/cataloguer.py
+-rw-r--r--   0        0        0    41753 2023-04-19 22:32:19.925511 instawow-2.2.0/src/instawow/cli.py
+-rw-r--r--   0        0        0     3702 2023-04-09 11:42:24.821116 instawow-2.2.0/src/instawow/common.py
+-rw-r--r--   0        0        0    12195 2023-04-19 22:39:20.139646 instawow-2.2.0/src/instawow/config.py
+-rw-r--r--   0        0        0     4949 2023-04-17 22:42:46.703539 instawow-2.2.0/src/instawow/db.py
+-rw-r--r--   0        0        0     1657 2023-04-10 23:11:08.500874 instawow-2.2.0/src/instawow/github_auth.py
+-rw-r--r--   0        0        0     3166 2023-04-10 23:13:28.902227 instawow-2.2.0/src/instawow/http.py
+-rw-r--r--   0        0        0    28602 2023-04-19 22:54:57.977209 instawow-2.2.0/src/instawow/manager.py
+-rw-r--r--   0        0        0     6900 2023-04-14 00:50:10.921100 instawow-2.2.0/src/instawow/matchers.py
+-rw-r--r--   0        0        0     3826 2023-04-17 22:43:42.642098 instawow-2.2.0/src/instawow/models.py
+-rw-r--r--   0        0        0     1194 2023-04-17 17:43:06.947727 instawow-2.2.0/src/instawow/plugins.py
+-rw-r--r--   0        0        0        0 2021-09-18 22:38:54.214209 instawow-2.2.0/src/instawow/py.typed
+-rw-r--r--   0        0        0     5355 2023-04-19 23:13:42.409688 instawow-2.2.0/src/instawow/resolvers.py
+-rw-r--r--   0        0        0     4016 2023-01-14 09:18:02.366070 instawow-2.2.0/src/instawow/results.py
+-rw-r--r--   0        0        0     8994 2023-04-19 22:44:32.270341 instawow-2.2.0/src/instawow/utils.py
+-rw-r--r--   0        0        0    12526 2023-04-22 09:14:01.757277 instawow-2.2.0/src/instawow/wa_updater.py
+-rw-r--r--   0        0        0        0 2022-10-01 14:46:03.853827 instawow-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3895 2023-04-15 10:35:01.565813 instawow-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2019-09-13 12:49:54.000000 instawow-2.2.0/tests/fixtures/FakeAddon/FakeAddon.lua
+-rw-r--r--   0        0        0      116 2019-09-13 12:49:54.000000 instawow-2.2.0/tests/fixtures/FakeAddon/FakeAddon.toc
+-rw-r--r--   0        0        0     8799 2022-12-15 05:52:01.534031 instawow-2.2.0/tests/fixtures/http/__init__.py
+-rw-r--r--   0        0        0  4816882 2022-08-31 22:25:56.442109 instawow-2.2.0/tests/fixtures/http/base-catalogue-v7.compact.json
+-rw-r--r--   0        0        0   210360 2022-08-31 20:23:48.857256 instawow-2.2.0/tests/fixtures/http/curse-addon--all.json
+-rw-r--r--   0        0        0      113 2022-08-31 20:23:50.334581 instawow-2.2.0/tests/fixtures/http/curse-addon-changelog.json
+-rw-r--r--   0        0        0    71851 2022-08-31 20:23:49.676910 instawow-2.2.0/tests/fixtures/http/curse-addon-files.json
+-rw-r--r--   0        0        0      115 2022-08-31 20:24:16.713339 instawow-2.2.0/tests/fixtures/http/github-oauth-login-access-token.json
+-rw-r--r--   0        0        0      187 2022-08-31 20:24:16.643118 instawow-2.2.0/tests/fixtures/http/github-oauth-login-device-code.json
+-rw-r--r--   0        0        0      376 2022-08-31 20:24:09.661693 instawow-2.2.0/tests/fixtures/http/github-release-molinari-release-json.json
+-rw-r--r--   0        0        0     6036 2022-08-31 20:24:08.368219 instawow-2.2.0/tests/fixtures/http/github-release-molinari.json
+-rw-r--r--   0        0        0     1895 2022-08-31 20:24:14.230192 instawow-2.2.0/tests/fixtures/http/github-release-no-assets.json
+-rw-r--r--   0        0        0     8518 2022-08-31 20:24:11.947838 instawow-2.2.0/tests/fixtures/http/github-release-no-release-json.json
+-rw-r--r--   0        0        0      398 2022-08-31 20:24:06.271014 instawow-2.2.0/tests/fixtures/http/github-release-release-json-release-json.json
+-rw-r--r--   0        0        0     8128 2022-08-31 20:24:04.451313 instawow-2.2.0/tests/fixtures/http/github-release-release-json.json
+-rw-r--r--   0        0        0     6715 2022-08-31 20:24:07.258377 instawow-2.2.0/tests/fixtures/http/github-repo-molinari.json
+-rw-r--r--   0        0        0     6813 2022-08-31 20:24:10.657644 instawow-2.2.0/tests/fixtures/http/github-repo-no-release-json.json
+-rw-r--r--   0        0        0     6740 2022-08-31 20:24:13.112037 instawow-2.2.0/tests/fixtures/http/github-repo-no-releases.json
+-rw-r--r--   0        0        0     5508 2022-08-31 20:24:02.620371 instawow-2.2.0/tests/fixtures/http/github-repo-release-json.json
+-rwxr-xr-x   0        0        0     4643 2022-10-04 08:31:31.924694 instawow-2.2.0/tests/fixtures/http/regen.sh
+-rw-r--r--   0        0        0      742 2022-09-12 20:30:46.898294 instawow-2.2.0/tests/fixtures/http/tukui-classic-addons.json
+-rw-r--r--   0        0        0      754 2022-09-12 20:30:49.198297 instawow-2.2.0/tests/fixtures/http/tukui-classic-wotlk-addons.json
+-rw-r--r--   0        0        0      738 2022-09-12 20:30:45.511712 instawow-2.2.0/tests/fixtures/http/tukui-retail-addons.json
+-rw-r--r--   0        0        0      790 2022-09-12 20:30:43.625964 instawow-2.2.0/tests/fixtures/http/tukui-ui--elvui.json
+-rw-r--r--   0        0        0      716 2022-09-12 20:30:41.827769 instawow-2.2.0/tests/fixtures/http/tukui-ui--tukui.json
+-rw-r--r--   0        0        0      938 2022-10-04 08:31:13.687772 instawow-2.2.0/tests/fixtures/http/wago-match-addons.json
+-rw-r--r--   0        0        0     2126 2022-08-31 20:23:52.860250 instawow-2.2.0/tests/fixtures/http/wowi-filedetails.json
+-rw-r--r--   0        0        0      924 2022-08-31 20:23:51.724107 instawow-2.2.0/tests/fixtures/http/wowi-filelist.json
+-rw-r--r--   0        0        0     1326 2023-02-10 14:46:48.151173 instawow-2.2.0/tests/plugin/instawow_test_plugin.py
+-rw-r--r--   0        0        0       92 2022-06-02 10:31:06.427153 instawow-2.2.0/tests/plugin/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-02-10 14:46:48.152376 instawow-2.2.0/tests/plugin/setup.py
+-rw-r--r--   0        0        0     5553 2023-04-22 09:14:58.522978 instawow-2.2.0/tests/test__slpp.py
+-rw-r--r--   0        0        0     9802 2023-01-14 09:18:02.341111 instawow-2.2.0/tests/test__sources.py
+-rw-r--r--   0        0        0     3124 2023-04-13 13:04:19.565989 instawow-2.2.0/tests/test__version.py
+-rw-r--r--   0        0        0    17242 2023-04-18 22:28:54.194396 instawow-2.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2192 2022-12-15 05:55:39.677042 instawow-2.2.0/tests/test_common.py
+-rw-r--r--   0        0        0     3676 2022-12-15 05:52:01.537348 instawow-2.2.0/tests/test_config.py
+-rw-r--r--   0        0        0      422 2022-12-15 05:44:18.270434 instawow-2.2.0/tests/test_github_oauth_flow.py
+-rw-r--r--   0        0        0     3134 2023-01-04 01:40:34.984676 instawow-2.2.0/tests/test_github_zip_parsing.py
+-rw-r--r--   0        0        0     4404 2023-01-04 01:39:11.965442 instawow-2.2.0/tests/test_json_rpc_api.py
+-rw-r--r--   0        0        0    10677 2023-04-15 10:24:48.644729 instawow-2.2.0/tests/test_manager.py
+-rw-r--r--   0        0        0     3813 2023-01-04 01:37:47.785586 instawow-2.2.0/tests/test_matchers.py
+-rw-r--r--   0        0        0     4491 2023-01-04 01:37:53.376282 instawow-2.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3483 2023-04-10 10:46:56.823221 instawow-2.2.0/tests/test_wa_updater.py
+-rw-r--r--   0        0        0     8980 1970-01-01 00:00:00.000000 instawow-2.2.0/PKG-INFO
```

### Comparing `instawow-2.1.1/COPYING` & `instawow-2.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/README.rst` & `instawow-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/gui-webview/src/instawow_gui/app.py` & `instawow-2.2.0/gui-webview/src/instawow_gui/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 from __future__ import annotations
 
+import asyncio
 import json
 import os
+from contextlib import suppress
 from functools import partial
 from typing import Any
 
+import anyio.from_thread
+import anyio.to_thread
 import toga
 import toga.constants
 import toga.style
 from loguru import logger
+from typing_extensions import Self
 
 from . import json_rpc_server
 
 
 class InstawowApp(toga.App):
-    def __init__(self, **kwargs: object) -> None:
+    def __init__(self, debug: bool, **kwargs: object) -> None:
         super().__init__(
             formal_name='instawow-gui',
             app_id='org.instawow.instawow_gui',
             app_name='instawow_gui',
             icon='resources/instawow_gui',
             **kwargs,
         )
+        self._debug = debug
 
     def startup(self) -> None:
         self.main_window = toga.MainWindow(title=self.formal_name, size=(800, 600))
 
         if os.name == 'nt':
             import ctypes
 
             # Enable high DPI support.
             ctypes.windll.user32.SetProcessDPIAware()
 
         self.main_window.content = web_view = toga.WebView(style=toga.style.Pack(flex=1))
 
+        if self._debug:
+            with suppress(AttributeError):
+                web_view._impl.native.configuration.preferences.setValue(
+                    True, forKey='developerExtrasEnabled'
+                )
+
         if os.name == 'nt':
             from toga_winforms.widgets.webview import TogaWebBrowser
 
             def configure_webview2(sender: TogaWebBrowser, event_args: Any):
                 if event_args.IsSuccess:
                     sender.CoreWebView2.Settings.AreBrowserAcceleratorKeysEnabled = False
 
@@ -50,49 +62,64 @@
             web_view.invoke_javascript(
                 f'document.dispatchEvent(new CustomEvent("togaSimulateKeypress", {event_args}));'
             )
 
         self.commands.add(
             toga.Command(
                 partial(dispatch_js_keyboard_event, action='toggleSearchFilter'),
-                label='Toggle Search Filter',
+                text='Toggle Search Filter',
                 shortcut=toga.Key.MOD_1 + toga.Key.G,
                 group=toga.Group.EDIT,
                 section=20,
                 order=10,
             ),
             toga.Command(
                 partial(dispatch_js_keyboard_event, action='activateViewInstalled'),
-                label='Installed',
+                text='Installed',
                 shortcut=toga.Key.MOD_1 + toga.Key.L,
                 group=toga.Group.WINDOW,
                 section=20,
                 order=10,
             ),
             toga.Command(
                 partial(dispatch_js_keyboard_event, action='activateViewReconcile'),
-                label='Unreconciled',
+                text='Unreconciled',
                 group=toga.Group.WINDOW,
                 section=20,
                 order=20,
             ),
             toga.Command(
                 partial(dispatch_js_keyboard_event, action='activateViewSearch'),
-                label='Search',
+                text='Search',
                 shortcut=toga.Key.MOD_1 + toga.Key.F,
                 group=toga.Group.WINDOW,
                 section=20,
                 order=30,
             ),
         )
 
-        async def startup() -> None:
-            web_app = await json_rpc_server.create_app(self.main_window)
-            server_url, serve = await json_rpc_server.run_app(web_app)
-            logger.debug(f'JSON-RPC server running on {server_url}')
-            web_view.url = str(server_url)
-            await serve()
+        async def startup(app: Self):
+            async with anyio.from_thread.BlockingPortal() as portal:
+
+                def run_json_rpc_server():
+                    async def run():
+                        web_app = await json_rpc_server.create_app((app.main_window, portal))
+                        server_url, serve_forever = await json_rpc_server.run_app(web_app)
+
+                        logger.debug(f'JSON-RPC server running on {server_url}')
+
+                        set_server_url = partial(setattr, web_view, 'url')
+                        portal.call(set_server_url, str(server_url))
+
+                        await serve_forever()
+
+                    # We don't want to inherit the parent thread's event loop policy,
+                    # i.e. the rubicon loop on macOS.
+                    policy = asyncio.DefaultEventLoopPolicy()
+                    policy.new_event_loop().run_until_complete(run())
+
+                await anyio.to_thread.run_sync(run_json_rpc_server)
 
-        serve_task = self._impl.loop.create_task(startup())
-        self.on_exit = lambda _: serve_task.cancel()
+                await portal.sleep_until_stopped()
 
+        self.add_background_task(startup)
         self.main_window.show()
```

### Comparing `instawow-2.1.1/gui-webview/src/instawow_gui/frontend/svelte-bundle.css` & `instawow-2.2.0/gui-webview/src/instawow_gui/frontend/svelte-bundle.css`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-.modal-wrapper.svelte-jd3rlo{position:fixed;top:0;bottom:0;left:0;right:0;z-index:30}.modal-wrapper.svelte-jd3rlo{display:flex;align-items:center;justify-content:center}.modal.svelte-jd3rlo{display:flex;flex-direction:column;max-height:75%}
 .content.svelte-vgp2pk.svelte-vgp2pk{overflow:auto}.form-grid.svelte-vgp2pk.svelte-vgp2pk{display:grid;grid-template-columns:1fr 2fr;column-gap:0.5rem;row-gap:0.75rem}.form-grid.svelte-vgp2pk label.svelte-vgp2pk,.form-grid.svelte-vgp2pk .label-like.svelte-vgp2pk{line-height:1.75em;color:var(--inverse-color-tone-a);text-align:right}.section-header.svelte-vgp2pk.svelte-vgp2pk{margin-bottom:1rem;padding-bottom:0.5rem;border-bottom:1px solid var(--inverse-color-tone-b);font-weight:500;text-align:center}.value-rows.svelte-vgp2pk.svelte-vgp2pk{display:flex;flex-direction:column;gap:0.25rem}.description.svelte-vgp2pk.svelte-vgp2pk{font-size:0.875em;color:var(--inverse-color-tone-b)}
+.modal-wrapper.svelte-jd3rlo{position:fixed;top:0;bottom:0;left:0;right:0;z-index:30}.modal-wrapper.svelte-jd3rlo{display:flex;align-items:center;justify-content:center}.modal.svelte-jd3rlo{display:flex;flex-direction:column;max-height:75%}
 .modal.svelte-1lyvqkk{position:absolute;top:calc(100% + 4px);left:0;right:0;z-index:10}
 .profile-switcher-wrapper.svelte-ys6f4f.svelte-ys6f4f{position:relative}.profile-switcher.svelte-ys6f4f.svelte-ys6f4f{display:flex;font-size:0.95em}.profile-switcher.svelte-ys6f4f>.svelte-ys6f4f:not(:first-child){margin-left:4px}.profile-switcher.svelte-ys6f4f button.svelte-ys6f4f,.profile-switcher.svelte-ys6f4f select.svelte-ys6f4f{line-height:2em;margin:0;padding:0 0.5em;border:0;border-radius:0.3333333333em;transition:all 0.2s;font-weight:500}.profile-switcher.svelte-ys6f4f button.svelte-ys6f4f:disabled,.profile-switcher.svelte-ys6f4f select.svelte-ys6f4f:disabled{opacity:0.5}.profile-switcher.svelte-ys6f4f button.svelte-ys6f4f:hover:not(:disabled),.profile-switcher.svelte-ys6f4f select.svelte-ys6f4f:hover:not(:disabled){background-color:var(--inverse-color-alpha-05)}.profile-switcher.svelte-ys6f4f button.svelte-ys6f4f:focus,.profile-switcher.svelte-ys6f4f select.svelte-ys6f4f:focus{background-color:var(--inverse-color-alpha-20)}.profile-switcher.svelte-ys6f4f button.svelte-ys6f4f{display:flex;place-items:center}.profile-switcher.svelte-ys6f4f select.svelte-ys6f4f{padding-left:0.65em;padding-right:1.25rem;box-shadow:inset 0 0 0 1px var(--inverse-color-alpha-10);background-image:var(--dropdown-arrow);background-size:10px;background-repeat:no-repeat;background-position:top calc(50% + 1px) right 7px;min-width:180px}.profile-switcher.svelte-ys6f4f .svelte-ys6f4f:first-child{border-top-left-radius:0.5em;border-bottom-left-radius:0.5em}.profile-switcher.svelte-ys6f4f .svelte-ys6f4f:last-child{border-top-right-radius:0.5em;border-bottom-right-radius:0.5em}.profile-switcher.svelte-ys6f4f .icon{height:1rem;width:1rem;vertical-align:text-bottom;fill:var(--inverse-color-tone-b)}
-form.svelte-pspf27 .start-date-suggestions.svelte-pspf27{list-style:none;margin:0;padding-left:0}form.svelte-pspf27 .form-grid.svelte-pspf27{display:grid;grid-template-columns:1fr 2fr;column-gap:0.5rem;row-gap:0.5rem}form.svelte-pspf27 label.svelte-pspf27{line-height:1.75em;color:var(--inverse-color-tone-a);text-align:right}form.svelte-pspf27 .start-date-suggestions.svelte-pspf27{display:inline-flex;gap:0.2rem;grid-column-start:2;margin-top:-0.3em;font-size:0.8em;font-weight:600}form.svelte-pspf27 .start-date-suggestions li.svelte-pspf27{cursor:pointer;padding:0.2rem 0.4rem;border-radius:0.2916666667em;background-color:var(--inverse-color-tone-b);color:var(--base-color)}form.svelte-pspf27 .start-date-suggestions li.disabled.svelte-pspf27{cursor:default;opacity:0.5}form.svelte-pspf27 .start-date-suggestions li.svelte-pspf27:first-child{border-top-left-radius:0.4375em;border-bottom-left-radius:0.4375em}form.svelte-pspf27 .start-date-suggestions li.svelte-pspf27:last-child{border-top-right-radius:0.4375em;border-bottom-right-radius:0.4375em}.form-control.checkbox-container.svelte-pspf27.svelte-pspf27{background-color:transparent;padding-left:0}
+form.svelte-1074j9 .start-date-suggestions.svelte-1074j9{list-style:none;margin:0;padding-left:0}form.svelte-1074j9 .form-grid.svelte-1074j9{display:grid;grid-template-columns:1fr 2fr;column-gap:0.5rem;row-gap:0.5rem}form.svelte-1074j9 label.svelte-1074j9{line-height:1.75em;color:var(--inverse-color-tone-a);text-align:right}form.svelte-1074j9 .start-date-suggestions.svelte-1074j9{display:inline-flex;gap:0.2rem;grid-column-start:2;margin-top:-0.3em;font-size:0.8em;font-weight:600}form.svelte-1074j9 .start-date-suggestions li button.svelte-1074j9{cursor:pointer;margin:0;padding:0.2rem 0.4rem;border:0;border-radius:0.2916666667em;background-color:var(--inverse-color-tone-b);color:var(--base-color)}form.svelte-1074j9 .start-date-suggestions li.disabled button.svelte-1074j9{cursor:default;opacity:0.5}form.svelte-1074j9 .start-date-suggestions li:first-child button.svelte-1074j9{border-top-left-radius:0.4375em;border-bottom-left-radius:0.4375em}form.svelte-1074j9 .start-date-suggestions li:last-child button.svelte-1074j9{border-top-right-radius:0.4375em;border-bottom-right-radius:0.4375em}.form-control.checkbox-container.svelte-1074j9.svelte-1074j9{background-color:transparent;padding-left:0}
 .content.svelte-n5l6oa{overflow:scroll;-webkit-user-select:text;user-select:text}.content.svelte-n5l6oa pre{white-space:pre-wrap}.content.svelte-n5l6oa h1{font-size:1.4em}.content.svelte-n5l6oa h2{font-size:1.2em}.content.svelte-n5l6oa h3{font-size:1em}.content.svelte-n5l6oa .link{word-break:break-all}
-.alerts.svelte-jtijg8.svelte-jtijg8{-webkit-backdrop-filter:blur(6px);backdrop-filter:blur(6px)}.alerts.svelte-jtijg8.svelte-jtijg8{border-radius:0.75em;box-shadow:0 1rem 3rem var(--inverse-color-alpha-10)}.alerts-wrapper.svelte-jtijg8.svelte-jtijg8{position:fixed;left:0;right:0;display:flex;justify-content:center;margin-top:calc(3rem + 4px);z-index:20}.alerts.svelte-jtijg8.svelte-jtijg8{max-width:75vw;padding:0 0.8rem;background-color:var(--alert-background-color);font-size:0.8em;display:grid;grid-template-columns:auto 6rem;grid-column-gap:0.8rem;word-break:break-all}.current-alert.svelte-jtijg8 h1.svelte-jtijg8{margin-bottom:0}.alert-nav.svelte-jtijg8.svelte-jtijg8{align-self:center;justify-self:center}.alert-nav.svelte-jtijg8 button.svelte-jtijg8{line-height:1.8em;margin:0;padding:0.5em;border-radius:0.45em;border:0;transition:all 0.2s}.alert-nav.svelte-jtijg8 button.svelte-jtijg8:disabled{opacity:0.5}.alert-nav.svelte-jtijg8 button.svelte-jtijg8:hover:not(:disabled){background-color:var(--inverse-color-alpha-05)}.alert-nav.svelte-jtijg8 button.svelte-jtijg8:focus{background-color:var(--inverse-color-alpha-10);box-shadow:inset 0 0 0 1px var(--inverse-color-alpha-20)}.alert-nav.svelte-jtijg8 .icon{display:block;height:1rem;width:1rem;fill:var(--inverse-color)}
 .choices.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{list-style:none;margin:0;padding-left:0}.addon-stub.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{transition:all 0.2s}.header.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74,.selection-controls.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{padding:0.4em 0.75em}.header.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{display:flex;flex-direction:row;align-items:baseline;justify-content:space-between;gap:1rem}.folders.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{overflow-x:hidden;white-space:nowrap;text-overflow:ellipsis;font-weight:700}.folders.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74:only-child{line-height:1.5rem}.folders.svelte-1xsfw74 .remaining-folders.svelte-1xsfw74.svelte-1xsfw74{font-size:0.8em;color:var(--inverse-color-tone-b)}.defn-or-version.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74,.choices.svelte-1xsfw74 li.svelte-1xsfw74.svelte-1xsfw74{font-family:Menlo, Monaco, Consolas, monospace;font-size:0.7rem}.selection-controls.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{margin-top:-0.25rem;padding-top:0;color:var(--inverse-color-tone-b)}.selection-controls.svelte-1xsfw74 .selection-grid.svelte-1xsfw74.svelte-1xsfw74{display:grid;grid-template-columns:1fr 2fr 1rem;column-gap:0.5rem}.selection-controls.svelte-1xsfw74 summary.svelte-1xsfw74.svelte-1xsfw74{list-style:none;line-height:1rem}.selection-controls.svelte-1xsfw74 summary.svelte-1xsfw74.svelte-1xsfw74::-webkit-details-marker,.selection-controls.svelte-1xsfw74 summary.svelte-1xsfw74.svelte-1xsfw74::marker{display:none}.selection-controls.svelte-1xsfw74 summary .svelte-1xsfw74.svelte-1xsfw74:nth-child(2){padding:0 0.2rem}.selection-controls.svelte-1xsfw74 summary .svelte-1xsfw74.svelte-1xsfw74:last-child{justify-self:right}.selection-controls.svelte-1xsfw74 summary.svelte-1xsfw74 .icon{display:block;height:1rem;width:1rem;fill:var(--inverse-color-tone-b)}.selection-controls[open].svelte-1xsfw74 .icon-collapsed{display:none !important}.selection-controls.svelte-1xsfw74:not([open]) .icon-expanded{display:none !important}.choices.svelte-1xsfw74 li.svelte-1xsfw74.svelte-1xsfw74{display:flex;padding:0 0.2rem;grid-column-start:2;line-height:1rem}.choices.svelte-1xsfw74 li.svelte-1xsfw74.svelte-1xsfw74:first-child{margin-top:0.18rem;padding-top:0.18rem;border-top:1px solid var(--inverse-color-tone-b)}.choices.svelte-1xsfw74 li label.svelte-1xsfw74.svelte-1xsfw74{flex-grow:1}.choices.svelte-1xsfw74 li label.svelte-1xsfw74.svelte-1xsfw74::before{content:"( ) "}.choices.svelte-1xsfw74 [type=radio].svelte-1xsfw74.svelte-1xsfw74{display:none}.choices.svelte-1xsfw74 [type=radio].svelte-1xsfw74:checked+label.svelte-1xsfw74::before{content:"(x) "}.unreconciled-message.svelte-1xsfw74.svelte-1xsfw74.svelte-1xsfw74{margin:0;font-size:0.75em;color:var(--inverse-color-tone-b)}
 svg.svelte-1iz2oiq{transform:rotate(-90deg)}circle.svelte-1iz2oiq{transition:stroke-dashoffset 0.35s;transform-origin:center;fill:transparent}.indeterminate.svelte-1iz2oiq{animation-duration:0.75s;animation-iteration-count:infinite;animation-name:svelte-1iz2oiq-rotate}@keyframes svelte-1iz2oiq-rotate{from{transform:rotate(0)}to{transform:rotate(1turn)}}
 menu.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{list-style:none;margin:0;padding-left:0}.addon-list-nav.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{display:grid;column-gap:1em;place-items:center}.addon-list-nav.svelte-nmk0ob .svelte-nmk0ob.svelte-nmk0ob:first-child{justify-self:left}.addon-list-nav.svelte-nmk0ob .svelte-nmk0ob.svelte-nmk0ob:last-child{justify-self:right}.control-set.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob,.addon-list-nav.svelte-nmk0ob>div.svelte-nmk0ob.svelte-nmk0ob{display:flex;align-items:center}menu.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{font-weight:500}.addon-list-nav.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{grid-template-columns:repeat(3, 1fr);height:3rem}.search.svelte-nmk0ob .search-control.svelte-nmk0ob.svelte-nmk0ob{border-top-right-radius:0.46875em;border-bottom-right-radius:0.46875em;box-shadow:inset 0 0 0 1px var(--inverse-color-alpha-10);font-size:1rem}.search.svelte-nmk0ob .search-control.svelte-nmk0ob.svelte-nmk0ob,.search.svelte-nmk0ob .search-control.svelte-nmk0ob.svelte-nmk0ob::-webkit-search-cancel-button{-webkit-appearance:none;appearance:none}.search.svelte-nmk0ob .search-control.svelte-nmk0ob.svelte-nmk0ob:not(:focus){text-align:center}.progress-indicator.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{height:18px;line-height:18px;margin:0 0.5rem}.progress-indicator.svelte-nmk0ob circle{stroke:currentColor}.control.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{display:block;min-width:min-content;border:0;transition:all 0.2s;line-height:1.875em;margin:0;padding:0 0.7em;border-radius:0.3125em;white-space:nowrap}.control.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob:disabled{opacity:0.5}.control.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob:hover:not(:disabled){background-color:var(--inverse-color-alpha-05)}.control.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob:focus{background-color:var(--inverse-color-alpha-10)}.control[type=checkbox].svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob,.control[type=radio].svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{position:absolute;opacity:0}.control[type=checkbox].svelte-nmk0ob:checked+label.svelte-nmk0ob.svelte-nmk0ob,.control[type=radio].svelte-nmk0ob:checked+label.svelte-nmk0ob.svelte-nmk0ob{background-color:var(--inverse-color-tone-b) !important;color:var(--base-color)}.control[type=checkbox].svelte-nmk0ob:checked+label.svelte-nmk0ob .icon,.control[type=radio].svelte-nmk0ob:checked+label.svelte-nmk0ob .icon{fill:var(--base-color)}.control[type=checkbox].svelte-nmk0ob:disabled+label.svelte-nmk0ob.svelte-nmk0ob,.control[type=radio].svelte-nmk0ob:disabled+label.svelte-nmk0ob.svelte-nmk0ob{opacity:0.5}.control[type=checkbox].svelte-nmk0ob:focus+label.svelte-nmk0ob.svelte-nmk0ob,.control[type=radio].svelte-nmk0ob:focus+label.svelte-nmk0ob.svelte-nmk0ob{background-color:var(--inverse-color-alpha-10)}.control.dirty.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{background-image:repeating-linear-gradient(-45deg, transparent 0 20px, rgba(250, 128, 114, 0.5) 20px 40px)}.control.reconciliation-stage-control.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{width:100%;padding-right:1.4rem;background-image:var(--dropdown-arrow);background-size:10px;background-repeat:no-repeat;background-position:top calc(50% + 1px) right 7px}.control.svelte-nmk0ob .icon{height:1rem;width:1rem;vertical-align:text-bottom;fill:var(--inverse-color-tone-b)}.control-set.svelte-nmk0ob.svelte-nmk0ob.svelte-nmk0ob{font-size:0.85em}.control-set.svelte-nmk0ob li.svelte-nmk0ob.svelte-nmk0ob:not(:first-child){margin-left:4px}.control-set.svelte-nmk0ob li.segmented-control.svelte-nmk0ob~.segmented-control.svelte-nmk0ob{margin-left:-1px}.control-set.svelte-nmk0ob li:first-child .control.svelte-nmk0ob.svelte-nmk0ob{border-top-left-radius:0.46875em;border-bottom-left-radius:0.46875em}.control-set.svelte-nmk0ob li:last-child .control.svelte-nmk0ob.svelte-nmk0ob{border-top-right-radius:0.46875em;border-bottom-right-radius:0.46875em}
 .context-menu.svelte-1irf7oq menu.svelte-1irf7oq{list-style:none;margin:0;padding-left:0}.context-menu-wrapper.svelte-1irf7oq.svelte-1irf7oq{position:fixed;top:0;bottom:0;left:0;right:0;z-index:30}.context-menu.svelte-1irf7oq.svelte-1irf7oq{-webkit-backdrop-filter:blur(6px);backdrop-filter:blur(6px)}.context-menu.svelte-1irf7oq.svelte-1irf7oq{border-radius:0.75em;box-shadow:0 1rem 3rem var(--inverse-color-alpha-10)}.context-menu.svelte-1irf7oq.svelte-1irf7oq{position:fixed;top:var(--menu-y-offset);left:var(--menu-x-offset);z-index:40;padding:0.5em 0;background-color:var(--base-color-alpha-65);cursor:default;white-space:nowrap}.context-menu.svelte-1irf7oq menu.svelte-1irf7oq{font-size:0.8em}
-li.svelte-1tilx9r.svelte-1tilx9r{padding:0 0.8rem;line-height:1.2rem}li.svelte-1tilx9r.svelte-1tilx9r:not(.divider):hover{background-color:rgb(24, 136, 255);color:#efefef}li.svelte-1tilx9r hr.svelte-1tilx9r{border:1px solid var(--inverse-color-alpha-20)}
+.menu-item.svelte-1gyrn85 button.svelte-1gyrn85{margin:0;padding:0 0.8rem;border:0;line-height:1.38rem;width:100%;text-align:left}.menu-item.svelte-1gyrn85 button.svelte-1gyrn85:focus,.menu-item.svelte-1gyrn85 button.svelte-1gyrn85:hover{background-color:rgb(24, 136, 255);color:#efefef}.menu-item.svelte-1gyrn85 hr.svelte-1gyrn85{margin:0.4rem;border:1px solid var(--inverse-color-alpha-20)}
 .addon-details.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8,.addon-actions.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{list-style:none;margin:0;padding-left:0}.addon.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{position:relative;display:flex;padding:0.4em 0.75em;border-radius:inherit;transition:all 0.2s}.addon.status-being-modified.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{pointer-events:none}.addon.status-outdated.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{background-image:repeating-linear-gradient(-45deg, transparent 0 20px, rgba(0, 255, 0, 0.1) 20px 40px)}.addon.status-pinned.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{background-image:repeating-linear-gradient(-45deg, transparent 0 20px, rgba(255, 215, 0, 0.1) 20px 40px)}.addon-details.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{flex-grow:1;align-items:baseline;gap:0.5em;overflow-x:hidden}.addon-details.two-col.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{display:flex;line-height:1.5rem}.addon-details.two-col.svelte-n5lp8 .name.svelte-n5lp8.svelte-n5lp8{flex-grow:1}.addon-details.two-col.svelte-n5lp8 .versions.svelte-n5lp8.svelte-n5lp8{margin-top:0}.addon-details.svelte-n5lp8 .name.svelte-n5lp8.svelte-n5lp8{font-weight:700;white-space:nowrap;text-overflow:ellipsis;overflow-x:hidden}.addon-details.svelte-n5lp8 .versions.svelte-n5lp8.svelte-n5lp8{float:right;text-align:right}.addon-details.svelte-n5lp8 .date.svelte-n5lp8.svelte-n5lp8{white-space:nowrap}.addon-details.svelte-n5lp8 .defn.svelte-n5lp8.svelte-n5lp8,.addon-details.svelte-n5lp8 .versions.svelte-n5lp8.svelte-n5lp8{margin-top:0.25rem;font-family:Menlo, Monaco, Consolas, monospace;font-size:0.7em;color:var(--inverse-color-tone-b)}.addon-details.svelte-n5lp8 .description.svelte-n5lp8.svelte-n5lp8{margin-top:0.25rem;padding-left:0.25rem;overflow-x:hidden;white-space:nowrap;text-overflow:ellipsis;font-size:0.8em}.addon-details.svelte-n5lp8:hover .description.svelte-n5lp8.svelte-n5lp8{display:block}.addon-actions.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{display:flex;flex-wrap:nowrap;align-self:center;padding-left:0.5rem}.addon-actions.svelte-n5lp8 li.svelte-n5lp8+li.svelte-n5lp8{margin-left:4px}.addon-actions.svelte-n5lp8 li:first-child button.svelte-n5lp8.svelte-n5lp8{border-top-left-radius:1em;border-bottom-left-radius:1em}.addon-actions.svelte-n5lp8 li:last-child button.svelte-n5lp8.svelte-n5lp8{border-top-right-radius:1em;border-bottom-right-radius:1em}.addon-actions.svelte-n5lp8 button.svelte-n5lp8.svelte-n5lp8{margin:0;padding:0 0.625rem;height:1.8em;line-height:1.8em;font-size:0.8em;font-weight:600;border:0;border-radius:0.75em;background-color:rgb(24, 136, 255);color:#efefef;transition:all 0.2s}.addon-actions.svelte-n5lp8 button.svelte-n5lp8.svelte-n5lp8:disabled{opacity:0.5}.addon-actions.svelte-n5lp8 button.svelte-n5lp8.svelte-n5lp8:focus{background-color:rgb(0, 104, 217)}.addon-actions.svelte-n5lp8 button.svelte-n5lp8 .icon{display:block;width:0.8rem;height:0.8rem;fill:#efefef}.progress-indicator.svelte-n5lp8.svelte-n5lp8.svelte-n5lp8{align-self:center;justify-self:right;margin-left:0.75em}.progress-indicator.svelte-n5lp8 circle{stroke:rgb(24, 136, 255)}
 .addon-list.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{list-style:none;margin:0;padding-left:0}.addon-list-wrapper.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{display:flex;flex-direction:column;flex:1;overflow-y:hidden}.addon-list-nav-wrapper.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{-webkit-backdrop-filter:blur(6px);backdrop-filter:blur(6px)}.placeholder.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{display:flex;flex-grow:1;place-items:center}.placeholder.svelte-1b3u0f7>div.svelte-1b3u0f7.svelte-1b3u0f7{flex-grow:1;text-align:center}.addon-list-wrapper.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{position:relative;overflow-y:auto;-webkit-user-select:none;user-select:none}.addon-list-nav-wrapper.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7,.addon-list.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{padding:0 0.8em}.addon-list-nav-wrapper.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{background-color:var(--base-color-tone-a-alpha-85);box-shadow:inset 0 -1px 0px 0 var(--base-color-tone-b);position:sticky;top:0;z-index:20}.preamble.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{display:grid;grid-template-columns:3rem 1fr;grid-column-gap:0.8rem;align-items:center;margin-top:0.4rem;padding:0 1.6rem;font-size:0.85em;background-image:linear-gradient(45deg, rgba(255, 192, 203, 0.2), rgba(255, 165, 0, 0.2));color:var(--inverse-color-tone-a)}.preamble.svelte-1b3u0f7 p.svelte-1b3u0f7.svelte-1b3u0f7{margin:0.75rem 0}.preamble.svelte-1b3u0f7 .icon{width:3rem;height:3rem;fill:var(--inverse-color-tone-b)}.addon-list.svelte-1b3u0f7.svelte-1b3u0f7.svelte-1b3u0f7{margin:0.8em 0}.addon-list.svelte-1b3u0f7 li.svelte-1b3u0f7.svelte-1b3u0f7{border-radius:4px}.addon-list.svelte-1b3u0f7 li.svelte-1b3u0f7+li.svelte-1b3u0f7{margin-top:4px}.addon-list.svelte-1b3u0f7 li.svelte-1b3u0f7.svelte-1b3u0f7:nth-child(odd){background-color:var(--base-color)}
+.alerts.svelte-jtijg8.svelte-jtijg8{-webkit-backdrop-filter:blur(6px);backdrop-filter:blur(6px)}.alerts.svelte-jtijg8.svelte-jtijg8{border-radius:0.75em;box-shadow:0 1rem 3rem var(--inverse-color-alpha-10)}.alerts-wrapper.svelte-jtijg8.svelte-jtijg8{position:fixed;left:0;right:0;display:flex;justify-content:center;margin-top:calc(3rem + 4px);z-index:20}.alerts.svelte-jtijg8.svelte-jtijg8{max-width:75vw;padding:0 0.8rem;background-color:var(--alert-background-color);font-size:0.8em;display:grid;grid-template-columns:auto 6rem;grid-column-gap:0.8rem;word-break:break-all}.current-alert.svelte-jtijg8 h1.svelte-jtijg8{margin-bottom:0}.alert-nav.svelte-jtijg8.svelte-jtijg8{align-self:center;justify-self:center}.alert-nav.svelte-jtijg8 button.svelte-jtijg8{line-height:1.8em;margin:0;padding:0.5em;border-radius:0.45em;border:0;transition:all 0.2s}.alert-nav.svelte-jtijg8 button.svelte-jtijg8:disabled{opacity:0.5}.alert-nav.svelte-jtijg8 button.svelte-jtijg8:hover:not(:disabled){background-color:var(--inverse-color-alpha-05)}.alert-nav.svelte-jtijg8 button.svelte-jtijg8:focus{background-color:var(--inverse-color-alpha-10);box-shadow:inset 0 0 0 1px var(--inverse-color-alpha-20)}.alert-nav.svelte-jtijg8 .icon{display:block;height:1rem;width:1rem;fill:var(--inverse-color)}
 .main.svelte-tax5nz.svelte-tax5nz{display:flex;flex-direction:column;flex:1;overflow-y:hidden}.wrapper.svelte-tax5nz.svelte-tax5nz{display:flex;flex-direction:column;height:100vh}.menubar.svelte-tax5nz.svelte-tax5nz{display:flex;align-items:center;min-height:55px}.menubar.svelte-tax5nz .instawow-version.svelte-tax5nz{flex-grow:1;text-align:right;font-family:Menlo, Monaco, Consolas, monospace;font-size:0.7em}.menubar.svelte-tax5nz .instawow-version span.svelte-tax5nz{color:var(--inverse-color-tone-a)}.main.svelte-tax5nz.svelte-tax5nz{padding:0;z-index:5;background-color:var(--base-color-tone-a);border-top:4px solid var(--random-border-color)}.menubar.svelte-tax5nz.svelte-tax5nz,.statusbar.svelte-tax5nz.svelte-tax5nz{padding:0 0.8em;-webkit-user-select:none;user-select:none}.statusbar.svelte-tax5nz.svelte-tax5nz{padding-top:0.5em;padding-bottom:0.5em;background-color:var(--base-color);box-shadow:inset 0 1px var(--base-color-tone-b)}.statusbar.svelte-tax5nz .status.svelte-tax5nz{font-size:0.8em;color:var(--inverse-color-tone-a)}
```

### Comparing `instawow-2.1.1/gui-webview/src/instawow_gui/json_rpc_server.py` & `instawow-2.2.0/gui-webview/src/instawow_gui/json_rpc_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from __future__ import annotations
 
 import asyncio
+import contextvars
 import json
 import os
 import typing
-from collections import defaultdict
-from collections.abc import Awaitable, Callable, Iterator
+from collections.abc import Awaitable, Callable, Iterator, Set
 from contextlib import AsyncExitStack, contextmanager
 from datetime import datetime
 from functools import partial
+from itertools import chain
 from pathlib import Path
 from typing import Any, Literal, TypeVar, cast
 
 import aiohttp
 import aiohttp.typedefs
 import aiohttp.web
+import anyio
 import click
 import iso8601
 import sqlalchemy as sa
-import toga
 from aiohttp_rpc import JsonRpcMethod
 from aiohttp_rpc import middlewares as rpc_middlewares
 from aiohttp_rpc.errors import InvalidParams, ServerError
 from aiohttp_rpc.server import WsJsonRpcServer
 from attrs import evolve, frozen
 from cattrs import Converter
 from cattrs.preconf.json import configure_converter
 from exceptiongroup import ExceptionGroup
 from loguru import logger
 from typing_extensions import Concatenate, ParamSpec, TypeAlias, TypedDict
 from yarl import URL
 
 from instawow import __version__, db, matchers, models
 from instawow import results as R
+from instawow._version import is_outdated
 from instawow.cataloguer import CatalogueEntry
-from instawow.common import Flavour, SourceMetadata, infer_flavour_from_path
+from instawow.common import Defn, Flavour, SourceMetadata, infer_flavour_from_path
 from instawow.config import Config, GlobalConfig, SecretStr, config_converter
 from instawow.github_auth import get_codes, poll_for_access_token
 from instawow.http import TraceRequestCtx, init_web_client
-from instawow.manager import LocksType, Manager, contextualise, is_outdated
-from instawow.resolvers import Defn
-from instawow.utils import read_resource_as_text, reveal_folder, uniq
+from instawow.manager import LocksType, Manager, bucketise_results, contextualise
+from instawow.utils import WeakValueDefaultDictionary, read_resource_as_text, reveal_folder, uniq
 from instawow.utils import run_in_thread as t
 
 from . import frontend
 
 _T = TypeVar('_T')
 _P = ParamSpec('_P')
 _ManagerBoundCoroFn: TypeAlias = Callable[Concatenate[Manager, _P], Awaitable[_T]]
 
+_toga_handle = contextvars.ContextVar[tuple[Any, anyio.from_thread.BlockingPortal]]('_toga_handle')
+
 
 LOCALHOST = '127.0.0.1'
 
 _converter = Converter(
     unstruct_collection_overrides={
-        # TODO: Replace with ``collections.abc.Set``
-        frozenset: sorted,
+        Set: sorted,
     }
 )
 configure_converter(_converter)
 _converter.register_structure_hook(Path, lambda v, _: Path(v))
 _converter.register_structure_hook(datetime, lambda v, _: iso8601.parse_date(v))
 _converter.register_unstructure_hook(Path, str)
 
@@ -91,15 +93,15 @@
     error_class: type[ServerError | InvalidParams] = ServerError,
     values: dict[Any, Any] | None = None,
 ) -> Iterator[None]:
     try:
         yield
     except BaseException as exc:
         logger.info(f'invalid request: {(values, exc)}')
-        raise error_class(data=_structure_excs(exc))
+        raise error_class(data=_structure_excs(exc)) from exc
 
 
 @t
 def _read_global_config() -> GlobalConfig:
     with _reraise_validation_error(_ConfigError):
         return GlobalConfig.read()
 
@@ -129,39 +131,33 @@
 @frozen(slots=False)
 class _DefnParamMixin:
     defns: list[Defn]
 
 
 class BaseParams:
     @classmethod
-    def bind(
-        cls, method: str, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> JsonRpcMethod:
+    def bind(cls, method: str, managers: _ManagersManager) -> JsonRpcMethod:
         async def respond(**kwargs: Any):
             with _reraise_validation_error(InvalidParams, kwargs):
                 self = _converter.structure(kwargs, cls)
-            return await self.respond(managers, app_window)
+            return await self.respond(managers)
 
         return JsonRpcMethod(respond, name=method)
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> Any:
+    async def respond(self, managers: _ManagersManager) -> Any:
         raise NotImplementedError
 
 
 @_register_method('config/write_profile')
 class WriteProfileConfigParams(_ProfileParamMixin, BaseParams):
     addon_dir: Path
     game_flavour: Flavour
     infer_game_flavour: bool
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> Config:
+    async def respond(self, managers: _ManagersManager) -> Config:
         async with managers.locks['modify profile', self.profile]:
             with _reraise_validation_error(_ConfigError):
                 config = config_converter.structure(
                     {
                         'global_config': await _read_global_config(),
                         'profile': self.profile,
                         'addon_dir': self.addon_dir,
@@ -181,134 +177,114 @@
             managers.unload_profile(config.profile)
 
             return config
 
 
 @_register_method('config/read_profile')
 class ReadProfileConfigParams(_ProfileParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> Config:
+    async def respond(self, managers: _ManagersManager) -> Config:
         return await _read_config(managers.global_config, self.profile)
 
 
 @_register_method('config/delete_profile')
 class DeleteProfileConfigParams(_ProfileParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> None:
+    async def respond(self, managers: _ManagersManager) -> None:
         async def delete_profile(manager: Manager):
             await t(manager.config.delete)()
             managers.unload_profile(self.profile)
 
         await managers.run(self.profile, delete_profile)
 
 
 @_register_method('config/list_profiles')
 class ListProfilesParams(BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[str]:
+    async def respond(self, managers: _ManagersManager) -> list[str]:
         return await t(managers.global_config.list_profiles)()
 
 
 @_register_method('config/update_global')
 class UpdateGlobalConfigParams(BaseParams):
     access_tokens: dict[str, typing.Union[str, None]]
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> GlobalConfig:
+    async def respond(self, managers: _ManagersManager) -> GlobalConfig:
         def update_global_config_cb(global_config: GlobalConfig):
             return evolve(
                 global_config,
                 access_tokens=evolve(
                     global_config.access_tokens,
                     **{k: t if t is None else SecretStr(t) for k, t in self.access_tokens.items()},
                 ),
             )
 
         return await managers.update_global_config(update_global_config_cb)
 
 
 @_register_method('config/read_global')
 class ReadGlobalConfigParams(BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> GlobalConfig:
+    async def respond(self, managers: _ManagersManager) -> GlobalConfig:
         return await _read_global_config()
 
 
 class GithubCodesResponse(TypedDict):
     user_code: str
     verification_uri: str
 
 
 @_register_method('config/initiate_github_auth_flow')
 class InitiateGithubAuthFlowParams(BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> GithubCodesResponse:
+    async def respond(self, managers: _ManagersManager) -> GithubCodesResponse:
         return await managers.initiate_github_auth_flow()
 
 
 class GithubAuthFlowStatusReport(TypedDict):
     status: Literal['success', 'failure']
 
 
 @_register_method('config/query_github_auth_flow_status')
 class QueryGithubAuthFlowStatusParams(BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> GithubAuthFlowStatusReport:
+    async def respond(self, managers: _ManagersManager) -> GithubAuthFlowStatusReport:
         return {'status': await managers.wait_for_github_auth_completion()}
 
 
 @_register_method('config/cancel_github_auth_flow')
 class CancelGithubAuthFlowParams(BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> None:
+    async def respond(self, managers: _ManagersManager) -> None:
         managers.cancel_github_auth_polling()
 
 
 @_register_method('sources/list')
 class ListSourcesParams(_ProfileParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> dict[str, SourceMetadata]:
+    async def respond(self, managers: _ManagersManager) -> dict[str, SourceMetadata]:
         manager = await managers.get_manager(self.profile)
         return {r.metadata.id: r.metadata for r in manager.resolvers.values()}
 
 
 @_register_method('list')
 class ListInstalledParams(_ProfileParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[models.Pkg]:
+    async def respond(self, managers: _ManagersManager) -> list[models.Pkg]:
         manager = await managers.get_manager(self.profile)
-        installed_pkgs = (
-            manager.database.execute(sa.select(db.pkg).order_by(sa.func.lower(db.pkg.c.name)))
-            .mappings()
-            .all()
-        )
-        return [models.Pkg.from_row_mapping(manager.database, p) for p in installed_pkgs]
+
+        with manager.database.connect() as connection:
+            installed_pkgs = (
+                connection.execute(sa.select(db.pkg).order_by(sa.func.lower(db.pkg.c.name)))
+                .mappings()
+                .all()
+            )
+            return [models.Pkg.from_row_mapping(connection, p) for p in installed_pkgs]
 
 
 @_register_method('search')
 class SearchParams(_ProfileParamMixin, BaseParams):
     search_terms: str
     limit: int
     sources: set[str]
     start_date: typing.Union[datetime, None]
     installed_only: bool
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[CatalogueEntry]:
+    async def respond(self, managers: _ManagersManager) -> list[CatalogueEntry]:
         return await managers.run(
             self.profile,
             partial(
                 Manager.search,
                 search_terms=self.search_terms,
                 limit=self.limit,
                 sources=self.sources,
@@ -337,49 +313,43 @@
                 if match:
                     source, alias = match
                     defn = evolve(defn, source=source, alias=alias)
             return defn
 
         return await manager.resolve(list(map(extract_source, self.defns)))
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[SuccessResult | ErrorResult]:
+    async def respond(self, managers: _ManagersManager) -> list[SuccessResult | ErrorResult]:
         results = await managers.run(self.profile, self._resolve)
         return [
             {'status': 'success', 'addon': r}
             if isinstance(r, models.Pkg)
             else {'status': r.status, 'message': r.message}
             for r in results.values()
         ]
 
 
 @_register_method('install')
 class InstallParams(_ProfileParamMixin, _DefnParamMixin, BaseParams):
     replace: bool
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[SuccessResult | ErrorResult]:
+    async def respond(self, managers: _ManagersManager) -> list[SuccessResult | ErrorResult]:
         results = await managers.run(
             self.profile, partial(Manager.install, defns=self.defns, replace=self.replace)
         )
         return [
             {'status': r.status, 'addon': r.pkg}
             if isinstance(r, R.PkgInstalled)
             else {'status': r.status, 'message': r.message}
             for r in results.values()
         ]
 
 
 @_register_method('update')
 class UpdateParams(_ProfileParamMixin, _DefnParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[SuccessResult | ErrorResult]:
+    async def respond(self, managers: _ManagersManager) -> list[SuccessResult | ErrorResult]:
         results = await managers.run(
             self.profile, partial(Manager.update, defns=self.defns, retain_defn_strategy=True)
         )
         return [
             {'status': r.status, 'addon': r.new_pkg}
             if isinstance(r, R.PkgUpdated)
             else {'status': r.status, 'addon': r.pkg}
@@ -389,50 +359,44 @@
         ]
 
 
 @_register_method('remove')
 class RemoveParams(_ProfileParamMixin, _DefnParamMixin, BaseParams):
     keep_folders: bool
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[SuccessResult | ErrorResult]:
+    async def respond(self, managers: _ManagersManager) -> list[SuccessResult | ErrorResult]:
         results = await managers.run(
             self.profile, partial(Manager.remove, defns=self.defns, keep_folders=self.keep_folders)
         )
         return [
             {'status': r.status, 'addon': r.old_pkg}
             if isinstance(r, R.PkgRemoved)
             else {'status': r.status, 'message': r.message}
             for r in results.values()
         ]
 
 
 @_register_method('pin')
 class PinParams(_ProfileParamMixin, _DefnParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[SuccessResult | ErrorResult]:
+    async def respond(self, managers: _ManagersManager) -> list[SuccessResult | ErrorResult]:
         results = await managers.run(self.profile, partial(Manager.pin, defns=self.defns))
         return [
             {'status': r.status, 'addon': r.pkg}
             if isinstance(r, R.PkgInstalled)
             else {'status': r.status, 'message': r.message}
             for r in results.values()
         ]
 
 
 @_register_method('get_changelog')
 class GetChangelogParams(_ProfileParamMixin, BaseParams):
     source: str
     changelog_url: str
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> str:
+    async def respond(self, managers: _ManagersManager) -> str:
         return await managers.run(
             self.profile,
             partial(Manager.get_changelog, source=self.source, uri=self.changelog_url),
         )
 
 
 class AddonMatch(TypedDict):
@@ -443,182 +407,157 @@
 class AddonMatch_AddonFolder(TypedDict):
     name: str
     version: str
 
 
 @_register_method('reconcile')
 class ReconcileParams(_ProfileParamMixin, BaseParams):
-    matcher: Literal[
-        'toc_source_ids', 'folder_hashes', 'folder_name_subsets', 'addon_names_with_folder_names'
-    ]
-
-    _MATCHERS = {
-        'toc_source_ids': matchers.match_toc_source_ids,
-        'folder_name_subsets': matchers.match_folder_name_subsets,
-        'folder_hashes': matchers.match_folder_hashes,
-        'addon_names_with_folder_names': matchers.match_addon_names_with_folder_names,
-    }
+    matcher: str
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[AddonMatch]:
-        leftovers = await managers.run(self.profile, t(matchers.get_unreconciled_folders))
-        match_groups = await managers.run(
-            self.profile, partial(self._MATCHERS[self.matcher], leftovers=leftovers)
-        )
-        resolved_defns = await managers.run(
-            self.profile,
-            partial(Manager.resolve, defns=uniq(d for _, b in match_groups for d in b)),
-        )
-        resolved_pkgs = {k: v for k, v in resolved_defns.items() if isinstance(v, models.Pkg)}
-        matched_pkgs = [
-            (a, m)
-            for a, s in match_groups
-            for m in ([i for i in (resolved_pkgs.get(d) for d in s) if i],)
-            if m
+    async def respond(self, managers: _ManagersManager) -> list[AddonMatch]:
+        manager = await managers.get_manager(self.profile)
+
+        leftovers = await t(matchers.get_unreconciled_folders)(manager)
+
+        match_groups = await matchers.DEFAULT_MATCHERS[self.matcher](manager, leftovers=leftovers)
+
+        resolved_defns = await manager.resolve(uniq(d for _, b in match_groups for d in b))
+        pkgs, _ = bucketise_results(resolved_defns.items())
+
+        matched_folders = [
+            (a, [i for i in (pkgs.get(d) for d in s) if i]) for a, s in match_groups
         ]
+        unmatched_folders = (
+            ([a], list[models.Pkg]())
+            for a in sorted(leftovers - frozenset(i for a, _ in matched_folders for i in a))
+        )
         return [
-            *(
-                AddonMatch(folders=[{'name': f.name, 'version': f.version} for f in a], matches=m)
-                for a, m in matched_pkgs
-            ),
-            *(
-                AddonMatch(folders=[{'name': f.name, 'version': f.version}], matches=[])
-                for f in sorted(leftovers - frozenset(i for a, _ in matched_pkgs for i in a))
-            ),
+            {'folders': [{'name': f.name, 'version': f.version} for f in a], 'matches': m}
+            for a, m in chain(matched_folders, unmatched_folders)
         ]
 
 
 class ReconcileInstalledCandidate(TypedDict):
     installed_addon: models.Pkg
     alternative_addons: list[models.Pkg]
 
 
 @_register_method('get_reconcile_installed_candidates')
 class GetReconcileInstalledCandidatesParams(_ProfileParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[ReconcileInstalledCandidate]:
+    async def respond(self, managers: _ManagersManager) -> list[ReconcileInstalledCandidate]:
         manager = await managers.get_manager(self.profile)
-        installed_pkgs = [
-            models.Pkg.from_row_mapping(manager.database, p)
-            for p in manager.database.execute(
-                sa.select(db.pkg).order_by(sa.func.lower(db.pkg.c.name))
-            )
-            .mappings()
-            .all()
-        ]
+
+        with manager.database.connect() as connection:
+            installed_pkgs = [
+                models.Pkg.from_row_mapping(connection, p)
+                for p in connection.execute(
+                    sa.select(db.pkg).order_by(sa.func.lower(db.pkg.c.name))
+                )
+                .mappings()
+                .all()
+            ]
+
         defn_groups = await managers.run(
             self.profile, partial(Manager.find_equivalent_pkg_defns, pkgs=installed_pkgs)
         )
         resolved_defns = await managers.run(
             self.profile,
             partial(Manager.resolve, defns=uniq(d for b in defn_groups.values() for d in b)),
         )
-        resolved_pkgs = {k: v for k, v in resolved_defns.items() if isinstance(v, models.Pkg)}
+        pkgs, _ = bucketise_results(resolved_defns.items())
         return [
             {'installed_addon': p, 'alternative_addons': m}
             for p, s in defn_groups.items()
-            for m in ([i for i in (resolved_pkgs.get(d) for d in s) if i],)
+            for m in ([i for i in (pkgs.get(d) for d in s) if i],)
             if m
         ]
 
 
 class DownloadProgressReport(TypedDict):
     defn: Defn
     progress: float
 
 
 @_register_method('get_download_progress')
 class GetDownloadProgressParams(_ProfileParamMixin, BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> list[DownloadProgressReport]:
+    async def respond(self, managers: _ManagersManager) -> list[DownloadProgressReport]:
         return [
             {'defn': p.to_defn(), 'progress': r}
             for p, r in await managers.get_manager_download_progress(self.profile)
         ]
 
 
 class GetVersionResult(TypedDict):
     installed_version: str
     new_version: str | None
 
 
 @_register_method('meta/get_version')
 class GetVersionParams(BaseParams):
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> GetVersionResult:
+    async def respond(self, managers: _ManagersManager) -> GetVersionResult:
         outdated, new_version = await is_outdated(managers.global_config)
         return {
             'installed_version': __version__,
             'new_version': new_version if outdated else None,
         }
 
 
 @_register_method('assist/open_url')
 class OpenUrlParams(BaseParams):
     url: str
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> None:
+    async def respond(self, managers: _ManagersManager) -> None:
         click.launch(self.url)
 
 
 @_register_method('assist/reveal_folder')
 class RevealFolderParams(BaseParams):
     path_parts: list[str]
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> None:
+    async def respond(self, managers: _ManagersManager) -> None:
         reveal_folder(os.path.join(*self.path_parts))
 
 
 class SelectFolderResult(TypedDict):
     selection: Path | None
 
 
 @_register_method('assist/select_folder')
 class SelectFolderParams(BaseParams):
     initial_folder: typing.Union[str, None]
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> SelectFolderResult:
-        if not app_window:
-            raise RuntimeError('No app to bind to')
+    async def respond(self, managers: _ManagersManager) -> SelectFolderResult:
+        main_window, portal = _toga_handle.get()
+
+        async def select_folder() -> Path | None:
+            return await main_window.select_folder_dialog('Select folder', self.initial_folder)
 
-        selection: Path | None
         try:
-            selection = await app_window.select_folder_dialog('Select folder', self.initial_folder)
+            selection = portal.start_task_soon(select_folder).result()
         except ValueError:
             selection = None
         return {'selection': selection}
 
 
 class ConfirmDialogueResult(TypedDict):
     ok: bool
 
 
 @_register_method('assist/confirm')
 class ConfirmDialogueParams(BaseParams):
     title: str
     message: str
 
-    async def respond(
-        self, managers: _ManagerWorkQueue, app_window: toga.MainWindow | None
-    ) -> ConfirmDialogueResult:
-        if not app_window:
-            raise RuntimeError('No app to bind to')
+    async def respond(self, managers: _ManagersManager) -> ConfirmDialogueResult:
+        main_window, portal = _toga_handle.get()
+
+        async def confirm() -> bool:
+            return await main_window.confirm_dialog(self.title, self.message)
 
-        ok: bool = await app_window.confirm_dialog(self.title, self.message)
-        return {'ok': ok}
+        return {'ok': portal.start_task_soon(confirm).result()}
 
 
 def _init_json_rpc_web_client(cache_dir: Path):
     async def do_on_request_end(
         client_session: aiohttp.ClientSession,
         trace_config_ctx: Any,
         params: aiohttp.TraceRequestEndParams,
@@ -645,98 +584,69 @@
     trace_config = aiohttp.TraceConfig()
     trace_config.on_request_end.append(do_on_request_end)
     trace_config.freeze()
 
     return (init_web_client(cache_dir, trace_configs=[trace_config]), progress_reporters)
 
 
-class _ManagerWorkQueue:
+class _ManagersManager:
     def __init__(self):
-        self._loop = asyncio.get_running_loop()
-
         self._exit_stack = AsyncExitStack()
 
-        self._queue: asyncio.Queue[
-            tuple[asyncio.Future[object], str, _ManagerBoundCoroFn[..., object]]
-        ] = asyncio.Queue()
+        self.locks: LocksType = WeakValueDefaultDictionary(asyncio.Lock)
 
-        self.locks: LocksType = defaultdict(asyncio.Lock)
-
-        self._managers: dict[str, tuple[Manager, Callable[[], None]]] = {}
+        self._managers = dict[str, Manager]()
 
         self._github_auth_device_codes = None
         self._github_auth_flow_task = None
 
     async def __aenter__(self):
         self.global_config = await _read_global_config()
         init_json_rpc_web_client, self._download_progress_reporters = _init_json_rpc_web_client(
             self.global_config.cache_dir
         )
         self._web_client = await self._exit_stack.enter_async_context(init_json_rpc_web_client)
         contextualise(web_client=self._web_client, locks=self.locks)
-        self._exit_stack.callback(self._loop.create_task(self._listen()).cancel)
 
     async def __aexit__(self, *args: object):
         self.cancel_github_auth_polling()
-        self._unload_all_profiles()
         await self._exit_stack.aclose()
 
     def unload_profile(self, profile: str):
         if profile in self._managers:
-            _, close_db_conn = self._managers.pop(profile)
-            close_db_conn()
+            del self._managers[profile]
 
     def _unload_all_profiles(self):
-        for profile in list(self._managers):
-            self.unload_profile(profile)
+        self._managers.clear()
 
     async def update_global_config(
         self, update_cb: Callable[[GlobalConfig], GlobalConfig]
     ) -> GlobalConfig:
         async with self.locks['update global config']:
             with _reraise_validation_error(_ConfigError):
                 self.global_config = update_cb(self.global_config)
                 await t(self.global_config.write)()
+
             self._unload_all_profiles()
+
             return self.global_config
 
-    async def _taskify(
-        self,
-        future: asyncio.Future[_T],
-        profile: str,
-        coro_fn: _ManagerBoundCoroFn[..., _T],
-    ):
+    async def run(self, profile: str, coro_fn: _ManagerBoundCoroFn[..., _T]) -> _T:
         try:
-            try:
-                manager, _ = self._managers[profile]
-            except KeyError:
-                async with self.locks['modify profile', profile]:
-                    try:
-                        manager, _ = self._managers[profile]
-                    except KeyError:
-                        manager, _ = self._managers[profile] = Manager.from_config(
-                            await _read_config(self.global_config, profile)
-                        )
-
-            result = await coro_fn(manager)
-        except BaseException as exc:
-            future.set_exception(exc)
-        else:
-            future.set_result(result)
+            manager = self._managers[profile]
+        except KeyError:
+            async with self.locks['modify profile', profile]:
+                try:
+                    manager = self._managers[profile]
+                except KeyError:
+                    manager = self._managers[profile] = Manager.from_config(
+                        await _read_config(self.global_config, profile)
+                    )
 
-    async def _listen(self):
-        while True:
-            item = await self._queue.get()
-            asyncio.create_task(self._taskify(*item))
-            self._queue.task_done()
-
-    async def run(self, profile: str, coro_fn: _ManagerBoundCoroFn[..., _T]) -> _T:
-        future = self._loop.create_future()
-        self._queue.put_nowait((future, profile, coro_fn))
-        return await future
+        return await coro_fn(manager)
 
     async def get_manager(self, profile: str):
         async def get_manager(manager: Manager):
             return manager
 
         return await self.run(profile, get_manager)
 
@@ -763,20 +673,20 @@
                             access_tokens=evolve(
                                 global_config.access_tokens, github=SecretStr(result)
                             ),
                         )
 
                     await self.update_global_config(update_global_config_cb)
 
-                def on_task_complete(future: object):
+                def on_task_complete(task: object):
                     self._github_auth_flow_task = None
                     self._github_auth_device_codes = None
 
                 self._github_auth_device_codes = codes = await get_codes(self._web_client)
-                self._github_auth_flow_task = self._loop.create_task(finalise_github_auth_flow())
+                self._github_auth_flow_task = asyncio.create_task(finalise_github_auth_flow())
                 self._github_auth_flow_task.add_done_callback(on_task_complete)
 
         return self._github_auth_device_codes
 
     async def wait_for_github_auth_completion(self):
         if self._github_auth_flow_task is not None:
             try:
@@ -786,18 +696,21 @@
         return 'success'
 
     def cancel_github_auth_polling(self):
         if self._github_auth_flow_task is not None:
             self._github_auth_flow_task.cancel()
 
 
-async def create_app(app_window: toga.MainWindow | None = None):
-    managers = _ManagerWorkQueue()
+async def create_app(toga_handle: tuple[Any, anyio.from_thread.BlockingPortal] | None = None):
+    if toga_handle:
+        _toga_handle.set(toga_handle)
+
+    managers = _ManagersManager()
 
-    async def listen(app: aiohttp.web.Application):
+    async def managers_listen(app: aiohttp.web.Application):
         async with managers:
             yield
 
     async def get_index(request: aiohttp.web.Request):
         return aiohttp.web.Response(
             content_type='text/html',
             text=read_resource_as_text(frontend, 'index.html'),
@@ -821,15 +734,15 @@
         return json.dumps(_converter.unstructure(value))
 
     rpc_server = WsJsonRpcServer(
         json_serialize=json_serialize,
         middlewares=rpc_middlewares.DEFAULT_MIDDLEWARES,  # pyright: ignore[reportUnknownMemberType]
     )
     rpc_server.add_methods(  # pyright: ignore[reportUnknownMemberType]
-        [m.bind(n, managers, app_window) for n, m in _methods]
+        [m.bind(n, managers) for n, m in _methods]
     )
 
     @aiohttp.web.middleware
     async def enforce_same_origin(
         request: aiohttp.web.Request,
         handler: aiohttp.typedefs.Handler,
     ):
@@ -857,15 +770,15 @@
             aiohttp.web.get('/', get_index),
             aiohttp.web.get(
                 r'/svelte-bundle{extension:(?:\.css|\.js(?:\.map)?)}', get_static_file
             ),
             aiohttp.web.get('/api', rpc_server.handle_http_request),
         ]
     )
-    app.cleanup_ctx.append(listen)
+    app.cleanup_ctx.append(managers_listen)
     app.freeze()
     return app
 
 
 async def run_app(app: aiohttp.web.Application):
     "Fire up the server."
     app_runner = aiohttp.web.AppRunner(app)
```

### Comparing `instawow-2.1.1/gui-webview/src/instawow_gui/resources/instawow_gui.icns` & `instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.icns`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/gui-webview/src/instawow_gui/resources/instawow_gui.ico` & `instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.ico`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/gui-webview/src/instawow_gui/resources/instawow_gui.png` & `instawow-2.2.0/gui-webview/src/instawow_gui/resources/instawow_gui.png`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/pyproject.toml` & `instawow-2.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 substitution.files = ["src/instawow/_version.py"]
 
 [tool.poetry]
 name = "instawow"
-version = "2.1.1"
+version = "2.2.0"
 description = "World of Warcraft add-on manager"
 license = "GPL-3.0-or-later"
 authors = [
   "layday <layday@protonmail.com>",
 ]
 readme = "README.rst"
 urls.homepage = "http://github.com/layday/instawow"
@@ -28,96 +28,116 @@
 ]
 scripts.instawow = "instawow.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 
 aiohttp = ">=3.8.2, <4"
-aiohttp-client-cache = ">=0.7.3"
-alembic = ">=1.7.0"
-attrs = ">=22.1.0"
+aiohttp-client-cache = ">=0.8.0"
+alembic = ">=1.9.0"
+attrs = ">=23.1.0"
 cattrs = ">=22.2.0"
-click = ">=8.0.0"
+click = ">=8.1.0"
 exceptiongroup = ">=1.0.0"
 iso8601 = ">=1.0.2"
-loguru = ">=0.5.3"
+loguru = ">=0.7.0"
 mako = ">=1.2.4"
+packaging = ">=23.0"
 pluggy = ">=0.13"
 prompt-toolkit = ">=3.0.29, <4"
 questionary = ">=1.10"
 rapidfuzz = ">=2.12.0"
-sqlalchemy = ">=1.4.23"
+sqlalchemy = ">=2.0.0"
 typing-extensions = ">=4.3.0"
 yarl = ">=1.8.1"
 
 aiohttp-rpc = { version = ">=1.0.0", optional = true }
-toga = { version = ">=0.3.0.dev33", optional = true }
+anyio = { version = ">=3.6.2", optional = true }
+toga = { version = ">=0.3.0", optional = true }
 
-aresponses = { version = ">=2.1.4 ", optional = true }
+aresponses = { version = ">=2.1.4", optional = true }
 coverage = { version = ">=6.2", extras = ["toml"], optional = true }
 pytest = { version = ">=6.2.5", optional = true }
 pytest-asyncio = { version = ">=0.17.0", optional = true }
 pytest-xdist = { version = ">=2.5.0", optional = true }
 
-sqlalchemy2-stubs = { version = "*", optional = true }
+types-certifi = { version = "*", optional = true }
 
 [tool.poetry.extras]
 gui = [
   "aiohttp-rpc",
+  "anyio",
   "toga",
 ]
 test = [
   "aresponses",
   "coverage",
   "pytest",
   "pytest-asyncio",
   "pytest-xdist",
 ]
 types = [
-  "sqlalchemy2-stubs",
+  "types-certifi",
 ]
 
 
-[tool.pyright]
-include = [
-  "src",
-  "gui-webview/src",
-  "tests/plugin",
-]
-ignore = [
-  "src/instawow/_migrations",
-]
-strict = [
-  "src",
-  "gui-webview/src/instawow_gui/json_rpc_server.py",
-  "tests/plugin",
-]
-
 [tool.ruff]
 select = [
-  "B0",     # bugbear (without opinionated rules)
-  "C4",     # comprehensions
-  "E",      # pycodestyle
-  "F",      # pyflakes
-  "I0",     # isort
-  "RUF100", # ruff: `UnusedNOQA`
-  "UP",     # pyupgrade
-  "W",      # pycodestyle
+  "B0",  # flake8-bugbear (without opinionated rules)
+  "C4",  # flake8-comprehensions
+  "DTZ", # flake8-datetimez
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "I",   # isort
+  "PGH", # pygrep-hooks
+  "PIE", # flake8-pie
+  "PT",  # flake8-pytest-style
+  "PYI", # flake8-pyi
+  "Q",   # flake8-quotes
+  "RUF", # ruff: unused-noqa
+  "TRY", # tryceratops
+  "UP",  # pyupgrade
+  "W",   # pycodestyle
+  "YTT", # flake8-2020
 ]
 ignore = [
-  "E501", # pycodestyle: `LineTooLong`
+  "E501",   # pycodestyle: line-too-long
+  "RUF001", # ruff: ambiguous-unicode-character-string
+  "RUF002", # ruff: ambiguous-unicode-character-docstring
+  "RUF003", # ruff: ambiguous-unicode-character-comment
+  "TRY003", # tryceratops: raise-vanilla-args
 ]
 line-length = 99
 target-version = "py39"
 
+[tool.ruff.per-file-ignores]
+"**.py" = [
+  "PYI",
+]
+"**.pyi" = [
+  "I002", # isort: missing-required-import
+]
+
+[tool.ruff.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
+
+[tool.ruff.flake8-quotes]
+docstring-quotes = "double"
+inline-quotes = "single"
+multiline-quotes = "single"
+
 [tool.ruff.isort]
 known-first-party = [
   "instawow",
   "instawow_gui",
 ]
+required-imports = [
+  "from __future__ import annotations",
+]
 
 [tool.ruff.pyupgrade]
 keep-runtime-typing = true
 
 [tool.black]
 line-length = 99
 skip-string-normalization = true
```

### Comparing `instawow-2.1.1/src/instawow/_addon_hashing.py` & `instawow-2.2.0/src/instawow/_addon_hashing.py`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/src/instawow/_cli_prompts.py` & `instawow-2.2.0/src/instawow/_cli_prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,46 +3,45 @@
 import asyncio
 from collections.abc import Sequence
 from functools import partial
 from typing import TYPE_CHECKING, Any
 
 import attrs
 import cattrs
-from attr import attrib as attrs_attrib
 from exceptiongroup import ExceptionGroup
 from prompt_toolkit.application import Application
 from prompt_toolkit.document import Document
 from prompt_toolkit.formatted_text.html import HTML
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.keys import Keys
-from prompt_toolkit.shortcuts.progress_bar import ProgressBar, formatters
+from prompt_toolkit.shortcuts.progress_bar import ProgressBar, ProgressBarCounter, formatters
 from prompt_toolkit.styles import Style
 from prompt_toolkit.validation import ValidationError, Validator
 from questionary import Choice
 from questionary import confirm as _confirm
 from questionary import password as _password
 from questionary import path as _path
 from questionary.prompts.common import InquirerControl, Separator, create_inquirer_layout
 from questionary.question import Question
 
-from . import _deferred_types
+from . import models
 
 if TYPE_CHECKING:
     ExceptionGroup = ExceptionGroup[Exception]
 
 
-class AttrFieldValidator(Validator):
+class AttrsFieldValidator(Validator):
     "One-off validators for attrs fields."
 
     def __init__(self, attribute: attrs.Attribute[object], converter: cattrs.Converter) -> None:
         self._field_name = attribute.name
         self._FieldWrapper = attrs.make_class(
             '_FieldWrapper',
             {
-                self._field_name: attrs_attrib(
+                self._field_name: attrs.field(
                     default=attribute.default,
                     validator=attribute.validator,
                     repr=attribute.repr,
                     hash=attribute.hash,
                     init=attribute.init,
                     metadata=attribute.metadata,
                     type=attribute.type,
@@ -56,21 +55,21 @@
         )
         self._converter = converter
 
     def validate(self, document: Document) -> None:
         try:
             self._converter.structure({self._field_name: document.text}, self._FieldWrapper)
         except ExceptionGroup as exc_group:
-            raise ValidationError(0, '\n'.join(map(str, exc_group.exceptions)))
+            raise ValidationError(0, '\n'.join(map(str, exc_group.exceptions))) from exc_group
         except Exception as exc:
-            raise ValidationError(0, str(exc))
+            raise ValidationError(0, str(exc)) from exc
 
 
 class PkgChoice(Choice):
-    def __init__(self, *args: Any, pkg: _deferred_types.models.Pkg, **kwargs: Any) -> None:
+    def __init__(self, *args: Any, pkg: models.Pkg, **kwargs: object) -> None:
         super().__init__(*args, **kwargs)
         self.pkg = pkg
 
 
 qstyle = Style(
     [
         ('qmark', 'fg:ansicyan'),
@@ -86,15 +85,15 @@
 skip = Choice([('underline', 's'), ('', 'kip')], SKIP)
 
 confirm = partial(_confirm, qmark='?', style=qstyle)
 path = partial(_path, qmark='>', style=qstyle)
 password = partial(_password, style=qstyle)
 
 
-def checkbox(message: str, choices: Sequence[Choice], **inquirer_kwargs: Any) -> Question:
+def checkbox(message: str, choices: Sequence[Choice], **inquirer_kwargs: object) -> Question:
     def get_prompt_tokens():
         tokens: list[tuple[str, str]] = [('class:question', message)]
         if ic.is_answered:
             tokens.append(('class:answer', '  done'))
         else:
             tokens.append(
                 (
@@ -169,15 +168,15 @@
     return Question(Application(layout=layout, key_bindings=bindings, style=qstyle))
 
 
 def select(
     message: str,
     choices: Sequence[str] | Sequence[Choice],
     initial_choice: str | Choice | None = None,
-    **inquirer_kwargs: Any,
+    **inquirer_kwargs: object,
 ) -> Question:
     def get_prompt_tokens():
         tokens: list[tuple[str, str]] = [('class:qmark', '- '), ('class:question', message)]
         if ic.is_answered:
             answer = ic.get_pointed_at()
             title = answer.title
             assert title
@@ -254,15 +253,15 @@
 def _format_mb(value: int):
     return f'{value / 2 ** 20:.1f}'
 
 
 class _DownloadProgress(formatters.Progress):
     template = '<current>{current:>3}</current>/<total>{total:>3}</total>MB'
 
-    def format(self, progress_bar: ProgressBar, progress: Any, width: int):
+    def format(self, progress_bar: ProgressBar, progress: ProgressBarCounter[object], width: int):
         return HTML(self.template).format(
             current=_format_mb(progress.items_completed),
             total=_format_mb(progress.total) if progress.total is not None else '?',
         )
 
 
 def make_progress_bar() -> ProgressBar:
```

### Comparing `instawow-2.1.1/src/instawow/_custom_slpp.py` & `instawow-2.2.0/src/instawow/_custom_slpp.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,33 +82,30 @@
         idx = 0
 
         self._next()
         while True:
             self._next_not_eq(WHITESPACE)
 
             if self.c == '}':
-
                 # Convert table to list if k(0) = 1 and k = k(n-1) + 1, ...
                 if (
                     table
                     and all(map(eq, table, count(1)))
                     # bool is a subclass of int in Python but not in Lua
                     and not any(isinstance(k, bool) for k in islice(table, 0, 2))
                 ):
                     table = list(table.values())
 
                 self._next()
                 return table
 
             elif self.c == ',':
-
                 self._next()
 
             else:
-
                 is_val_long_string_literal = False
 
                 if self.c == '[':
                     self._next()
                     if self.c == '[':
                         is_val_long_string_literal = True
 
@@ -183,19 +180,19 @@
             if match_bare_word.match(new_s):
                 s = new_s
             else:
                 break
 
         self._next()
 
-        if s == "true":
+        if s == 'true':
             return True
-        elif s == "false":
+        elif s == 'false':
             return False
-        elif s == "nil":
+        elif s == 'nil':
             return None
         return s
 
     def _decode_number(self):
         def get_digits():
             n = ''
 
@@ -212,40 +209,37 @@
 
         n = ''
 
         if self.c == '-':
             c = self.c
             self._next()
             if self.c == '-':
-
                 # This is a comment - skip to the end of the line
                 self._next_eq(NEWLINE)
                 return None
 
             elif not self.c or self.c not in DIGITS:
                 raise ParseError('malformed number (no digits after minus sign)', c + self.c)
 
             n += c
 
         n += self.c + get_digits()
         if n == '0' and self.c in HEXDELIMS:
-
             n += self.c
 
             for c in self._iter_text:
                 if c in HEXDIGITS:
                     n += c
                 else:
                     self.c = c
                     break
             else:
                 self.c = _sentinel
 
         else:
-
             if self.c == '.':
                 n += self.c + get_digits()
 
             if self.c in EXPONENTS:
                 n += self.c
                 self._next()  # +-
                 n += self.c + get_digits()
```

### Comparing `instawow-2.1.1/src/instawow/_import_wrapper.py` & `instawow-2.2.0/src/instawow/_import_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def __getattr__(name: str) -> object:
     """Defer importing own modules until attempting to access an attribute.
 
     Importing this in ``__init__`` will overwrite relative imports.
     """
-    fullname = __package__ + '.' + name
+    fullname = __spec__.parent + '.' + name
     try:
         return sys.modules[fullname]
     except KeyError:
         spec = importlib.util.find_spec(fullname)
         if spec is None:
             # ``AttributeError`` is converted to an ``ImportError`` by the import machinery
             raise AttributeError
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/alembic.ini` & `instawow-2.2.0/src/instawow/_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/src/instawow/_migrations/env.py` & `instawow-2.2.0/src/instawow/_migrations/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from alembic import context
 from sqlalchemy import engine_from_config, pool
 
 from instawow.db import metadata as target_metadata
 
 
 def run_offline() -> None:
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py` & `instawow-2.2.0/src/instawow/_migrations/versions/2bfcfe824fe0_remove_pkgoptions_strategy_constraint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Remove ``PkgOptions`` strategy constraint.
 """
+from __future__ import annotations
+
 from alembic import op
 from sqlalchemy import Enum, String
 
 # revision identifiers, used by Alembic.
 revision = '2bfcfe824fe0'
 down_revision = '58a8306c3a5b'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py` & `instawow-2.2.0/src/instawow/_migrations/versions/3b37d2faccd2_add_missing_unique_constraint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Add UNIQUE constraint that was missing from ``pkg_dep``.
 """
+from __future__ import annotations
+
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '3b37d2faccd2'
 down_revision = '7204944522b1'
 branch_labels = None
 depends_on = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py` & `instawow-2.2.0/src/instawow/_migrations/versions/43aa3610e92a_populate_version_table_from_installed_pkgs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Populate the version table from installed packages.
 """
+from __future__ import annotations
+
 from alembic import op
 from sqlalchemy import String, column, table
 
 # revision identifiers, used by Alembic.
 revision = '43aa3610e92a'
 down_revision = 'd3f542de5ff4'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py` & `instawow-2.2.0/src/instawow/_migrations/versions/58a8306c3a5b_make_basenames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Make basenames out of add-on paths.
 """
+from __future__ import annotations
+
 from pathlib import Path
 
 from alembic import context, op
 from sqlalchemy import String, column, table
 
 # revision identifiers, used by Alembic.
 revision = '58a8306c3a5b'
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py` & `instawow-2.2.0/src/instawow/_migrations/versions/7204944522b1_add_dependency_table.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Add dependency table.
 """
+from __future__ import annotations
+
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '7204944522b1'
 down_revision = '2bfcfe824fe0'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py` & `instawow-2.2.0/src/instawow/_migrations/versions/764fa963cc71_add_changelog_column.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Add the package changelog column.
 
 Revision ID: 764fa963cc71
 Revises: e4921edb1154
 Create Date: 2021-03-20 02:46:24.528320
 
 """
+from __future__ import annotations
+
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '764fa963cc71'
 down_revision = 'e4921edb1154'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py` & `instawow-2.2.0/src/instawow/_migrations/versions/8f6ba74cfa82_rename_origin_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Rename the 'origin' column to 'source'.
 """
+from __future__ import annotations
+
 from functools import partial
 
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '8f6ba74cfa82'
 down_revision = '3b37d2faccd2'
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py` & `instawow-2.2.0/src/instawow/_migrations/versions/98716a7301f8_renovate_pkg_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Renovate ``pkg_options``.
 
 Revision ID: 98716a7301f8
 Revises: e13430219249
 Create Date: 2022-10-23 16:18:51.169154
 
 """
+from __future__ import annotations
+
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '98716a7301f8'
 down_revision = 'e13430219249'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py` & `instawow-2.2.0/src/instawow/_migrations/versions/9b8df9661cdb_add_pkg_version_log_fk.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Create foreign key constraint on ``pkg_version_log``.
 
 Revision ID: 9b8df9661cdb
 Revises: 764fa963cc71
 Create Date: 2021-09-25 18:29:27.577648
 
 """
+from __future__ import annotations
+
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '9b8df9661cdb'
 down_revision = '764fa963cc71'
 branch_labels = None
 depends_on = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py` & `instawow-2.2.0/src/instawow/_migrations/versions/d3f542de5ff4_add_version_log_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Create the ``pkg_version_log`` table to track previously-installed package versions.
 """
+from __future__ import annotations
+
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = 'd3f542de5ff4'
 down_revision = 'f3f9957de30c'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/e13430219249_add_cascade.py` & `instawow-2.2.0/src/instawow/_migrations/versions/e13430219249_add_cascade.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Add cascade deletes to the pkg table's dependents.
 
 Revision ID: e13430219249
 Revises: 75f69831f74f
 Create Date: 2022-04-30 22:29:49.359123
 
 """
+from __future__ import annotations
+
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = 'e13430219249'
 down_revision = '75f69831f74f'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py` & `instawow-2.2.0/src/instawow/_migrations/versions/e4921edb1154_replace_uq_with_pk_constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Replace the ``pkg_dep`` UNIQUE constraint with a pk.
 
 Revision ID: e4921edb1154
 Revises: 43aa3610e92a
 Create Date: 2020-09-08 14:39:34.957011
 
 """
+from __future__ import annotations
+
 from contextlib import suppress
 
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = 'e4921edb1154'
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py` & `instawow-2.2.0/src/instawow/_migrations/versions/e4ae835a34be_change_pkg_options_strategy_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Change the `pkg_options` table's `strategy` column to be
 one of 'default', 'latest'.
 """
+from __future__ import annotations
+
 from functools import partial, update_wrapper
 
 from alembic import op
 from sqlalchemy import Enum, String
 from sqlalchemy.sql import column, table
 
 # revision identifiers, used by Alembic.
```

### Comparing `instawow-2.1.1/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py` & `instawow-2.2.0/src/instawow/_migrations/versions/f3f9957de30c_drop_file_id.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Drop the package table's ``file_id`` column.
 """
+from __future__ import annotations
+
 import sqlalchemy as sa
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = 'f3f9957de30c'
 down_revision = '8f6ba74cfa82'
 branch_labels = None
```

### Comparing `instawow-2.1.1/src/instawow/_sources/cfcore.py` & `instawow-2.2.0/src/instawow/_sources/cfcore.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 import iso8601
 from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypedDict
 from yarl import URL
 
-from .. import _deferred_types, manager, models
+from .. import manager, models
 from .. import results as R
 from ..cataloguer import BaseCatalogueEntry
-from ..common import ChangelogFormat, Flavour, SourceMetadata, Strategy
+from ..common import ChangelogFormat, Defn, Flavour, SourceMetadata, Strategy
 from ..config import GlobalConfig
-from ..http import CACHE_INDEFINITELY, make_generic_progress_ctx
-from ..resolvers import BaseResolver, Defn, HeadersIntent
+from ..http import CACHE_INDEFINITELY, ClientSessionType, make_generic_progress_ctx
+from ..resolvers import BaseResolver, HeadersIntent
 from ..utils import gather, uniq
 
 _T = TypeVar('_T')
 
 
 class _CfCoreModLinks(TypedDict):
     websiteUrl: str
@@ -347,15 +347,14 @@
         if not files:
             raise R.PkgFilesMissing
 
         def make_filter_fns() -> Generator[Callable[[_CfCoreFile], bool], None, None]:
             yield lambda f: not f.get('exposeAsAlternative', False)
 
             if not defn.strategies.any_flavour:
-
                 type_id = self._manager.config.game_flavour.to_flavour_keyed_enum(
                     _CfCoreSortableGameVersionTypeId
                 )
                 yield lambda f: any(
                     s['gameVersionTypeId'] == type_id for s in f['sortableGameVersions']
                 )
 
@@ -410,17 +409,15 @@
             headers=await self.make_request_headers(),
             raise_for_status=True,
         ) as response:
             response_json: _CfCoreStringDataResponse = await response.json()
             return response_json['data']
 
     @classmethod
-    async def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
-    ) -> AsyncIterator[BaseCatalogueEntry]:
+    async def catalogue(cls, web_client: ClientSessionType) -> AsyncIterator[BaseCatalogueEntry]:
         from aiohttp import ClientTimeout
 
         flavours_and_version_types = [
             (f, f.to_flavour_keyed_enum(_CfCoreSortableGameVersionTypeId)) for f in Flavour
         ]
 
         def excise_flavours(files: list[_CfCoreFile]):
```

### Comparing `instawow-2.1.1/src/instawow/_sources/github.py` & `instawow-2.2.0/src/instawow/_sources/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from collections.abc import AsyncIterator, Iterable
 from datetime import datetime, timedelta
 from itertools import tee, zip_longest
-from typing import Literal
+from typing import Any, Literal
 
 import iso8601
 from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypedDict
 from yarl import URL
 
-from .. import _deferred_types, models
+from .. import models
 from .. import results as R
 from ..cataloguer import BaseCatalogueEntry, CatalogueSameAs
-from ..common import ChangelogFormat, Flavour, FlavourVersionRange, SourceMetadata, Strategy
-from ..http import CACHE_INDEFINITELY
-from ..resolvers import BaseResolver, Defn, HeadersIntent
+from ..common import ChangelogFormat, Defn, Flavour, FlavourVersionRange, SourceMetadata, Strategy
+from ..http import CACHE_INDEFINITELY, ClientSessionType
+from ..resolvers import BaseResolver, HeadersIntent
 from ..utils import (
     StrEnum,
     TocReader,
     as_plain_text_data_url,
     extract_byte_range_offset,
     find_addon_zip_tocs,
 )
@@ -182,21 +182,21 @@
                             )
                         )
                         addon_zip_stream.write(await directory_range_response.read())
 
                         try:
                             dynamic_addon_zip = zipfile.ZipFile(addon_zip_stream)
                         except zipfile.BadZipFile:
-                            from zipfile import _ECD_OFFSET, _EndRecData  # pyright: ignore
+                            zipfile_internal: Any = zipfile
 
-                            end_rec_data = _EndRecData(addon_zip_stream)  # pyright: ignore
+                            end_rec_data = zipfile_internal._EndRecData(addon_zip_stream)
                             if end_rec_data is None:
                                 break
 
-                            directory_offset = f'{end_rec_data[_ECD_OFFSET]}-'
+                            directory_offset = f'{end_rec_data[zipfile_internal._ECD_OFFSET]}-'
                         else:
                             break
 
             if dynamic_addon_zip is None:
                 logger.warning('directory marker not found')
                 continue
 
@@ -269,15 +269,14 @@
                 break
 
         return matching_asset
 
     async def _find_matching_asset_from_release_json(
         self, assets: list[_GithubRelease_Asset], release_json_asset: _GithubRelease_Asset
     ):
-
         download_headers = await self.make_request_headers(HeadersIntent.download)
 
         async with self._manager.web_client.get(
             release_json_asset['url'],
             expire_after=timedelta(days=1),
             headers=download_headers,
             raise_for_status=True,
@@ -404,17 +403,15 @@
             date_published=iso8601.parse_date(release['published_at']),
             version=release['tag_name'],
             changelog_url=as_plain_text_data_url(release['body']),
             options=models.PkgOptions.from_strategy_values(defn.strategies),
         )
 
     @classmethod
-    async def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
-    ) -> AsyncIterator[BaseCatalogueEntry]:
+    async def catalogue(cls, web_client: ClientSessionType) -> AsyncIterator[BaseCatalogueEntry]:
         import csv
         from io import StringIO
 
         logger.debug(f'retrieving {cls._generated_catalogue_csv_url}')
 
         async with web_client.get(
             cls._generated_catalogue_csv_url, raise_for_status=True
```

### Comparing `instawow-2.1.1/src/instawow/_sources/instawow.py` & `instawow-2.2.0/src/instawow/_sources/instawow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from collections.abc import AsyncIterator
 from datetime import datetime, timezone
 
-from .. import _deferred_types, models
+from .. import models
 from .. import results as R
 from ..cataloguer import BaseCatalogueEntry
-from ..common import ChangelogFormat, Flavour, SourceMetadata
-from ..resolvers import BaseResolver, Defn
+from ..common import ChangelogFormat, Defn, Flavour, SourceMetadata
+from ..http import ClientSessionType
+from ..resolvers import BaseResolver
 from ..utils import run_in_thread
 
 
 class InstawowResolver(BaseResolver):
     metadata = SourceMetadata(
         id='instawow',
         name='instawow',
@@ -49,17 +50,15 @@
             date_published=datetime.now(timezone.utc),
             version=await run_in_thread(builder.get_version)(),
             changelog_url=builder.changelog_path.as_uri(),
             options=models.PkgOptions.from_strategy_values(defn.strategies),
         )
 
     @classmethod
-    async def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
-    ) -> AsyncIterator[BaseCatalogueEntry]:
+    async def catalogue(cls, web_client: ClientSessionType) -> AsyncIterator[BaseCatalogueEntry]:
         yield BaseCatalogueEntry(
             source=cls.metadata.id,
             id='1',
             slug='weakauras-companion-autoupdate',
             name='WeakAuras Companion',
             url='https://github.com/layday/instawow',
             game_flavours=frozenset(Flavour),
```

### Comparing `instawow-2.1.1/src/instawow/_sources/tukui.py` & `instawow-2.2.0/src/instawow/_sources/tukui.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from datetime import datetime, timedelta, timezone
 from typing import Literal
 
 from loguru import logger
 from typing_extensions import TypedDict
 from yarl import URL
 
-from .. import _deferred_types, manager, models
+from .. import manager, models
 from .. import results as R
 from ..cataloguer import BaseCatalogueEntry
-from ..common import ChangelogFormat, Flavour, SourceMetadata
-from ..http import make_generic_progress_ctx
-from ..resolvers import BaseResolver, Defn
+from ..common import ChangelogFormat, Defn, Flavour, SourceMetadata
+from ..http import ClientSessionType, make_generic_progress_ctx
+from ..resolvers import BaseResolver
 from ..utils import StrEnum, as_plain_text_data_url, gather, slugify
 
 
 class _TukuiUi(TypedDict):
     author: str
     category: str
     changelog: str
@@ -168,17 +168,15 @@
                 # but link to the changelog tab on the add-on page
                 else as_plain_text_data_url(metadata['changelog'])
             ),
             options=models.PkgOptions.from_strategy_values(defn.strategies),
         )
 
     @classmethod
-    async def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
-    ) -> AsyncIterator[BaseCatalogueEntry]:
+    async def catalogue(cls, web_client: ClientSessionType) -> AsyncIterator[BaseCatalogueEntry]:
         for flavours, query in [
             (frozenset(Flavour), {'ui': 'tukui'}),
             (frozenset({Flavour.retail}), {'ui': 'elvui'}),
             *(
                 (frozenset({Flavour.from_flavour_keyed_enum(p)}), {p.value: ''})
                 for p in _TukuiFlavourQueryParam
             ),
```

### Comparing `instawow-2.1.1/src/instawow/_sources/wago.py` & `instawow-2.2.0/src/instawow/_sources/wago.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import iso8601
 from typing_extensions import TypedDict
 from yarl import URL
 
 from .. import models
 from .. import results as R
-from ..common import AddonHashMethod, ChangelogFormat, SourceMetadata, Strategy
+from ..common import AddonHashMethod, ChangelogFormat, Defn, SourceMetadata, Strategy
 from ..http import make_generic_progress_ctx
-from ..resolvers import BaseResolver, Defn, HeadersIntent, TFolderHashCandidate
+from ..resolvers import BaseResolver, HeadersIntent, TFolderHashCandidate
 from ..utils import StrEnum, as_plain_text_data_url, run_in_thread
 
 _WagoStability = Literal['stable', 'beta', 'alpha']
 
 
 class _WagoGameVersion(StrEnum):
     retail = 'retail'
```

### Comparing `instawow-2.1.1/src/instawow/_sources/wowi.py` & `instawow-2.2.0/src/instawow/_sources/wowi.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from typing import Literal
 
 from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypedDict
 from yarl import URL
 
-from .. import _deferred_types, manager, models
+from .. import manager, models
 from .. import results as R
 from ..cataloguer import BaseCatalogueEntry
-from ..common import ChangelogFormat, Flavour, FlavourVersionRange, SourceMetadata
-from ..http import make_generic_progress_ctx
-from ..resolvers import BaseResolver, Defn
+from ..common import ChangelogFormat, Defn, Flavour, FlavourVersionRange, SourceMetadata
+from ..http import ClientSessionType, make_generic_progress_ctx
+from ..resolvers import BaseResolver
 from ..utils import as_plain_text_data_url, gather, slugify, uniq
 
 
 class _WowiCommonTerms(TypedDict):
     UID: str  # Unique add-on ID
     UICATID: str  # ID of category add-on is placed in
     UIVersion: str  # Add-on version
@@ -171,17 +171,15 @@
             date_published=self._timestamp_to_datetime(metadata['UIDate']),
             version=metadata['UIVersion'],
             changelog_url=as_plain_text_data_url(metadata['UIChangeLog']),
             options=models.PkgOptions.from_strategy_values(defn.strategies),
         )
 
     @classmethod
-    async def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
-    ) -> AsyncIterator[BaseCatalogueEntry]:
+    async def catalogue(cls, web_client: ClientSessionType) -> AsyncIterator[BaseCatalogueEntry]:
         logger.debug(f'retrieving {cls._list_api_url}')
 
         async with web_client.get(cls._list_api_url, raise_for_status=True) as response:
             items: list[_WowiListApiItem] = await response.json()
 
         for item in items:
             if item['UICATID'] == '160':
```

### Comparing `instawow-2.1.1/src/instawow/_wa_templates/COPYING.WeakAuras-Companion` & `instawow-2.2.0/src/instawow/_wa_templates/COPYING.WeakAuras-Companion`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/src/instawow/_wa_templates/init.lua` & `instawow-2.2.0/src/instawow/_wa_templates/init.lua`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/src/instawow/cataloguer.py` & `instawow-2.2.0/src/instawow/cataloguer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections.abc import Set
 from datetime import datetime
 from functools import cached_property
 
 from attrs import asdict, frozen
 from cattrs import Converter
 from cattrs.preconf.json import configure_converter
 from typing_extensions import Self
@@ -13,16 +14,15 @@
 
 BASE_CATALOGUE_VERSION = 7
 CATALOGUE_VERSION = 4
 
 
 catalogue_converter = Converter(
     unstruct_collection_overrides={
-        # TODO: Replace with ``collections.abc.Set``
-        frozenset: sorted,
+        Set: sorted,
     }
 )
 configure_converter(catalogue_converter)
 
 
 @frozen(kw_only=True)
 class CatalogueSameAs:
```

### Comparing `instawow-2.1.1/src/instawow/cli.py` & `instawow-2.2.0/src/instawow/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 import asyncio
 import enum
-import sys
 import textwrap
-from collections.abc import Awaitable, Callable, Collection, Iterable, Sequence, Set
+from collections.abc import Awaitable, Callable, Collection, Iterable, Mapping, Sequence, Set
 from datetime import datetime, timezone
 from functools import cached_property, partial
 from itertools import chain, repeat
 from pathlib import Path
 from typing import Any, Literal, NoReturn, TypeVar, overload
 
 import click
+import click.types
 from attrs import asdict, evolve, fields, resolve_types
 from loguru import logger
+from typing_extensions import Self
 
-from . import __version__, _deferred_types, db, models
+from . import __version__, db, models
 from . import manager as _manager
 from . import results as R
-from .common import ChangelogFormat, Flavour, Strategy
+from .common import ChangelogFormat, Defn, Flavour, Strategy
 from .config import Config, GlobalConfig, config_converter, setup_logging
 from .http import TraceRequestCtx, init_web_client
 from .plugins import load_plugins
-from .resolvers import Defn
 from .utils import StrEnum, all_eq, gather, reveal_folder, tabulate, uniq
 
 _T = TypeVar('_T')
 _TStrEnum = TypeVar('_TStrEnum', bound=StrEnum)
 
 
 class Report:
@@ -64,61 +64,49 @@
             f'{textwrap.fill(r.message, initial_indent=" " * 2, subsequent_indent=" " * 4)}'
             for a, r in self.results
             if self.filter_fn(r)
         )
 
     def generate(self) -> None:
         mw: _CtxObjWrapper | None = click.get_current_context().obj
+
         if mw and mw.manager.config.global_config.auto_update_check:
+            from ._version import is_outdated
+
             outdated, new_version = mw.run_with_progress(
-                _manager.is_outdated(mw.manager.config.global_config)
+                is_outdated(mw.manager.config.global_config)
             )
             if outdated:
                 click.echo(f'{self.WARNING_SYMBOL} instawow v{new_version} is available')
 
         report = str(self)
         if report:
             click.echo(report)
 
     def generate_and_exit(self) -> NoReturn:
         self.generate()
         ctx = click.get_current_context()
         ctx.exit(self.exit_code)
 
 
-def _override_asyncio_loop_policy():
-    # The proactor event loop which became the default loop on Windows
-    # in Python 3.8 is causing issues with aiohttp.
-    # See https://github.com/aio-libs/aiohttp/issues/4324
-    if sys.platform == 'win32' and sys.version_info < (3, 11):
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-
-
-def _apply_patches():
-    _override_asyncio_loop_policy()
-
-
 class _CtxObjWrapper:
     def __init__(self, ctx: click.Context) -> None:
         self._ctx = ctx
 
     @cached_property
     def manager(self) -> _manager.Manager:
         global_config = GlobalConfig.read().ensure_dirs()
         try:
             config = Config.read(global_config, self._ctx.params['profile']).ensure_dirs()
         except FileNotFoundError:
             config = self._ctx.invoke(configure)
 
         setup_logging(config.logging_dir, *self._ctx.params['debug'])
 
-        manager, close_db_conn = _manager.Manager.from_config(config)
-        self._ctx.call_on_close(close_db_conn)
-
-        return manager
+        return _manager.Manager.from_config(config)
 
     def run_with_progress(self, awaitable: Awaitable[_T]) -> _T:
         cache_dir = self.manager.config.global_config.cache_dir
         params = self._ctx.params
 
         if any(params['debug']):
 
@@ -126,26 +114,26 @@
                 async with init_web_client(cache_dir, no_cache=params['no_cache']) as web_client:
                     _manager.contextualise(web_client=web_client)
                     return await awaitable
 
         else:
             from contextlib import contextmanager
 
-            from aiohttp import TraceConfig, hdrs
+            import aiohttp
             from prompt_toolkit.shortcuts import ProgressBar, ProgressBarCounter
 
             from ._cli_prompts import make_progress_bar
 
             def init_cli_web_client(progress_bar: ProgressBar, tickers: set[asyncio.Task[None]]):
                 TICK_INTERVAL = 0.1
 
                 async def do_on_request_end(
-                    client_session: _deferred_types.aiohttp.ClientSession,
+                    client_session: aiohttp.ClientSession,
                     trace_config_ctx: Any,
-                    params: _deferred_types.aiohttp.TraceRequestEndParams,
+                    params: aiohttp.TraceRequestEndParams,
                 ):
                     trace_request_ctx: TraceRequestCtx = trace_config_ctx.trace_request_ctx
                     if trace_request_ctx:
                         response = params.response
                         label = (
                             'Downloading '
                             + defn_to_urn(
@@ -159,15 +147,15 @@
                         # When the total is ``None`` the progress bar is
                         # in an "indeterminate" state.
                         # We cannot display progress for encoded responses because
                         # the size before decoding is not exposed by the
                         # aiohttp streaming API
                         total = (
                             None
-                            if hdrs.CONTENT_ENCODING in response.headers
+                            if aiohttp.hdrs.CONTENT_ENCODING in response.headers
                             else response.content_length
                         )
 
                         counters = progress_bar.counters
 
                         async def ticker():
                             counter = ProgressBarCounter[object](
@@ -180,15 +168,15 @@
                                     progress_bar.invalidate()
                                     await asyncio.sleep(TICK_INTERVAL)
                             finally:
                                 counters.remove(counter)
 
                         tickers.add(asyncio.create_task(ticker()))
 
-                trace_config = TraceConfig()
+                trace_config = aiohttp.TraceConfig()
                 trace_config.on_request_end.append(do_on_request_end)
                 trace_config.freeze()
                 return init_web_client(
                     cache_dir, no_cache=params['no_cache'], trace_configs=[trace_config]
                 )
 
             @contextmanager
@@ -213,15 +201,15 @@
 def _with_manager(fn: Callable[..., object]):
     def wrapper(ctx: click.Context, __: click.Parameter, value: object):
         return fn(ctx.obj.manager, value)
 
     return wrapper
 
 
-class _StrEnumParam(click.Choice):
+class _StrEnumChoiceParam(click.Choice):
     def __init__(
         self,
         choice_enum: type[_TStrEnum],
         case_sensitive: bool = True,
     ) -> None:
         super().__init__(
             choices=list(choice_enum),
@@ -230,14 +218,49 @@
         self.__choice_enum = choice_enum
 
     def convert(self, value: Any, param: click.Parameter | None, ctx: click.Context | None) -> Any:
         converted_value = super().convert(value, param, ctx)
         return self.__choice_enum(converted_value)
 
 
+class _ManyOptionalChoiceValueParam(click.types.CompositeParamType):
+    def __init__(
+        self,
+        choice_param: click.Choice,
+        *,
+        value_types: Mapping[str, click.types.ParamType] = {},
+    ) -> None:
+        super().__init__()
+        self.__choice_param = choice_param
+        self.__value_types = value_types
+
+    def __parse_value(self, value: tuple[str, ...]):
+        return (
+            (k, v, self.__choice_param, vc)
+            for r in value
+            for k, _, v in (r.partition('='),)
+            for vc in (self.__value_types.get(k),)
+        )
+
+    @property
+    def arity(self) -> int:
+        return -1
+
+    def convert(
+        self, value: tuple[str, ...], param: click.Parameter | None, ctx: click.Context | None
+    ) -> Any:
+        return {
+            kc.convert(k, param, ctx): vc.convert(v, param, ctx) if vc and v else (v or None)
+            for k, v, kc, vc in self.__parse_value(value)
+        }
+
+    def get_metavar(self, param: click.Parameter) -> str:
+        return f'{{{",".join(self.__choice_param.choices)}}}[=VALUE]'
+
+
 def _register_plugin_commands(group: click.Group):
     plugin_hook = load_plugins()
     additional_commands = (c for g in plugin_hook.instawow_add_commands() for c in g)
     for command in additional_commands:
         group.add_command(command)
     return group
 
@@ -250,15 +273,15 @@
     _: click.Context, __: click.Parameter, value: float
 ) -> tuple[bool, bool, bool]:
     return (value > 0, value > 1, value > 2)
 
 
 @_register_plugin_commands
 @click.group(context_settings={'help_option_names': ('-h', '--help')})
-@click.version_option(__version__, prog_name=__package__)
+@click.version_option(__version__, prog_name=__spec__.parent)
 @click.option(
     '--debug',
     '-d',
     count=True,
     help='Log incrementally more things.  Additive.',
     callback=_parse_debug_option,
 )
@@ -273,15 +296,14 @@
     '-p',
     default='__default__',
     help='Activate the specified profile.',
 )
 @click.pass_context
 def cli(ctx: click.Context, **__: object) -> None:
     "Add-on manager for World of Warcraft."
-    _apply_patches()
     ctx.obj = _CtxObjWrapper(ctx)
 
 
 main = logger.catch(reraise=True)(cli)
 
 
 @overload
@@ -331,15 +353,15 @@
 
 def _extend_strategies(strategy: Strategy, ctx: click.Context, __: click.Parameter, value: bool):
     strategies = ctx.params.setdefault('strategies', set())
     if value:
         strategies.add(strategy)
 
 
-@cli.command()
+@cli.command
 @click.argument(
     'addons', nargs=-1, expose_value=False, callback=_parse_into_defn_and_extend_addons
 )
 @click.option(
     '--version',
     expose_value=False,
     multiple=True,
@@ -382,15 +404,15 @@
             for a in addons
         ]
 
     results = mw.run_with_progress(mw.manager.install(addons, replace))
     Report(results.items()).generate_and_exit()
 
 
-@cli.command()
+@cli.command
 @click.argument('addons', nargs=-1, callback=_with_manager(_parse_into_defn))
 @click.pass_obj
 def update(mw: _CtxObjWrapper, addons: Sequence[Defn]) -> None:
     "Update installed add-ons."
     import sqlalchemy as sa
 
     def filter_results(result: R.ManagerResult):
@@ -399,39 +421,40 @@
         # provided that they are not pinned
         if addons or not isinstance(result, R.PkgUpToDate):
             return True
         else:
             return result.is_pinned
 
     def installed_pkgs_to_defns():
-        return [
-            models.Pkg.from_row_mapping(mw.manager.database, p).to_defn()
-            for p in mw.manager.database.execute(sa.select(db.pkg)).mappings().all()
-        ]
+        with mw.manager.database.connect() as connection:
+            return [
+                models.Pkg.from_row_mapping(connection, p).to_defn()
+                for p in connection.execute(sa.select(db.pkg)).mappings().all()
+            ]
 
     results = mw.run_with_progress(mw.manager.update(addons or installed_pkgs_to_defns(), False))
     Report(results.items(), filter_results).generate_and_exit()
 
 
-@cli.command()
+@cli.command
 @click.argument('addons', nargs=-1, required=True, callback=_with_manager(_parse_into_defn))
 @click.option(
     '--keep-folders',
     is_flag=True,
     default=False,
-    help="Do not delete the add-on folders.",
+    help='Do not delete the add-on folders.',
 )
 @click.pass_obj
 def remove(mw: _CtxObjWrapper, addons: Sequence[Defn], keep_folders: bool) -> None:
     "Remove add-ons."
     results = mw.run_with_progress(mw.manager.remove(addons, keep_folders))
     Report(results.items()).generate_and_exit()
 
 
-@cli.command()
+@cli.command
 @click.argument('addon', callback=_with_manager(_parse_into_defn))
 @click.option(
     '--version',
     help='Version to roll back to.',
 )
 @click.option(
     '--undo',
@@ -478,15 +501,15 @@
     Report(
         mw.run_with_progress(
             mw.manager.update([reconstructed_defn.with_version(selection)], True)
         ).items()
     ).generate_and_exit()
 
 
-@cli.command()
+@cli.command
 @click.option('--auto', '-a', is_flag=True, default=False, help='Do not ask for user input.')
 @click.option(
     '--installed',
     'rereconcile',
     is_flag=True,
     default=False,
     help='Re-reconcile installed add-ons.',
@@ -494,22 +517,15 @@
 @click.option(
     '--list-unreconciled', is_flag=True, default=False, help='List unreconciled add-ons and exit.'
 )
 @click.pass_obj
 def reconcile(mw: _CtxObjWrapper, auto: bool, rereconcile: bool, list_unreconciled: bool) -> None:
     "Reconcile pre-installed add-ons."
     from ._cli_prompts import PkgChoice, ask, confirm, select, skip
-    from .matchers import (
-        AddonFolder,
-        get_unreconciled_folders,
-        match_addon_names_with_folder_names,
-        match_folder_hashes,
-        match_folder_name_subsets,
-        match_toc_source_ids,
-    )
+    from .matchers import DEFAULT_MATCHERS, AddonFolder, get_unreconciled_folders
 
     def construct_choice(pkg: models.Pkg, highlight_version: bool, disabled: bool):
         defn = pkg.to_defn()
         return PkgChoice(
             [
                 ('', f'{defn_to_urn(defn)}=='),
                 ('class:highlight-sub' if highlight_version else '', pkg.version),
@@ -544,22 +560,24 @@
                 construct_choice(installed_pkg, highlight_version, True),
                 *(construct_choice(p, highlight_version, False) for p in pkgs),
                 skip,
             ]
             selection = ask(select(installed_pkg.name, choices))
             return selection or None
 
-        installed_pkgs = [
-            models.Pkg.from_row_mapping(mw.manager.database, p)
-            for p in mw.manager.database.execute(
-                sa.select(db.pkg).order_by(sa.func.lower(db.pkg.c.name))
-            )
-            .mappings()
-            .all()
-        ]
+        with mw.manager.database.connect() as connection:
+            installed_pkgs = [
+                models.Pkg.from_row_mapping(connection, p)
+                for p in connection.execute(
+                    sa.select(db.pkg).order_by(sa.func.lower(db.pkg.c.name))
+                )
+                .mappings()
+                .all()
+            ]
+
         groups = mw.run_with_progress(mw.manager.find_equivalent_pkg_defns(installed_pkgs))
         selections = [
             (p, s)
             for (p, _), s in zip(
                 groups.items(), gather_selections(groups.items(), select_alternative_pkg)
             )
             if s
@@ -625,21 +643,15 @@
             return pkgs[0].to_defn()
 
         select_pkg_ = pick_first_pkg if auto else select_pkg
         confirm_install = (
             (lambda: True) if auto else (lambda: ask(confirm('Install selected add-ons?')))
         )
 
-        # Match in order of increasing heuristicitivenessitude
-        for fn in [
-            match_toc_source_ids,
-            match_folder_name_subsets,
-            match_folder_hashes,
-            match_addon_names_with_folder_names,
-        ]:
+        for fn in DEFAULT_MATCHERS.values():
             groups = mw.run_with_progress(fn(mw.manager, leftovers))
             selections = [s for s in gather_selections(groups, select_pkg_) if s is not None]
             if selections and confirm_install():
                 results = mw.run_with_progress(mw.manager.install(selections, True))
                 Report(results.items()).generate()
 
             leftovers = get_unreconciled_folders(mw.manager)
@@ -657,15 +669,15 @@
 
 
 def _parse_iso_date_into_datetime(_: click.Context, __: click.Parameter, value: str | None):
     if value is not None:
         return datetime.strptime(value, '%Y-%m-%d').replace(tzinfo=timezone.utc)
 
 
-@cli.command()
+@cli.command
 @click.argument('search-terms', nargs=-1, required=True, callback=_concat_search_terms)
 @click.option(
     '--limit',
     '-l',
     default=10,
     type=click.IntRange(1, 20, clamp=True),
     help='A number to limit results to.',
@@ -723,116 +735,125 @@
 @click.argument(
     'addons', nargs=-1, callback=_with_manager(partial(_parse_into_defn, raise_invalid=False))
 )
 @click.option(
     '--format',
     '-f',
     'output_format',
-    type=_StrEnumParam(_ListFormat),
+    type=_StrEnumChoiceParam(_ListFormat),
     default=_ListFormat.simple,
     show_default=True,
     help='Change the output format.',
 )
 @click.pass_obj
 def list_installed(mw: _CtxObjWrapper, addons: Sequence[Defn], output_format: _ListFormat) -> None:
     "List installed add-ons."
     import sqlalchemy as sa
 
-    def format_deps(pkg: models.Pkg):
-        return (
-            defn_to_urn(Defn(pkg.source, s or e.id))
-            for e in pkg.deps
-            for s in (
-                mw.manager.database.execute(
-                    sa.select(db.pkg.c.slug).filter_by(source=pkg.source, id=e.id)
-                ).scalar_one_or_none(),
+    with mw.manager.database.connect() as connection:
+
+        def format_deps(pkg: models.Pkg):
+            return (
+                defn_to_urn(Defn(pkg.source, s or e.id))
+                for e in pkg.deps
+                for s in (
+                    connection.execute(
+                        sa.select(db.pkg.c.slug).filter_by(source=pkg.source, id=e.id)
+                    ).scalar_one_or_none(),
+                )
             )
-        )
 
-    def row_mappings_to_pkgs():
-        return map(models.Pkg.from_row_mapping, repeat(mw.manager.database), pkg_mappings)
+        def row_mappings_to_pkgs():
+            return map(models.Pkg.from_row_mapping, repeat(connection), pkg_mappings)
 
-    pkg_mappings = (
-        mw.manager.database.execute(
-            sa.select(db.pkg)
-            .filter(
-                sa.or_(
-                    *(
-                        db.pkg.c.slug.contains(d.alias)
-                        if d.source == '*'
-                        else (db.pkg.c.source == d.source)
-                        & ((db.pkg.c.id == d.alias) | (db.pkg.c.slug == d.alias))
-                        for d in addons
+        pkg_mappings = (
+            connection.execute(
+                (
+                    sa.select(db.pkg).filter(
+                        sa.or_(
+                            *(
+                                db.pkg.c.slug.contains(d.alias)
+                                if d.source == '*'
+                                else (db.pkg.c.source == d.source)
+                                & ((db.pkg.c.id == d.alias) | (db.pkg.c.slug == d.alias))
+                                for d in addons
+                            )
+                        )
                     )
-                )
-                if addons
-                else True
+                    if addons
+                    else sa.select(db.pkg)
+                ).order_by(db.pkg.c.source, sa.func.lower(db.pkg.c.name))
             )
-            .order_by(db.pkg.c.source, sa.func.lower(db.pkg.c.name))
+            .mappings()
+            .all()
         )
-        .mappings()
-        .all()
-    )
 
-    if output_format is _ListFormat.json:
-        import json
-
-        click.echo(
-            json.dumps(
-                models.pkg_converter.unstructure(row_mappings_to_pkgs(), list[models.Pkg]),
-                indent=2,
+        if output_format is _ListFormat.json:
+            from cattrs.preconf.json import (
+                make_converter,  # pyright: ignore[reportUnknownVariableType]
             )
-        )
 
-    elif output_format is _ListFormat.detailed:
-        formatter = click.HelpFormatter(max_width=99)
-        for pkg in row_mappings_to_pkgs():
-            with formatter.section(defn_to_urn(pkg.to_defn())):
-                formatter.write_dl(
-                    [
-                        ('name', pkg.name),
-                        ('description', textwrap.shorten(pkg.description, 280)),
-                        ('url', pkg.url),
-                        ('version', pkg.version),
-                        ('date_published', pkg.date_published.isoformat(' ', 'minutes')[:-6]),
-                        ('folders', ', '.join(f.name for f in pkg.folders)),
-                        ('deps', ', '.join(format_deps(pkg))),
-                        ('options', '\n'.join(f'{s}={v}' for s, v in asdict(pkg.options).items())),
-                    ]
+            json_converter = make_converter()
+            click.echo(
+                json_converter.dumps(  # pyright: ignore[reportUnknownMemberType]
+                    row_mappings_to_pkgs(),
+                    list[models.Pkg],
+                    indent=2,
                 )
-        click.echo(formatter.getvalue(), nl=False)
+            )
 
-    else:
-        click.echo(
-            ''.join(f'{defn_to_urn(Defn(p["source"], p["slug"]))}\n' for p in pkg_mappings),
-            nl=False,
-        )
+        elif output_format is _ListFormat.detailed:
+            formatter = click.HelpFormatter(max_width=99)
+            for pkg in row_mappings_to_pkgs():
+                with formatter.section(defn_to_urn(pkg.to_defn())):
+                    formatter.write_dl(
+                        [
+                            ('name', pkg.name),
+                            ('description', textwrap.shorten(pkg.description, 280)),
+                            ('url', pkg.url),
+                            ('version', pkg.version),
+                            ('date_published', pkg.date_published.isoformat(' ', 'minutes')[:-6]),
+                            ('folders', ', '.join(f.name for f in pkg.folders)),
+                            ('deps', ', '.join(format_deps(pkg))),
+                            (
+                                'options',
+                                '\n'.join(f'{s}={v}' for s, v in asdict(pkg.options).items()),
+                            ),
+                        ]
+                    )
+            click.echo(formatter.getvalue(), nl=False)
+
+        else:
+            click.echo(
+                ''.join(f'{defn_to_urn(Defn(p["source"], p["slug"]))}\n' for p in pkg_mappings),
+                nl=False,
+            )
 
 
 @cli.command(hidden=True)
 @click.argument('addon', callback=_with_manager(partial(_parse_into_defn, raise_invalid=False)))
 @click.pass_context
 def info(ctx: click.Context, addon: Defn) -> None:
     "Alias of `list -f detailed`."
     ctx.invoke(list_installed, addons=(addon,), output_format=_ListFormat.detailed)
 
 
-@cli.command()
+@cli.command
 @click.argument('addon', callback=_with_manager(partial(_parse_into_defn, raise_invalid=False)))
 @click.pass_obj
 def reveal(mw: _CtxObjWrapper, addon: Defn) -> None:
     "Bring an add-on up in your file manager."
     pkg = mw.manager.get_pkg(addon, partial_match=True)
     if pkg:
         reveal_folder(mw.manager.config.addon_dir / pkg.folders[0].name)
     else:
         Report([(addon, R.PkgNotInstalled())]).generate_and_exit()
 
 
-@cli.command()
+@cli.command
 @click.argument(
     'addon', callback=_with_manager(partial(_parse_into_defn, raise_invalid=False)), required=False
 )
 @click.option(
     '--convert/--no-convert',
     default=True,
     show_default=True,
@@ -894,41 +915,45 @@
             click.echo_via_pager(changelog)
         else:
             Report([(addon, R.PkgNotInstalled())]).generate_and_exit()
 
     else:
         import sqlalchemy as sa
 
-        join_clause = (db.pkg.c.source == db.pkg_version_log.c.pkg_source) & (
-            db.pkg.c.id == db.pkg_version_log.c.pkg_id
-        )
-
-        last_installed_changelog_urls = mw.manager.database.execute(
-            sa.select(db.pkg.c.source, db.pkg.c.slug, db.pkg.c.changelog_url)
-            .join(db.pkg_version_log, join_clause)
-            .filter(
-                db.pkg_version_log.c.install_time
-                >= sa.select(
-                    sa.func.datetime(sa.func.max(db.pkg_version_log.c.install_time), '-1 minute')
-                )
-                .join(db.pkg, join_clause)
-                .scalar_subquery()
+        with mw.manager.database.connect() as connection:
+            join_clause = (db.pkg.c.source == db.pkg_version_log.c.pkg_source) & (
+                db.pkg.c.id == db.pkg_version_log.c.pkg_id
             )
-        ).all()
+            last_installed_changelog_urls = connection.execute(
+                sa.select(db.pkg.c.source, db.pkg.c.slug, db.pkg.c.changelog_url)
+                .join(db.pkg_version_log, join_clause)
+                .filter(
+                    db.pkg_version_log.c.install_time
+                    >= sa.select(
+                        sa.func.datetime(
+                            sa.func.max(db.pkg_version_log.c.install_time), '-1 minute'
+                        )
+                    )
+                    .join(db.pkg, join_clause)
+                    .scalar_subquery()
+                )
+            ).all()
+
         changelogs = mw.run_with_progress(
             gather(
                 mw.manager.get_changelog(m.source, m.changelog_url)
                 for m in last_installed_changelog_urls
             )
         )
         if convert:
             do_convert = make_converter()
             changelogs = (
                 do_convert(m.source, c) for m, c in zip(last_installed_changelog_urls, changelogs)
             )
+
         click.echo_via_pager(
             '\n\n'.join(
                 format_combined_changelog_entry(m.source, m.slug, c)
                 for m, c in zip(last_installed_changelog_urls, changelogs)
             )
         )
 
@@ -950,134 +975,165 @@
         access_token = await poll_for_access_token(
             web_client, codes['device_code'], codes['interval']
         )
         return access_token
 
 
 class _EditableConfigOptions(StrEnum):
-    addon_dir = 'addon_dir'
-    game_flavour = 'game_flavour'
-    auto_update_check = 'auto_update_check'
-    github_access_token = 'access_tokens.github'
-    cfcore_access_token = 'access_tokens.cfcore'
-    wago_access_token = 'access_tokens.wago'
+    AddonDir = 'addon_dir'
+    GameFlavour = 'game_flavour'
+    AutoUpdateCheck = 'global_config.auto_update_check'
+    GithubAccessToken = 'global_config.access_tokens.github'
+    CfcoreAccessToken = 'global_config.access_tokens.cfcore'
+    WagoAddonsAccessToken = 'global_config.access_tokens.wago_addons'
+
+    path: tuple[str, ...]
+
+    def __new__(cls, value: str) -> Self:
+        self = str.__new__(cls, value)
+        self.path = tuple(value.split('.'))
+        return self
 
 
-@cli.command()
+@cli.command
 @click.option(
     '--show-active',
     is_flag=True,
     default=False,
     expose_value=False,
     is_eager=True,
     callback=_show_active_config,
     help='Show the active configuration and exit.',
 )
 @click.argument(
-    'config-options',
+    'editable-config-values',
     nargs=-1,
-    type=_StrEnumParam(_EditableConfigOptions),
+    type=_ManyOptionalChoiceValueParam(
+        _StrEnumChoiceParam(_EditableConfigOptions),
+        value_types={
+            _EditableConfigOptions.AutoUpdateCheck: click.types.BoolParamType(),
+        },
+    ),
 )
 @click.pass_context
 def configure(
     ctx: click.Context,
-    config_options: Collection[_EditableConfigOptions],
+    editable_config_values: Mapping[_EditableConfigOptions, Any],
 ) -> Config:
-    "Configure instawow."
-    from ._cli_prompts import AttrFieldValidator, ask, confirm, password, path, select
+    """Configure instawow.
+
+    You can pass configuration keys as arguments to reconfigure an existing
+    profile.  Pass a value to bypass the interactive prompt.  For example:
+
+    \b
+    * ``configure addon_dir`` will initiate an interactive session
+      with autocompletion
+    * ``configure "addon_dir=~/foo"` will set ``addon_dir``'s value
+      to ``~/foo`` directly
+    """
+    from ._cli_prompts import AttrsFieldValidator, ask, confirm, password, path, select
     from .common import infer_flavour_from_path
 
     profile = ctx.find_root().params['profile']
 
-    orig_global_config = GlobalConfig.read()
-
-    if not config_options:
-        config_options = {
-            _EditableConfigOptions.addon_dir,
-            _EditableConfigOptions.game_flavour,
-        }
-        if orig_global_config.access_tokens.github is None:
-            config_options.add(_EditableConfigOptions.github_access_token)
+    existing_global_config = GlobalConfig.read()
 
-    global_config_values = asdict(orig_global_config)
+    config_values: dict[str, Any] | None = None
     try:
-        profile_config_values = asdict(Config.read(orig_global_config, profile))
-        del profile_config_values['global_config']
+        config_values = asdict(Config.read(existing_global_config, profile))
+    except FileNotFoundError:
+        pass
     except Exception:
-        profile_config_values = {
-            'profile': profile,
+        logger.exception('unable to read existing config')
+
+    if config_values is None:
+        config_values = {'profile': profile, 'global_config': asdict(existing_global_config)}
+
+    editable_config_values = dict(editable_config_values)
+    if not editable_config_values:
+        default_keys = {
+            _EditableConfigOptions.AddonDir,
+            _EditableConfigOptions.GameFlavour,
         }
+        if existing_global_config.access_tokens.github is None:
+            default_keys.add(_EditableConfigOptions.GithubAccessToken)
+
+        editable_config_values = dict.fromkeys(default_keys)
 
-    addon_dir = None
-    if _EditableConfigOptions.addon_dir in config_options:
-        addon_dir = ask(
+    interactive_editable_config_keys = {k for k, v in editable_config_values.items() if v is None}
+
+    if _EditableConfigOptions.AddonDir in interactive_editable_config_keys:
+        editable_config_values[_EditableConfigOptions.AddonDir] = ask(
             path(
                 'Add-on directory:',
                 only_directories=True,
-                validate=AttrFieldValidator(
-                    fields(resolve_types(Config)).addon_dir,  # pyright: ignore
+                validate=AttrsFieldValidator(
+                    fields(resolve_types(Config)).addon_dir,
                     config_converter,
                 ),
             )
         )
-        profile_config_values['addon_dir'] = addon_dir
 
-    if _EditableConfigOptions.game_flavour in config_options:
-        game_flavour = ask(
+    if _EditableConfigOptions.GameFlavour in interactive_editable_config_keys:
+        editable_config_values[_EditableConfigOptions.GameFlavour] = ask(
             select(
                 'Game flavour:',
                 choices=list(Flavour),
-                initial_choice=infer_flavour_from_path(addon_dir)
-                if addon_dir is not None
-                else None,
+                initial_choice=config_values.get('addon_dir')
+                and infer_flavour_from_path(config_values['addon_dir']),
             )
         )
-        profile_config_values['game_flavour'] = game_flavour
 
-    if _EditableConfigOptions.auto_update_check in config_options:
-        global_config_values['auto_update_check'] = ask(
+    if _EditableConfigOptions.AutoUpdateCheck in interactive_editable_config_keys:
+        editable_config_values[_EditableConfigOptions.AutoUpdateCheck] = ask(
             confirm('Periodically check for instawow updates?')
         )
 
-    if _EditableConfigOptions.github_access_token in config_options and ask(
+    if _EditableConfigOptions.GithubAccessToken in interactive_editable_config_keys and ask(
         confirm('Set up GitHub authentication?')
     ):
-        github_access_token = asyncio.run(_github_oauth_flow())
-        global_config_values['access_tokens']['github'] = github_access_token
+        editable_config_values[_EditableConfigOptions.GithubAccessToken] = asyncio.run(
+            _github_oauth_flow()
+        )
 
-    if _EditableConfigOptions.cfcore_access_token in config_options:
+    if _EditableConfigOptions.CfcoreAccessToken in interactive_editable_config_keys:
         click.echo(
             textwrap.fill(
                 'An access token is required to use CurseForge. '
                 'Log in to https://console.curseforge.com/ to generate an access token.'
             )
         )
-        global_config_values['access_tokens']['cfcore'] = ask(
-            password('CFCore access token:', validate=bool)
+        editable_config_values[_EditableConfigOptions.CfcoreAccessToken] = (
+            ask(password('CFCore access token:')) or None
         )
 
-    if _EditableConfigOptions.wago_access_token in config_options:
+    if _EditableConfigOptions.WagoAddonsAccessToken in interactive_editable_config_keys:
         click.echo(
             textwrap.fill(
                 'An access token is required to use Wago Addons. '
                 'Wago issues tokens to Patreon subscribers above a certain tier. '
                 'See https://addons.wago.io/patreon for more information.'
             )
         )
-        global_config_values['access_tokens']['wago_addons'] = ask(
-            password('Wago Addons access token:', validate=bool)
+        editable_config_values[_EditableConfigOptions.WagoAddonsAccessToken] = (
+            ask(password('Wago Addons access token:')) or None
         )
 
-    global_config = config_converter.structure(global_config_values, GlobalConfig).write()
-    config = config_converter.structure(
-        {**profile_config_values, 'global_config': global_config}, Config
-    ).write()
+    for key, value in editable_config_values.items():
+        parent = config_values
+        for part in key.path[:-1]:
+            parent = parent[part]
+        parent[key.path[-1]] = value
+
+    config = config_converter.structure(config_values, Config)
+    config.global_config.write()
+    config.write()
 
     click.echo('Configuration written to:')
-    click.echo(f'  {global_config.config_file}')
+    click.echo(f'  {config.global_config.config_file}')
     click.echo(f'  {config.config_file}')
 
     return config
 
 
 @cli.group('weakauras-companion')
 def _weakauras_group() -> None:
@@ -1097,21 +1153,21 @@
 @click.pass_obj
 def list_installed_wago_auras(mw: _CtxObjWrapper) -> None:
     "List WeakAuras installed from Wago."
     from .wa_updater import WaCompanionBuilder
 
     aura_groups = WaCompanionBuilder(mw.manager).extract_installed_auras()
     installed_auras = sorted(
-        (g.addon_name, textwrap.fill(a.id, width=30, max_lines=1), a.url)
+        (g.addon_name, a.id, a.url)
         for g in aura_groups
         for v in g.root.values()
         for a in v
         if not a.parent
     )
-    click.echo(tabulate([('in file', 'name', 'URL'), *installed_auras]))
+    click.echo(tabulate([('type', 'name', 'URL'), *installed_auras]))
 
 
 @cli.command(hidden=True)
 @click.option(
     '--start-date',
     callback=_parse_iso_date_into_datetime,
     help='Omit results before this date.',
@@ -1132,22 +1188,24 @@
     )
     catalogue_path.with_suffix(f'.compact{catalogue_path.suffix}').write_text(
         json.dumps(catalogue_json, separators=(',', ':')),
         encoding='utf-8',
     )
 
 
-@cli.command()
+@cli.command
 @click.pass_context
 def gui(ctx: click.Context) -> None:
     "Fire up the GUI."
     from instawow_gui.app import InstawowApp
 
     global_config = GlobalConfig.read().ensure_dirs()
     dummy_jsonrpc_config = Config.make_dummy_config(
         global_config=global_config, profile='__jsonrpc__'
     ).ensure_dirs()
 
     params = ctx.find_root().params
     setup_logging(dummy_jsonrpc_config.logging_dir, *params['debug'])
 
-    InstawowApp(version=__version__).main_loop()  # pyright: ignore[reportUnknownMemberType]
+    InstawowApp(
+        debug=any(params['debug']), version=__version__
+    ).main_loop()  # pyright: ignore[reportUnknownMemberType]
```

### Comparing `instawow-2.1.1/src/instawow/common.py` & `instawow-2.2.0/src/instawow/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import os
 import typing
 from pathlib import PurePath
 from typing import Literal, Protocol, TypeVar
 
-from attrs import asdict, frozen
+from attrs import asdict, evolve, frozen
 from typing_extensions import Self
 
 from .utils import StrEnum, fill
 
 _TEnum = TypeVar('_TEnum', bound=enum.Enum)
 
 
@@ -79,25 +79,14 @@
 
 class Strategy(StrEnum):
     any_flavour = enum.auto()
     any_release_type = enum.auto()
     version_eq = enum.auto()
 
 
-@frozen
-class StrategyValues:
-    any_flavour: Literal[True, None] = None
-    any_release_type: Literal[True, None] = None
-    version_eq: typing.Union[str, None] = None
-
-    @property
-    def filled_strategies(self) -> frozenset[Strategy]:
-        return frozenset(Strategy(p) for p, v in asdict(self).items() if v is not None)
-
-
 class ChangelogFormat(StrEnum):
     html = enum.auto()
     markdown = enum.auto()
     raw = enum.auto()
 
 
 @frozen
@@ -105,9 +94,31 @@
     id: str
     name: str
     strategies: frozenset[Strategy]
     changelog_format: ChangelogFormat
     addon_toc_key: str | None
 
 
+@frozen
+class StrategyValues:
+    any_flavour: Literal[True, None] = None
+    any_release_type: Literal[True, None] = None
+    version_eq: typing.Union[str, None] = None
+
+    @property
+    def filled_strategies(self) -> frozenset[Strategy]:
+        return frozenset(Strategy(p) for p, v in asdict(self).items() if v is not None)
+
+
+@frozen(hash=True)
+class Defn:
+    source: str
+    alias: str
+    id: typing.Union[str, None] = None
+    strategies: StrategyValues = StrategyValues()
+
+    def with_version(self, version: str) -> Self:
+        return evolve(self, strategies=evolve(self.strategies, version_eq=version))
+
+
 class AddonHashMethod(enum.Enum):
     wowup = enum.auto()
```

### Comparing `instawow-2.1.1/src/instawow/config.py` & `instawow-2.2.0/src/instawow/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,25 @@
 from cattrs import Converter
 from cattrs.gen import make_dict_unstructure_fn, override
 from cattrs.preconf.json import configure_converter
 from loguru import logger
 from typing_extensions import Self
 
 from .common import Flavour
-from .utils import trash
+from .utils import add_exc_note, trash
 
 _T = TypeVar('_T')
 
 _MISSING = object()
 
 
 class SecretStr(str):
     pass
 
 
-def _convert_secret_string(value: str):
-    return '**********' if value else ''
-
-
 def _expand_path(value: Path):
     return Path(os.path.abspath(os.path.expanduser(value)))
 
 
 def _is_writable_dir(value: Path):
     return value.is_dir() and os.access(value, os.W_OK)
 
@@ -49,17 +45,16 @@
 
 def _enrich_validator_exc(validator: Callable[[object, Attribute[_T], _T], None]):
     def wrapper(model: object, attr: Attribute[_T], value: _T):
         try:
             validator(model, attr, value)
         except BaseException as exc:
             note = f'Structuring class {model.__class__.__name__} @ attribute {attr.name}'
-            notes = [*getattr(exc, '__notes__', []), note]
-            exc.__notes__ = notes  # pyright: ignore
-            raise exc
+            add_exc_note(exc, note)
+            raise
 
     return wrapper
 
 
 @_enrich_validator_exc
 def _validate_path_is_writable_dir(_model: object, _attr: Attribute[Path], value: Path):
     if not _is_writable_dir(value):
@@ -128,16 +123,25 @@
     converter.register_structure_hook(Path, lambda v, _: Path(v))
     converter.register_unstructure_hook(Path, str)
     return converter
 
 
 @lru_cache(1)
 def _make_display_converter():
+    def convert_secret_string(value: str):
+        return '**********'
+
+    def convert_global_config(global_config: GlobalConfig):
+        return converter.unstructure_attrs_asdict(global_config) | {
+            'profiles': global_config.list_profiles()
+        }
+
     converter = make_config_converter()
-    converter.register_unstructure_hook(SecretStr, _convert_secret_string)
+    converter.register_unstructure_hook(GlobalConfig, convert_global_config)
+    converter.register_unstructure_hook(SecretStr, convert_secret_string)
     return converter
 
 
 @lru_cache(2)
 def _make_write_converter(config_cls: Any, fields_to_include: frozenset[str]):
     converter = make_config_converter()
     converter.register_unstructure_hook(
@@ -203,15 +207,15 @@
     def read(cls) -> Self:
         env_only_config = cls.from_env()
         config_values = _read_config(env_only_config.config_file, missing_ok=True)
         return cls.from_env(**config_values) if config_values else env_only_config
 
     def list_profiles(self) -> list[str]:
         "Get the names of the profiles contained in ``config_dir``."
-        profiles = [c.parent.name for c in self.config_dir.glob('profiles/*/config.json')]
+        profiles = [c.parent.name for c in self.profiles_dir.glob('*/config.json')]
         return profiles
 
     def ensure_dirs(self) -> Self:
         _ensure_dirs(
             [
                 self.config_dir,
                 self.temp_dir,
@@ -226,14 +230,22 @@
         return self
 
     @property
     def cache_dir(self) -> Path:
         return self.temp_dir / 'cache'
 
     @property
+    def logging_dir(self) -> Path:
+        return self.config_dir / 'logs'
+
+    @property
+    def profiles_dir(self) -> Path:
+        return self.config_dir / 'profiles'
+
+    @property
     def config_file(self) -> Path:
         return self.config_dir / 'config.json'
 
 
 @frozen
 class Config:
     global_config: GlobalConfig
@@ -283,15 +295,15 @@
         return self
 
     def delete(self) -> None:
         trash((self.profile_dir,), dest=self.global_config.temp_dir, missing_ok=True)
 
     @property
     def profile_dir(self) -> Path:
-        return self.global_config.config_dir / 'profiles' / self.profile
+        return self.global_config.profiles_dir / self.profile
 
     @property
     def logging_dir(self) -> Path:
         return self.profile_dir / 'logs'
 
     @property
     def plugin_dir(self) -> Path:
@@ -339,46 +351,46 @@
         SimpleQueue=queue.Queue, Event=threading.Event, Lock=threading.Lock
     )
 
 
 def _intercept_logging_module_calls(log_level: str):  # pragma: no cover
     import logging
 
-    class InterceptHandler(logging.Handler):
-        logging_filename = getattr(logging, '__file__', None)
+    logging_filename = getattr(logging, '__file__', None)
 
+    class InterceptHandler(logging.Handler):
         def emit(self, record: logging.LogRecord) -> None:
             # Get the corresponding Loguru level if it exists
             try:
                 level = logger.level(record.levelname).name
             except ValueError:
                 level = record.levelno
 
             # Find caller from where the logged message originated
-            frame = logging.currentframe()
-            depth = 2
-            while frame and frame.f_code.co_filename == self.logging_filename:
+            depth = 6
+            frame = sys._getframe(depth)  # pyright: ignore[reportPrivateUsage]
+            while frame and frame.f_code.co_filename == logging_filename:
                 frame = frame.f_back
                 depth += 1
 
             logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
-    logging.basicConfig(handlers=[InterceptHandler()], level=log_level)
+    logging.basicConfig(handlers=[InterceptHandler()], level=log_level, force=True)
 
 
 def setup_logging(
     logging_dir: Path, log_to_stderr: bool, debug: bool, intercept_logging_module_calls: bool
 ) -> None:
+    _patch_loguru_enqueue()
+
     log_level = 'DEBUG' if debug else 'INFO'
 
     if intercept_logging_module_calls:
         _intercept_logging_module_calls(log_level)
 
-    _patch_loguru_enqueue()
-
     values = {
         'level': log_level,
         'enqueue': True,
     }
     logger.configure(
         handlers=[
             {
```

### Comparing `instawow-2.1.1/src/instawow/db.py` & `instawow-2.2.0/src/instawow/db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import sqlite3
-from contextlib import contextmanager
 from datetime import datetime, timezone
 from enum import IntEnum
 
 from sqlalchemy import (
     Boolean,
     Column,
     DateTime,
+    Engine,
     ForeignKeyConstraint,
     MetaData,
     String,
     Table,
     TypeDecorator,
     create_engine,
     func,
     text,
 )
 from sqlalchemy.event import listen
 from sqlalchemy.exc import OperationalError
-from sqlalchemy.future import Connection, Engine
 
 
 class TZDateTime(TypeDecorator[datetime]):
     impl = DateTime
     cache_ok = True
 
     def process_bind_param(self, value: datetime | None, dialect: object) -> datetime | None:
@@ -145,42 +144,27 @@
     dbapi_connection.execute('PRAGMA foreign_keys = ON')
 
 
 def prepare_database(uri: str, revision: str) -> Engine:
     "Connect to and optionally create or migrate the database from a configuration object."
     engine = create_engine(
         uri,
-        # We wanna be able to operate on the database from executor threads
-        # when performing disk I/O
-        connect_args={'check_same_thread': False},
         # echo=True,
-        future=True,
     )
     listen(engine, 'connect', _set_sqlite_pragma)
 
     database_state = _get_database_state(engine, revision)
     if database_state is not _DatabaseState.current:
         import alembic.command
         import alembic.config
 
         alembic_config = alembic.config.Config()
-        alembic_config.set_main_option('script_location', f'{__package__}:_migrations')
+        alembic_config.set_main_option('script_location', f'{__spec__.parent}:_migrations')
         alembic_config.set_main_option('sqlalchemy.url', str(engine.url))
 
         if database_state is _DatabaseState.uninitialised:
             metadata.create_all(engine)
             alembic.command.stamp(alembic_config, revision)
         else:
             alembic.command.upgrade(alembic_config, revision)
 
     return engine
-
-
-@contextmanager
-def faux_transact(connection: Connection):
-    try:
-        yield
-    except BaseException:
-        connection.rollback()
-        raise
-    else:
-        connection.commit()
```

### Comparing `instawow-2.1.1/src/instawow/github_auth.py` & `instawow-2.2.0/src/instawow/github_auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 
 from typing_extensions import TypedDict
 
-from . import _deferred_types
+from . import http
 
 CLIENT_ID = 'aa178904bdf5143e93ec'
 
 
 class DeviceCodeResponse(TypedDict):
     device_code: str
     user_code: str
@@ -19,26 +19,26 @@
 
 class AccessTokenResponse(TypedDict):
     access_token: str
     token_type: str
     scope: str
 
 
-async def get_codes(web_client: _deferred_types.aiohttp.ClientSession) -> DeviceCodeResponse:
+async def get_codes(web_client: http.ClientSessionType) -> DeviceCodeResponse:
     async with web_client.post(
         'https://github.com/login/device/code',
         headers={'Accept': 'application/json'},
         json={'client_id': CLIENT_ID},
         raise_for_status=True,
     ) as response:
         return await response.json()
 
 
 async def poll_for_access_token(
-    web_client: _deferred_types.aiohttp.ClientSession, device_code: str, polling_interval: int = 5
+    web_client: http.ClientSessionType, device_code: str, polling_interval: int = 5
 ) -> str:
     while True:
         async with web_client.post(
             'https://github.com/login/oauth/access_token',
             headers={'Accept': 'application/json'},
             json={
                 'client_id': CLIENT_ID,
```

### Comparing `instawow-2.1.1/src/instawow/http.py` & `instawow-2.2.0/src/instawow/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from __future__ import annotations
 
 from collections.abc import AsyncIterator
 from contextlib import asynccontextmanager
 from functools import lru_cache, partial
 from pathlib import Path
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Literal
 
 from loguru import logger
 from typing_extensions import TypeAlias, TypedDict
 
-from . import _deferred_types
+from . import models
 from .utils import read_resource_as_text
 
+if TYPE_CHECKING:
+    import aiohttp
+
+    ClientSessionType: TypeAlias = aiohttp.ClientSession
+else:
+    ClientSessionType = type
+
 _USER_AGENT = 'instawow (+https://github.com/layday/instawow)'
 
 _DEFAULT_EXPIRE = 0  # Do not cache by default.
 
 CACHE_INDEFINITELY = -1
 
 
@@ -23,23 +30,21 @@
     report_progress: Literal['generic']
     label: str
 
 
 class _PkgDownloadTraceRequestCtx(TypedDict):
     report_progress: Literal['pkg_download']
     profile: str
-    pkg: _deferred_types.models.Pkg
+    pkg: models.Pkg
 
 
 TraceRequestCtx: TypeAlias = '_GenericDownloadTraceRequestCtx | _PkgDownloadTraceRequestCtx | None'
 
 
-def make_pkg_progress_ctx(
-    profile: str, pkg: _deferred_types.models.Pkg
-) -> _PkgDownloadTraceRequestCtx:
+def make_pkg_progress_ctx(profile: str, pkg: models.Pkg) -> _PkgDownloadTraceRequestCtx:
     return {'report_progress': 'pkg_download', 'profile': profile, 'pkg': pkg}
 
 
 def make_generic_progress_ctx(label: str) -> _GenericDownloadTraceRequestCtx:
     return {'report_progress': 'generic', 'label': label}
 
 
@@ -52,16 +57,16 @@
     else:
         logger.info('loading certifi certs')
         return read_resource_as_text(certifi, 'cacert.pem', encoding='ascii')
 
 
 @asynccontextmanager
 async def init_web_client(
-    cache_dir: Path | None, *, no_cache: bool = False, **kwargs: Any
-) -> AsyncIterator[_deferred_types.aiohttp.ClientSession]:
+    cache_dir: Path | None, *, no_cache: bool = False, **kwargs: object
+) -> AsyncIterator[ClientSessionType]:
     from aiohttp import ClientSession, ClientTimeout, TCPConnector
 
     make_connector = partial(TCPConnector, limit_per_host=10)
     certifi_certs = _load_certifi_certs()
     if certifi_certs:
         import ssl
 
@@ -76,29 +81,28 @@
         'timeout': ClientTimeout(connect=60, sock_connect=10, sock_read=20),
         **kwargs,
     }
 
     if cache_dir is not None:
         from aiohttp_client_cache.session import CachedSession
 
-        from ._http_cache_db import SQLiteBackend, acquire_cache_db_conn
+        from ._http_cache_db import SQLiteBackend, acquire_cache_connection
 
-        with acquire_cache_db_conn(cache_dir / '_aiohttp-cache.sqlite') as db_conn:
+        with acquire_cache_connection(cache_dir) as connection:
             cache_backend = SQLiteBackend(
                 allowed_codes=[200, 206],
                 allowed_methods=['GET', 'POST'],
-                db_conn=db_conn,
+                connection=connection,
                 expire_after=_DEFAULT_EXPIRE,
                 include_headers=True,
             )
             if no_cache:
                 cache_backend.disabled = True
 
             async with CachedSession(
                 cache=cache_backend,
                 **kwargs,
             ) as client_session:
                 yield client_session
     else:
-
         async with ClientSession(**kwargs) as client_session:
             yield client_session
```

### Comparing `instawow-2.1.1/src/instawow/manager.py` & `instawow-2.2.0/src/instawow/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 from __future__ import annotations
 
-import asyncio
 import contextvars as cv
+import enum
 import json
-from collections import defaultdict
 from collections.abc import Awaitable, Callable, Collection, Iterable, Mapping, Sequence, Set
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, contextmanager
 from datetime import datetime, timedelta
-from functools import cached_property, wraps
-from itertools import chain, filterfalse, product, repeat, starmap, takewhile
+from functools import cached_property, lru_cache, wraps
+from itertools import chain, filterfalse, product, repeat, starmap
 from pathlib import Path, PurePath
+from shutil import move
 from tempfile import NamedTemporaryFile
 from typing import NoReturn, TypeVar
 
 import sqlalchemy as sa
-import sqlalchemy.future as sa_future
 from attrs import evolve
 from loguru import logger
-from typing_extensions import Concatenate, ParamSpec, TypeAlias
+from typing_extensions import Concatenate, ParamSpec, Self, TypeAlias
 from yarl import URL
 
-from . import _deferred_types, db, models
+from . import db, http, models
 from . import results as R
 from ._sources.cfcore import CfCoreResolver
 from ._sources.github import GithubResolver
 from ._sources.instawow import InstawowResolver
 from ._sources.tukui import TukuiResolver
 from ._sources.wago import WagoResolver
 from ._sources.wowi import WowiResolver
 from .cataloguer import (
     BASE_CATALOGUE_VERSION,
-    CATALOGUE_VERSION,
     Catalogue,
     CatalogueEntry,
-    catalogue_converter,
 )
-from .common import Strategy
-from .config import Config, GlobalConfig
+from .common import Defn, Strategy
+from .config import Config
 from .http import make_generic_progress_ctx, make_pkg_progress_ctx
 from .plugins import load_plugins
-from .resolvers import Defn, HeadersIntent, Resolver
+from .resolvers import HeadersIntent, Resolver
 from .utils import (
+    StrEnum,
+    WeakValueDefaultDictionary,
     bucketise,
     chain_dict,
     file_uri_to_path,
     find_addon_zip_tocs,
     gather,
     is_file_uri,
-    is_not_stale,
     make_zip_member_filter_fn,
-    move,
     normalise_names,
     shasum,
     time_op,
     trash,
     uniq,
 )
 from .utils import run_in_thread as t
 
 _P = ParamSpec('_P')
 _T = TypeVar('_T')
 _ResultOrError: TypeAlias = '_T | R.ManagerError | R.InternalError'
 
 DB_REVISION = '98716a7301f8'
 
+_AsyncNamedTemporaryFile = t(NamedTemporaryFile)
 _move_async = t(move)
 
 
 _ERROR_CLASSES = (R.ManagerError, R.InternalError)
 
 
-def _bucketise_results(
+def bucketise_results(
     value: Iterable[tuple[Defn, _ResultOrError[_T]]],
 ) -> tuple[Mapping[Defn, _T], Mapping[Defn, _ResultOrError[NoReturn]]]:
     def get_bucket_dict(key: bool):
         return dict(buckets.get(key, ()))
 
     buckets = bucketise(value, lambda v: isinstance(v[1], _ERROR_CLASSES))
-    return (get_bucket_dict(False), get_bucket_dict(True))  # pyright: ignore
+    return (
+        get_bucket_dict(False),
+        get_bucket_dict(True),
+    )  # pyright: ignore[reportGeneralTypeIssues]
 
 
 @asynccontextmanager
 async def _open_temp_writer():
-    loop = asyncio.get_running_loop()
-    fh = await loop.run_in_executor(None, lambda: NamedTemporaryFile(delete=False))
+    fh = await _AsyncNamedTemporaryFile(delete=False)
     path = Path(fh.name)
     try:
         yield (path, t(fh.write))
     except BaseException:
         await t(fh.close)()
         await t(path.unlink)()
         raise
@@ -142,29 +142,35 @@
 
     async def __aexit__(self, *args: object):
         pass
 
 
 def _with_lock(
     lock_name: str,
+    *,
     manager_bound: bool = True,
 ):
     def outer(
         coro_fn: Callable[Concatenate[Manager, _P], Awaitable[_T]]
     ) -> Callable[Concatenate[Manager, _P], Awaitable[_T]]:
         @wraps(coro_fn)
         async def inner(self: Manager, *args: _P.args, **kwargs: _P.kwargs):
-            async with self.locks[(id(self), lock_name) if manager_bound else lock_name]:
+            async with self.locks[(lock_name, id(self)) if manager_bound else lock_name]:
                 return await coro_fn(self, *args, **kwargs)
 
         return inner
 
     return outer
 
 
+class _StandardLocks(StrEnum):
+    LoadCatalogue = enum.auto()
+    MutatePkgs = enum.auto()
+
+
 class _Resolvers(dict[str, Resolver]):
     @cached_property
     def priority_dict(self) -> _ResolverPriorityDict:
         return _ResolverPriorityDict(self)
 
     @cached_property
     def addon_toc_key_and_id_pairs(self) -> Collection[tuple[str, str]]:
@@ -179,60 +185,65 @@
     def __init__(self, resolvers: _Resolvers) -> None:
         super().__init__((n, i) for i, n in enumerate(resolvers))
 
     def __missing__(self, key: str) -> float:
         return float('inf')
 
 
-_web_client: cv.ContextVar[_deferred_types.aiohttp.ClientSession] = cv.ContextVar('_web_client')
+_web_client = cv.ContextVar[http.ClientSessionType]('_web_client')
 
-LocksType: TypeAlias = defaultdict[object, AbstractAsyncContextManager[None]]
+LocksType: TypeAlias = Mapping[object, AbstractAsyncContextManager[None]]
 
-_dummy_locks: LocksType = defaultdict(_DummyLock)
-_locks: cv.ContextVar[LocksType] = cv.ContextVar('_locks', default=_dummy_locks)
+_locks = cv.ContextVar[LocksType]('_locks', default=WeakValueDefaultDictionary(_DummyLock))
 
 
 def contextualise(
     *,
-    web_client: _deferred_types.aiohttp.ClientSession | None = None,
+    web_client: http.ClientSessionType | None = None,
     locks: LocksType | None = None,
 ) -> None:
     "Set variables for the current context."
     if web_client is not None:
         _web_client.set(web_client)
     if locks is not None:
         _locks.set(locks)
 
 
+@lru_cache(1)
+def _parse_catalogue(raw_catalogue: bytes):
+    with time_op(lambda t: logger.debug(f'parsed catalogue in {t:.3f}s')):
+        return Catalogue.from_base_catalogue(json.loads(raw_catalogue), None)
+
+
 class Manager:
     RESOLVERS: Sequence[type[Resolver]] = [
         GithubResolver,
         CfCoreResolver,
         WowiResolver,
         TukuiResolver,
         InstawowResolver,
         WagoResolver,
     ]
-    "Default resolvers."
+    'Default resolvers.'
 
     _base_catalogue_url = (
         f'https://raw.githubusercontent.com/layday/instawow-data/data/'
         f'base-catalogue-v{BASE_CATALOGUE_VERSION}.compact.json'
     )
-    _catalogue_filename = f'catalogue-v{CATALOGUE_VERSION}.json'
+    _catalogue_ttl = timedelta(hours=4)
 
     _normalise_search_terms = staticmethod(normalise_names(''))
 
     def __init__(
         self,
         config: Config,
-        database: sa_future.Connection,
+        database: sa.Engine,
     ) -> None:
         self.config: Config = config
-        self.database: sa_future.Connection = database
+        self.database: sa.Engine = database
 
         builtin_resolver_classes = list(self.RESOLVERS)
 
         for resolver, access_token in (
             (r, getattr(self.config.global_config.access_tokens, r.requires_access_token, None))
             for r in self.RESOLVERS
             if r.requires_access_token is not None
@@ -242,29 +253,27 @@
 
         plugin_hook = load_plugins()
         resolver_classes = chain(
             (r for g in plugin_hook.instawow_add_resolvers() for r in g), builtin_resolver_classes
         )
         self.resolvers = _Resolvers((r.metadata.id, r(self)) for r in resolver_classes)
 
-        self._catalogue = None
-
     @classmethod
-    def from_config(cls, config: Config) -> tuple[Manager, Callable[[], None]]:
+    def from_config(cls, config: Config) -> Self:
         "Instantiate the manager from a configuration object."
-        db_conn = db.prepare_database(config.db_uri, DB_REVISION).connect()
-        return (cls(config, db_conn), db_conn.close)
+        database = db.prepare_database(config.db_uri, DB_REVISION)
+        return cls(config, database)
 
     @property
     def locks(self) -> LocksType:
         "Lock factory used to synchronise async operations."
         return _locks.get()
 
     @property
-    def web_client(self) -> _deferred_types.aiohttp.ClientSession:
+    def web_client(self) -> http.ClientSessionType:
         return _web_client.get()
 
     def pair_uri(self, value: str) -> tuple[str, str] | None:
         "Attempt to extract the definition source and alias from a URI."
 
         def from_urn():
             source, _, alias = value.partition(':')
@@ -277,65 +286,68 @@
             for a in (r.get_alias_from_url(URL(value)),)
             if a
         )
         return next(chain(aliases_from_url, from_urn(), (None,)))
 
     def check_pkg_exists(self, defn: Defn) -> bool:
         "Check that a package exists in the database."
-        return (
-            self.database.execute(
-                sa.select(sa.text('1'))
-                .select_from(db.pkg)
-                .where(
-                    db.pkg.c.source == defn.source,
-                    (db.pkg.c.id == defn.alias)
-                    | (db.pkg.c.id == defn.id)
-                    | (db.pkg.c.slug == defn.alias),
-                )
-            ).scalar()
-            == 1
-        )
+        with self.database.connect() as connection:
+            return (
+                connection.execute(
+                    sa.select(sa.text('1'))
+                    .select_from(db.pkg)
+                    .where(
+                        db.pkg.c.source == defn.source,
+                        (db.pkg.c.id == defn.alias)
+                        | (db.pkg.c.id == defn.id)
+                        | (db.pkg.c.slug == defn.alias),
+                    )
+                ).scalar()
+                == 1
+            )
 
     def get_pkg(self, defn: Defn, partial_match: bool = False) -> models.Pkg | None:
         "Retrieve a package from the database."
-        maybe_row_mapping = (
-            self.database.execute(
-                sa.select(db.pkg).where(
-                    db.pkg.c.source == defn.source,
-                    (db.pkg.c.id == defn.alias)
-                    | (db.pkg.c.id == defn.id)
-                    | (db.pkg.c.slug == defn.alias),
-                )
-            )
-            .mappings()
-            .one_or_none()
-        )
-        if maybe_row_mapping is None and partial_match:
+        with self.database.connect() as connection:
             maybe_row_mapping = (
-                self.database.execute(
-                    sa.select(db.pkg)
-                    .where(db.pkg.c.slug.contains(defn.alias))
-                    .order_by(db.pkg.c.name)
+                connection.execute(
+                    sa.select(db.pkg).where(
+                        db.pkg.c.source == defn.source,
+                        (db.pkg.c.id == defn.alias)
+                        | (db.pkg.c.id == defn.id)
+                        | (db.pkg.c.slug == defn.alias),
+                    )
                 )
                 .mappings()
-                .first()
+                .one_or_none()
             )
-        if maybe_row_mapping is not None:
-            return models.Pkg.from_row_mapping(self.database, maybe_row_mapping)
+            if maybe_row_mapping is None and partial_match:
+                maybe_row_mapping = (
+                    connection.execute(
+                        sa.select(db.pkg)
+                        .where(db.pkg.c.slug.contains(defn.alias))
+                        .order_by(db.pkg.c.name)
+                    )
+                    .mappings()
+                    .first()
+                )
+            if maybe_row_mapping is not None:
+                return models.Pkg.from_row_mapping(connection, maybe_row_mapping)
 
     @t
     def _install_pkg(self, pkg: models.Pkg, archive: Path, replace: bool) -> R.PkgInstalled:
         "Install a package."
         with _open_pkg_archive(archive) as (top_level_folders, extract):
-            installed_conflicts = self.database.execute(
-                sa.select(db.pkg)
-                .distinct()
-                .join(db.pkg_folder)
-                .where(db.pkg_folder.c.name.in_(top_level_folders))
-            ).all()
+            with self.database.connect() as connection:
+                installed_conflicts = connection.execute(
+                    sa.select(db.pkg)
+                    .distinct()
+                    .join(db.pkg_folder)
+                    .where(db.pkg_folder.c.name.in_(top_level_folders))
+                ).all()
             if installed_conflicts:
                 raise R.PkgConflictsWithInstalled(installed_conflicts)
 
             if replace:
                 trash(
                     [self.config.addon_dir / f for f in top_level_folders],
                     dest=self.config.global_config.temp_dir,
@@ -347,94 +359,85 @@
                 }
                 if unreconciled_conflicts:
                     raise R.PkgConflictsWithUnreconciled(unreconciled_conflicts)
 
             extract(self.config.addon_dir)
 
         pkg = evolve(pkg, folders=[models.PkgFolder(name=f) for f in sorted(top_level_folders)])
-        pkg.insert(self.database)
+        with self.database.begin() as transaction:
+            pkg.insert(transaction)
+
         return R.PkgInstalled(pkg)
 
     @t
     def _update_pkg(self, old_pkg: models.Pkg, new_pkg: models.Pkg, archive: Path) -> R.PkgUpdated:
         "Update a package."
         with _open_pkg_archive(archive) as (top_level_folders, extract):
-            installed_conflicts = self.database.execute(
-                sa.select(db.pkg)
-                .distinct()
-                .join(db.pkg_folder)
-                .where(
-                    db.pkg_folder.c.pkg_source != new_pkg.source,
-                    db.pkg_folder.c.pkg_id != new_pkg.id,
-                    db.pkg_folder.c.name.in_(top_level_folders),
-                )
-            ).all()
+            with self.database.connect() as connection:
+                installed_conflicts = connection.execute(
+                    sa.select(db.pkg)
+                    .distinct()
+                    .join(db.pkg_folder)
+                    .where(
+                        db.pkg_folder.c.pkg_source != new_pkg.source,
+                        db.pkg_folder.c.pkg_id != new_pkg.id,
+                        db.pkg_folder.c.name.in_(top_level_folders),
+                    )
+                ).all()
             if installed_conflicts:
                 raise R.PkgConflictsWithInstalled(installed_conflicts)
 
             unreconciled_conflicts = top_level_folders - {f.name for f in old_pkg.folders} & {
                 f.name for f in self.config.addon_dir.iterdir()
             }
             if unreconciled_conflicts:
                 raise R.PkgConflictsWithUnreconciled(unreconciled_conflicts)
 
             trash(
                 [self.config.addon_dir / f.name for f in old_pkg.folders],
                 dest=self.config.global_config.temp_dir,
                 missing_ok=True,
             )
-            old_pkg.delete(self.database)
-
             extract(self.config.addon_dir)
 
         new_pkg = evolve(
             new_pkg, folders=[models.PkgFolder(name=f) for f in sorted(top_level_folders)]
         )
-        new_pkg.insert(self.database)
+        with self.database.begin() as transaction:
+            old_pkg.delete(transaction)
+            new_pkg.insert(transaction)
+
         return R.PkgUpdated(old_pkg, new_pkg)
 
     @t
     def _remove_pkg(self, pkg: models.Pkg, keep_folders: bool) -> R.PkgRemoved:
         "Remove a package."
         if not keep_folders:
             trash(
                 [self.config.addon_dir / f.name for f in pkg.folders],
                 dest=self.config.global_config.temp_dir,
                 missing_ok=True,
             )
 
-        pkg.delete(self.database)
+        with self.database.begin() as transaction:
+            pkg.delete(transaction)
+
         return R.PkgRemoved(pkg)
 
-    @_with_lock('load catalogue', False)
+    @_with_lock(_StandardLocks.LoadCatalogue, manager_bound=False)
     async def synchronise(self) -> Catalogue:
         "Fetch the catalogue from the interwebs and load it."
-        catalogue_json = self.config.global_config.temp_dir / self._catalogue_filename
-        if await t(is_not_stale)(catalogue_json, timedelta(hours=4)):
-            if self._catalogue is None:
-                with time_op(lambda t: logger.debug(f'loaded catalogue from cache in {t:.3f}s')):
-                    raw_catalogue = await t(catalogue_json.read_bytes)()
-                    self._catalogue = catalogue_converter.structure(
-                        json.loads(raw_catalogue), Catalogue
-                    )
-        else:
-            async with self.web_client.get(
-                self._base_catalogue_url,
-                raise_for_status=True,
-                trace_request_ctx=make_generic_progress_ctx('Synchronising catalogue'),
-            ) as response:
-                raw_catalogue = await response.json(content_type=None)
-
-            self._catalogue = Catalogue.from_base_catalogue(raw_catalogue, None)
-            await t(catalogue_json.write_text)(
-                json.dumps(catalogue_converter.unstructure(self._catalogue)),
-                encoding='utf-8',
-            )
-
-        return self._catalogue
+        async with self.web_client.get(
+            self._base_catalogue_url,
+            expire_after=self._catalogue_ttl,
+            raise_for_status=True,
+            trace_request_ctx=make_generic_progress_ctx('Synchronising catalogue'),
+        ) as response:
+            raw_catalogue = await response.read()
+        return _parse_catalogue(raw_catalogue)
 
     async def find_equivalent_pkg_defns(
         self, pkgs: Collection[models.Pkg]
     ) -> dict[models.Pkg, list[Defn]]:
         "Given a list of packages, find ``Defn``s of each package from other sources."
         from .matchers import AddonFolder
 
@@ -575,28 +578,26 @@
         catalogue = await self.synchronise()
 
         ew = 0.5
         dw = 1 - ew
 
         threshold = 0 if search_terms == '*' else 70
 
-        if not sources:
-            sources = self.resolvers.keys()
-        else:
+        if sources:
             unknown_sources = sources - self.resolvers.keys()
             if unknown_sources:
                 raise ValueError(f'Unknown sources: {", ".join(unknown_sources)}')
 
         def make_filter_fns():
             def filter_game_flavour(entry: CatalogueEntry):
                 return self.config.game_flavour in entry.game_flavours
 
             yield filter_game_flavour
 
-            if sources is not None:
+            if sources:
 
                 def filter_sources(entry: CatalogueEntry):
                     return entry.source in sources
 
                 yield filter_sources
 
             if start_date is not None:
@@ -608,20 +609,23 @@
                 yield filter_age
 
         filter_fns = list(make_filter_fns())
 
         s = self._normalise_search_terms(search_terms)
 
         if installed_only:
-            entries = (
-                e
-                for p in self.database.execute(sa.select(db.pkg.c.source, db.pkg.c.id)).all()
-                for e in (catalogue.keyed_entries.get(p),)
-                if e
-            )
+            with self.database.connect() as connection:
+                entries = (
+                    e
+                    for p in connection.execute(sa.select(db.pkg.c.source, db.pkg.c.id))
+                    .tuples()
+                    .all()
+                    for e in (catalogue.keyed_entries.get(p),)
+                    if e
+                )
         else:
             entries = catalogue.entries
 
         tokens_to_entries = bucketise(
             ((e.normalised_name, e) for e in entries if all(f(e) for f in filter_fns)),
             key=lambda v: v[0],
         )
@@ -670,53 +674,49 @@
         return all((self.config.addon_dir / p.name).exists() for p in pkg.folders)
 
     async def _should_update_pkg(self, old_pkg: models.Pkg, new_pkg: models.Pkg) -> bool:
         return old_pkg.version != new_pkg.version or (
             not await self._check_installed_pkg_integrity(old_pkg)
         )
 
-    @_with_lock('change state')
+    @_with_lock(_StandardLocks.MutatePkgs)
     async def install(
         self, defns: Sequence[Defn], replace: bool
     ) -> Mapping[Defn, _ResultOrError[R.PkgInstalled]]:
         "Install packages from a definition list."
         # We'll weed out installed deps from the results after resolving -
         # doing it this way isn't particularly efficient but avoids having to
         # deal with local state in ``resolve``
         resolve_results = await self.resolve(
             [d for d in defns if not self.check_pkg_exists(d)], with_deps=True
         )
-        pkgs, resolve_errors = _bucketise_results(
+        pkgs, resolve_errors = bucketise_results(
             (d, r) for d, r in resolve_results.items() if not self.check_pkg_exists(d)
         )
-        archive_paths, download_errors = _bucketise_results(
+        archive_paths, download_errors = bucketise_results(
             zip(
                 pkgs,
                 await gather(
                     (self._download_pkg_archive(r) for r in pkgs.values()),
                     capture_manager_exc_async,
                 ),
             )
         )
-        results = chain_dict(
-            defns,
-            R.PkgAlreadyInstalled(),
-            resolve_errors.items(),
-            download_errors.items(),
-            [
-                (
-                    d,
-                    await capture_manager_exc_async(self._install_pkg(pkgs[d], a, replace)),
-                )
+        results = (
+            dict.fromkeys(defns, R.PkgAlreadyInstalled())
+            | resolve_errors
+            | download_errors
+            | {
+                d: await capture_manager_exc_async(self._install_pkg(pkgs[d], a, replace))
                 for d, a in archive_paths.items()
-            ],
+            }
         )
         return results
 
-    @_with_lock('change state')
+    @_with_lock(_StandardLocks.MutatePkgs)
     async def update(
         self, defns: Sequence[Defn], retain_defn_strategy: bool
     ) -> Mapping[Defn, _ResultOrError[R.PkgInstalled | R.PkgUpdated]]:
         """Update installed packages from a definition list.
 
         A ``retain_defn_strategy`` value of false will instruct ``update``
         to extract the strategy from the installed package; otherwise
@@ -732,68 +732,64 @@
             for d, p in defns_to_pkgs.items()
         }
         resolve_results = await self.resolve(resolve_defns, with_deps=True)
         # Discard the reconstructed ``Defn``s
         orig_defn_resolve_results = (
             (resolve_defns.get(d, d), r) for d, r in resolve_results.items()
         )
-        pkgs, resolve_errors = _bucketise_results(orig_defn_resolve_results)
+        pkgs, resolve_errors = bucketise_results(orig_defn_resolve_results)
         updatables = {
             d: (o, n)
             for d, n in pkgs.items()
             for o in (defns_to_pkgs.get(d),)
             if not o or await self._should_update_pkg(o, n)
         }
-        archive_paths, download_errors = _bucketise_results(
+        archive_paths, download_errors = bucketise_results(
             zip(
                 updatables,
                 await gather(
                     (self._download_pkg_archive(n) for _, n in updatables.values()),
                     capture_manager_exc_async,
                 ),
             )
         )
-        results = chain_dict(
-            defns,
-            R.PkgNotInstalled(),
-            resolve_errors.items(),
-            (
-                (d, R.PkgUpToDate(is_pinned=pkgs[d].options.version_eq))
+        results = (
+            dict.fromkeys(defns, R.PkgNotInstalled())
+            | resolve_errors
+            | {
+                d: R.PkgUpToDate(is_pinned=pkgs[d].options.version_eq)
                 for d in pkgs.keys() - updatables.keys()
-            ),
-            download_errors.items(),
-            [
-                (
-                    d,
-                    await capture_manager_exc_async(
-                        self._update_pkg(o, n, a) if o else self._install_pkg(n, a, False)
-                    ),
+            }
+            | download_errors
+            | {
+                d: await capture_manager_exc_async(
+                    self._update_pkg(o, n, a) if o else self._install_pkg(n, a, False)
                 )
                 for d, a in archive_paths.items()
                 for o, n in (updatables[d],)
-            ],
+            }
         )
         return results
 
-    @_with_lock('change state')
+    @_with_lock(_StandardLocks.MutatePkgs)
     async def remove(
         self, defns: Sequence[Defn], keep_folders: bool
     ) -> Mapping[Defn, _ResultOrError[R.PkgRemoved]]:
         "Remove packages by their definition."
         return {
             d: (
                 await capture_manager_exc_async(self._remove_pkg(p, keep_folders))
                 if p
                 else R.PkgNotInstalled()
             )
             for d in defns
             for p in (self.get_pkg(d),)
         }
 
-    @_with_lock('change state')
+    @_with_lock(_StandardLocks.MutatePkgs)
     async def pin(self, defns: Sequence[Defn]) -> Mapping[Defn, _ResultOrError[R.PkgInstalled]]:
         """Pin and unpin installed packages.
 
         instawow does not have true pinning.  This flips ``Strategy.version_eq``
         on for installed packages from sources that support it.
         The net effect is the same as if the package
         had been reinstalled with the ``version_eq`` strategy.
@@ -812,53 +808,18 @@
             if not pkg:
                 raise R.PkgNotInstalled
 
             version = defn.strategies.version_eq
             if version and pkg.version != version:
                 R.PkgFilesNotMatching(defn.strategies)
 
-            with db.faux_transact(self.database):
-                self.database.execute(
+            with self.database.begin() as transaction:
+                transaction.execute(
                     sa.update(db.pkg_options)
                     .filter_by(pkg_source=pkg.source, pkg_id=pkg.id)
                     .values(version_eq=version is not None)
                 )
 
             new_pkg = evolve(pkg, options=evolve(pkg.options, version_eq=version is not None))
             return R.PkgInstalled(new_pkg)
 
         return {d: await capture_manager_exc_async(pin(d)) for d in defns}
-
-
-async def is_outdated(global_config: GlobalConfig) -> tuple[bool, str]:
-    """Check on PyPI to see if instawow is outdated.
-
-    The response is cached for 24 hours.
-    """
-
-    if not global_config.auto_update_check:
-        return (False, '')
-
-    from . import __version__
-
-    if __version__ == '0+dev':
-        return (False, '')
-
-    from aiohttp.client import ClientError
-
-    from .http import init_web_client
-
-    def parse_version(version: str):
-        version_parts = takewhile(lambda p: all(c in '0123456789' for c in p), version.split('.'))
-        return tuple(map(int, version_parts))
-
-    try:
-        async with init_web_client(
-            global_config.cache_dir, raise_for_status=True
-        ) as web_client, web_client.get(
-            'https://pypi.org/pypi/instawow/json', expire_after=timedelta(days=1)
-        ) as response:
-            version = (await response.json())['info']['version']
-    except ClientError:
-        version = __version__
-
-    return (parse_version(version) > parse_version(__version__), version)
```

### Comparing `instawow-2.1.1/src/instawow/matchers.py` & `instawow-2.2.0/src/instawow/matchers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 import re
-from collections.abc import Awaitable, Iterable
+from collections.abc import Awaitable, Iterable, Mapping
 from functools import cached_property
 from itertools import chain, product
 from pathlib import Path
 from typing import Protocol, TypeVar
 
 import sqlalchemy as sa
 from attrs import field, frozen
 from typing_extensions import Self
 
 from . import manager
 from ._addon_hashing import generate_wowup_addon_hash
-from .common import AddonHashMethod, Flavour
+from .common import AddonHashMethod, Defn, Flavour
 from .db import pkg_folder
-from .resolvers import Defn
 from .utils import (
     TocReader,
     assert_decorated_type,
     bucketise,
     gather,
     merge_intersecting_sets,
     uniq,
@@ -88,15 +87,17 @@
 
     @cached_property
     def version(self) -> str:
         return self.toc_reader['Version', 'X-Packaged-Version', 'X-Curse-Packaged-Version'] or ''
 
 
 def _get_unreconciled_folders(manager: manager.Manager):
-    pkg_folders = manager.database.execute(sa.select(pkg_folder.c.name)).scalars().all()
+    with manager.database.connect() as connection:
+        pkg_folders = connection.execute(sa.select(pkg_folder.c.name)).scalars().all()
+
     unreconciled_folder_paths = (
         p
         for p in manager.config.addon_dir.iterdir()
         if p.name not in pkg_folders and p.is_dir() and not p.is_symlink()
     )
     for path in unreconciled_folder_paths:
         addon_folder = AddonFolder.from_addon_path(manager.config.game_flavour, path)
@@ -195,7 +196,16 @@
     addon_names_to_catalogue_entries = bucketise(
         catalogue.entries, key=lambda i: normalise(i.name)
     )
     matches = (
         (a, addon_names_to_catalogue_entries.get(normalise(a.name))) for a in sorted(leftovers)
     )
     return [([a], uniq(Defn(i.source, i.id) for i in m)) for a, m in matches if m]
+
+
+# In order of increasing heuristicitivenessitude
+DEFAULT_MATCHERS: Mapping[str, Matcher] = {
+    'toc_source_ids': match_toc_source_ids,
+    'folder_name_subsets': match_folder_name_subsets,
+    'folder_hashes': match_folder_hashes,
+    'addon_names_with_folder_names': match_addon_names_with_folder_names,
+}
```

### Comparing `instawow-2.1.1/src/instawow/models.py` & `instawow-2.2.0/src/instawow/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 from datetime import datetime
-from typing import Any
 
 import sqlalchemy as sa
-import sqlalchemy.future as sa_future
 from attrs import asdict, frozen
 from cattrs import Converter
-from cattrs.preconf.json import configure_converter
 from typing_extensions import Self
 
 from . import db
-from .common import StrategyValues
-from .resolvers import Defn
-
-pkg_converter = Converter()
-configure_converter(pkg_converter)
+from .common import Defn, StrategyValues
 
 _db_pkg_converter = Converter()
 _db_pkg_converter.register_structure_hook(datetime, lambda d, _: d)
 
 
 @frozen(kw_only=True)
 class PkgOptions:
@@ -66,15 +59,15 @@
     options: PkgOptions  # pkg_options
     folders: list[PkgFolder] = []  # pkg_folder
     deps: list[PkgDep] = []  # pkg_dep
     logged_versions: list[PkgLoggedVersion] = []  # pkg_version_log
 
     @classmethod
     def from_row_mapping(
-        cls, connection: sa_future.Connection, row_mapping: Mapping[str, Any]
+        cls, connection: sa.Connection, row_mapping: Mapping[str, object]
     ) -> Self:
         source_and_id = {'pkg_source': row_mapping['source'], 'pkg_id': row_mapping['id']}
         return _db_pkg_converter.structure(
             {
                 **row_mapping,
                 'options': connection.execute(sa.select(db.pkg_options).filter_by(**source_and_id))
                 .mappings()
@@ -95,35 +88,34 @@
                 )
                 .mappings()
                 .all(),
             },
             cls,
         )
 
-    def insert(self, connection: sa_future.Connection) -> None:
+    def insert(self, transaction: sa.Connection) -> None:
         values = asdict(self)
         source_and_id = {'pkg_source': values['source'], 'pkg_id': values['id']}
-        with db.faux_transact(connection):
-            connection.execute(sa.insert(db.pkg), [values])
-            connection.execute(
-                sa.insert(db.pkg_folder), [{**f, **source_and_id} for f in values['folders']]
-            )
-            connection.execute(sa.insert(db.pkg_options), [{**values['options'], **source_and_id}])
-            if values['deps']:
-                connection.execute(
-                    sa.insert(db.pkg_dep), [{**d, **source_and_id} for d in values['deps']]
-                )
-            connection.execute(
-                sa.insert(db.pkg_version_log).prefix_with('OR IGNORE'),
-                [{'version': values['version'], **source_and_id}],
+
+        transaction.execute(sa.insert(db.pkg), [values])
+        transaction.execute(
+            sa.insert(db.pkg_folder), [{**f, **source_and_id} for f in values['folders']]
+        )
+        transaction.execute(sa.insert(db.pkg_options), [{**values['options'], **source_and_id}])
+        if values['deps']:
+            transaction.execute(
+                sa.insert(db.pkg_dep), [{**d, **source_and_id} for d in values['deps']]
             )
+        transaction.execute(
+            sa.insert(db.pkg_version_log).prefix_with('OR IGNORE'),
+            [{'version': values['version'], **source_and_id}],
+        )
 
-    def delete(self, connection: sa_future.Connection) -> None:
-        with db.faux_transact(connection):
-            connection.execute(sa.delete(db.pkg).filter_by(source=self.source, id=self.id))
+    def delete(self, transaction: sa.Connection) -> None:
+        transaction.execute(sa.delete(db.pkg).filter_by(source=self.source, id=self.id))
 
     def to_defn(self) -> Defn:
         return Defn(
             source=self.source,
             alias=self.slug,
             id=self.id,
             strategies=StrategyValues(
```

### Comparing `instawow-2.1.1/src/instawow/plugins.py` & `instawow-2.2.0/src/instawow/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Protocol
 
 import click
 import pluggy
 
 from . import resolvers
 
-_project_name = __package__
+_project_name = __spec__.parent
 _entry_point = f'{_project_name}.plugins'
 
 hookspec = pluggy.HookspecMarker(_project_name)
 hookimpl = pluggy.HookimplMarker(_project_name)
 
 
 class InstawowPlugin:
```

### Comparing `instawow-2.1.1/src/instawow/resolvers.py` & `instawow-2.2.0/src/instawow/resolvers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 from __future__ import annotations
 
 import enum
-import typing
 import urllib.parse
 from collections.abc import AsyncIterator, Collection, Iterable, Sequence
 from functools import update_wrapper
 from pathlib import Path
 from typing import Any, ClassVar, Protocol, TypeVar
 
-from attrs import evolve, frozen
 from typing_extensions import Self
 from yarl import URL
 
-from . import _deferred_types, models
+from . import http, manager, models
 from . import results as R
 from .cataloguer import BaseCatalogueEntry
-from .common import AddonHashMethod, SourceMetadata, StrategyValues
+from .common import AddonHashMethod, Defn, SourceMetadata
 from .config import GlobalConfig
 from .http import CACHE_INDEFINITELY
 from .utils import file_uri_to_path, gather, run_in_thread
 
 
-@frozen(hash=True)
-class Defn:
-    source: str
-    alias: str
-    id: typing.Union[str, None] = None
-    strategies: StrategyValues = StrategyValues()
-
-    def with_version(self, version: str) -> Self:
-        return evolve(
-            self,
-            strategies=evolve(self.strategies, version_eq=version),
-        )
-
-
 class FolderHashCandidate(Protocol):
     name: str
 
     def hash_contents(self, __method: AddonHashMethod) -> str:
         ...
 
 
@@ -49,15 +33,15 @@
     download = enum.auto()
 
 
 class Resolver(Protocol):
     metadata: ClassVar[SourceMetadata]
     requires_access_token: ClassVar[str | None]
 
-    def __init__(self, manager: _deferred_types.manager.Manager) -> None:
+    def __init__(self, manager: manager.Manager) -> None:
         ...
 
     @classmethod
     def get_alias_from_url(cls, url: URL) -> str | None:
         "Attempt to extract a ``Defn`` alias from a given URL."
         ...
 
@@ -84,38 +68,36 @@
     async def get_folder_hash_matches(
         self, candidates: Collection[TFolderHashCandidate]
     ) -> Iterable[tuple[Defn, frozenset[TFolderHashCandidate]]]:
         "Find ``Defn``s from folder fingerprint."
         ...
 
     @classmethod
-    def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
-    ) -> AsyncIterator[BaseCatalogueEntry]:
+    def catalogue(cls, web_client: http.ClientSessionType) -> AsyncIterator[BaseCatalogueEntry]:
         "Enumerate add-ons from the source."
         ...
 
 
 class BaseResolver(Resolver, Protocol):
-    _manager: _deferred_types.manager.Manager
+    _manager: manager.Manager
 
-    def __init__(self, manager: _deferred_types.manager.Manager) -> None:
+    def __init__(self, manager: manager.Manager) -> None:
         self._manager = manager
 
     __orig_init = __init__
 
     def __init_subclass__(cls) -> None:
         # ``Protocol`` clobbers ``__init__`` in Python < 3.11.  The fix was
         # also backported to 3.9 and 3.10 at some point.
         if cls.__init__ is _DummyResolver.__init__:
             cls.__init__ = cls.__orig_init
 
         if cls.resolve_one is not super().resolve_one:
 
-            async def resolve_one(self: Self, defn: Defn, metadata: Any) -> models.Pkg:
+            async def resolve_one(self: type[Self], defn: Defn, metadata: Any) -> models.Pkg:
                 extraneous_strategies = (
                     defn.strategies.filled_strategies - self.metadata.strategies
                 )
                 if extraneous_strategies:
                     raise R.PkgStrategiesUnsupported(extraneous_strategies)
                 return await cls_resolve_one(self, defn, metadata)
 
@@ -168,15 +150,15 @@
     async def get_folder_hash_matches(
         self, candidates: Collection[TFolderHashCandidate]
     ) -> Iterable[tuple[Defn, frozenset[TFolderHashCandidate]]]:
         return []
 
     @classmethod
     async def catalogue(
-        cls, web_client: _deferred_types.aiohttp.ClientSession
+        cls, web_client: http.ClientSessionType
     ) -> AsyncIterator[BaseCatalogueEntry]:
         return
         yield
 
 
-class _DummyResolver(Resolver):  # pyright: ignore
+class _DummyResolver(Resolver):  # pyright: ignore  # noqa: PGH003
     pass
```

### Comparing `instawow-2.1.1/src/instawow/results.py` & `instawow-2.2.0/src/instawow/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,16 @@
 class PkgFilesNotMatching(ManagerError):
     def __init__(self, strategies: StrategyValues) -> None:
         super().__init__()
         self._strategies = strategies
 
     @property
     def message(self) -> str:
-        return 'no files found for: ' + "; ".join(
-            f"{s}={v!r}" for s, v in asdict(self._strategies).items()
+        return 'no files found for: ' + '; '.join(
+            f'{s}={v!r}' for s, v in asdict(self._strategies).items()
         )
 
 
 class PkgNotInstalled(ManagerError):
     @property
     def message(self) -> str:
         return 'package is not installed'
```

### Comparing `instawow-2.1.1/src/instawow/utils.py` & `instawow-2.2.0/src/instawow/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     Hashable,
     Iterable,
     Iterator,
     Sequence,
     Set,
 )
 from contextlib import contextmanager
-from datetime import datetime, timedelta
 from functools import partial, wraps
 from itertools import chain, groupby, islice, repeat
 from pathlib import Path, PurePath
-from shutil import move as _move
+from shutil import move
 from tempfile import mkdtemp
 from types import ModuleType
 from typing import Any, Generic, TypeVar, overload
+from weakref import WeakValueDictionary
 
 from typing_extensions import ParamSpec
 
 _T = TypeVar('_T')
 _U = TypeVar('_U')
 _THashable = TypeVar('_THashable', bound=Hashable)
 _P = ParamSpec('_P')
@@ -142,29 +142,17 @@
     it: Iterable[Awaitable[object]], wrapper: Callable[..., Awaitable[object]] | None = None
 ) -> Sequence[object]:
     if wrapper is not None:
         it = map(wrapper, it)
     return await asyncio.gather(*it)
 
 
-@overload
-def run_in_thread(
-    fn: type[list[object]],
-) -> Callable[[Iterable[_U]], Awaitable[list[_U]]]:
-    ...
-
-
-@overload
 def run_in_thread(fn: Callable[_P, _U]) -> Callable[_P, Awaitable[_U]]:
-    ...
-
-
-def run_in_thread(fn: Callable[..., object]) -> Callable[..., Awaitable[object]]:
     @wraps(fn)
-    def wrapper(*args: object, **kwargs: object):
+    def wrapper(*args: _P.args, **kwargs: _P.kwargs):
         loop = asyncio.get_running_loop()
         return loop.run_in_executor(None, partial(fn, *args, **kwargs))
 
     return wrapper
 
 
 def tabulate(rows: Sequence[tuple[object, ...]], *, max_col_width: int = 60) -> str:
@@ -174,66 +162,52 @@
     def apply_max_col_width(value: object):
         return fill(str(value), width=max_col_width, max_lines=1)
 
     def calc_resultant_col_widths(rows: Sequence[tuple[str, ...]]):
         cols = zip(*rows)
         return [max(map(len, c)) for c in cols]
 
-    rows = [tuple(apply_max_col_width(i) for i in r) for r in rows]
-    head, *tail = rows
+    norm_rows = [tuple(apply_max_col_width(i) for i in r) for r in rows]
+    head, *tail = norm_rows
 
-    base_template = '  '.join(f'{{{{{{0}}{w}}}}}' for w in calc_resultant_col_widths(rows))
+    base_template = '  '.join(f'{{{{{{0}}{w}}}}}' for w in calc_resultant_col_widths(norm_rows))
     row_template = base_template.format(':<')
     table = '\n'.join(
         (
             base_template.format(':^').format(*head),
             base_template.format('0:-<').format(''),
             *(row_template.format(*r) for r in tail),
         )
     )
     return table
 
 
-def move(src: str | os.PathLike[str], dest: str | os.PathLike[str]) -> Any:
-    return _move(
-        os.fspath(src),  # See https://bugs.python.org/issue32689
-        dest,
-    )
-
-
 def trash(paths: Collection[PurePath], *, dest: PurePath, missing_ok: bool = False) -> None:
     if not paths:
         return
 
     exc_classes = FileNotFoundError if missing_ok else ()
 
     first_path_name = next(iter(paths)).name
     parent_folder = mkdtemp(dir=dest, prefix=f'deleted-{first_path_name}-')
 
     for path in paths:
         try:
-            move(path, dest=parent_folder)
+            move(path, parent_folder)
         except exc_classes:
             pass
 
 
 def shasum(*values: object) -> str:
     "Base-16-encode a string using SHA-256 truncated to 32 characters."
     from hashlib import sha256
 
     return sha256(''.join(map(str, filter(None, values))).encode()).hexdigest()[:32]
 
 
-def is_not_stale(path: Path, ttl: timedelta) -> bool:
-    "Check if a file is older than ``ttl``."
-    return path.exists() and (
-        (datetime.now() - datetime.fromtimestamp(path.stat().st_mtime)) < ttl
-    )
-
-
 def find_addon_zip_tocs(names: Iterable[str]) -> Iterator[tuple[str, str]]:
     "Find top-level folders in a list of ZIP member paths."
     for name in names:
         if name.count(posixpath.sep) == 1:
             head, tail = posixpath.split(name)
             if tail.startswith(head) and tail[-4:].lower() == '.toc':
                 yield (name, head)
@@ -298,7 +272,32 @@
 
 
 @contextmanager
 def time_op(on_complete: Callable[[float], None]) -> Iterator[None]:
     start = time.perf_counter()
     yield
     on_complete(time.perf_counter() - start)
+
+
+class WeakValueDefaultDictionary(WeakValueDictionary[_T, _U]):
+    def __init__(self, default_factory: Callable[[], _U]) -> None:
+        super().__init__()
+        self.__default_factory = default_factory
+
+    def __getitem__(self, key: _T) -> _U:
+        try:
+            return super().__getitem__(key)
+        except KeyError:
+            default = self[key] = self.__default_factory()
+            return default
+
+
+def add_exc_note(exc: BaseException, note: str) -> None:
+    if sys.version_info >= (3, 11):
+        exc.add_note(note)
+
+    else:
+        exc_without_notes: Any = exc
+
+        if not hasattr(exc, '__notes__'):
+            exc_without_notes.__notes__ = list[str]()
+        exc_without_notes.__notes__.append(note)
```

### Comparing `instawow-2.1.1/src/instawow/wa_updater.py` & `instawow-2.2.0/src/instawow/wa_updater.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,56 @@
 from __future__ import annotations
 
 import json
 import typing
-from collections.abc import Iterable, Iterator, Sequence
+from collections.abc import Iterable, Iterator, Mapping, Sequence
 from datetime import timedelta
 from functools import reduce
 from itertools import chain, product
-from typing import Any, Literal
+from typing import Literal
 
 from attrs import frozen
 from cattrs import Converter
 from loguru import logger
 from typing_extensions import NotRequired as N
 from typing_extensions import TypeAlias, TypedDict
 from yarl import URL
 
 from .http import CACHE_INDEFINITELY, make_generic_progress_ctx
 from .manager import Manager
 from .utils import StrEnum, bucketise, gather, read_resource_as_text, shasum, time_op
 from .utils import run_in_thread as t
 
+_LuaTable: TypeAlias = Mapping[str, '_LuaTable']
+_Auras: TypeAlias = 'WeakAuras | Plateroos'
+_Match: TypeAlias = tuple[Sequence['WeakAura | Plateroo'], '_WagoApiResponse', str]
+
+
+class _WagoApiResponse(TypedDict):
+    _id: str  # +   # Alphanumeric ID
+    name: str  # +  # User-facing name
+    slug: str  # +  # Slug if it has one; otherwise same as ``_id``
+    url: str
+    created: str  # ISO datetime
+    modified: str  # ISO datetime
+    game: str  # "classic" or xpac, e.g. "bfa"
+    username: N[str]  # +  # Author username
+    version: int  # +   # Version counter, incremented with every update
+    # Semver auto-generated from ``version`` - for presentation only
+    versionString: str
+    changelog: _WagoApiResponse_Changelog  # +
+    forkOf: N[str]  # Only present on forks
+    regionType: N[str]  # Only present on WAs
+
+
+class _WagoApiResponse_Changelog(TypedDict):
+    format: N[Literal['bbcode', 'markdown']]
+    text: N[str]
+
+
 _CHECK_API_URL = URL('https://data.wago.io/api/check')
 _IMPORT_STRING_API_URL = URL('https://data.wago.io/api/raw/encoded')
 
 _aura_converter = Converter()
 _aura_converter.register_structure_hook(URL, lambda v, _: URL(v))
 _aura_converter.register_unstructure_hook(URL, str)
 
@@ -33,105 +60,80 @@
     id: str
     uid: str
     parent: typing.Union[str, None] = None
     url: URL
     version: int
 
     @classmethod
-    def from_lua_table(cls, lua_table: Any):
+    def from_lua_table(cls, lua_table: _LuaTable):
         url_string = lua_table.get('url')
         if url_string is not None:
             weakaura = _aura_converter.structure(lua_table, cls)
             if weakaura.url.host == 'wago.io':
                 return weakaura
 
 
 @frozen(kw_only=True)
 class Plateroo(WeakAura):
     uid: str = ''
 
     @classmethod
-    def from_lua_table(cls, lua_table: Any):
+    def from_lua_table(cls, lua_table: _LuaTable):
         return super().from_lua_table({**lua_table, 'id': lua_table['Name']})
 
 
 @frozen
 class WeakAuras:
     api_ep = 'weakauras'
     addon_name = 'WeakAuras'
 
     root: dict[str, list[WeakAura]]
 
     @classmethod
-    def from_lua_table(cls, lua_table: Any):
-        auras = (WeakAura.from_lua_table(t) for t in lua_table['displays'].values())
+    def from_lua_table(cls, lua_table: _LuaTable):
+        raw_auras = lua_table['WeakAurasSaved']['displays']
+        auras = (WeakAura.from_lua_table(t) for t in raw_auras.values())
         sorted_auras = sorted(filter(None, auras), key=lambda a: a.id)
         return cls(bucketise(sorted_auras, key=lambda a: a.url.parts[1]))
 
 
 @frozen
 class Plateroos:
     api_ep = 'plater'
     addon_name = 'Plater'
 
     root: dict[str, list[Plateroo]]
 
     @classmethod
-    def from_lua_table(cls, lua_table: Any):
+    def from_lua_table(cls, lua_table: _LuaTable):
+        raw_auras = lua_table['PlaterDB']['profiles']
         auras = (
             Plateroo.from_lua_table(t)
-            for n, p in lua_table['profiles'].items()
+            for n, p in raw_auras.items()
             for t in chain(
                 ({**p, 'Name': f'__profile_{n}__'},),
                 p.get('script_data') or (),
                 p.get('hook_data') or (),
             )
         )
         sorted_auras = sorted(filter(None, auras), key=lambda a: a.id)
         return cls({a.url.parts[1]: [a] for a in sorted_auras})
 
 
-def _merge_auras(auras: Iterable[WeakAuras | Plateroos]):
+def _merge_auras(auras: Iterable[_Auras]):
     return {
         t: t(reduce(lambda a, b: a | b, (i.root for i in a)))
-        for t, a in bucketise(auras, key=type['WeakAuras | Plateroos']).items()
+        for t, a in bucketise(auras, key=type).items()
     }
 
 
-class _WagoApiResponse(TypedDict):
-    _id: str  # +   # Alphanumeric ID
-    name: str  # +  # User-facing name
-    slug: str  # +  # Slug if it has one; otherwise same as ``_id``
-    url: str
-    created: str  # ISO datetime
-    modified: str  # ISO datetime
-    game: str  # "classic" or xpac, e.g. "bfa"
-    username: N[str]  # +  # Author username
-    version: int  # +   # Version counter, incremented with every update
-    # Semver auto-generated from ``version`` - for presentation only
-    versionString: str
-    changelog: _WagoApiResponse_Changelog  # +
-    forkOf: N[str]  # Only present on forks
-    regionType: N[str]  # Only present on WAs
-
-
-class _WagoApiResponse_Changelog(TypedDict):
-    format: N[Literal['bbcode', 'markdown']]
-    text: N[str]
-
-
 class _TocNumber(StrEnum):
-    retail = '100002'
+    retail = '100007'
     vanilla_classic = '11403'
-    classic = '30400'
-
-
-_Aura: TypeAlias = 'WeakAura | Plateroo'
-_Auras: TypeAlias = 'WeakAuras | Plateroos'
-_Matches: TypeAlias = list[tuple[Sequence[_Aura], '_WagoApiResponse', str]]
+    classic = '30401'
 
 
 class WaCompanionBuilder:
     """A WeakAuras Companion port for shellfolk."""
 
     def __init__(self, manager: Manager) -> None:
         self._manager = manager
@@ -146,17 +148,15 @@
         if access_token:
             return {'api-key': access_token}
 
     @staticmethod
     def extract_auras(model: type[_Auras], source: str) -> _Auras:
         from ._custom_slpp import loads
 
-        lua_table = loads(f'{{{source}}}')
-        (aura_table,) = lua_table.values()
-        return model.from_lua_table(aura_table)
+        return model.from_lua_table(loads(f'{{{source}}}'))
 
     def extract_installed_auras(self) -> Iterator[_Auras]:
         flavour_root = self._manager.config.addon_dir.parents[1]
         saved_vars_by_account = flavour_root.glob('WTF/Account/*/SavedVariables')
         for saved_vars, model in product(
             saved_vars_by_account,
             [WeakAuras, Plateroos],
@@ -165,28 +165,28 @@
             if not file.exists():
                 logger.info(f'{file} not found')
             else:
                 content = file.read_text(encoding='utf-8-sig', errors='replace')
                 aura_group_cache = self._manager.config.global_config.cache_dir / shasum(content)
                 if aura_group_cache.exists():
                     logger.info(f'loading {file} from cache at {aura_group_cache}')
-                    aura_groups_json = json.loads(aura_group_cache.read_bytes())
-                    aura_groups = _aura_converter.structure({'root': aura_groups_json}, model)
+                    aura_group_json = json.loads(aura_group_cache.read_bytes())
+                    aura_group = _aura_converter.structure({'root': aura_group_json}, model)
                 else:
                     with time_op(
                         lambda t: logger.debug(
                             f'extracted {model.__name__} in {t:.3f}s'  # noqa: B023
                         )
                     ):
-                        aura_groups = self.extract_auras(model, content)
+                        aura_group = self.extract_auras(model, content)
                     aura_group_cache.write_text(
-                        json.dumps(_aura_converter.unstructure(aura_groups.root)),
+                        json.dumps(_aura_converter.unstructure(aura_group.root)),
                         encoding='utf-8',
                     )
-                yield aura_groups
+                yield aura_group
 
     async def _fetch_wago_metadata(self, api_ep: str, aura_ids: Iterable[str]):
         async with self._manager.web_client.get(
             (_CHECK_API_URL / api_ep).with_query(ids=','.join(aura_ids)),
             expire_after=timedelta(minutes=30),
             headers=self._make_request_headers(),
             trace_request_ctx=make_generic_progress_ctx('Fetching aura metadata'),
@@ -197,46 +197,48 @@
                 return metadata
 
             response.raise_for_status()
 
             metadata = await response.json()
             return sorted(metadata, key=lambda r: r['slug'])
 
-    async def _fetch_wago_import_string(self, aura: _WagoApiResponse):
+    async def _fetch_wago_import_string(self, remote_aura: _WagoApiResponse):
         async with self._manager.web_client.get(
-            _IMPORT_STRING_API_URL.with_query(id=aura['_id']).with_fragment(str(aura['version'])),
+            _IMPORT_STRING_API_URL.with_query(id=remote_aura['_id']).with_fragment(
+                str(remote_aura['version'])
+            ),
             expire_after=CACHE_INDEFINITELY,
             headers=self._make_request_headers(),
             raise_for_status=True,
-            trace_request_ctx=make_generic_progress_ctx(f"Fetching aura '{aura['slug']}'"),
+            trace_request_ctx=make_generic_progress_ctx(f"Fetching aura '{remote_aura['slug']}'"),
         ) as response:
             return await response.text()
 
-    async def get_remote_auras(self, auras: _Auras) -> _Matches:
-        if not auras.root:
+    async def get_remote_auras(self, aura_group: _Auras) -> list[_Match]:
+        if not aura_group.root:
             return []
 
-        metadata = await self._fetch_wago_metadata(auras.api_ep, auras.root)
+        metadata = await self._fetch_wago_metadata(aura_group.api_ep, aura_group.root)
         import_strings = await gather(self._fetch_wago_import_string(r) for r in metadata)
         return [
-            (auras.root.get(r['slug']) or auras.root[r['_id']], r, i)
+            (aura_group.root.get(r['slug']) or aura_group.root[r['_id']], r, i)
             for r, i in zip(metadata, import_strings)
         ]
 
-    def _generate_addon(self, auras: Iterable[tuple[type[_Auras], _Matches]]):
+    def _generate_addon(self, auras: Iterable[tuple[type[_Auras], list[_Match]]]):
         from zipfile import ZipFile, ZipInfo
 
         from mako.template import Template
 
         from . import _wa_templates
 
         def render_template(filename: str, ctx: dict[str, object]):
             return Template(read_resource_as_text(_wa_templates, filename)).render(**ctx)
 
-        aura_dict = dict.fromkeys((WeakAuras, Plateroos), []) | dict(auras)
+        aura_dict = dict.fromkeys((WeakAuras, Plateroos), list[_Match]()) | dict(auras)
 
         self.addon_zip_path.parent.mkdir(exist_ok=True)
         with ZipFile(self.addon_zip_path, 'w') as file:
 
             def write_tpl(filename: str, ctx: dict[str, object]):
                 # Not using a plain string as the first argument to ``writestr``
                 # 'cause the timestamp would be set to the current time
@@ -313,15 +315,15 @@
 
         self.version_txt_path.write_text(
             addon_version,
             encoding='utf-8',
         )
 
     async def build(self) -> None:
-        installed_auras = await t(list)(self.extract_installed_auras())
+        installed_auras = await t(list[_Auras])(self.extract_installed_auras())
         installed_auras_by_type = _merge_auras(installed_auras)
         aura_groups = await gather(
             self.get_remote_auras(r) for r in installed_auras_by_type.values()
         )
         await t(self._generate_addon)(zip(installed_auras_by_type, aura_groups))
 
     def get_version(self) -> str:
```

### Comparing `instawow-2.1.1/tests/conftest.py` & `instawow-2.2.0/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,22 +107,20 @@
     async with init_web_client(iw_config.global_config.cache_dir) as web_client:
         yield web_client
 
 
 @pytest.fixture
 def iw_manager(iw_config: Config, iw_web_client: aiohttp.ClientSession):
     contextualise(web_client=iw_web_client)
-    manager, close_db_conn = Manager.from_config(iw_config)
-    yield manager
-    close_db_conn()
+    return Manager.from_config(iw_config)
 
 
 @pytest.fixture(autouse=True, params=['all'])
 @should_mock
-def iw_mock_aiohttp_requests(
+def _iw_mock_aiohttp_requests(
     request: pytest.FixtureRequest, aresponses: _StrictResponsesMockServer
 ):
     if request.param == 'all':
         routes = ROUTES.values()
     else:
         routes = (ROUTES[k] for k in ROUTES.keys() & request.param)
```

### Comparing `instawow-2.1.1/tests/fixtures/http/__init__.py` & `instawow-2.2.0/tests/fixtures/http/__init__.py`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/base-catalogue-v7.compact.json` & `instawow-2.2.0/tests/fixtures/http/base-catalogue-v7.compact.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/curse-addon--all.json` & `instawow-2.2.0/tests/fixtures/http/curse-addon--all.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/curse-addon-files.json` & `instawow-2.2.0/tests/fixtures/http/curse-addon-files.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-release-molinari.json` & `instawow-2.2.0/tests/fixtures/http/github-release-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-release-no-assets.json` & `instawow-2.2.0/tests/fixtures/http/github-release-no-assets.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-release-no-release-json.json` & `instawow-2.2.0/tests/fixtures/http/github-release-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-release-release-json.json` & `instawow-2.2.0/tests/fixtures/http/github-release-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-repo-molinari.json` & `instawow-2.2.0/tests/fixtures/http/github-repo-molinari.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-repo-no-release-json.json` & `instawow-2.2.0/tests/fixtures/http/github-repo-no-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-repo-no-releases.json` & `instawow-2.2.0/tests/fixtures/http/github-repo-no-releases.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/github-repo-release-json.json` & `instawow-2.2.0/tests/fixtures/http/github-repo-release-json.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/regen.sh` & `instawow-2.2.0/tests/fixtures/http/regen.sh`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/tukui-classic-addons.json` & `instawow-2.2.0/tests/fixtures/http/tukui-classic-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/tukui-classic-wotlk-addons.json` & `instawow-2.2.0/tests/fixtures/http/tukui-classic-wotlk-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/tukui-retail-addons.json` & `instawow-2.2.0/tests/fixtures/http/tukui-retail-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/tukui-ui--elvui.json` & `instawow-2.2.0/tests/fixtures/http/tukui-ui--elvui.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/tukui-ui--tukui.json` & `instawow-2.2.0/tests/fixtures/http/tukui-ui--tukui.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/wago-match-addons.json` & `instawow-2.2.0/tests/fixtures/http/wago-match-addons.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/wowi-filedetails.json` & `instawow-2.2.0/tests/fixtures/http/wowi-filedetails.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/fixtures/http/wowi-filelist.json` & `instawow-2.2.0/tests/fixtures/http/wowi-filelist.json`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/plugin/instawow_test_plugin.py` & `instawow-2.2.0/tests/plugin/instawow_test_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from datetime import datetime
+from __future__ import annotations
+
+from datetime import datetime, timezone
 
 import click
 
 import instawow.plugins
-from instawow.common import ChangelogFormat, SourceMetadata
+from instawow.common import ChangelogFormat, Defn, SourceMetadata
 from instawow.models import Pkg, PkgOptions
-from instawow.resolvers import BaseResolver, Defn
+from instawow.resolvers import BaseResolver
 
 
 @click.command()
 def foo():
     "don't foo where you bar"
     print('success!')
 
@@ -29,15 +31,15 @@
             source=self.metadata.id,
             id='bar',
             slug='bar',
             name='Bar',
             description='The quintessential bar add-on, brought to you by yours truly',
             url='http://example.com/',
             download_url='file:///...',
-            date_published=datetime.now(),
+            date_published=datetime.now(timezone.utc),
             version='0',
             changelog_url='data:,',
             options=PkgOptions.from_strategy_values(defn.strategies),
         )
 
 
 @instawow.plugins.hookimpl
```

### Comparing `instawow-2.1.1/tests/test__slpp.py` & `instawow-2.2.0/tests/test__slpp.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,26 +73,26 @@
 
 def test_array_like_table():
     # keyword values
     assert loads('{ false, true }') == [False, True]
     # nil is erased
     assert loads('{ nil }') == {}
     # string literals
-    assert loads('{ "10" }') == ["10"]
+    assert loads('{ "10" }') == ['10']
     # trailing zero
     assert loads('{ 0, 1, 0 }') == [0, 1, 0]
 
 
 def test_dict_like_table():
     # bracketed keyword keys
     assert loads('{ [10] = 11 }') == {10: 11}
     assert loads('{ [false] = 0 }') == {False: 0}
     assert loads('{ [true] = 1 }') == {True: 1}
     # bracketed string keys
-    assert loads('{ [ [[10]] ] = 1 }') == {"10": 1}
+    assert loads('{ [ [[10]] ] = 1 }') == {'10': 1}
     assert loads('{ [ [[false]] ] = "" }') == {'false': ''}
     # syntax error
     with pytest.raises(ParseError):
         loads('{ [[false]] = "" }')
 
 
 def test_boolean_keys_are_not_numeric():
@@ -167,7 +167,24 @@
             'dict': {
                 False: 'value',
                 'array': [3, '6', 4],
                 'mixed': {1: 43, 2: 54.3, 3: False, 'string': 'value', 4: 9},
             },
         }
     )
+
+
+def test_parse_undelimited_entries():
+    # Not valid Lua but we allow it for the purpose of parsing saved var scripts
+    # containing more than one variable.
+    assert (
+        loads(
+            '''{
+                foo = {}
+                bar = 1
+            }'''
+        )
+        == {
+            'foo': {},
+            'bar': 1,
+        }
+    )
```

### Comparing `instawow-2.1.1/tests/test__sources.py` & `instawow-2.2.0/tests/test__sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from yarl import URL
 
 from instawow import results as R
 from instawow._sources.cfcore import CfCoreResolver
 from instawow._sources.github import GithubResolver
 from instawow._sources.tukui import TukuiResolver
 from instawow._sources.wowi import WowiResolver
-from instawow.common import Flavour, Strategy, StrategyValues
+from instawow.common import Defn, Flavour, Strategy, StrategyValues
 from instawow.manager import Manager
 from instawow.models import Pkg
-from instawow.resolvers import Defn, Resolver
+from instawow.resolvers import Resolver
 
 
 @pytest.mark.parametrize(
     'iw_config_values',
     Flavour,
     indirect=True,
 )
@@ -33,18 +33,18 @@
 
     assert type(results[flavourful]) is Pkg
 
     if (
         iw_manager.config.game_flavour is Flavour.vanilla_classic
         or iw_manager.config.game_flavour is Flavour.classic
     ):
+        assert type(results[retail_only]) is R.PkgFilesNotMatching
         assert (
-            type(results[retail_only]) is R.PkgFilesNotMatching
-            and results[retail_only].message
-            == "no files found for: any_flavour=None; any_release_type=None; version_eq=None"
+            results[retail_only].message
+            == 'no files found for: any_flavour=None; any_release_type=None; version_eq=None'
         )
     elif iw_manager.config.game_flavour is Flavour.retail:
         assert type(results[retail_only]) is Pkg
     else:
         assert_never(iw_manager.config.game_flavour)
 
 
@@ -57,15 +57,16 @@
     results = await iw_manager.resolve([flavourful, retail_only])
     assert all(type(r) is Pkg for r in results.values())
 
 
 async def test_curse_version_pinning(iw_manager: Manager):
     defn = Defn('curse', 'molinari', strategies=StrategyValues(version_eq='80000.58-Release'))
     results = await iw_manager.resolve([defn])
-    assert results[defn].options.version_eq is True and results[defn].version == '80000.58-Release'
+    assert results[defn].options.version_eq is True
+    assert results[defn].version == '80000.58-Release'
 
 
 async def test_curse_deps_retrieved(iw_manager: Manager):
     defn = Defn('curse', 'bigwigs-voice-korean')
 
     results = await iw_manager.resolve([defn], with_deps=True)
     assert {'bigwigs-voice-korean', 'big-wigs'} == {d.slug for d in results.values()}
@@ -101,21 +102,24 @@
 async def test_tukui_basic(iw_manager: Manager):
     regular_addon = Defn('tukui', '1' if iw_manager.config.game_flavour is Flavour.retail else '2')
     tukui_suite = Defn('tukui', '-1')
     elvui_suite = Defn('tukui', '-2')
 
     results = await iw_manager.resolve([regular_addon, tukui_suite, elvui_suite])
 
-    assert type(results[regular_addon]) is Pkg and (
+    assert type(results[regular_addon]) is Pkg
+    assert (
         results[regular_addon].name == 'MerathilisUI'
         if iw_manager.config.game_flavour is Flavour.retail
         else 'ElvUI'
     )
-    assert type(results[tukui_suite]) is Pkg and results[tukui_suite].name == 'Tukui'
-    assert type(results[elvui_suite]) is Pkg and results[elvui_suite].name == 'ElvUI'
+    assert type(results[tukui_suite]) is Pkg
+    assert results[tukui_suite].name == 'Tukui'
+    assert type(results[elvui_suite]) is Pkg
+    assert results[elvui_suite].name == 'ElvUI'
 
 
 async def test_tukui_ui_suite_aliases_for_retail(iw_manager: Manager):
     tukui_id = Defn('tukui', '-1')
     tukui_slug = Defn('tukui', 'tukui')
     elvui_id = Defn('tukui', '-2')
     elvui_slug = Defn('tukui', 'elvui')
@@ -140,18 +144,16 @@
     release_json = Defn('github', 'nebularg/PackagerTest')
     releaseless = Defn('github', 'AdiAddons/AdiBags')
     nonexistent = Defn('github', 'layday/foobar')
 
     results = await iw_manager.resolve([release_json, releaseless, nonexistent])
 
     assert type(results[release_json]) is Pkg
-    assert (
-        type(results[releaseless]) is R.PkgFilesMissing
-        and results[releaseless].message == 'release not found'
-    )
+    assert type(results[releaseless]) is R.PkgFilesMissing
+    assert results[releaseless].message == 'release not found'
     assert type(results[nonexistent]) is R.PkgNonexistent
 
 
 async def test_github_changelog_is_data_url(iw_manager: Manager):
     defn = Defn('github', 'p3lim-wow/Molinari')
     results = await iw_manager.resolve([defn])
     assert results[defn].changelog_url.startswith('data:,')
@@ -163,15 +165,15 @@
         (Flavour.retail, 'mainline', 30400),
         (Flavour.classic, 'wrath', 90207),
         (Flavour.vanilla_classic, 'classic', 90207),
     ],
     indirect=('iw_config_values',),
 )
 @pytest.mark.parametrize(
-    'iw_mock_aiohttp_requests',
+    '_iw_mock_aiohttp_requests',
     [
         {
             URL('//api.github.com/repos/nebularg/PackagerTest'),
             URL('//api.github.com/repos/nebularg/PackagerTest/releases?per_page=10'),
         }
     ],
     indirect=True,
@@ -184,19 +186,19 @@
     interface: int,
 ):
     aresponses.add(
         'api.github.com',
         re.compile(r'^/repos/nebularg/PackagerTest/releases/assets/'),
         'GET',
         {
-            "releases": [
+            'releases': [
                 {
-                    "filename": "TestGit-v1.9.7.zip",
-                    "nolib": False,
-                    "metadata": [{"flavor": flavor, "interface": interface}],
+                    'filename': 'TestGit-v1.9.7.zip',
+                    'nolib': False,
+                    'metadata': [{'flavor': flavor, 'interface': interface}],
                 }
             ]
         },
     )
 
     defn = Defn('github', 'nebularg/PackagerTest')
     results = await iw_manager.resolve([defn])
@@ -222,19 +224,16 @@
         Strategy.any_flavour,
         Strategy.any_release_type,
     } - resolver.metadata.strategies:
         strategy_defn = evolve(defn, strategies=StrategyValues(**{strategy: True}))
 
         results = await iw_manager.resolve([strategy_defn])
 
-        assert (
-            type(results[strategy_defn]) is R.PkgStrategiesUnsupported
-            and results[strategy_defn].message
-            == f"strategies are not valid for source: {strategy}"
-        )
+        assert type(results[strategy_defn]) is R.PkgStrategiesUnsupported
+        assert results[strategy_defn].message == f'strategies are not valid for source: {strategy}'
 
 
 @pytest.mark.parametrize(
     ('resolver', 'url', 'extracted_alias'),
     [
         (CfCoreResolver, 'https://www.curseforge.com/wow/addons/molinari', 'molinari'),
         (CfCoreResolver, 'https://www.curseforge.com/wow/addons/molinari/download', 'molinari'),
```

### Comparing `instawow-2.1.1/tests/test_cli.py` & `instawow-2.2.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 @pytest.fixture
 def run(
     monkeypatch: pytest.MonkeyPatch,
     event_loop: asyncio.AbstractEventLoop,
     iw_config: Config,
 ):
     monkeypatch.setattr('asyncio.run', event_loop.run_until_complete)
-    yield partial(CliRunner().invoke, cli, catch_exceptions=False)
+    return partial(CliRunner().invoke, cli, catch_exceptions=False)
 
 
 @pytest.fixture
 def install_molinari_and_run(
     run: C[[str], Result],
 ):
     run('install curse:molinari')
-    yield run
+    return run
 
 
 @pytest.fixture
 def pretend_install_molinari_and_run(
     iw_config: Config,
     run: C[[str], Result],
 ):
@@ -60,15 +60,15 @@
     molinari.mkdir()
     (molinari / 'Molinari.toc').write_text(
         '''\
 ## X-Curse-Project-ID: 20338
 ## X-WoWI-ID: 13188
 '''
     )
-    yield run
+    return run
 
 
 @pytest.mark.parametrize(
     'alias',
     [
         'curse:molinari',
         'wowi:13188-molinari',
@@ -249,21 +249,32 @@
         'Waiting...\n'
         'Configuration written to:\n'
         f'  {iw_config.global_config.config_dir / "config.json"}\n'
         f'  {iw_config.global_config.config_dir / "profiles/foo/config.json"}\n'
     )
 
 
-def test_configure__update_existing_profile_with_opts(
+def test_configure__update_existing_profile_interactively(
     feed_pt: C[[str], None],
     iw_config: Config,
     run: C[[str], Result],
 ):
     feed_pt('Y\r')
-    assert run('configure auto_update_check').output == (
+    assert run('configure global_config.auto_update_check').output == (
+        'Configuration written to:\n'
+        f'  {iw_config.global_config.config_dir / "config.json"}\n'
+        f'  {iw_config.global_config.config_dir / "profiles/__default__/config.json"}\n'
+    )
+
+
+def test_configure__update_existing_profile_directly(
+    iw_config: Config,
+    run: C[[str], Result],
+):
+    assert run('configure global_config.auto_update_check=0').output == (
         'Configuration written to:\n'
         f'  {iw_config.global_config.config_dir / "config.json"}\n'
         f'  {iw_config.global_config.config_dir / "profiles/__default__/config.json"}\n'
     )
 
 
 @pytest.mark.parametrize('options', ['', '--undo'])
@@ -281,15 +292,15 @@
 def test_rollback__unsupported(
     run: C[[str], Result],
     options: str,
 ):
     assert run('install wowi:13188-molinari').exit_code == 0
     assert (
         run(f'rollback {options} wowi:13188-molinari').output
-        == "✗ wowi:13188-molinari\n  strategies are not valid for source: version_eq\n"
+        == '✗ wowi:13188-molinari\n  strategies are not valid for source: version_eq\n'
     )
 
 
 def test_rollback__single_version(
     run: C[[str], Result],
 ):
     assert run('install curse:molinari').exit_code == 0
@@ -529,15 +540,15 @@
 ):
     assert install_molinari_and_run('view-changelog --no-convert').output.startswith(
         'curse:molinari:\n  <h3>Changes in 90200.82-Release:</h3>'
     )
 
 
 @pytest.mark.parametrize(
-    'command, exit_code',
+    ('command', 'exit_code'),
     [
         ('list mol', 0),
         ('info foo', 0),
         ('reveal mol', 0),
         ('reveal foo', 1),
     ],
 )
```

### Comparing `instawow-2.1.1/tests/test_common.py` & `instawow-2.2.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/test_config.py` & `instawow-2.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `instawow-2.1.1/tests/test_github_zip_parsing.py` & `instawow-2.2.0/tests/test_github_zip_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 import aiohttp.hdrs
 import aiohttp.web
 import pytest
 from aresponses import ResponsesMockServer
 from yarl import URL
 
 from instawow._sources.github import GithubResolver
-from instawow.common import Flavour
+from instawow.common import Defn, Flavour
 from instawow.manager import Manager
-from instawow.resolvers import Defn
 from instawow.results import PkgFilesNotMatching
 
 ADDON_NAME = 'RaidFadeMore'
 
 ZIPS = {
     'flavoured-toc-only': {
         'toc_files': {
@@ -67,15 +66,15 @@
     return {
         'addon': addon.getvalue(),
         'flavours': request.param['flavours'],
     }
 
 
 @pytest.mark.parametrize(
-    'iw_mock_aiohttp_requests',
+    '_iw_mock_aiohttp_requests',
     [
         {
             URL('//api.github.com/repos/ketho-wow/RaidFadeMore'),
             URL('//api.github.com/repos/ketho-wow/RaidFadeMore/releases?per_page=10'),
         }
     ],
     indirect=True,
```

### Comparing `instawow-2.1.1/tests/test_json_rpc_api.py` & `instawow-2.2.0/tests/test_json_rpc_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,16 @@
         'jsonrpc': '2.0',
         'method': 'install',
         'params': {},
         'id': request.node.name,
     }
     await ws.send_json(rpc_request, dumps=dumps)
     rpc_response = await ws.receive_json()
-    assert rpc_response['error'] and rpc_response['error']['code'] == -32602
+    assert rpc_response['error']
+    assert rpc_response['error']['code'] == -32602
 
 
 @pytest.mark.xfail
 async def test_install_with_uninitialised_profile(
     request: pytest.FixtureRequest,
     ws: ClientWebSocketResponse,
 ):
@@ -139,8 +140,9 @@
             'defns': [{'source': 'curse', 'name': 'molinari'}],
             'replace': False,
         },
         'id': request.node.name,
     }
     await ws.send_json(rpc_request, dumps=dumps)
     rpc_response = await ws.receive_json()
-    assert rpc_response['error'] and rpc_response['error']['code'] == -32001
+    assert rpc_response['error']
+    assert rpc_response['error']['code'] == -32001
```

### Comparing `instawow-2.1.1/tests/test_matchers.py` & `instawow-2.2.0/tests/test_matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import pytest
 
-from instawow.common import AddonHashMethod, Flavour
+from instawow.common import AddonHashMethod, Defn, Flavour
 from instawow.manager import Manager
 from instawow.matchers import (
     AddonFolder,
     Matcher,
     get_unreconciled_folders,
     match_addon_names_with_folder_names,
     match_folder_hashes,
     match_folder_name_subsets,
     match_toc_source_ids,
 )
-from instawow.resolvers import Defn
 
 MOLINARI_HASH = '2da096db5769138b5428a068343cddf3'
 
 
 def write_addons(iw_manager: Manager, *addons: str):
     for addon in addons:
         (iw_manager.config.addon_dir / addon).mkdir()
@@ -35,15 +34,15 @@
         toc_file.write(
             '''\
 ## X-Curse-Project-ID: 20338
 ## X-WoWI-ID: 13188
 ''',
         )
 
-    yield molinari_folder
+    return molinari_folder
 
 
 def test_can_extract_defns_from_addon_folder_toc(iw_manager: Manager, molinari: Path):
     addon_folder = AddonFolder.from_addon_path(iw_manager.config.game_flavour, molinari)
     assert addon_folder.get_defns_from_toc_keys(
         iw_manager.resolvers.addon_toc_key_and_id_pairs
     ) == {Defn('curse', '20338'), Defn('wowi', '13188')}
```

### Comparing `instawow-2.1.1/tests/test_utils.py` & `instawow-2.2.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     run_in_thread,
     tabulate,
 )
 
 
 @pytest.fixture
 def fake_addon_toc():
-    yield Path(__file__).parent / 'fixtures' / 'FakeAddon' / 'FakeAddon.toc'
+    return Path(__file__).parent / 'fixtures' / 'FakeAddon' / 'FakeAddon.toc'
 
 
 def test_find_addon_zip_tocs_can_find_explicit_dirs():
     assert {h for _, h in find_addon_zip_tocs(['b/', 'b/b.toc'])} == {'b'}
 
 
 def test_find_addon_zip_tocs_can_find_implicit_dirs():
```

### Comparing `instawow-2.1.1/tests/test_wa_updater.py` & `instawow-2.2.0/tests/test_wa_updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import pytest
 from yarl import URL
 
+from instawow.common import Defn
 from instawow.manager import Manager
 from instawow.models import Pkg
-from instawow.resolvers import Defn
 from instawow.wa_updater import WaCompanionBuilder, WeakAura, WeakAuras
 
 
 @pytest.fixture
-def wa_saved_vars(iw_manager: Manager):
+def _wa_saved_vars(iw_manager: Manager):
     saved_vars = (
         iw_manager.config.addon_dir.parents[1] / 'WTF' / 'Account' / 'test' / 'SavedVariables'
     )
     saved_vars.mkdir(parents=True)
     (saved_vars / WeakAuras.addon_name).with_suffix('.lua').write_text(
         '''\
 WeakAurasSaved = {
@@ -26,15 +26,15 @@
 }
 '''
     )
 
 
 @pytest.fixture
 def builder(iw_manager: Manager):
-    yield WaCompanionBuilder(iw_manager)
+    return WaCompanionBuilder(iw_manager)
 
 
 def test_can_parse_empty_displays_table(builder: WaCompanionBuilder):
     assert (
         builder.extract_auras(
             WeakAuras,
             '''\
@@ -117,17 +117,16 @@
     )
 
 
 def test_can_build_addon_with_empty_seq(builder: WaCompanionBuilder):
     builder._generate_addon([])
 
 
-async def test_can_build_addon_with_mock_saved_vars(
-    builder: WaCompanionBuilder, wa_saved_vars: None
-):
+@pytest.mark.usefixtures('_wa_saved_vars')
+async def test_can_build_addon_with_mock_saved_vars(builder: WaCompanionBuilder):
     await builder.build()
 
 
 def test_build_is_reproducible(builder: WaCompanionBuilder):
     builder._generate_addon([])
     checksum = builder.get_version()
     builder._generate_addon([])
@@ -135,18 +134,18 @@
 
 
 def test_changelog_is_generated(builder: WaCompanionBuilder):
     builder._generate_addon([])
     assert builder.changelog_path.read_text() == 'n/a'
 
 
-async def test_can_resolve_wa_companion_pkg(builder: WaCompanionBuilder):
+async def test_can_resolve_wa_companion_pkg(builder: WaCompanionBuilder, iw_manager: Manager):
     await builder.build()
     defn = Defn('instawow', 'weakauras-companion')
-    resolve_results = await builder._manager.resolve([defn])
+    resolve_results = await iw_manager.resolve([defn])
     assert type(resolve_results[defn]) is Pkg
 
 
-async def test_can_resolve_wa_companion_autoupdate_pkg(builder: WaCompanionBuilder):
+async def test_can_resolve_wa_companion_autoupdate_pkg(iw_manager: Manager):
     defn = Defn('instawow', 'weakauras-companion-autoupdate')
-    resolve_results = await builder._manager.resolve([defn])
+    resolve_results = await iw_manager.resolve([defn])
     assert type(resolve_results[defn]) is Pkg
```

### Comparing `instawow-2.1.1/setup.py` & `instawow-2.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,245 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: instawow
+Version: 2.2.0
+Summary: World of Warcraft add-on manager
+License: GPL-3.0-or-later
+Author: layday
+Author-email: layday@protonmail.com
+Requires-Python: >=3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: gui
+Provides-Extra: test
+Provides-Extra: types
+Requires-Dist: aiohttp (>=3.8.2,<4)
+Requires-Dist: aiohttp-client-cache (>=0.8.0)
+Requires-Dist: aiohttp-rpc (>=1.0.0) ; extra == "gui"
+Requires-Dist: alembic (>=1.9.0)
+Requires-Dist: anyio (>=3.6.2) ; extra == "gui"
+Requires-Dist: aresponses (>=2.1.4) ; extra == "test"
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: cattrs (>=22.2.0)
+Requires-Dist: click (>=8.1.0)
+Requires-Dist: coverage[toml] (>=6.2) ; extra == "test"
+Requires-Dist: exceptiongroup (>=1.0.0)
+Requires-Dist: iso8601 (>=1.0.2)
+Requires-Dist: loguru (>=0.7.0)
+Requires-Dist: mako (>=1.2.4)
+Requires-Dist: packaging (>=23.0)
+Requires-Dist: pluggy (>=0.13)
+Requires-Dist: prompt-toolkit (>=3.0.29,<4)
+Requires-Dist: pytest (>=6.2.5) ; extra == "test"
+Requires-Dist: pytest-asyncio (>=0.17.0) ; extra == "test"
+Requires-Dist: pytest-xdist (>=2.5.0) ; extra == "test"
+Requires-Dist: questionary (>=1.10)
+Requires-Dist: rapidfuzz (>=2.12.0)
+Requires-Dist: sqlalchemy (>=2.0.0)
+Requires-Dist: toga (>=0.3.0) ; extra == "gui"
+Requires-Dist: types-certifi ; extra == "types"
+Requires-Dist: typing-extensions (>=4.3.0)
+Requires-Dist: yarl (>=1.8.1)
+Project-URL: homepage, http://github.com/layday/instawow
+Description-Content-Type: text/x-rst
+
+*instawow*
+==========
+
+.. image:: https://img.shields.io/matrix/wow-addon-management:matrix.org
+   :target: https://matrix.to/#/#wow-addon-management:matrix.org?via=matrix.org
+   :alt: Matrix channel
+
+*instawow* is an add-on manager for World of Warcraft.
+It can be used to install, update and remove add-ons from GitHub,
+CurseForge, WoWInterface and Tukui.
+*instawow* has an interoperable CLI and GUI, fuzzy search with download scoring
+and several other goodies.
+
+.. list-table::
+   :widths: 50 50
+
+   * - .. figure:: https://asciinema.org/a/8m36ncAoyTmig4MXfQM8YjE6a.svg
+          :target: https://asciinema.org/a/8m36ncAoyTmig4MXfQM8YjE6a?autoplay=1
+          :alt: Asciicast demonstrating the operation of instawow
+          :width: 640
+     - .. figure:: https://raw.githubusercontent.com/layday/instawow/main/gui-webview/screenshots/v1.34.1.png
+          :target: https://github.com/layday/instawow/releases/latest
+          :alt: instawow-gui main window
+          :width: 640
+
+Installation
+------------
+
+You can download pre-built binaries of *instawow* from GitHub:
+
+- `Binaries <https://github.com/layday/instawow/releases/latest>`__
+
+If you'd prefer to install *instawow* from source, you are able to choose from:
+
+- `pipx <https://github.com/pipxproject/pipx>`__:
+  ``pipx install instawow`` or ``pipx install instawow[gui]`` for the GUI
+- Vanilla pip:
+  ``python -m pip install -U instawow`` or ``python -m pip install -U instawow[gui]`` for the GUI
+
+CLI operation
+-------------
+
+tl;dr
+~~~~~
+
+Begin by running ``instawow reconcile``
+to register previously-installed add-ons with *instawow*
+(or ``instawow reconcile --auto`` to do the same without user input).
+To install add-ons, you can search for them using the ``search`` command::
+
+    instawow search molinari
+
+In addition, *instawow* is able to interpret add-on URLs and *instawow*-specific
+URNs of slugs and host IDs.
+All of the following will install Molinari from CurseForge::
+
+    instawow install https://www.curseforge.com/wow/addons/molinari
+    instawow install curse:molinari
+    instawow install curse:20338
+
+You can ``update`` add-ons and ``remove`` them just as you'd install them.
+If ``update`` is invoked without arguments, it will update all of your
+installed add-ons.  You can ``list`` add-ons and view detailed information about
+them using ``list --format detailed``.
+For ``list`` and similarly non-destructive commands, the source can be omitted
+and the slug can be abbreviated, e.g. ``instawow reveal moli``
+will open the Molinari add-on folder in your file manager.
+
+Add-on reconciliation
+~~~~~~~~~~~~~~~~~~~~~
+
+Add-on reconciliation is not automatic – *instawow* makes a point
+of not automatically assuming ownership of your add-ons.
+However, you can automate reconciliation with ``reconcile --auto``
+and *instawow* will prioritise add-ons from CurseForge.
+Reconciled add-ons are reinstalled because the installed version cannot be
+extracted reliably.
+
+Add-on search
+~~~~~~~~~~~~~
+
+*instawow* comes with a rudimentary ``search`` command
+with results ranked based on edit distance and popularity.
+Search uses a collated add-on catalogue which is updated
+`once daily <https://github.com/layday/instawow-data/tree/data>`__.
+You can install multiple add-ons directly from search.
+
+Reverting add-on updates
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+*instawow* keeps a log of all versions of an add-on it has previously
+installed.
+Add-on updates can be undone using the ``instawow rollback`` command.
+Add-ons which have been rolled back are pinned and will not receive updates.
+Rollbacks can themselves be undone with ``instawow rollback --undo``,
+which will install the latest version of the specified add-on using
+the ``default`` strategy.
+
+Profiles
+~~~~~~~~
+
+*instawow* supports multiple game versions by means of profiles.
+Assuming your default profile is configured for retail,
+you can create a pristine profile for classic with::
+
+    instawow -p classic configure
+
+"``classic``" is simply the name of the profile; you will be asked to select
+the game flavour that it corresponds to.  You can have several profiles
+of the same flavour (think alpha, beta and PTR).
+
+``-p`` is a global option. You can prefix any *instawow* command with ``-p``.
+For instance, to update your Classic add-ons, you would run::
+
+    instawow -p classic update
+
+You can omit ``-p`` for the default profile if one exists.
+
+Migrating Classic profiles
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+With the exception of "Classic Era" profiles
+(``vanilla_classic`` in *instawow* parlance), classic profiles will start
+receiving updates for the latest Classic release once it is supported by
+*instawow*.  No user intervention is necessary, save for updating *instawow*.
+
+WeakAura updater
+~~~~~~~~~~~~~~~~
+
+*instawow* contains a WeakAura updater modelled after
+`WeakAuras Companion <https://weakauras.wtf/>`__.  To use the updater
+and provided that you have WeakAuras installed::
+
+    instawow weakauras-companion build
+    instawow install instawow:weakauras-companion
+
+You will have to rebuild the companion add-on prior to updating
+to receive aura updates.  If you would like to check for updates on
+every invocation of ``instawow update``, install the
+``instawow:weakauras-companion-autoupdate`` variant::
+
+    instawow install instawow:weakauras-companion-autoupdate
+    instawow update
+
+Plug-ins
+~~~~~~~~
+
+*instawow* can be extended using plug-ins.  Plug-ins can be used to add support
+for arbitrary hosts and add new commands to the CLI.  You will find a sample
+plug-in in ``tests/plugin``.
+
+Metadata sourcing
+-----------------
+
+CurseForge
+~~~~~~~~~~
+
+CurseForge is set to retire its unauthenticated add-on API by the end of Q1 2022.
+CurseForge will be issuing keys for the new API conditionally and which
+add-on managers are obligated to conceal.
+The new API is therefore unworkable for add-on managers except through a
+proxy service, which the author of this particular add-on manager cannot afford.
+At the same time, CurseForge will be providing the option for authors to unlist
+their add-ons from the new API, and downloads intitiated through the new API
+will not count towards author credits for the ad revenue sharing programme.
+
+GitHub
+~~~~~~
+
+*instawow* supports WoW add-ons *released* on GitHub – that is to say that
+the repository must have a release (tags won't work) and the release must
+have an add-on ZIP file attached to it as an asset.
+*instawow* will not install or build add-ons directly from
+source, or from tarballs or 'zipballs', and will not validate
+the contents of the ZIP file.
+
+Transparency
+------------
+
+Web requests initiated by *instawow* can be identified by its user agent string.
+
+Every 24 hours, on launch, *instawow* will query `PyPI <https://pypi.org>`__ –
+the canonical Python package index – to check for *instawow* updates.
+
+Contributing
+------------
+
+Bug reports and fixes are welcome.  Do open an issue before committing to
+making any significant changes.
+
+Related work
+------------
+
+The author of `strongbox <https://github.com/ogri-la/strongbox>`__ has been
+cataloguing similar software.  If you are unhappy
+with *instawow*, you might find one of these
+`other <https://ogri-la.github.io/wow-addon-managers/>`__ add-on managers more
+to your liking.
 
-package_dir = \
-{'': 'src',
- 'instawow_gui': 'gui-webview/src/instawow_gui',
- 'instawow_gui.frontend': 'gui-webview/src/instawow_gui/frontend',
- 'instawow_gui.resources': 'gui-webview/src/instawow_gui/resources'}
-
-packages = \
-['instawow',
- 'instawow._migrations',
- 'instawow._migrations.versions',
- 'instawow._sources',
- 'instawow._wa_templates',
- 'instawow_gui',
- 'instawow_gui.frontend',
- 'instawow_gui.resources']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp-client-cache>=0.7.3',
- 'aiohttp>=3.8.2,<4',
- 'alembic>=1.7.0',
- 'attrs>=22.1.0',
- 'cattrs>=22.2.0',
- 'click>=8.0.0',
- 'exceptiongroup>=1.0.0',
- 'iso8601>=1.0.2',
- 'loguru>=0.5.3',
- 'mako>=1.2.4',
- 'pluggy>=0.13',
- 'prompt-toolkit>=3.0.29,<4',
- 'questionary>=1.10',
- 'rapidfuzz>=2.12.0',
- 'sqlalchemy>=1.4.23',
- 'typing-extensions>=4.3.0',
- 'yarl>=1.8.1']
-
-extras_require = \
-{'gui': ['aiohttp-rpc>=1.0.0', 'toga>=0.3.0.dev33'],
- 'test': ['aresponses>=2.1.4',
-          'coverage[toml]>=6.2',
-          'pytest>=6.2.5',
-          'pytest-asyncio>=0.17.0',
-          'pytest-xdist>=2.5.0'],
- 'types': ['sqlalchemy2-stubs']}
-
-entry_points = \
-{'console_scripts': ['instawow = instawow.cli:main']}
-
-setup_kwargs = {
-    'name': 'instawow',
-    'version': '2.1.1',
-    'description': 'World of Warcraft add-on manager',
-    'long_description': '*instawow*\n==========\n\n.. image:: https://img.shields.io/matrix/wow-addon-management:matrix.org\n   :target: https://matrix.to/#/#wow-addon-management:matrix.org?via=matrix.org\n   :alt: Matrix channel\n\n*instawow* is an add-on manager for World of Warcraft.\nIt can be used to install, update and remove add-ons from GitHub,\nCurseForge, WoWInterface and Tukui.\n*instawow* has an interoperable CLI and GUI, fuzzy search with download scoring\nand several other goodies.\n\n.. list-table::\n   :widths: 50 50\n\n   * - .. figure:: https://asciinema.org/a/8m36ncAoyTmig4MXfQM8YjE6a.svg\n          :target: https://asciinema.org/a/8m36ncAoyTmig4MXfQM8YjE6a?autoplay=1\n          :alt: Asciicast demonstrating the operation of instawow\n          :width: 640\n     - .. figure:: https://raw.githubusercontent.com/layday/instawow/main/gui-webview/screenshots/v1.34.1.png\n          :target: https://github.com/layday/instawow/releases/latest\n          :alt: instawow-gui main window\n          :width: 640\n\nInstallation\n------------\n\nYou can download pre-built binaries of *instawow* from GitHub:\n\n- `Binaries <https://github.com/layday/instawow/releases/latest>`__\n\nIf you\'d prefer to install *instawow* from source, you are able to choose from:\n\n- `pipx <https://github.com/pipxproject/pipx>`__:\n  ``pipx install instawow`` or ``pipx install instawow[gui]`` for the GUI\n- Vanilla pip:\n  ``python -m pip install -U instawow`` or ``python -m pip install -U instawow[gui]`` for the GUI\n\nCLI operation\n-------------\n\ntl;dr\n~~~~~\n\nBegin by running ``instawow reconcile``\nto register previously-installed add-ons with *instawow*\n(or ``instawow reconcile --auto`` to do the same without user input).\nTo install add-ons, you can search for them using the ``search`` command::\n\n    instawow search molinari\n\nIn addition, *instawow* is able to interpret add-on URLs and *instawow*-specific\nURNs of slugs and host IDs.\nAll of the following will install Molinari from CurseForge::\n\n    instawow install https://www.curseforge.com/wow/addons/molinari\n    instawow install curse:molinari\n    instawow install curse:20338\n\nYou can ``update`` add-ons and ``remove`` them just as you\'d install them.\nIf ``update`` is invoked without arguments, it will update all of your\ninstalled add-ons.  You can ``list`` add-ons and view detailed information about\nthem using ``list --format detailed``.\nFor ``list`` and similarly non-destructive commands, the source can be omitted\nand the slug can be abbreviated, e.g. ``instawow reveal moli``\nwill open the Molinari add-on folder in your file manager.\n\nAdd-on reconciliation\n~~~~~~~~~~~~~~~~~~~~~\n\nAdd-on reconciliation is not automatic – *instawow* makes a point\nof not automatically assuming ownership of your add-ons.\nHowever, you can automate reconciliation with ``reconcile --auto``\nand *instawow* will prioritise add-ons from CurseForge.\nReconciled add-ons are reinstalled because the installed version cannot be\nextracted reliably.\n\nAdd-on search\n~~~~~~~~~~~~~\n\n*instawow* comes with a rudimentary ``search`` command\nwith results ranked based on edit distance and popularity.\nSearch uses a collated add-on catalogue which is updated\n`once daily <https://github.com/layday/instawow-data/tree/data>`__.\nYou can install multiple add-ons directly from search.\n\nReverting add-on updates\n~~~~~~~~~~~~~~~~~~~~~~~~\n\n*instawow* keeps a log of all versions of an add-on it has previously\ninstalled.\nAdd-on updates can be undone using the ``instawow rollback`` command.\nAdd-ons which have been rolled back are pinned and will not receive updates.\nRollbacks can themselves be undone with ``instawow rollback --undo``,\nwhich will install the latest version of the specified add-on using\nthe ``default`` strategy.\n\nProfiles\n~~~~~~~~\n\n*instawow* supports multiple game versions by means of profiles.\nAssuming your default profile is configured for retail,\nyou can create a pristine profile for classic with::\n\n    instawow -p classic configure\n\n"``classic``" is simply the name of the profile; you will be asked to select\nthe game flavour that it corresponds to.  You can have several profiles\nof the same flavour (think alpha, beta and PTR).\n\n``-p`` is a global option. You can prefix any *instawow* command with ``-p``.\nFor instance, to update your Classic add-ons, you would run::\n\n    instawow -p classic update\n\nYou can omit ``-p`` for the default profile if one exists.\n\nMigrating Classic profiles\n^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nWith the exception of "Classic Era" profiles\n(``vanilla_classic`` in *instawow* parlance), classic profiles will start\nreceiving updates for the latest Classic release once it is supported by\n*instawow*.  No user intervention is necessary, save for updating *instawow*.\n\nWeakAura updater\n~~~~~~~~~~~~~~~~\n\n*instawow* contains a WeakAura updater modelled after\n`WeakAuras Companion <https://weakauras.wtf/>`__.  To use the updater\nand provided that you have WeakAuras installed::\n\n    instawow weakauras-companion build\n    instawow install instawow:weakauras-companion\n\nYou will have to rebuild the companion add-on prior to updating\nto receive aura updates.  If you would like to check for updates on\nevery invocation of ``instawow update``, install the\n``instawow:weakauras-companion-autoupdate`` variant::\n\n    instawow install instawow:weakauras-companion-autoupdate\n    instawow update\n\nPlug-ins\n~~~~~~~~\n\n*instawow* can be extended using plug-ins.  Plug-ins can be used to add support\nfor arbitrary hosts and add new commands to the CLI.  You will find a sample\nplug-in in ``tests/plugin``.\n\nMetadata sourcing\n-----------------\n\nCurseForge\n~~~~~~~~~~\n\nCurseForge is set to retire its unauthenticated add-on API by the end of Q1 2022.\nCurseForge will be issuing keys for the new API conditionally and which\nadd-on managers are obligated to conceal.\nThe new API is therefore unworkable for add-on managers except through a\nproxy service, which the author of this particular add-on manager cannot afford.\nAt the same time, CurseForge will be providing the option for authors to unlist\ntheir add-ons from the new API, and downloads intitiated through the new API\nwill not count towards author credits for the ad revenue sharing programme.\n\nGitHub\n~~~~~~\n\n*instawow* supports WoW add-ons *released* on GitHub – that is to say that\nthe repository must have a release (tags won\'t work) and the release must\nhave an add-on ZIP file attached to it as an asset.\n*instawow* will not install or build add-ons directly from\nsource, or from tarballs or \'zipballs\', and will not validate\nthe contents of the ZIP file.\n\nTransparency\n------------\n\nWeb requests initiated by *instawow* can be identified by its user agent string.\n\nEvery 24 hours, on launch, *instawow* will query `PyPI <https://pypi.org>`__ –\nthe canonical Python package index – to check for *instawow* updates.\n\nContributing\n------------\n\nBug reports and fixes are welcome.  Do open an issue before committing to\nmaking any significant changes.\n\nRelated work\n------------\n\nThe author of `strongbox <https://github.com/ogri-la/strongbox>`__ has been\ncataloguing similar software.  If you are unhappy\nwith *instawow*, you might find one of these\n`other <https://ogri-la.github.io/wow-addon-managers/>`__ add-on managers more\nto your liking.\n',
-    'author': 'layday',
-    'author_email': 'layday@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9',
-}
-
-
-setup(**setup_kwargs)
```

