# Comparing `tmp/smartboiler-0.0.3.0.0.5.9.4.tar.gz` & `tmp/smartboiler-0.0.3.0.0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.5.9.4.tar", last modified: Thu Apr  4 12:07:46 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.6.0.tar", last modified: Sat Apr  6 08:20:29 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.5.9.4.tar` & `smartboiler-0.0.3.0.0.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-04 12:07:44.000000 smartboiler-0.0.3.0.0.5.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.132151 smartboiler-0.0.3.0.0.5.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/web_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-04 12:07:41.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:07:46.136151 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 12:07:46.000000 smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-06 08:20:28.000000 smartboiler-0.0.3.0.0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:20:29.525961 smartboiler-0.0.3.0.0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/src/smartboiler/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/src/smartboiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-06 08:20:24.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:20:29.529961 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-06 08:20:29.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-06 08:20:29.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:20:29.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 08:20:29.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-06 08:20:29.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 08:20:29.000000 smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.5.9.4/PKG-INFO` & `smartboiler-0.0.3.0.0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.9.4
+Version: 0.0.3.0.0.6.0
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.9.4/README.md` & `smartboiler-0.0.3.0.0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/setup.py` & `smartboiler-0.0.3.0.0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.5.9.4',  # Required
+    version='0.0.3.0.0.6.0',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/command_line.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/command_line.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/data_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,19 +152,19 @@
             "measurement": "°C",
         },
         "boiler_relay_status": {
             "sql_query": f'SELECT last("value") AS "boiler_relay_status" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.relay_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "state",
         },
         "device_longitude": {
-            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(linear)',
             "measurement": "state",
         },
         "device_latitude": {
-            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
+            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(linear)',
             "measurement": "state",
         },
         
     } 
 
     def haversine_dist(self, x1, x2, y1, y2):
         return haversine((x1, x2), (y1, y2), unit="km")
@@ -407,51 +407,60 @@
         window = 3
 
         df["longtime_mean"] = (
             df["consumed_heat_kWh"]
             .rolling(window=window, min_periods=1, center=True)
             .mean()
         )
-        # df['longtime_mean'] = df['consumed_heat_kWh']
-        df["longtime_std"] = (
-            df["consumed_heat_kWh"].rolling(window=window, min_periods=1).std()
-        )
-        df["longtime_min"] = (
-            df["consumed_heat_kWh"].rolling(window=window, min_periods=1).min()
-        )
-        df["longtime_max"] = (
-            df["consumed_heat_kWh"].rolling(window=window, min_periods=1).max()
-        )
-        df["longtime_median"] = (
-            df["consumed_heat_kWh"].rolling(window=window, min_periods=1).median()
-        )
-        df["longtime_skew"] = (
-            df["consumed_heat_kWh"].rolling(window=window, min_periods=1).skew()
-        )
+
 
         # drop consumed_heat_kWh
+        
+        df['last_3_week_mean'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).mean().reset_index(level=[0,1], drop=True)
+        df['last_3_week_mean'] = df['last_3_week_mean'].fillna(method='ffill')
+        
+        df['last_3_week_std'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).std().reset_index(level=[0,1], drop=True)
+        df['last_3_week_std'] = df['last_3_week_std'].fillna(method='ffill')
+        
+        df['last_3_week_max'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).max().reset_index(level=[0,1], drop=True)
+        df['last_3_week_max'] = df['last_3_week_max'].fillna(method='ffill')
+        
+        df['last_3_week_min'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).min().reset_index(level=[0,1], drop=True)
+        df['last_3_week_min'] = df['last_3_week_min'].fillna(method='ffill')
+        
+        df['last_3_week_skew'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).skew().reset_index(level=[0,1], drop=True)
+        df['last_3_week_skew'] = df['last_3_week_skew'].fillna(method='ffill')
+        
+        df['last_3_week_median'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).median().reset_index(level=[0,1], drop=True)
+        df['last_3_week_median'] = df['last_3_week_median'].fillna(method='ffill') 
+        
         df = df.drop(columns=["consumed_heat_kWh"])
