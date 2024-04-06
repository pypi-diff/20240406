# Comparing `tmp/sybil_engine-6.6.0.tar.gz` & `tmp/sybil_engine-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil_engine-6.6.0.tar", last modified: Sat Apr  6 12:02:45 2024, max compression
+gzip compressed data, was "sybil_engine-6.6.1.tar", last modified: Sat Apr  6 12:04:10 2024, max compression
```

## Comparing `sybil_engine-6.6.0.tar` & `sybil_engine-6.6.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.055930 sybil_engine-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-06 12:02:45.055930 sybil_engine-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:02:45.055930 sybil_engine-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.039930 sybil_engine-6.6.0/sybil_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.039930 sybil_engine-6.6.0/sybil_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/config/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.043930 sybil_engine-6.6.0/sybil_engine/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/erc20_test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/erc20contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/transaction_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/contract/weth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.043930 sybil_engine-6.6.0/sybil_engine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/data/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/data/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/data/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/data/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/data/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.043930 sybil_engine-6.6.0/sybil_engine/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/account_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.043930 sybil_engine-6.6.0/sybil_engine/domain/balance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/balance/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/balance/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/dex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/domain/generic_swap_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.043930 sybil_engine-6.6.0/sybil_engine/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/module/execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/module/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/module/module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/module/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.047930 sybil_engine-6.6.0/sybil_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/app_account_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/arguments_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/binance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/cex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/fee_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/gas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/l0_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/okx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/scal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/validation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/wallet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/sybil_engine/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.051930 sybil_engine-6.6.0/sybil_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-06 12:02:45.000000 sybil_engine-6.6.0/sybil_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-06 12:02:45.000000 sybil_engine-6.6.0/sybil_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:02:45.000000 sybil_engine-6.6.0/sybil_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 12:02:45.000000 sybil_engine-6.6.0/sybil_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 12:02:45.000000 sybil_engine-6.6.0/sybil_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.047930 sybil_engine-6.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.051930 sybil_engine-6.6.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/data/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/data/test_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.051930 sybil_engine-6.6.0/test/module/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.051930 sybil_engine-6.6.0/test/module/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/contract/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/mock_fail_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/mock_not_enoguth_native_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/repeatable_mock_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.051930 sybil_engine-6.6.0/test/module/swap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/swap/mock_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/swap/mock_test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/swap/test_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/swap/test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/test_execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/test_module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/module/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:45.051930 sybil_engine-6.6.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/utils/test_binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/utils/test_create_app_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 12:02:37.000000 sybil_engine-6.6.0/test/utils/test_validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.579858 sybil_engine-6.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-06 12:04:10.579858 sybil_engine-6.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:04:10.579858 sybil_engine-6.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.567858 sybil_engine-6.6.1/sybil_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.567858 sybil_engine-6.6.1/sybil_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/config/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.567858 sybil_engine-6.6.1/sybil_engine/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/erc20_test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/erc20contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/transaction_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/contract/weth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.567858 sybil_engine-6.6.1/sybil_engine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/data/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/data/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/data/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/data/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/data/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.571858 sybil_engine-6.6.1/sybil_engine/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/account_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.571858 sybil_engine-6.6.1/sybil_engine/domain/balance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/balance/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/balance/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/domain/generic_swap_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.571858 sybil_engine-6.6.1/sybil_engine/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/module/execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/module/module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/module/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.575858 sybil_engine-6.6.1/sybil_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/app_account_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/arguments_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/binance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/cex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/fee_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-06 12:04:05.000000 sybil_engine-6.6.1/sybil_engine/utils/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/gas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/l0_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/okx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/scal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/validation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/wallet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/sybil_engine/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.579858 sybil_engine-6.6.1/sybil_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-06 12:04:10.000000 sybil_engine-6.6.1/sybil_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-06 12:04:10.000000 sybil_engine-6.6.1/sybil_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:04:10.000000 sybil_engine-6.6.1/sybil_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 12:04:10.000000 sybil_engine-6.6.1/sybil_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 12:04:10.000000 sybil_engine-6.6.1/sybil_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.575858 sybil_engine-6.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.575858 sybil_engine-6.6.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/data/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/data/test_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.575858 sybil_engine-6.6.1/test/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.575858 sybil_engine-6.6.1/test/module/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/contract/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/mock_fail_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/mock_not_enoguth_native_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/repeatable_mock_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.579858 sybil_engine-6.6.1/test/module/swap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/swap/mock_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/swap/mock_test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/swap/test_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/swap/test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/test_execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/test_module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/module/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:10.579858 sybil_engine-6.6.1/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/utils/test_binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/utils/test_create_app_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 12:04:06.000000 sybil_engine-6.6.1/test/utils/test_validation_utils.py
```

### Comparing `sybil_engine-6.6.0/PKG-INFO` & `sybil_engine-6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.6.0
+Version: 6.6.1
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
```

### Comparing `sybil_engine-6.6.0/README.md` & `sybil_engine-6.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/setup.py` & `sybil_engine-6.6.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = file.readlines()
 
 setup(
     name='sybil_engine',
-    version='6.6.0',
+    version='6.6.1',
     py_modules=['sybil_engine'],
     packages=find_packages(),
     install_requires=requirements,
     data_files=[('', ['requirements.txt'])],
     author='Indeoo',
     author_email='indeooars@gmail.com',
     description='Engine for web3 smart contracts automatization.',
```

### Comparing `sybil_engine-6.6.0/sybil_engine/app.py` & `sybil_engine-6.6.1/sybil_engine/app.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/config/app_config.py` & `sybil_engine-6.6.1/sybil_engine/config/app_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/contract/contract.py` & `sybil_engine-6.6.1/sybil_engine/contract/contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/contract/erc20_test_contract.py` & `sybil_engine-6.6.1/sybil_engine/contract/erc20_test_contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/contract/erc20contract.py` & `sybil_engine-6.6.1/sybil_engine/contract/erc20contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/contract/send.py` & `sybil_engine-6.6.1/sybil_engine/contract/send.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/contract/transaction_executor.py` & `sybil_engine-6.6.1/sybil_engine/contract/transaction_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/contract/weth.py` & `sybil_engine-6.6.1/sybil_engine/contract/weth.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/data/contracts.py` & `sybil_engine-6.6.1/sybil_engine/data/contracts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/data/networks.py` & `sybil_engine-6.6.1/sybil_engine/data/networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/data/pairs.py` & `sybil_engine-6.6.1/sybil_engine/data/pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/data/tokens.py` & `sybil_engine-6.6.1/sybil_engine/data/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/domain/balance/balance.py` & `sybil_engine-6.6.1/sybil_engine/domain/balance/balance.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/domain/balance/balance_utils.py` & `sybil_engine-6.6.1/sybil_engine/domain/balance/balance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/domain/balance/tokens.py` & `sybil_engine-6.6.1/sybil_engine/domain/balance/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/domain/dex.py` & `sybil_engine-6.6.1/sybil_engine/domain/dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/domain/generic_swap_facade.py` & `sybil_engine-6.6.1/sybil_engine/domain/generic_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/module/execution_planner.py` & `sybil_engine-6.6.1/sybil_engine/module/execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/module/module.py` & `sybil_engine-6.6.1/sybil_engine/module/module.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/module/module_executor.py` & `sybil_engine-6.6.1/sybil_engine/module/module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/module/modules.py` & `sybil_engine-6.6.1/sybil_engine/module/modules.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/accumulator.py` & `sybil_engine-6.6.1/sybil_engine/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/app_account_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/app_account_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         app_accounts.append(
             AppAccount(
                 row['ADS_ID'],
                 proxy,
                 account,
                 row['CEX_ADDRESS'],
                 row['STARKNET_ADDRESS'],
-                row['NOTES']
+                notes
             )
         )
 
     logger.info(f"Loaded {len(app_accounts)} accounts")
     random.shuffle(app_accounts)
 
     return app_accounts
```

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/arguments_parser.py` & `sybil_engine-6.6.1/sybil_engine/utils/arguments_parser.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/binance_prices.py` & `sybil_engine-6.6.1/sybil_engine/utils/binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/binance_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/binance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/configuration_loader.py` & `sybil_engine-6.6.1/sybil_engine/utils/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/decryptor.py` & `sybil_engine-6.6.1/sybil_engine/utils/decryptor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/fee_storage.py` & `sybil_engine-6.6.1/sybil_engine/utils/fee_storage.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/gas_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/gas_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/logs.py` & `sybil_engine-6.6.1/sybil_engine/utils/logs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/okx_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/okx_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/retry.py` & `sybil_engine-6.6.1/sybil_engine/utils/retry.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/scal_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/scal_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/telegram.py` & `sybil_engine-6.6.1/sybil_engine/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/validation_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine/utils/web3_utils.py` & `sybil_engine-6.6.1/sybil_engine/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/sybil_engine.egg-info/PKG-INFO` & `sybil_engine-6.6.1/sybil_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.6.0
+Version: 6.6.1
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
```

### Comparing `sybil_engine-6.6.0/sybil_engine.egg-info/SOURCES.txt` & `sybil_engine-6.6.1/sybil_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/__init__.py` & `sybil_engine-6.6.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/data/test_networks.py` & `sybil_engine-6.6.1/test/data/test_networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/data/test_pairs.py` & `sybil_engine-6.6.1/test/data/test_pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/contract/mock_router.py` & `sybil_engine-6.6.1/test/module/contract/mock_router.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/swap/mock_dex.py` & `sybil_engine-6.6.1/test/module/swap/mock_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/swap/mock_test_swap_facade.py` & `sybil_engine-6.6.1/test/module/swap/mock_test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/swap/test_dex.py` & `sybil_engine-6.6.1/test/module/swap/test_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/swap/test_swap_facade.py` & `sybil_engine-6.6.1/test/module/swap/test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/test_execution_planner.py` & `sybil_engine-6.6.1/test/module/test_execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/module/test_module_executor.py` & `sybil_engine-6.6.1/test/module/test_module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/test_config.py` & `sybil_engine-6.6.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/utils/test_binance_prices.py` & `sybil_engine-6.6.1/test/utils/test_binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/utils/test_create_app_accounts.py` & `sybil_engine-6.6.1/test/utils/test_create_app_accounts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.0/test/utils/test_validation_utils.py` & `sybil_engine-6.6.1/test/utils/test_validation_utils.py`

 * *Files identical despite different names*
