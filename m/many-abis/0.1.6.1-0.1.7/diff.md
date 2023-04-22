# Comparing `tmp/many_abis-0.1.6.1.tar.gz` & `tmp/many_abis-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many_abis-0.1.6.1.tar", last modified: Sun Apr  9 16:28:05 2023, max compression
+gzip compressed data, was "many_abis-0.1.7.tar", last modified: Sat Apr 22 05:36:07 2023, max compression
```

## Comparing `many_abis-0.1.6.1.tar` & `many_abis-0.1.7.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/abis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.850290 many_abis-0.1.6.1/many_abis/assets/dex/aave/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/atoken.abi
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_core.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/collector.abi
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/incentives_controller.abi
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/pool_admin.abi
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/price_oracle.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/protocal_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/weth_gateway.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.850290 many_abis-0.1.6.1/many_abis/assets/dex/joe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/pair.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/pancake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi
--rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/master_chef_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)    24647 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter.abi
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter_v2.abi
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/router_v3.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/self_permit.abi
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/staker.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/bsc/
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/bsc/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/exchange.abi
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/factory.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.858290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/pair.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/factory.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/multicall.abi
--rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi
--rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/pool.abi
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/quoter.abi
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/router.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/erc/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC1155.abi
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC20.abi
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC721.abi
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/erc/ERC777.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/tokens/
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/tokens/weth9.abi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/many_abis/assets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/assets/utils/chains.json
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/many_abis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:28:05.854290 many_abis-0.1.6.1/many_abis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 16:28:05.000000 many_abis-0.1.6.1/many_abis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:28:05.862290 many_abis-0.1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-09 16:27:52.000000 many_abis-0.1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-22 05:36:07.493439 many_abis-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-22 05:35:53.000000 many_abis-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/abis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/aave/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/aave/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/atoken.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool_core.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/aave/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/collector.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/incentives_controller.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    34411 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/pool_admin.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/price_oracle.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/protocal_data_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/aave/v2/weth_gateway.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/joe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/joe/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/joe/v2/factory.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/joe/v2/pair.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/joe/v2/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/pancake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/master_chef_v3.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    24647 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/pool_v3.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/quoter.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/quoter_v2.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/router_v3.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/self_permit.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/pancake/v3/staker.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis/assets/dex/uniswap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/uniswap/bsc/
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/bsc/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.489439 many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/exchange.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/factory.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/factory.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/pair.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/factory.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/multicall.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/pool.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/quoter.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/router.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/erc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC1155.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC20.abi
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC721.abi
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/erc/ERC777.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/tokens/weth9.abi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.493439 many_abis-0.1.7/many_abis/assets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    21093 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/assets/utils/chains.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 05:35:53.000000 many_abis-0.1.7/many_abis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:36:07.485439 many_abis-0.1.7/many_abis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 05:36:07.000000 many_abis-0.1.7/many_abis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 05:36:07.493439 many_abis-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-22 05:35:53.000000 many_abis-0.1.7/setup.py
```

### Comparing `many_abis-0.1.6.1/PKG-INFO` & `many_abis-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: many_abis
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: A simple way to get different DEXs abis for block chains.
 Home-page: https://github.com/ackness/many_abis
 Author: Yong
 Author-email: ackness8@gmail.com
 License: MIT
 Keywords: abi,dex,block chain,bsc,eth,matic,heco,kcc,pancakeswap,mdex,quickswap,uniswap,koffeeswap
 Description-Content-Type: text/markdown
 
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.6.1-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.7-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
 
@@ -23,17 +23,17 @@
 
 ---
 
 Now we support dex:
 
 ---
 
