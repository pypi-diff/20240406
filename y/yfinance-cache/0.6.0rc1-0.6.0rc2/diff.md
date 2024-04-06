# Comparing `tmp/yfinance-cache-0.6.0rc1.tar.gz` & `tmp/yfinance-cache-0.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfinance-cache-0.6.0rc1.tar", last modified: Mon Apr  1 19:50:05 2024, max compression
+gzip compressed data, was "yfinance-cache-0.6.0rc2.tar", last modified: Sat Apr  6 09:32:20 2024, max compression
```

## Comparing `yfinance-cache-0.6.0rc1.tar` & `yfinance-cache-0.6.0rc2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/LICENSE
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5294 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/README.md
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/pyproject.toml
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      832 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/setup.cfg
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.166226 yfinance-cache-0.6.0rc1/tests/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc1/tests/context.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_cache.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_datetime-assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_market_schedules_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_asx.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_nze.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_tlv.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_missing_intervals_usa.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1d.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1h.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1w.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_time_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_utils.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yf_assumptions.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_adjust.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_backend.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_financials.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_interface.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/tests/test_yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc1/tests/utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.160226 yfinance-cache-0.6.0rc1/yfinance_cache/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/__init__.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_cache_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_dat.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    87870 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_financials_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_logging.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_multi.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_options.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_prices_manager.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39045 2024-03-31 21:41:16.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_ticker.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_time.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-02-25 13:22:49.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_upgrade.py
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25378 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc1/yfinance_cache/yfc_utils.py
-drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-01 19:50:05.167226 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/PKG-INFO
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/SOURCES.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/dependency_links.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/requires.txt
--rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-01 19:50:05.000000 yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/top_level.txt
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1068 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/LICENSE
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5294 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/README.md
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      104 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/pyproject.toml
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      832 2024-04-06 09:32:20.270808 yfinance-cache-0.6.0rc2/setup.cfg
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/tests/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1675 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc2/tests/context.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     8469 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_cache.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      991 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_datetime-assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74555 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    70793 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    74237 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    71006 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24913 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    24789 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32509 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    23272 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_market_schedules_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_asx.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12079 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_nze.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13799 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_tlv.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    13077 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_missing_intervals_usa.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25165 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1d.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16811 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1h.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    17013 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1w.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2447 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_time_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1698 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_utils.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2955 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yf_assumptions.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    32294 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_adjust.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_backend.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    12467 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_financials.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    40121 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_interface.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     4270 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/tests/test_yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5085 2024-03-31 21:37:18.000000 yfinance-cache-0.6.0rc2/tests/utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.263808 yfinance-cache-0.6.0rc2/yfinance_cache/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      354 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/__init__.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    16324 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_cache_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    52610 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_dat.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    89156 2024-04-05 21:52:36.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_financials_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2197 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_logging.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     6792 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_multi.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     1453 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_options.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)   204038 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_prices_manager.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    39045 2024-03-31 21:41:16.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_ticker.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    81302 2024-02-10 20:46:25.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_time.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)      653 2024-02-25 13:22:49.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_upgrade.py
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)    25378 2024-03-31 21:40:24.000000 yfinance-cache-0.6.0rc2/yfinance_cache/yfc_utils.py
+drwxr-xr-x   0 gonzo     (1000) gonzo     (1000)        0 2024-04-06 09:32:20.269808 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     5989 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/PKG-INFO
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)     2316 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)        1 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       79 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/requires.txt
+-rw-r--r--   0 gonzo     (1000) gonzo     (1000)       21 2024-04-06 09:32:20.000000 yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/top_level.txt
```

### Comparing `yfinance-cache-0.6.0rc1/LICENSE` & `yfinance-cache-0.6.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/PKG-INFO` & `yfinance-cache-0.6.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.6.0rc1
+Version: 0.6.0rc2
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yfinance-cache-0.6.0rc1/README.md` & `yfinance-cache-0.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/setup.cfg` & `yfinance-cache-0.6.0rc2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = yfinance-cache
-version = 0.6.0rc1
+version = 0.6.0rc2
 author = ValueRaider
 author_email = ValueRaider@protonmail.com
 description = Smart caching wrapper for 'yfinance' module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ValueRaider/yfinance-cache
 project_urls =
