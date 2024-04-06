# Comparing `tmp/backtrader_bybit-2.0.7.tar.gz` & `tmp/backtrader_bybit-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_bybit-2.0.7.tar", last modified: Mon Mar 18 06:37:10 2024, max compression
+gzip compressed data, was "backtrader_bybit-2.0.8.tar", last modified: Sat Apr  6 04:52:18 2024, max compression
```

## Comparing `backtrader_bybit-2.0.7.tar` & `backtrader_bybit-2.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 06:37:10.918732 backtrader_bybit-2.0.7/
--rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_bybit-2.0.7/LICENSE
--rw-rw-rw-   0        0        0    31184 2024-03-18 06:37:10.918732 backtrader_bybit-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    29811 2024-03-18 06:34:30.000000 backtrader_bybit-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 06:37:10.912736 backtrader_bybit-2.0.7/backtrader_bybit/
--rw-rw-rw-   0        0        0       36 2024-02-03 14:15:41.000000 backtrader_bybit-2.0.7/backtrader_bybit/__init__.py
--rw-rw-rw-   0        0        0     9171 2024-02-05 17:46:55.000000 backtrader_bybit-2.0.7/backtrader_bybit/bybit_broker.py
--rw-rw-rw-   0        0        0    13877 2024-03-08 08:45:43.000000 backtrader_bybit-2.0.7/backtrader_bybit/bybit_feed.py
--rw-rw-rw-   0        0        0     6277 2024-03-06 06:57:44.000000 backtrader_bybit-2.0.7/backtrader_bybit/bybit_store.py
--rw-rw-rw-   0        0        0      828 2024-02-04 18:39:19.000000 backtrader_bybit-2.0.7/backtrader_bybit/enums.py
-drwxrwxrwx   0        0        0        0 2024-03-18 06:37:10.917736 backtrader_bybit-2.0.7/backtrader_bybit.egg-info/
--rw-rw-rw-   0        0        0    31184 2024-03-18 06:37:10.000000 backtrader_bybit-2.0.7/backtrader_bybit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-03-18 06:37:10.000000 backtrader_bybit-2.0.7/backtrader_bybit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 06:37:10.000000 backtrader_bybit-2.0.7/backtrader_bybit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-18 06:37:10.000000 backtrader_bybit-2.0.7/backtrader_bybit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-18 06:37:10.000000 backtrader_bybit-2.0.7/backtrader_bybit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 06:37:10.919731 backtrader_bybit-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2174 2024-03-18 04:27:37.000000 backtrader_bybit-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:52:18.536586 backtrader_bybit-2.0.8/
+-rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_bybit-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0    31184 2024-04-06 04:52:18.536586 backtrader_bybit-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    29811 2024-03-18 06:34:30.000000 backtrader_bybit-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 04:52:18.531586 backtrader_bybit-2.0.8/backtrader_bybit/
+-rw-rw-rw-   0        0        0       36 2024-02-03 14:15:41.000000 backtrader_bybit-2.0.8/backtrader_bybit/__init__.py
+-rw-rw-rw-   0        0        0     9171 2024-02-05 17:46:55.000000 backtrader_bybit-2.0.8/backtrader_bybit/bybit_broker.py
+-rw-rw-rw-   0        0        0    13887 2024-04-06 04:39:55.000000 backtrader_bybit-2.0.8/backtrader_bybit/bybit_feed.py
+-rw-rw-rw-   0        0        0     6277 2024-03-06 06:57:44.000000 backtrader_bybit-2.0.8/backtrader_bybit/bybit_store.py
+-rw-rw-rw-   0        0        0      828 2024-02-04 18:39:19.000000 backtrader_bybit-2.0.8/backtrader_bybit/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:52:18.535589 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/
+-rw-rw-rw-   0        0        0    31184 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 04:52:18.000000 backtrader_bybit-2.0.8/backtrader_bybit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 04:52:18.537585 backtrader_bybit-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2174 2024-04-06 04:51:48.000000 backtrader_bybit-2.0.8/setup.py
```

### Comparing `backtrader_bybit-2.0.7/LICENSE` & `backtrader_bybit-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.7/PKG-INFO` & `backtrader_bybit-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader_bybit
-Version: 2.0.7
+Version: 2.0.8
 Summary: Bybit API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_bybit
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_bybit/blob/master/README.md
 Keywords: trading,development
