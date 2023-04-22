# Comparing `tmp/OctoBot-Backtesting-1.8.1.tar.gz` & `tmp/OctoBot-Backtesting-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Backtesting-1.8.1.tar", last modified: Mon Apr 17 16:53:37 2023, max compression
+gzip compressed data, was "OctoBot-Backtesting-1.8.2.tar", last modified: Sat Apr 22 08:49:51 2023, max compression
```

## Comparing `OctoBot-Backtesting-1.8.1.tar` & `OctoBot-Backtesting-1.8.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.566236 OctoBot-Backtesting-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.554236 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/exchange_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:53:37.566236 OctoBot-Backtesting-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.554236 OctoBot-Backtesting-1.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_data_file_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_exchange_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/importers/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/importers/test_exchange_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/producers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/util/test_backtesting_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-22 08:49:51.000000 OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/octobot_backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/exchange_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/api/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.317968 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.321968 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.313968 OctoBot-Backtesting-1.8.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_data_file_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_exchange_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/api/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/importers/test_exchange_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/producers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:51.325968 OctoBot-Backtesting-1.8.2/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-22 08:49:08.000000 OctoBot-Backtesting-1.8.2/tests/util/test_backtesting_util.py
```

### Comparing `OctoBot-Backtesting-1.8.1/CHANGELOG.md` & `OctoBot-Backtesting-1.8.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.8.2] - 2022-04-21
+### Updated
+- [ExchangeCollector] handle exchange credentials
+
 ## [1.8.1] - 2022-04-17
 ### Updated
 - [ExchangeCollector] delete_all
 
 ## [1.8.0] - 2022-12-23
 ### Updated
 - [ChannelsManager] drop unused producers and priority levels
```

### Comparing `OctoBot-Backtesting-1.8.1/LICENSE` & `OctoBot-Backtesting-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/PKG-INFO` & `OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: OctoBot-Backtesting
-Version: 1.8.1
+Version: 1.8.2
 Summary: OctoBot project backtesting engine
 Home-page: https://github.com/Drakkar-Software/OctoBot-Backtesting
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/SOURCES.txt` & `OctoBot-Backtesting-1.8.2/OctoBot_Backtesting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/PKG-INFO` & `OctoBot-Backtesting-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: OctoBot-Backtesting
-Version: 1.8.1
+Version: 1.8.2
 Summary: OctoBot project backtesting engine
 Home-page: https://github.com/Drakkar-Software/OctoBot-Backtesting
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `OctoBot-Backtesting-1.8.1/README.md` & `OctoBot-Backtesting-1.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Backtesting [1.8.1](https://github.com/Drakkar-Software/OctoBot-Backtesting/blob/master/CHANGELOG.md)
+# OctoBot-Backtesting [1.8.2](https://github.com/Drakkar-Software/OctoBot-Backtesting/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/aa0b156e99604b3c98923fffeaea6a49)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Backtesting?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Backtesting&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Backtesting.svg)](https://pypi.python.org/pypi/OctoBot-Backtesting/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Backtesting/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Backtesting?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Backtesting/workflows/OctoBot-Backtesting-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Backtesting/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Backtesting/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Backtesting)
 
 OctoBot backtesting engine package.
```

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import logging
 
 PROJECT_NAME = "OctoBot-Backtesting"
-VERSION = "1.8.1"
+VERSION = "1.8.2"
 
 logging.getLogger('aiosqlite').setLevel(logging.ERROR)