-- arbitrum-one:
+- arbitrum:
   - [1] [SushiSwap](https://app.sushi.com/en/swap)
-- avax-c:
+- avalanche:
   - [1] [traderjoexyz](https://traderjoexyz.com/#/home)
 - bsc:
   - [1] [ApeSwap Finance](https://app.apeswap.finance/swap)
   - [2] [BiSwap](https://exchange.biswap.org/#/swap)
   - [3] [MDEX (BSC)](https://bsc.mdex.co/#/swap/)
   - [4] [PancakeSwap v2](https://pancakeswap.finance/swap)
   - [5] [PancakeSwap v3](https://pancakeswap.finance/swap)
@@ -51,15 +51,15 @@
   - [2] [SpookySwap](https://spookyswap.finance/)
 - heco:
   - [1] [MDEX (HECO)](https://ht.mdex.co/#/swap/)
 - kcc:
   - [1] [KoffeeSwap](https://koffeeswap.exchange/)
 - moonriver:
   - [1] [Solarbeam](https://app.solarbeam.io/exchange/swap)
-- okex:
+- okx:
   - [1] [CherrySwap](https://www.cherryswap.net/)
 - polygon:
   - [1] [QuickSwap](https://quickswap.exchange/)
 - optimism:
   - [1] [Uniswap V3](https://app.uniswap.org/#/swap)
   - [2] [Velodrome V1](https://app.velodrome.finance/swap)
 
@@ -105,15 +105,15 @@
     ma.CHAIN_CONTRACT_API.BSC
 )
 
 # ======================================================================
 # chains
 chains = ma.all_chains()
 print(chains)
-# ['arbitrum-one', 'avax-c', 'bsc', 'bsc-test', 'cronos', 'eth', 'fantom', 'heco', 'kcc', 'moonriver', 'okex', 'polygon']
+# ['arbitrum', 'avalanche', 'bsc', 'bsc-test', 'cronos', 'eth', 'fantom', 'heco', 'kcc', 'moonriver', 'okx', 'polygon', 'optimism']
 
 # different methods to get chain
 bsc = ma.get_chain_by_id(chain_id=56)
 bsc = ma.get_chain_by_name(name="bsc")
 bsc = ma.get_chain(name="bsc")
 bsc = ma.get_chain(chain_id=56)
 bsc = ma.chain(name="bsc")
```

### Comparing `many_abis-0.1.6.1/README.md` & `many_abis-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.6.1-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.7-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
 
@@ -12,17 +12,17 @@
 
 ---
 
 Now we support dex:
 
 ---
 
-- arbitrum-one:
+- arbitrum:
   - [1] [SushiSwap](https://app.sushi.com/en/swap)
-- avax-c:
+- avalanche:
   - [1] [traderjoexyz](https://traderjoexyz.com/#/home)
 - bsc:
   - [1] [ApeSwap Finance](https://app.apeswap.finance/swap)
   - [2] [BiSwap](https://exchange.biswap.org/#/swap)
   - [3] [MDEX (BSC)](https://bsc.mdex.co/#/swap/)
   - [4] [PancakeSwap v2](https://pancakeswap.finance/swap)
   - [5] [PancakeSwap v3](https://pancakeswap.finance/swap)
@@ -40,15 +40,15 @@
   - [2] [SpookySwap](https://spookyswap.finance/)
 - heco:
   - [1] [MDEX (HECO)](https://ht.mdex.co/#/swap/)
 - kcc:
   - [1] [KoffeeSwap](https://koffeeswap.exchange/)
 - moonriver:
   - [1] [Solarbeam](https://app.solarbeam.io/exchange/swap)
-- okex:
+- okx:
   - [1] [CherrySwap](https://www.cherryswap.net/)
 - polygon:
   - [1] [QuickSwap](https://quickswap.exchange/)
 - optimism:
   - [1] [Uniswap V3](https://app.uniswap.org/#/swap)
   - [2] [Velodrome V1](https://app.velodrome.finance/swap)
 
@@ -94,15 +94,15 @@
     ma.CHAIN_CONTRACT_API.BSC
 )
 
 # ======================================================================
 # chains
 chains = ma.all_chains()
 print(chains)
-# ['arbitrum-one', 'avax-c', 'bsc', 'bsc-test', 'cronos', 'eth', 'fantom', 'heco', 'kcc', 'moonriver', 'okex', 'polygon']
+# ['arbitrum', 'avalanche', 'bsc', 'bsc-test', 'cronos', 'eth', 'fantom', 'heco', 'kcc', 'moonriver', 'okx', 'polygon', 'optimism']
 
 # different methods to get chain
 bsc = ma.get_chain_by_id(chain_id=56)
 bsc = ma.get_chain_by_name(name="bsc")
 bsc = ma.get_chain(name="bsc")
 bsc = ma.get_chain(chain_id=56)
 bsc = ma.chain(name="bsc")
```

### Comparing `many_abis-0.1.6.1/many_abis/abis.py` & `many_abis-0.1.7/many_abis/abis.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/atoken.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v1/atoken.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool_addresses_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v1/lending_pool_core.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v1/lending_pool_core.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/collector.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/collector.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/incentives_controller.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/incentives_controller.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_addresses_provider_registry.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_collateral_manager.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_pool_configurator.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/lending_rate_oracle.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/pool_admin.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/pool_admin.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/price_oracle.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/price_oracle.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/protocal_data_provider.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/protocal_data_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/ui_incentive_data_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/ui_pool_data_provider.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/aave/v2/weth_gateway.abi` & `many_abis-0.1.7/many_abis/assets/dex/aave/v2/weth_gateway.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/factory.abi` & `many_abis-0.1.7/many_abis/assets/dex/joe/v2/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/pair.abi` & `many_abis-0.1.7/many_abis/assets/dex/joe/v2/pair.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/joe/v2/router.abi` & `many_abis-0.1.7/many_abis/assets/dex/joe/v2/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/master_chef_v3.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/master_chef_v3.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/quoter.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/quoter_v2.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/quoter_v2.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/router_v3.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/router_v3.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/self_permit.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/self_permit.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/pancake/v3/staker.abi` & `many_abis-0.1.7/many_abis/assets/dex/pancake/v3/staker.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/bsc/router.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/bsc/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/exchange.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/exchange.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v1/factory.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v1/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/factory.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/pair.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/pair.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v2/router.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v2/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/factory.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/factory.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/multicall.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/multicall.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/non_fungible_position_manage.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/pool.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/pool.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/quoter.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/quoter.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/dex/uniswap/v3/router.abi` & `many_abis-0.1.7/many_abis/assets/dex/uniswap/v3/router.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/erc/ERC1155.abi` & `many_abis-0.1.7/many_abis/assets/erc/ERC1155.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/erc/ERC20.abi` & `many_abis-0.1.7/many_abis/assets/erc/ERC20.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/erc/ERC721.abi` & `many_abis-0.1.7/many_abis/assets/erc/ERC721.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/erc/ERC777.abi` & `many_abis-0.1.7/many_abis/assets/erc/ERC777.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/tokens/weth9.abi` & `many_abis-0.1.7/many_abis/assets/tokens/weth9.abi`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/assets/utils/chains.json` & `many_abis-0.1.7/many_abis/assets/utils/chains.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'arbitrum'": "OrderedDict([('chain_id', 42161), ('charts', OrderedDict([('Sell/Buy On "*

 * *               "SushiSwap', 'https://app.sushi.com/en/swap'), ('SushiSwap', "*

 * *               "'https://app.sushi.com/en/swap'), ('default', "*

 * *               "'https://dexscreener.com/arbitrum/{lp_address}'), ('dexscreener', "*

 * *               "'https://dexscreener.com/arbitrum/{lp_address}')])), ('dex', "*

 * *               "OrderedDict([('sushi', OrderedDict([('factory_address', "*

 * *               "'0xc35DADB65012eC5796536bD9 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "arbitrum-one": {
+    "arbitrum": {
         "chain_id": 42161,
         "charts": {
             "Sell/Buy On SushiSwap": "https://app.sushi.com/en/swap",
             "SushiSwap": "https://app.sushi.com/en/swap",
             "default": "https://dexscreener.com/arbitrum/{lp_address}",
             "dexscreener": "https://dexscreener.com/arbitrum/{lp_address}"
         },
@@ -31,15 +31,15 @@
         },
         "weth": {
             "address": "0x82aF49447D8a07e3bd95BD0d56f35241523fBab1",
             "name": "Wrapped ETH",
             "symbol": "WETH"
         }
     },
-    "avax-c": {
+    "avalanche": {
         "chain_id": 43114,
         "charts": {
             "ChartEX": "https://chartex.pro/dashboard",
             "Sell/Buy On traderjoexyz": "https://traderjoexyz.com/#/trade",
             "default": "https://dexscreener.com/avalanche/{lp_address}",
             "dexscreener": "https://dexscreener.com/avalanche/{lp_address}"
         },
@@ -442,15 +442,15 @@
         },
         "weth": {
             "address": "0x98878B06940aE243284CA214f92Bb71a2b032B8A",
             "name": "Wrapped MOVR",
             "symbol": "WMOVR"
         }
     },
-    "okex": {
+    "okx": {
         "chain_id": 66,
         "charts": {
             "Sell/Buy On CherrySwap": "https://www.cherryswap.net/#/swap?outputCurrency={address}",
             "default": "https://dexscreener.com/oec/{lp_address}",
             "dexscreener": "https://dexscreener.com/oec/{lp_address}"
         },
         "dex": {
```

### Comparing `many_abis-0.1.6.1/many_abis/chains.py` & `many_abis-0.1.7/many_abis/chains.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/constants.py` & `many_abis-0.1.7/many_abis/constants.py`

 * *Files identical despite different names*

### Comparing `many_abis-0.1.6.1/many_abis/utils.py` & `many_abis-0.1.7/many_abis/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,7 +30,13 @@
 
 def print_all_dex():
     from .chains import CHAINS
     for name, chain in CHAINS.items():
         print(f"- {name}:")
         for j, (d_name, dex) in enumerate(chain.dex.items()):
             print(f"  - [{j + 1}] [{dex.name}]({dex.website})")
+
+
+def supported_abis():
+    from .abis import ALL_ABIS_NAME
+    # print(ALL_ABIS_NAME)
+    return ALL_ABIS_NAME
```

### Comparing `many_abis-0.1.6.1/many_abis.egg-info/PKG-INFO` & `many_abis-0.1.7/many_abis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: many-abis
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: A simple way to get different DEXs abis for block chains.
 Home-page: https://github.com/ackness/many_abis
 Author: Yong
 Author-email: ackness8@gmail.com
 License: MIT
 Keywords: abi,dex,block chain,bsc,eth,matic,heco,kcc,pancakeswap,mdex,quickswap,uniswap,koffeeswap
 Description-Content-Type: text/markdown
 
 # Many Abis
 
-![Version](https://img.shields.io/badge/many--abis-v0.1.6.1-green)
+![Version](https://img.shields.io/badge/many--abis-v0.1.7-green)
 ![Pypi](https://img.shields.io/pypi/dm/many-abis)
 
 ![GitHub Org's stars](https://img.shields.io/github/stars/ackness/many_abis?style=social)
 ![GitHub forks](https://img.shields.io/github/forks/ackness/many_abis?style=social)
 
 ---
 
@@ -23,17 +23,17 @@
 
 ---
 
 Now we support dex:
 
 ---
 
-- arbitrum-one:
+- arbitrum:
   - [1] [SushiSwap](https://app.sushi.com/en/swap)
-- avax-c:
+- avalanche:
   - [1] [traderjoexyz](https://traderjoexyz.com/#/home)
 - bsc:
   - [1] [ApeSwap Finance](https://app.apeswap.finance/swap)
   - [2] [BiSwap](https://exchange.biswap.org/#/swap)
   - [3] [MDEX (BSC)](https://bsc.mdex.co/#/swap/)
   - [4] [PancakeSwap v2](https://pancakeswap.finance/swap)
   - [5] [PancakeSwap v3](https://pancakeswap.finance/swap)
@@ -51,15 +51,15 @@
   - [2] [SpookySwap](https://spookyswap.finance/)
 - heco:
   - [1] [MDEX (HECO)](https://ht.mdex.co/#/swap/)
 - kcc:
   - [1] [KoffeeSwap](https://koffeeswap.exchange/)
 - moonriver:
   - [1] [Solarbeam](https://app.solarbeam.io/exchange/swap)
-- okex:
+- okx:
   - [1] [CherrySwap](https://www.cherryswap.net/)
 - polygon:
   - [1] [QuickSwap](https://quickswap.exchange/)
 - optimism:
   - [1] [Uniswap V3](https://app.uniswap.org/#/swap)
   - [2] [Velodrome V1](https://app.velodrome.finance/swap)
 
@@ -105,15 +105,15 @@
     ma.CHAIN_CONTRACT_API.BSC
 )
 
 # ======================================================================
 # chains
 chains = ma.all_chains()
 print(chains)
-# ['arbitrum-one', 'avax-c', 'bsc', 'bsc-test', 'cronos', 'eth', 'fantom', 'heco', 'kcc', 'moonriver', 'okex', 'polygon']
+# ['arbitrum', 'avalanche', 'bsc', 'bsc-test', 'cronos', 'eth', 'fantom', 'heco', 'kcc', 'moonriver', 'okx', 'polygon', 'optimism']
 
 # different methods to get chain
 bsc = ma.get_chain_by_id(chain_id=56)
 bsc = ma.get_chain_by_name(name="bsc")
 bsc = ma.get_chain(name="bsc")
 bsc = ma.get_chain(chain_id=56)
 bsc = ma.chain(name="bsc")
```

### Comparing `many_abis-0.1.6.1/many_abis.egg-info/SOURCES.txt` & `many_abis-0.1.7/many_abis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 many_abis/assets/dex/aave/v2/weth_gateway.abi
 many_abis/assets/dex/joe/v2/factory.abi
 many_abis/assets/dex/joe/v2/pair.abi
 many_abis/assets/dex/joe/v2/router.abi
 many_abis/assets/dex/pancake/v3/IPeriphery_payments_with_fee.abi
 many_abis/assets/dex/pancake/v3/master_chef_v3.abi
 many_abis/assets/dex/pancake/v3/non_fungible_position_manager.abi
+many_abis/assets/dex/pancake/v3/pool_v3.abi
 many_abis/assets/dex/pancake/v3/quoter.abi
 many_abis/assets/dex/pancake/v3/quoter_v2.abi
 many_abis/assets/dex/pancake/v3/router_v3.abi
 many_abis/assets/dex/pancake/v3/self_permit.abi
 many_abis/assets/dex/pancake/v3/staker.abi
 many_abis/assets/dex/uniswap/bsc/router.abi
 many_abis/assets/dex/uniswap/v1/exchange.abi
```

### Comparing `many_abis-0.1.6.1/setup.py` & `many_abis-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # print(find_packages())
 setup(
     name='many_abis',
     packages=['many_abis'],
     package_dir={'many_abis': 'many_abis'},
     package_data={'': [
         '**/*.abi', '**/*.json']},
-    version='0.1.6.1',
+    version='0.1.7',
     license='MIT',
     description='A simple way to get different DEXs abis for block chains.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Yong',
     author_email='ackness8@gmail.com',
     url='https://github.com/ackness/many_abis',
```