```

### Comparing `backtrader_bybit-2.0.7/README.md` & `backtrader_bybit-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.7/backtrader_bybit/bybit_broker.py` & `backtrader_bybit-2.0.8/backtrader_bybit/bybit_broker.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.7/backtrader_bybit/bybit_feed.py` & `backtrader_bybit-2.0.8/backtrader_bybit/bybit_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,18 +200,18 @@
             else:
                 if self.interval == 'D': delta_time = 60 * 24
                 if self.interval == 'W': delta_time = 60 * 24 * 7
                 if self.interval == 'M': delta_time = 60 * 24 * 30
 
             total_minutes = (datetime.now() - self.start_date).total_seconds() // 60
             num_requests = int(total_minutes // (self.limit * delta_time))
-            self.start_date = round(self.start_date.timestamp()*1000)
 
             # get all rows by limit per request
             for i in range(num_requests+1):
+                self.start_date = round(self.start_date.timestamp() * 1000)
                 _now = datetime.now()
                 klines = self._store.bybit_session.get_kline(
                     category=self._store.category,
                     symbol=self.symbol,
                     interval=self.interval,
                     start=self.start_date,  # in milliseconds
                     # end=round(_now.timestamp()*1000),  # in milliseconds
@@ -244,19 +244,19 @@
                     print("Exception (try set from_date in utc format):", e)
 
                 # change self.start_date at every request
                 if self.all_history_data:
                     self.start_date = self.all_history_data[-1][0]  # timestamp
                     # b = self.start_date
                     self.start_date = datetime.fromtimestamp(int(self.start_date) / 1000) + timedelta(minutes=delta_time)
-                    self.start_date = round(int(self.start_date.timestamp()) * 1000)
+                    # self.start_date = round(int(self.start_date.timestamp()) * 1000)
                     # print(f"\t --> {datetime.fromtimestamp(int(b) / 1000)} {datetime.fromtimestamp(int(self.start_date) / 1000)}")
                 else:
                     self.start_date = datetime.fromtimestamp(int(self.start_date) / 1000) + timedelta(minutes=delta_time * self.limit)
-                    self.start_date = round(int(self.start_date.timestamp()) * 1000)
+                    # self.start_date = round(int(self.start_date.timestamp()) * 1000)
 
         else:
             self._start_live()
 
     def get_previous_future_candle_time(self, ):
         # timeframe = "D1"
         now = datetime.now()
```

### Comparing `backtrader_bybit-2.0.7/backtrader_bybit/bybit_store.py` & `backtrader_bybit-2.0.8/backtrader_bybit/bybit_store.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.7/backtrader_bybit/enums.py` & `backtrader_bybit-2.0.8/backtrader_bybit/enums.py`

 * *Files identical despite different names*

### Comparing `backtrader_bybit-2.0.7/backtrader_bybit.egg-info/PKG-INFO` & `backtrader_bybit-2.0.8/backtrader_bybit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader-bybit
-Version: 2.0.7
+Version: 2.0.8
 Summary: Bybit API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_bybit
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_bybit/blob/master/README.md
 Keywords: trading,development
```

### Comparing `backtrader_bybit-2.0.7/setup.py` & `backtrader_bybit-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the relevant file
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='backtrader_bybit',
-      version='2.0.7',
+      version='2.0.8',
       author='wiseplat',
       author_email='oshpagin@gmail.com',
       license='MIT License',
       description='Bybit API integration with Backtrader',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/WISEPLAT/backtrader_bybit',
```