```

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/backtesting.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file_converters.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/data_file_converters.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/exchange_data_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/exchange_data_collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,48 +19,53 @@
 
 def exchange_historical_data_collector_factory(exchange_name,
                                                exchange_type,
                                                tentacles_setup_config,
                                                symbols,
                                                time_frames=None,
                                                start_timestamp=None,
-                                               end_timestamp=None):
+                                               end_timestamp=None,
+                                               config=None):
     return _exchange_collector_factory(collectors.AbstractExchangeHistoryCollector,
                                        exchange_name,
                                        exchange_type,
                                        tentacles_setup_config,
                                        symbols,
                                        time_frames,
                                        start_timestamp,
-                                       end_timestamp)
+                                       end_timestamp,
+                                       config)
 
 
 def exchange_bot_snapshot_data_collector_factory(exchange_name,
                                                  tentacles_setup_config,
                                                  symbols,
                                                  exchange_id,
                                                  time_frames=None,
                                                  start_timestamp=None,
-                                                 end_timestamp=None):
+                                                 end_timestamp=None,
+                                                 config=None):
     collector = _exchange_collector_factory(collectors.AbstractExchangeBotSnapshotCollector,
                                             exchange_name,
                                             None,
                                             tentacles_setup_config,
                                             symbols,
                                             time_frames,
                                             start_timestamp,
-                                            end_timestamp)
+                                            end_timestamp,
+                                            config)
     collector.register_exchange_id(exchange_id)
     return collector
 
 
 def _exchange_collector_factory(collector_parent_class, exchange_name, exchange_type, tentacles_setup_config, symbols,
-                                time_frames, start_timestamp, end_timestamp):
+                                time_frames, start_timestamp, end_timestamp, config):
     collector_class = tentacles_management.get_single_deepest_child_class(collector_parent_class)
-    collector_instance = collector_class({}, exchange_name, exchange_type, tentacles_setup_config, symbols, time_frames,
+    collector_instance = collector_class(config or {}, exchange_name, exchange_type,
+                                         tentacles_setup_config, symbols, time_frames,
                                          use_all_available_timeframes=time_frames is None,
                                          start_timestamp=start_timestamp, end_timestamp=end_timestamp)
     return collector_instance
 
 
 async def initialize_and_run_data_collector(data_collector):
     await data_collector.initialize()
```

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/importer.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/api/importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtest_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/channels_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/data_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
+import copy
 import json
 import os.path as path
 import os
 import time
 
 import aiohttp
 
@@ -32,15 +33,15 @@
 
 class DataCollector:
     IMPORTER = importers.DataImporter
 
     def __init__(self, config,
                  path=constants.BACKTESTING_FILE_PATH,
                  data_format=enums.DataFormats.REGULAR_COLLECTOR_DATA):
-        self.config = config
+        self.config = copy.deepcopy(config)
         self.path = path
         self.logger = logging.get_logger(self.__class__.__name__)
 
         self.should_stop = False
         self.file_name = data.get_backtesting_file_name(self.__class__,
                                                         self.get_file_identifier,
                                                         data_format=data_format)
```

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/exchanges/exchange_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,17 @@
 
     async def initialize(self):
         self.create_database()
         await self.database.initialize()
 
         # set config from params
         self.config[commons_constants.CONFIG_TIME_FRAME] = self.time_frames
-        self.config[commons_constants.CONFIG_EXCHANGES] = {self.exchange_name: {}}
+        # get exchange credentials if available
+        existing_exchange_config = self.config.get(commons_constants.CONFIG_EXCHANGES, {}).get(self.exchange_name, {})
+        self.config[commons_constants.CONFIG_EXCHANGES] = {self.exchange_name: existing_exchange_config}
         self.config[commons_constants.CONFIG_CRYPTO_CURRENCIES] = {"Symbols": {
             commons_constants.CONFIG_CRYPTO_PAIRS: [str(symbol) for symbol in self.symbols]}}
 
     def _load_timeframes_if_necessary(self):
         if self.use_all_available_timeframes:
             self._load_all_available_timeframes()
         self.config[commons_constants.CONFIG_TIME_FRAME] = self.time_frames
```

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/collectors/social/social_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/constants.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/converters/data_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/data/data_file_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/enums.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/errors.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/data_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/exchange_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/exchanges/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/importers/social/social_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/channel/time_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/time/time_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/util/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.pxd` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.py` & `OctoBot-Backtesting-1.8.2/octobot_backtesting/util/backtesting_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/setup.py` & `OctoBot-Backtesting-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/api/__init__.py` & `OctoBot-Backtesting-1.8.2/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/api/test_backtesting.py` & `OctoBot-Backtesting-1.8.2/tests/api/test_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/api/test_data_file.py` & `OctoBot-Backtesting-1.8.2/tests/api/test_data_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/api/test_data_file_converters.py` & `OctoBot-Backtesting-1.8.2/tests/api/test_data_file_converters.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/api/test_exchange_data_collector.py` & `OctoBot-Backtesting-1.8.2/tests/api/test_exchange_data_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/api/test_importer.py` & `OctoBot-Backtesting-1.8.2/tests/api/test_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/importers/__init__.py` & `OctoBot-Backtesting-1.8.2/tests/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/importers/test_exchange_importer.py` & `OctoBot-Backtesting-1.8.2/tests/importers/test_exchange_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/producers/__init__.py` & `OctoBot-Backtesting-1.8.2/tests/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/util/__init__.py` & `OctoBot-Backtesting-1.8.2/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.1/tests/util/test_backtesting_util.py` & `OctoBot-Backtesting-1.8.2/tests/util/test_backtesting_util.py`

 * *Files identical despite different names*

