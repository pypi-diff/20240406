# Comparing `tmp/algotik_tse-0.3.8.tar.gz` & `tmp/algotik_tse-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algotik_tse-0.3.8.tar", last modified: Wed Feb 28 19:00:42 2024, max compression
+gzip compressed data, was "algotik_tse-0.3.9.tar", last modified: Fri Mar  8 20:08:06 2024, max compression
```

## Comparing `algotik_tse-0.3.8.tar` & `algotik_tse-0.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.275674 algotik_tse-0.3.8/
--rw-rw-rw-   0        0        0      171 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3699 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      939 2024-02-28 18:58:14.000000 algotik_tse-0.3.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1595 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      313 2023-12-17 16:24:29.000000 algotik_tse-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7814 2024-02-28 19:00:42.274579 algotik_tse-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5742 2024-02-28 18:58:14.000000 algotik_tse-0.3.8/README.md
--rw-rw-rw-   0        0        0     1139 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.149248 algotik_tse-0.3.8/algotik_tse/
--rw-rw-rw-   0        0        0     2314 2024-02-28 18:58:14.000000 algotik_tse-0.3.8/algotik_tse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.208054 algotik_tse-0.3.8/algotik_tse/core/
--rw-rw-rw-   0        0        0        0 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/algotik_tse/core/__init__.py
--rw-rw-rw-   0        0        0    12107 2024-02-02 20:38:12.000000 algotik_tse-0.3.8/algotik_tse/core/currency.py
--rw-rw-rw-   0        0        0      991 2024-01-04 21:25:10.000000 algotik_tse-0.3.8/algotik_tse/core/helper.py
--rw-rw-rw-   0        0        0     2128 2024-01-04 20:38:27.000000 algotik_tse-0.3.8/algotik_tse/core/search.py
--rw-rw-rw-   0        0        0     3615 2024-01-05 08:38:56.000000 algotik_tse-0.3.8/algotik_tse/core/shareholders.py
--rw-rw-rw-   0        0        0    44456 2024-01-11 08:58:02.000000 algotik_tse-0.3.8/algotik_tse/core/stock.py
--rw-rw-rw-   0        0        0     3964 2024-02-02 16:09:26.000000 algotik_tse-0.3.8/algotik_tse/core/stock_detail.py
--rw-rw-rw-   0        0        0     9520 2024-02-28 18:58:14.000000 algotik_tse-0.3.8/algotik_tse/core/stock_list.py
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.214854 algotik_tse-0.3.8/algotik_tse/providers/
--rw-rw-rw-   0        0        0        0 2024-02-02 16:25:36.000000 algotik_tse-0.3.8/algotik_tse/providers/__init__.py
--rw-rw-rw-   0        0        0      813 2024-02-02 19:21:20.000000 algotik_tse-0.3.8/algotik_tse/providers/tgju_convertor.py
--rw-rw-rw-   0        0        0     5684 2024-02-28 18:58:14.000000 algotik_tse-0.3.8/algotik_tse/settings.py
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.271443 algotik_tse-0.3.8/algotik_tse.egg-info/
--rw-rw-rw-   0        0        0     7814 2024-02-28 19:00:42.000000 algotik_tse-0.3.8/algotik_tse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2024-02-28 19:00:42.000000 algotik_tse-0.3.8/algotik_tse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 19:00:42.000000 algotik_tse-0.3.8/algotik_tse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-17 16:08:00.000000 algotik_tse-0.3.8/algotik_tse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2024-02-28 19:00:42.000000 algotik_tse-0.3.8/algotik_tse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-28 19:00:42.000000 algotik_tse-0.3.8/algotik_tse.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.258522 algotik_tse-0.3.8/docs/
--rw-rw-rw-   0        0        0      632 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/authors.rst
--rw-rw-rw-   0        0        0     4998 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/history.rst
--rw-rw-rw-   0        0        0      328 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/index.rst
--rw-rw-rw-   0        0        0     1217 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/readme.rst
--rw-rw-rw-   0        0        0       84 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/docs/usage.rst
--rw-rw-rw-   0        0        0      452 2024-02-28 19:00:42.278060 algotik_tse-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1889 2024-02-28 18:58:14.000000 algotik_tse-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 19:00:42.267255 algotik_tse-0.3.8/tests/
--rw-rw-rw-   0        0        0       42 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/tests/__init__.py
--rw-rw-rw-   0        0        0      589 2023-12-17 15:28:57.000000 algotik_tse-0.3.8/tests/test_algotik_tse.py
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.813216 algotik_tse-0.3.9/
+-rw-rw-rw-   0        0        0      171 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3699 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1049 2024-03-08 19:53:46.000000 algotik_tse-0.3.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1595 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      313 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7924 2024-03-08 20:08:06.813216 algotik_tse-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5742 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/README.md
+-rw-rw-rw-   0        0        0     1139 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.766234 algotik_tse-0.3.9/algotik_tse/
+-rw-rw-rw-   0        0        0     2314 2024-03-08 19:54:38.000000 algotik_tse-0.3.9/algotik_tse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.788221 algotik_tse-0.3.9/algotik_tse/core/
+-rw-rw-rw-   0        0        0        0 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/__init__.py
+-rw-rw-rw-   0        0        0    12323 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/currency.py
+-rw-rw-rw-   0        0        0      991 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/helper.py
+-rw-rw-rw-   0        0        0     2128 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/search.py
+-rw-rw-rw-   0        0        0     3720 2024-03-08 19:47:07.000000 algotik_tse-0.3.9/algotik_tse/core/shareholders.py
+-rw-rw-rw-   0        0        0    44456 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/stock.py
+-rw-rw-rw-   0        0        0     3964 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/stock_detail.py
+-rw-rw-rw-   0        0        0     9520 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/core/stock_list.py
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.791219 algotik_tse-0.3.9/algotik_tse/providers/
+-rw-rw-rw-   0        0        0        0 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/providers/__init__.py
+-rw-rw-rw-   0        0        0      839 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/providers/tgju_convertor.py
+-rw-rw-rw-   0        0        0     5684 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/algotik_tse/settings.py
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.811217 algotik_tse-0.3.9/algotik_tse.egg-info/
+-rw-rw-rw-   0        0        0     7924 2024-03-08 20:08:06.000000 algotik_tse-0.3.9/algotik_tse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2024-03-08 20:08:06.000000 algotik_tse-0.3.9/algotik_tse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-08 20:08:06.000000 algotik_tse-0.3.9/algotik_tse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-08 20:08:06.000000 algotik_tse-0.3.9/algotik_tse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2024-03-08 20:08:06.000000 algotik_tse-0.3.9/algotik_tse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-03-08 20:08:06.000000 algotik_tse-0.3.9/algotik_tse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.807220 algotik_tse-0.3.9/docs/
+-rw-rw-rw-   0        0        0      632 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/authors.rst
+-rw-rw-rw-   0        0        0     4998 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/history.rst
+-rw-rw-rw-   0        0        0      328 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/index.rst
+-rw-rw-rw-   0        0        0     1217 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/readme.rst
+-rw-rw-rw-   0        0        0       84 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/docs/usage.rst
+-rw-rw-rw-   0        0        0      452 2024-03-08 20:08:06.814216 algotik_tse-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1889 2024-03-08 19:53:14.000000 algotik_tse-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-08 20:08:06.810218 algotik_tse-0.3.9/tests/
+-rw-rw-rw-   0        0        0       42 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-03-07 20:59:05.000000 algotik_tse-0.3.9/tests/test_algotik_tse.py
```

### Comparing `algotik_tse-0.3.8/CONTRIBUTING.rst` & `algotik_tse-0.3.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/HISTORY.rst` & `algotik_tse-0.3.9/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -44,7 +44,12 @@
 * seventh release on PyPI.
 * Add currencies and coins in beta phase.
 
 0.3.8 (2024-02-27)
 ------------------
 * eighth release on PyPI.
 * Add payeh market color in stocklist.