-
-        df["longtime_std"] = df["longtime_std"].fillna(method="ffill")
-        df["longtime_std"] = df["longtime_std"].fillna(method="ffill")
-        df["longtime_skew"] = df["longtime_mean"].fillna(method="ffill")
-
         # transform weekday, minute, hour to sin cos
         df["weekday_sin"] = np.sin(2 * df["weekday"] * np.pi / 7)
         df["weekday_cos"] = np.cos(2 * df["weekday"] * np.pi / 7)
 
         df["hour_sin"] = np.sin(2 * df["hour"] * np.pi / 24)
         df["hour_cos"] = np.cos(2 * df["hour"] * np.pi / 24)
 
         df["minute_sin"] = np.sin(2 * df["minute"] * np.pi / 60)
         df["minute_cos"] = np.cos(2 * df["minute"] * np.pi / 60)
 
         df = df[
             [
                 "longtime_mean",
+                
+                
+                # "last_3_week_mean",
+                # "last_3_week_median",
+                "last_3_week_skew",
+                "last_3_week_std",
+                # "last_3_week_min",
+                # "last_3_week_max",
+                
+                
                 # "longtime_min",
                 # "longtime_max",
                 "distance_from_home",
                 # # "speed",
                 "speed_towards_home",
                 "count",
                 "heading_to_home_sin",
```

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/forecast.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import numpy as np
 import pandas as pd
 from scipy import stats
 from pickle import load
 from pickle import dump
 
 
-from smartboiler.data_handler import DataHandler
+from data_handler import DataHandler
 
 
 class Forecast:
     def __init__(
         self,
         dataHandler: DataHandler,
         start_of_data: datetime,
@@ -39,15 +39,15 @@
         self.lookback = 32
 
         self.delay = 1
         self.predicted_columns = predicted_columns
         self.dataHandler = dataHandler
         self.scaler = RobustScaler()
         self.start_of_data = start_of_data
-        
+
         self.model_path = model_path
         self.scaler_path = scaler_path
 
     def train_model(
         self,
         begin_of_training=None,
         end_of_training=None,
@@ -60,25 +60,23 @@
                 end_of_training = datetime.now()
             print("begin of training: ", begin_of_training)
             print("end of training : ", end_of_training)
             df_training_data, _ = self.dataHandler.get_data_for_training_model(
                 left_time_interval=begin_of_training,
                 right_time_interval=end_of_training,
                 predicted_columns=self.predicted_columns,
-
                 dropna=False,
             )
 
         self.num_of_features = len(df_training_data.columns) - 1
         self.df_train_norm = df_training_data.copy()
         self.df_train_norm[df_training_data.columns] = self.scaler.fit_transform(
             df_training_data
         )
-        dump(self.scaler, open(self.scaler_path, 'wb'))
-
+        dump(self.scaler, open(self.scaler_path, "wb"))
 
         self.train_gen = self.mul_generator(
             dataframe=self.df_train_norm,
             target_names=self.predicted_columns,
             lookback=self.lookback,
             delay=self.delay,
             min_index=0,
@@ -104,54 +102,55 @@
             (self.df_train_norm.shape[0] * 0.1 - self.lookback) // self.batch_size
         )
         # This is how many steps to draw from `train_gen`
         # in order to see the whole train set:
         self.train_steps = int(
             (self.df_train_norm.shape[0] * 0.9 - self.lookback) // self.batch_size
         )
-        
+
         callbacks = [
             EarlyStopping(
                 monitor="loss",
                 min_delta=0,
                 patience=10,
                 verbose=2,
                 mode="auto",
                 restore_best_weights=True,
             ),
-
-            ModelCheckpoint(verbose=1, filepath=self.model_path, save_best_only=True, save_weights_only=True)
-            ]
+            ModelCheckpoint(
+                verbose=1,
+                filepath=self.model_path,
+                save_best_only=True,
+                save_weights_only=True,
+            ),
+        ]
 
         print("Start training")
         history = self.model.fit(
             self.train_gen,
             steps_per_epoch=self.train_steps,
             epochs=100,
             shuffle=False,
             validation_data=self.valid_gen,
             validation_steps=self.val_steps,
             callbacks=callbacks,
             verbose=2,
         )
-        
+
         self.model.save(self.model_path)
         print("End training")
 
-
     def load_model(
         self,
         left_time_interval=datetime.now() - timedelta(days=4),
         right_time_interval=datetime.now(),
     ):
-        
-        self.scaler = load(open(self.scaler_path, 'rb'))
-        self.model.load_weights(self.model_path)
-
 
+        self.scaler = load(open(self.scaler_path, "rb"))
+        self.model.load_weights(self.model_path)
 
     def generator(
         self,
         dataframe,
         target_name,
         lookback,
         delay,
@@ -160,15 +159,15 @@
         shuffle=False,
         batch_size=128,
         step=6,
     ):
         data_without_target = dataframe.copy()
         data_without_target = data_without_target.drop(columns=[target_name]).values
         data_without_target = data_without_target.astype(np.float32)
-        
+
         data = dataframe.values
         data = data.astype(np.float32)
         target_indx = dataframe.columns.get_loc(target_name)
 
         if max_index is None:
             max_index = len(data) - delay - 1
         i = min_index + lookback
@@ -179,70 +178,67 @@
                 )
             else:
                 if i + batch_size >= max_index:
                     i = min_index + lookback
                 rows = np.arange(i, min(i + batch_size, max_index))
                 i += len(rows)
 
-            samples = np.zeros((len(rows), lookback // step, data_without_target.shape[-1]))
+            samples = np.zeros(
+                (len(rows), lookback // step, data_without_target.shape[-1])
+            )
             targets = np.zeros((len(rows),))
-            
+
             for j, row in enumerate(rows):
                 indices = range(rows[j] - lookback, rows[j], step)
                 # samples without column with target
                 samples[j] = data_without_target[indices]
                 targets[j] = data[rows[j] + delay][target_indx]
             yield samples, targets
-            
+
     def r2_keras(self, y_true, y_pred):
         """Coefficient of Determination"""
         SS_res = K.sum(K.square(y_true - y_pred))
         SS_tot = K.sum(K.square(y_true - K.mean(y_true)))
         return 1 - SS_res / (SS_tot + K.epsilon())
 
-
-
     def build_model(self):
 
         model = Sequential()
-        model.add(Input(shape=(None,11)))
+        model.add(Input(shape=(None, 13)))
 
         # Add LSTM layer
         model.add(LSTM(100))
         model.add(Dense(1))
 
         self.model = model
         self.model.compile(loss="mae", optimizer="adam")
         return model
 
     def fit_model(self):
         pass
 
-        
         # self.model.save(self.model_path)
 
-
-        
-        
-
     def add_empty_row(self, df, date_time, predicted_value):
 
         last_row_values = df.iloc[-1].values
 
         new_row_df = pd.DataFrame(
             columns=df.columns,
             data=[
                 [
                     predicted_value,
                     last_row_values[1],
                     last_row_values[2],
                     last_row_values[3],
                     last_row_values[4],
                     last_row_values[5],
-
+                    last_row_values[6],
+                    last_row_values[7],
+                    
                     np.sin(2 * np.pi * date_time.weekday() / 7),
                     np.cos(2 * np.pi * date_time.weekday() / 7),
                     np.sin(2 * np.pi * date_time.hour / 24),
                     np.cos(2 * np.pi * date_time.hour / 24),
                     np.sin(2 * np.pi * date_time.minute / 60),
                     np.cos(2 * np.pi * date_time.minute / 60),
                 ]
@@ -305,94 +301,89 @@
 
                 # Assign values for each target column
                 for k, target_indx in enumerate(target_indices):
                     targets[j][k] = data[rows[j] + delay][target_indx]
 
             yield samples, targets
 
-    def get_forecast_next_steps(self, left_time_interval=None, right_time_interval=None):
+    def get_forecast_next_steps(
+        self, left_time_interval=None, right_time_interval=None
+    ):
         # Define the indices for the different predictions and truths
         if left_time_interval is None:
-            left_time_interval = datetime.now() - timedelta(days=5)
+            left_time_interval = datetime.now() - timedelta(days=30)
         if right_time_interval is None:
             right_time_interval = datetime.now()
-            
-        
-        forecast_future = pd.DataFrame()
-        
-        #set minutes to 0
-        left_time_interval = left_time_interval.replace(minute=0)
-        right_time_interval = right_time_interval.replace(minute=0)
 
+        forecast_future = pd.DataFrame()
 
         df_all = self.dataHandler.get_data_for_prediction(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
-        
+
         num_targets = len(self.predicted_columns)
         len_columns = len(df_all.columns)
-        
-        df_all = df_all.dropna()
-        df_all = df_all.reset_index(drop=True)
-        
         forecast_future = pd.DataFrame()
 
+        # print last row of df all
+
+        forecast_future = pd.DataFrame()
+        
         current_forecast_begin_date = right_time_interval + timedelta(hours=1)
 
         df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
         current_forecast_begin_date += timedelta(hours=1)
 
         # prediction for next 6 hours
         for i in range(0, 6):
-            print(df_all["minute_cos"])
+
+                        
             df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
             current_forecast_begin_date += timedelta(hours=1)
 
-            
-            df_predict_norm = df_all.copy()
+            df_test_norm = df_all.reset_index(drop=True).dropna().copy()
 
-            df_predict_norm[df_all.columns] = self.scaler.transform(df_all)
-            # create predict df with values
-            predict_gen = self.mul_generator(
+            # df_test_norm = df_test_zuka.copy()
+            df_test_norm[df_test_norm.columns] = self.scaler.transform(df_test_norm)
 
-                dataframe=df_predict_norm,
+            test_gen = self.mul_generator(
+                dataframe=df_test_norm,
                 target_names=self.predicted_columns,
                 lookback=self.lookback,
                 delay=self.delay,
                 min_index=0,
                 max_index=None,
                 step=1,
                 shuffle=False,
-                batch_size=df_predict_norm.shape[0],
+                batch_size=df_test_norm.shape[0],
             )
-
-            (X, y_truth) = next(predict_gen)
-
+            
+            (X, y_truth) = next(test_gen)
+            
+            num_targets = len(self.predicted_columns)
+            len_columns = len(df_test_norm.columns)
+            num_features = len_columns - num_targets
+            
             y_pred = self.model.predict(X, verbose=0)
-            # np.expand_dims(y_truth,axis=1).shape
             y_pred_inv = np.concatenate(
-                (y_pred, np.zeros((y_pred.shape[0], len_columns - num_targets))), axis=1
+                (y_pred, np.zeros((y_pred.shape[0], num_features))), axis=1
             )
-            y_pred_inv = self.scaler.inverse_transform(y_pred_inv)
 
+            y_pred_inv = self.scaler.inverse_transform(y_pred_inv)
             # get last predicted value
-            y_pred_inv = y_pred_inv[-1, :]
-            
+            y_pred_inv = y_pred_inv[-1, 0]
             # y_pred_inv[0] is min 0
-            if y_pred_inv[0] < 0:
-                y_pred_inv[0] = 0
-            
-            df_all.iloc[-2][0] = y_pred_inv[0]
+            if y_pred_inv < 0:
+                y_pred_inv = 0
 
+            # set last longtimemean value
+            df_all.iloc[-2, df_all.columns.get_loc("longtime_mean")] = y_pred_inv
 
-            # append y_pred_inv to df_all
-            # df_all.iloc[-1, :num_targets] = y_pred_inv[:num_targets]
-            # drop first row
-            df_all = df_all[1:]
+            # df_all = df_all[1:]
 
             forecast_future = pd.concat(
                 [
                     forecast_future,
                     df_all.iloc[[-2], df_all.columns.get_loc("longtime_mean")],
                 ],
                 axis=0,
```

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/machine_learning_forecaster.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/optimization.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/optimization.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/static/style.css` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/static/style.css`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/templates/index.html` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/templates/index.html`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/utils.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/utils.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/web_server.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/web_server.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.5.9.4
+Version: 0.0.3.0.0.6.0
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.5.9.4/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.6.0/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