```

### Comparing `yfinance-cache-0.6.0rc1/tests/context.py` & `yfinance-cache-0.6.0rc2/tests/context.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_cache.py` & `yfinance-cache-0.6.0rc2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_datetime-assumptions.py` & `yfinance-cache-0.6.0rc2/tests/test_datetime-assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_intervals_asx.py` & `yfinance-cache-0.6.0rc2/tests/test_market_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_intervals_nze.py` & `yfinance-cache-0.6.0rc2/tests/test_market_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_intervals_tlv.py` & `yfinance-cache-0.6.0rc2/tests/test_market_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_intervals_usa.py` & `yfinance-cache-0.6.0rc2/tests/test_market_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_schedules_asx.py` & `yfinance-cache-0.6.0rc2/tests/test_market_schedules_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_schedules_nze.py` & `yfinance-cache-0.6.0rc2/tests/test_market_schedules_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_schedules_tlv.py` & `yfinance-cache-0.6.0rc2/tests/test_market_schedules_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_market_schedules_usa.py` & `yfinance-cache-0.6.0rc2/tests/test_market_schedules_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_asx.py` & `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_asx.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_nze.py` & `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_nze.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_tlv.py` & `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_tlv.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_missing_intervals_usa.py` & `yfinance-cache-0.6.0rc2/tests/test_missing_intervals_usa.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1d.py` & `yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1d.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1h.py` & `yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1h.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_price_data_aging_1w.py` & `yfinance-cache-0.6.0rc2/tests/test_price_data_aging_1w.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_time_utils.py` & `yfinance-cache-0.6.0rc2/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_utils.py` & `yfinance-cache-0.6.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_yf_assumptions.py` & `yfinance-cache-0.6.0rc2/tests/test_yf_assumptions.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_yfc_adjust.py` & `yfinance-cache-0.6.0rc2/tests/test_yfc_adjust.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_yfc_backend.py` & `yfinance-cache-0.6.0rc2/tests/test_yfc_backend.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_yfc_financials.py` & `yfinance-cache-0.6.0rc2/tests/test_yfc_financials.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_yfc_interface.py` & `yfinance-cache-0.6.0rc2/tests/test_yfc_interface.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/test_yfc_ticker.py` & `yfinance-cache-0.6.0rc2/tests/test_yfc_ticker.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/tests/utils.py` & `yfinance-cache-0.6.0rc2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_cache_manager.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_cache_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_dat.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_dat.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_financials_manager.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_financials_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,18 +366,35 @@
                     #             # print("- df_new:", df_new.columns, df_new.shape)
                     #             # print("- metadata old:") ; pprint(md_old)
                     #             raise Exception(f'Why asking Yahoo for {finType} when nothing new ready?')
                 elif not df_new.empty:
                     if df_pruned.empty:
                         df = df_new
                     else:
-                        print("- df:", df.columns) ; print(df)
-                        print("- df_new:", df_new.columns) ; print(df_new)
-                        print("- df_pruned:") ; print(df_pruned)
-                        raise Exception('need to implement merging 2x financials tables, review, particularly row names')
+                        # Before merging, check for new/missing fields. Insert any with value NaN.
+                        missing_keys = [k for k in df_pruned.index if not k in df_new.index]
+                        new_keys = [k for k in df_new.index if not k in df_pruned.index]
+                        actions = []
+                        for k in missing_keys:
+                            actions.append((k, "missing", df_pruned.index.get_loc(k)))
+                        for k in new_keys:
+                            actions.append((k, "new", df_new.index.get_loc(k)))
+                        actions = sorted(actions, key=lambda x: x[2])
+                        for a in actions:
+                            k = a[0]
+                            if a[1] == 'missing':
+                                empty_row = pd.DataFrame(data={c:[np.nan] for c in df_new.columns}, index=[k])
+                                idx = df_pruned.index.get_loc(k)
+                                df_new = pd.concat([df_new.iloc[:idx], empty_row, df_new.iloc[idx:]])
+                            else:
+                                empty_row = pd.DataFrame(data={c:[np.nan] for c in df_pruned.columns}, index=[k])
+                                idx = df_new.index.get_loc(k)
+                                df_pruned = pd.concat([df_pruned.iloc[:idx], empty_row, df_pruned.iloc[idx:]])
+                        df_new = df_new.reindex(df_pruned.index)
+                        df = pd.concat([df_new, df_pruned], axis=1)
             yfcm.StoreCacheDatum(self.ticker, name, df, metadata=md)
 
         self._fin_tbl_cache[cache_key] = df
         return df
 
     def _get_interval_from_table(self, tbl):
         debug = False
@@ -498,15 +515,17 @@
                     do_calc = True
                 elif hasattr(next_r, 'confidence'):
                     try:
                         d_exchange < next_r.release_date
                     except yfcd.AmbiguousComparisonException:
                         print("- next release date is estimated, time to recalc:", next_r)
                         do_calc = True
-                raise Exception('review cached release dates:')
+                # print("- releases:") ; pprint(releases)
+                # print("- md:") ; pprint(md)
+                # raise Exception('review cached release dates')
 
         if do_calc:
             releases = self._calc_release_dates(period, refresh, check)
             md = {'CalcDate':pd.Timestamp.now()}
             if releases is None:
                 yfcm.StoreCacheDatum(self.ticker, cache_key, [], metadata=md)
             else:
```

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_logging.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_logging.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_multi.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_multi.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_options.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_options.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_prices_manager.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_prices_manager.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_ticker.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_ticker.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_time.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_time.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_upgrade.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_upgrade.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache/yfc_utils.py` & `yfinance-cache-0.6.0rc2/yfinance_cache/yfc_utils.py`

 * *Files identical despite different names*

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/PKG-INFO` & `yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfinance-cache
-Version: 0.6.0rc1
+Version: 0.6.0rc2
 Summary: Smart caching wrapper for 'yfinance' module
 Home-page: https://github.com/ValueRaider/yfinance-cache
 Author: ValueRaider
 Author-email: ValueRaider@protonmail.com
 Project-URL: Bug Tracker, https://github.com/ValueRaider/yfinance-cache/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yfinance-cache-0.6.0rc1/yfinance_cache.egg-info/SOURCES.txt` & `yfinance-cache-0.6.0rc2/yfinance_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