+
+0.3.9 (2024-03-08)
+------------------
+* ninth release on PyPI.
+* bug fix in shareholders change_amount.
```

### Comparing `algotik_tse-0.3.8/LICENSE` & `algotik_tse-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/PKG-INFO` & `algotik_tse-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algotik_tse
-Version: 0.3.8
+Version: 0.3.9
 Summary: Get all data from TSETMC.com (Tehran Bourse).
 Home-page: https://github.com/mohsenalipour/algotik_tse
 Author: Mohsen Alipour
 Author-email: alipour@algotik.ir
 License: GNU General Public License v3
 Keywords: algotik_tse
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -256,7 +256,12 @@
 * seventh release on PyPI.
 * Add currencies and coins in beta phase.
 
 0.3.8 (2024-02-27)
 ------------------
 * eighth release on PyPI.
 * Add payeh market color in stocklist.
+
+0.3.9 (2024-03-08)
+------------------
+* ninth release on PyPI.
+* bug fix in shareholders change_amount.
```

### Comparing `algotik_tse-0.3.8/README.md` & `algotik_tse-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/README.rst` & `algotik_tse-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse/__init__.py` & `algotik_tse-0.3.9/algotik_tse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-version 0.3.8
+version 0.3.9
 Main module code by @Python4finance
 New version code by Mohsen Alipour alipour@algotik.ir
-last Edit: 2024-02-27
+last Edit: 2024-03-08
 * Base: old.tsetmc.com
 
 Sample:
 import algotik_tse as att
 
 att.stockdetail(stock='شبندر')
 you get all detail information of the stock!
@@ -38,14 +38,14 @@
 
 att.currency_coin(['ربع سکه', 'euro'])
 you cand get historical price of currencies and coins!
 """
 
 __author__ = """Mohsen Alipour"""
 __email__ = 'alipour@algotik.ir'
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 
 from algotik_tse.core.stock_detail import stockdetail, stock_information, stock_statistics
 from algotik_tse.core.stock_list import stocklist
 from algotik_tse.core.stock import stock, stock_RI, stock_RL, stock_capital_increase
 from algotik_tse.core.shareholders import shareholders
 from algotik_tse.core.currency import currency_coin
```

### Comparing `algotik_tse-0.3.8/algotik_tse/core/currency.py` & `algotik_tse-0.3.9/algotik_tse/core/currency.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-import requests
-import pandas as pd
-import numpy as np
-from algotik_tse.settings import settings
-from algotik_tse.providers.tgju_convertor import tgju_convertor
-from algotik_tse.core.helper import date_fix
-
-
-def currency_coin(currency_coin_name="", start=None, end=None, values=0, output_type="standard",
-                  date_format="jalali", progress=True, save_to_file=False, multi_currencies_drop=True,
-                  return_type=None):
-    """
-        Get symbol or symbols price history from tsetmc
-        :param currency_coin_name:currency or coin name in persian or english, or a list of currency or  in
-                                    persian (['euro', 'سکه امامی'])
-                                Default value is 'dollar'.
-        :param start:           you can choose strat date (from) to get historical price.
-                                enter date in jalali only in isoformat ('1401-10-01')
-                                    and gregorian in isoformat("2022-12-22") or
-                                    ("2022") or ("2022-12")
-                                Default value is None.
-                                if start=None and end=None, value can apply to price data.
-        :param end:             you can choos end date (to) to get historical price.
-                                enter date in jalali only in isoformat ('1401-10-01')
-                                    and gregorian in isoformat ("2022-12-22") or
-                                    ("2022") or ("2022-12")
-                                Default value is None.
-                                if start=None and end=None, 'values' can apply to price data.
-        :param values:          Specifies the number of price data since today
-                                Default value is 225.
-                                'values' can be applied when start=None and end=None.
-        :param output_type:     you can choose between 'standard' and 'complete'.
-                                Default value is 'standard'.
-                                if output_type='standard', you get OHLC in output.
-                                if output_type='complete', you get OHLC and 'Weekday', 'Ticker' in output.
-        :param date_format:     you can choose between 'jalali' and 'gregorian' and 'both'.
-                                Default value is 'jalali'.
-                                if date_format='jalali', you get historical price with
-                                    jalali date index and 'Weekday_fa' in complete mode
-                                    in output.
-                                if output_type='gregorian', you get historical price
-                                    with gregorian date index and 'Weekday' in complete
-                                    mode in output.
-                                if output_type='both', you get historical price with
-                                    gregorian date index and 'J-Date'(jalali date),
-                                    'Weekday', 'Weekday_fa' in complete mode in output.
-        :param progress:        if True, show progress and report in console.
-                                Default value is True.
-        :param save_to_file:    if True, save currency(ies) or coin(s) historical data with customized
-                                    columns in .csv format.
-                                Default value is False.
-                                the file name is 'currency.csv' in same root that
-                                    your file is there. for example: 'dollar.csv'
-        :param multi_currencies_drop:if True, when you enter currency or coin list, it will delete
-                                    rows of none data (dropna) in combined historical df.
-                                Default value is True.
-        :param return_type:     you can choose between 'simple', 'log' and 'both', or enter ['simple', 'Close', 5] format.
-                                if return_type='simple', you get simple return in 1 day on Close.
-                                    with simple return 'returns' in complete mode in output.
-                                if return_type='log', you get log return in 1 day on Close.
-                                    with log return 'returns' in complete mode in output.
-                                if return_type='both', you get simple and log return in 1 day onClose.
-                                    with both return 'simple_returns' and 'log_returns' in complete mode in output.
-                                if return_type=['simple', 'Close', 5], you get simple return in 5 day on Close.
-                                    with this 'returns' in complete mode in output.
-
-        :return: pandas dataframe or None
-        """
-
-    def __get_currency_history(currency__name):
-        url_word = settings.currency_web_word[currency__name]['web_word']
-        new_start, new_end = date_fix(start=start, end=end)
-        detail = requests.get(settings.url_currency_from_tgju.format(url_word), headers=settings.headers)
-        if detail.status_code == 200:
-            df = tgju_convertor(detail.json()['data'])
-            if values is not None or start is not None or end is not None:
-                if values != 0:
-                    df = df.iloc[-values:]
-                else:
-                    if end is None:
-                        df = df.loc[new_start:]
-                    else:
-                        df = df.loc[new_start:new_end]
-
-            df["Weekday_No"] = df["Date"].dt.weekday
-            df["Weekday"] = df["Weekday_No"].apply(lambda x: settings.en_weekdays[x])
-            df["Weekday_fa"] = df["Weekday_No"].apply(lambda x: settings.fa_weekdays[x])
-            df.drop("Weekday_No", axis=1, inplace=True)
-            df['Ticker'] = settings.currency_web_word[currency__name]['persian_word']
-
-            if date_format == 'jalali':
-                df.set_index('J-Date', drop=True, inplace=True)
-                df.drop(columns=["Date", "Weekday"], inplace=True)
-            elif date_format == 'gregorian':
-                df.set_index('Date', drop=True, inplace=True)
-                df.drop(columns=["J-Date", 'Weekday_fa'], inplace=True)
-            elif date_format == 'both':
-                df.set_index('Date', drop=True, inplace=True)
-            else:
-                print("please select date_format between 'jalali', 'gregorian ', 'both' ")
-                return None
-
-            if output_type == "standard":
-                df = df.loc[:, "Open High Low Close".split()]
-            elif output_type == 'complete':
-                pass
-            else:
-                print("output_type should select between 'standard' or 'complete'")
-                return None
-
-            if return_type is not None:
-                price = 'Close'
-                if isinstance(return_type, str):
-                    if return_type == 'simple':
-                        df['returns'] = df[price].pct_change()
-                    elif return_type == 'log':
-                        df['returns'] = np.log(df[price] / df[price].shift(1))
-                    elif return_type == 'both':
-                        df['simple_returns'] = df[price].pct_change()
-                        df['log_returns'] = np.log(df[price] / df[price].shift(1))
-                    else:
-                        print("return_type should select between 'simple', 'log' or ''both")
-                        return None
-                elif isinstance(return_type, list) and len(return_type) == 3:
-                    # ['simple', 'Close', 2]
-                    if return_type[0] == 'simple':
-                        df['returns'] = df[return_type[1]].pct_change(return_type[2])
-                    elif return_type[0] == 'log':
-                        df['returns'] = np.log(
-                            df[return_type[1]] / df[return_type[1]].shift(return_type[2]))
-                    elif return_type[0] == 'both':
-                        df['simple_returns'] = df[return_type[1]].pct_change(return_type[2])
-                        df['log_returns'] = np.log(
-                            df[return_type[1]] / df[return_type[1]].shift(return_type[2]))
-                    else:
-                        print("return_type[0] should select between 'simple', 'log' or ''both")
-                        return None
-                else:
-                    print(
-                        "return_type should select between 'simple', 'log' or 'both' or enter a list like this: ['simple', 'Close', 3]")
-                    return None
-            return df
-        else:
-            print("Connection Error!!!")
-            return None
-
-    if currency_coin_name == "":
-        currency_coin_name = "dollar"
-        if progress:
-            print("1/1: Getting historical price of {}".format(currency_coin_name))
-        df = __get_currency_history(currency__name=currency_coin_name)
-        if progress and df is not None:
-            print("1/1: Completed!")
-        if save_to_file and df is not None:
-            if progress:
-                print("Saving to file: {}.csv".format(currency_coin_name))
-            df.to_csv(currency_coin_name + ".csv", encoding="utf-8-sig")
-        return df
-    else:
-        if isinstance(currency_coin_name, str):
-            currency_coin_name = currency_coin_name if currency_coin_name.isascii() else settings.currency_persian[
-                currency_coin_name]
-            if progress:
-                print("1/1: Getting historical price of {}".format(currency_coin_name))
-            df = __get_currency_history(currency__name=currency_coin_name)
-            if progress and df is not None:
-                print("1/1: Completed!")
-            if save_to_file and df is not None:
-                if progress:
-                    print("Saving to file: {}.csv".format(currency_coin_name))
-                df.to_csv(currency_coin_name + ".csv", encoding="utf-8-sig")
-            return df
-        elif isinstance(currency_coin_name, list):
-            n = 1
-            df_dict = {}
-            file_name_str = ''
-            for cur in currency_coin_name:
-                cur = cur if cur.isascii() else settings.currency_persian[cur]
-                if progress:
-                    print("{}/{}: Getting historical price of {}".format(n, len(currency_coin_name), cur))
-                df = __get_currency_history(currency__name=cur)
-                if df is not None:
-                    file_name_str += "-" + cur
-                    df_dict[cur] = df
-                else:
-                    print("{} not Found!".format(cur))
-                n += 1
-            if progress:
-                print('{}/{} Completed!'.format(len(currency_coin_name), len(currency_coin_name)))
-
-            if len(list(df_dict.keys())) == 0:
-                print('None of the entered currencies exist!!')
-                return None
-            elif len(list(df_dict.keys())) == 1:
-                df = df_dict[list(df_dict.keys())[0]]
-                if save_to_file and df is not None:
-                    if progress:
-                        print("Saving to file: {}.csv".format(file_name_str[1:]))
-                    df.to_csv(file_name_str[1:] + ".csv", encoding="utf-8-sig")
-                return df
-            else:
-                df = pd.concat(df_dict, axis=1)
-                multi_assets_columns = df.columns
-                reversed_multi_assets_columns = []
-                for column_index in multi_assets_columns:
-                    reversed_multi_assets_columns.append(column_index[::-1])
-                new_index = pd.MultiIndex.from_tuples(reversed_multi_assets_columns)
-                df.columns = new_index
-
-                if multi_currencies_drop:
-                    df.dropna(inplace=True)
-                if save_to_file and df is not None:
-                    if progress:
-                        print("Saving to file: {}.csv".format(file_name_str[1:]))
-                    df.to_csv(file_name_str[1:] + ".csv", encoding="utf-8-sig")
-                return df
+import requests
+import pandas as pd
+import numpy as np
+from algotik_tse.settings import settings
+from algotik_tse.providers.tgju_convertor import tgju_convertor
+from algotik_tse.core.helper import date_fix
+
+
+def currency_coin(currency_coin_name="", start=None, end=None, values=0, output_type="standard",
+                  date_format="jalali", progress=True, save_to_file=False, multi_currencies_drop=True,
+                  return_type=None):
+    """
+        Get symbol or symbols price history from tsetmc
+        :param currency_coin_name:currency or coin name in persian or english, or a list of currency or  in
+                                    persian (['euro', 'سکه امامی'])
+                                Default value is 'dollar'.
+        :param start:           you can choose strat date (from) to get historical price.
+                                enter date in jalali only in isoformat ('1401-10-01')
+                                    and gregorian in isoformat("2022-12-22") or
+                                    ("2022") or ("2022-12")
+                                Default value is None.
+                                if start=None and end=None, value can apply to price data.
+        :param end:             you can choos end date (to) to get historical price.
+                                enter date in jalali only in isoformat ('1401-10-01')
+                                    and gregorian in isoformat ("2022-12-22") or
+                                    ("2022") or ("2022-12")
+                                Default value is None.
+                                if start=None and end=None, 'values' can apply to price data.
+        :param values:          Specifies the number of price data since today
+                                Default value is 225.
+                                'values' can be applied when start=None and end=None.
+        :param output_type:     you can choose between 'standard' and 'complete'.
+                                Default value is 'standard'.
+                                if output_type='standard', you get OHLC in output.
+                                if output_type='complete', you get OHLC and 'Weekday', 'Ticker' in output.
+        :param date_format:     you can choose between 'jalali' and 'gregorian' and 'both'.
+                                Default value is 'jalali'.
+                                if date_format='jalali', you get historical price with
+                                    jalali date index and 'Weekday_fa' in complete mode
+                                    in output.
+                                if output_type='gregorian', you get historical price
+                                    with gregorian date index and 'Weekday' in complete
+                                    mode in output.
+                                if output_type='both', you get historical price with
+                                    gregorian date index and 'J-Date'(jalali date),
+                                    'Weekday', 'Weekday_fa' in complete mode in output.
+        :param progress:        if True, show progress and report in console.
+                                Default value is True.
+        :param save_to_file:    if True, save currency(ies) or coin(s) historical data with customized
+                                    columns in .csv format.
+                                Default value is False.
+                                the file name is 'currency.csv' in same root that
+                                    your file is there. for example: 'dollar.csv'
+        :param multi_currencies_drop:if True, when you enter currency or coin list, it will delete
+                                    rows of none data (dropna) in combined historical df.
+                                Default value is True.
+        :param return_type:     you can choose between 'simple', 'log' and 'both', or enter ['simple', 'Close', 5] format.
+                                if return_type='simple', you get simple return in 1 day on Close.
+                                    with simple return 'returns' in complete mode in output.
+                                if return_type='log', you get log return in 1 day on Close.
+                                    with log return 'returns' in complete mode in output.
+                                if return_type='both', you get simple and log return in 1 day onClose.
+                                    with both return 'simple_returns' and 'log_returns' in complete mode in output.
+                                if return_type=['simple', 'Close', 5], you get simple return in 5 day on Close.
+                                    with this 'returns' in complete mode in output.
+
+        :return: pandas dataframe or None
+        """
+
+    def __get_currency_history(currency__name):
+        url_word = settings.currency_web_word[currency__name]['web_word']
+        new_start, new_end = date_fix(start=start, end=end)
+        detail = requests.get(settings.url_currency_from_tgju.format(url_word), headers=settings.headers)
+        if detail.status_code == 200:
+            df = tgju_convertor(detail.json()['data'])
+            if values is not None or start is not None or end is not None:
+                if values != 0:
+                    df = df.iloc[-values:]
+                else:
+                    if end is None:
+                        df = df.loc[new_start:]
+                    else:
+                        df = df.loc[new_start:new_end]
+
+            df["Weekday_No"] = df["Date"].dt.weekday
+            df["Weekday"] = df["Weekday_No"].apply(lambda x: settings.en_weekdays[x])
+            df["Weekday_fa"] = df["Weekday_No"].apply(lambda x: settings.fa_weekdays[x])
+            df.drop("Weekday_No", axis=1, inplace=True)
+            df['Ticker'] = settings.currency_web_word[currency__name]['persian_word']
+
+            if date_format == 'jalali':
+                df.set_index('J-Date', drop=True, inplace=True)
+                df.drop(columns=["Date", "Weekday"], inplace=True)
+            elif date_format == 'gregorian':
+                df.set_index('Date', drop=True, inplace=True)
+                df.drop(columns=["J-Date", 'Weekday_fa'], inplace=True)
+            elif date_format == 'both':
+                df.set_index('Date', drop=True, inplace=True)
+            else:
+                print("please select date_format between 'jalali', 'gregorian ', 'both' ")
+                return None
+
+            if output_type == "standard":
+                df = df.loc[:, "Open High Low Close".split()]
+            elif output_type == 'complete':
+                pass
+            else:
+                print("output_type should select between 'standard' or 'complete'")
+                return None
+
+            if return_type is not None:
+                price = 'Close'
+                if isinstance(return_type, str):
+                    if return_type == 'simple':
+                        df['returns'] = df[price].pct_change()
+                    elif return_type == 'log':
+                        df['returns'] = np.log(df[price] / df[price].shift(1))
+                    elif return_type == 'both':
+                        df['simple_returns'] = df[price].pct_change()
+                        df['log_returns'] = np.log(df[price] / df[price].shift(1))
+                    else:
+                        print("return_type should select between 'simple', 'log' or ''both")
+                        return None
+                elif isinstance(return_type, list) and len(return_type) == 3:
+                    # ['simple', 'Close', 2]
+                    if return_type[0] == 'simple':
+                        df['returns'] = df[return_type[1]].pct_change(return_type[2])
+                    elif return_type[0] == 'log':
+                        df['returns'] = np.log(
+                            df[return_type[1]] / df[return_type[1]].shift(return_type[2]))
+                    elif return_type[0] == 'both':
+                        df['simple_returns'] = df[return_type[1]].pct_change(return_type[2])
+                        df['log_returns'] = np.log(
+                            df[return_type[1]] / df[return_type[1]].shift(return_type[2]))
+                    else:
+                        print("return_type[0] should select between 'simple', 'log' or ''both")
+                        return None
+                else:
+                    print(
+                        "return_type should select between 'simple', 'log' or 'both' or enter a list like this: ['simple', 'Close', 3]")
+                    return None
+            return df
+        else:
+            print("Connection Error!!!")
+            return None
+
+    if currency_coin_name == "":
+        currency_coin_name = "dollar"
+        if progress:
+            print("1/1: Getting historical price of {}".format(currency_coin_name))
+        df = __get_currency_history(currency__name=currency_coin_name)
+        if progress and df is not None:
+            print("1/1: Completed!")
+        if save_to_file and df is not None:
+            if progress:
+                print("Saving to file: {}.csv".format(currency_coin_name))
+            df.to_csv(currency_coin_name + ".csv", encoding="utf-8-sig")
+        return df
+    else:
+        if isinstance(currency_coin_name, str):
+            currency_coin_name = currency_coin_name if currency_coin_name.isascii() else settings.currency_persian[
+                currency_coin_name]
+            if progress:
+                print("1/1: Getting historical price of {}".format(currency_coin_name))
+            df = __get_currency_history(currency__name=currency_coin_name)
+            if progress and df is not None:
+                print("1/1: Completed!")
+            if save_to_file and df is not None:
+                if progress:
+                    print("Saving to file: {}.csv".format(currency_coin_name))
+                df.to_csv(currency_coin_name + ".csv", encoding="utf-8-sig")
+            return df
+        elif isinstance(currency_coin_name, list):
+            n = 1
+            df_dict = {}
+            file_name_str = ''
+            for cur in currency_coin_name:
+                cur = cur if cur.isascii() else settings.currency_persian[cur]
+                if progress:
+                    print("{}/{}: Getting historical price of {}".format(n, len(currency_coin_name), cur))
+                df = __get_currency_history(currency__name=cur)
+                if df is not None:
+                    file_name_str += "-" + cur
+                    df_dict[cur] = df
+                else:
+                    print("{} not Found!".format(cur))
+                n += 1
+            if progress:
+                print('{}/{} Completed!'.format(len(currency_coin_name), len(currency_coin_name)))
+
+            if len(list(df_dict.keys())) == 0:
+                print('None of the entered currencies exist!!')
+                return None
+            elif len(list(df_dict.keys())) == 1:
+                df = df_dict[list(df_dict.keys())[0]]
+                if save_to_file and df is not None:
+                    if progress:
+                        print("Saving to file: {}.csv".format(file_name_str[1:]))
+                    df.to_csv(file_name_str[1:] + ".csv", encoding="utf-8-sig")
+                return df
+            else:
+                df = pd.concat(df_dict, axis=1)
+                multi_assets_columns = df.columns
+                reversed_multi_assets_columns = []
+                for column_index in multi_assets_columns:
+                    reversed_multi_assets_columns.append(column_index[::-1])
+                new_index = pd.MultiIndex.from_tuples(reversed_multi_assets_columns)
+                df.columns = new_index
+
+                if multi_currencies_drop:
+                    df.dropna(inplace=True)
+                if save_to_file and df is not None:
+                    if progress:
+                        print("Saving to file: {}.csv".format(file_name_str[1:]))
+                    df.to_csv(file_name_str[1:] + ".csv", encoding="utf-8-sig")
+                return df
```

### Comparing `algotik_tse-0.3.8/algotik_tse/core/helper.py` & `algotik_tse-0.3.9/algotik_tse/core/helper.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse/core/search.py` & `algotik_tse-0.3.9/algotik_tse/core/search.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse/core/shareholders.py` & `algotik_tse-0.3.9/algotik_tse/core/shareholders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-import requests
-import pandas as pd
-from algotik_tse.core.search import search_stock
-from algotik_tse.settings import Settings
-from algotik_tse.core.helper import date_fix
-
-settings = Settings()
-
-
-def shareholders(stock="", date=None, shh_id=False):
-    """
-    Get all shareholders of an instrument (company)
-    :param stock: name of stock
-                  Default value is 'شتران'.
-    :param date: date for get shareholders in specific date, if None the function return last shareholders
-                  Default value is None
-    :param shh_id: if is True, shareholder id will be shown in df and if is False, shareholder not show
-                  Default value is False
-
-    :return: pandas dataframe
-    """
-    web_id = search_stock(search_txt=stock)
-    if len(web_id) != 0:
-        try:
-            if date is None:
-                share_holder_id_name = 'shareHolderShareID'
-                _shareholders_base_url = settings.url_last_share_holders
-                response = requests.get(url=_shareholders_base_url.format(web_id), headers=settings.headers)
-            else:
-                share_holder_id_name = 'shareHolderID'
-                new_start, new_end = date_fix(start=date)
-                new_start = new_start.replace("-", "")
-                _shareholders_base_url = settings.url_share_holders_history
-                url = _shareholders_base_url.format(web_id, new_start)
-                response = requests.get(url=url, headers=settings.headers)
-            if response.status_code == 200:
-                share_holders = response.json()['shareHolder'] if date is None else response.json()['shareShareholder']
-                share_holders_df = pd.DataFrame(share_holders)
-                share_holders_columns = ['shareHolderName', 'numberOfShares', 'perOfShares', 'change', 'changeAmount',
-                                         'dEven']
-                if shh_id:
-                    share_holders_columns.append(share_holder_id_name)
-                share_holders_df = share_holders_df.loc[:, share_holders_columns]
-                share_holders_df.rename(columns={'shareHolderName': 'share_holder_name',
-                                                 'numberOfShares': 'number_of_shares',
-                                                 'perOfShares': 'percentage_of_shares', 'change': 'change_state',
-                                                 'changeAmount': 'change_amount', 'dEven': 'date'}, inplace=True)
-                if shh_id:
-                    share_holders_df.rename(columns={share_holder_id_name: 'share_holder_id'}, inplace=True)
-                if date is not None:
-                    share_holders_df['first_row'] = share_holders_df.groupby('share_holder_name')['number_of_shares'].transform('first')
-                    share_holders_df['last_row'] = share_holders_df.groupby('share_holder_name')[
-                        'number_of_shares'].transform('last')
-                    share_holders_df['change_amount'] = share_holders_df['first_row'] - share_holders_df['last_row']
-                    share_holders_df = share_holders_df.drop(['first_row', 'last_row'], axis=1)
-                    share_holders_df = share_holders_df.loc[share_holders_df['date'] == share_holders_df['date'].max(),
-                                       :]
-                else:
-                    share_holders_df['date'] = settings.today.replace('-', '')
-                return share_holders_df
-        except:
-            print("Connection Error!!!")
-            return None
-    else:
-        print("Stock Not Found, Please try again ...")
-        return None
+import requests
+import pandas as pd
+from algotik_tse.core.search import search_stock
+from algotik_tse.settings import Settings
+from algotik_tse.core.helper import date_fix
+
+settings = Settings()
+
+
+def shareholders(stock="", date=None, shh_id=False):
+    """
+    Get all shareholders of an instrument (company)
+    :param stock: name of stock
+                  Default value is 'شتران'.
+    :param date: date for get shareholders in specific date, if None the function return last shareholders
+                  Default value is None
+    :param shh_id: if is True, shareholder id will be shown in df and if is False, shareholder not show
+                  Default value is False
+
+    :return: pandas dataframe
+    """
+    web_id = search_stock(search_txt=stock)
+    if len(web_id) != 0:
+        try:
+            if date is None:
+                share_holder_id_name = 'shareHolderShareID'
+                _shareholders_base_url = settings.url_last_share_holders
+                response = requests.get(url=_shareholders_base_url.format(web_id), headers=settings.headers)
+            else:
+                share_holder_id_name = 'shareHolderID'
+                new_start, new_end = date_fix(start=date)
+                new_start = new_start.replace("-", "")
+                _shareholders_base_url = settings.url_share_holders_history
+                url = _shareholders_base_url.format(web_id, new_start)
+                response = requests.get(url=url, headers=settings.headers)
+            if response.status_code == 200:
+                share_holders = response.json()['shareHolder'] if date is None else response.json()['shareShareholder']
+                share_holders_df = pd.DataFrame(share_holders)
+                share_holders_columns = ['shareHolderName', 'numberOfShares', 'perOfShares', 'change', 'changeAmount',
+                                         'dEven']
+
+                share_holders_columns.append(share_holder_id_name)
+                share_holders_df = share_holders_df.loc[:, share_holders_columns]
+                share_holders_df.rename(columns={'shareHolderName': 'share_holder_name',
+                                                 'numberOfShares': 'number_of_shares',
+                                                 'perOfShares': 'percentage_of_shares', 'change': 'change_state',
+                                                 'changeAmount': 'change_amount', 'dEven': 'date',
+                                                 share_holder_id_name: 'share_holder_id'}, inplace=True)
+
+                if date is not None:
+                    share_holders_df['first_row'] = share_holders_df.groupby('share_holder_id')['number_of_shares'].transform('first')
+                    share_holders_df['last_row'] = share_holders_df.groupby('share_holder_id')[
+                        'number_of_shares'].transform('last')
+                    share_holders_df['change_amount'] = share_holders_df['first_row'] - share_holders_df['last_row']
+                    share_holders_df = share_holders_df.drop(['first_row', 'last_row'], axis=1)
+                    share_holders_df = share_holders_df.loc[share_holders_df['date'] == share_holders_df['date'].max(),
+                                       :]
+                else:
+                    share_holders_df['date'] = settings.today.replace('-', '')
+                if not shh_id:
+                    share_holders_df.drop(columns=['share_holder_id'], inplace=True)
+                return share_holders_df
+        except:
+            print("Connection Error!!!")
+            return None
+    else:
+        print("Stock Not Found, Please try again ...")
+        return None
```

### Comparing `algotik_tse-0.3.8/algotik_tse/core/stock.py` & `algotik_tse-0.3.9/algotik_tse/core/stock.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse/core/stock_detail.py` & `algotik_tse-0.3.9/algotik_tse/core/stock_detail.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse/core/stock_list.py` & `algotik_tse-0.3.9/algotik_tse/core/stock_list.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse/providers/tgju_convertor.py` & `algotik_tse-0.3.9/algotik_tse/providers/tgju_convertor.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import pandas as pd
-
-
-def tgju_convertor(json_input):
-    price = {
-        'J-Date': [],
-        'Date': [],
-        'Open': [],
-        'High': [],
-        'Low': [],
-        'Close': [],
-    }
-    for date_price in json_input:
-        price['J-Date'].append(date_price[7].replace("/", "-"))
-        price['Date'].append(date_price[6].replace("/", "-"))
-        price['Open'].append(float(date_price[0].replace(",", "")))
-        price['High'].append(float(date_price[2].replace(",", "")))
-        price['Low'].append(float(date_price[1].replace(",", "")))
-        price['Close'].append(float(date_price[3].replace(",", "")))
-
-    df = pd.DataFrame(price)
-    df = df[::-1]
-    df.dropna(inplace=True)
-    df['Date'] = pd.to_datetime(df['Date'])
-    df.set_index('Date', inplace=True, drop=False)
-    return df
+import pandas as pd
+
+
+def tgju_convertor(json_input):
+    price = {
+        'J-Date': [],
+        'Date': [],
+        'Open': [],
+        'High': [],
+        'Low': [],
+        'Close': [],
+    }
+    for date_price in json_input:
+        price['J-Date'].append(date_price[7].replace("/", "-"))
+        price['Date'].append(date_price[6].replace("/", "-"))
+        price['Open'].append(float(date_price[0].replace(",", "")))
+        price['High'].append(float(date_price[2].replace(",", "")))
+        price['Low'].append(float(date_price[1].replace(",", "")))
+        price['Close'].append(float(date_price[3].replace(",", "")))
+
+    df = pd.DataFrame(price)
+    df = df[::-1]
+    df.dropna(inplace=True)
+    df['Date'] = pd.to_datetime(df['Date'])
+    df.set_index('Date', inplace=True, drop=False)
+    return df
```

### Comparing `algotik_tse-0.3.8/algotik_tse/settings.py` & `algotik_tse-0.3.9/algotik_tse/settings.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/algotik_tse.egg-info/PKG-INFO` & `algotik_tse-0.3.9/algotik_tse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algotik_tse
-Version: 0.3.8
+Version: 0.3.9
 Summary: Get all data from TSETMC.com (Tehran Bourse).
 Home-page: https://github.com/mohsenalipour/algotik_tse
 Author: Mohsen Alipour
 Author-email: alipour@algotik.ir
 License: GNU General Public License v3
 Keywords: algotik_tse
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -256,7 +256,12 @@
 * seventh release on PyPI.
 * Add currencies and coins in beta phase.
 
 0.3.8 (2024-02-27)
 ------------------
 * eighth release on PyPI.
 * Add payeh market color in stocklist.
+
+0.3.9 (2024-03-08)
+------------------
+* ninth release on PyPI.
+* bug fix in shareholders change_amount.
```

### Comparing `algotik_tse-0.3.8/algotik_tse.egg-info/SOURCES.txt` & `algotik_tse-0.3.9/algotik_tse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/docs/Makefile` & `algotik_tse-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/docs/conf.py` & `algotik_tse-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/docs/installation.rst` & `algotik_tse-0.3.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/docs/make.bat` & `algotik_tse-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `algotik_tse-0.3.8/setup.py` & `algotik_tse-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     include_package_data=True,
     keywords='algotik_tse',
     name='algotik_tse',
     packages=find_packages(include=['algotik_tse', 'algotik_tse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mohsenalipour/algotik_tse',
-    version='0.3.8',
+    version='0.3.9',
     zip_safe=False,
 )
```

### Comparing `algotik_tse-0.3.8/tests/test_algotik_tse.py` & `algotik_tse-0.3.9/tests/test_algotik_tse.py`

 * *Files identical despite different names*

