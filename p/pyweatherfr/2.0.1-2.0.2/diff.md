# Comparing `tmp/pyweatherfr-2.0.1.tar.gz` & `tmp/pyweatherfr-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-2.0.1.tar", last modified: Sat Apr  6 10:42:40 2024, max compression
+gzip compressed data, was "pyweatherfr-2.0.2.tar", last modified: Sat Apr  6 14:52:37 2024, max compression
```

## Comparing `pyweatherfr-2.0.1.tar` & `pyweatherfr-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:40.763970 pyweatherfr-2.0.1/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    35192 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:52:37.272758 pyweatherfr-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 14:52:37.272758 pyweatherfr-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:52:37.272758 pyweatherfr-2.0.2/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37201 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:52:37.272758 pyweatherfr-2.0.2/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 14:52:37.000000 pyweatherfr-2.0.2/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 14:52:37.272758 pyweatherfr-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 14:52:33.000000 pyweatherfr-2.0.2/setup.py
```

### Comparing `pyweatherfr-2.0.1/LICENSE.txt` & `pyweatherfr-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.1/PKG-INFO` & `pyweatherfr-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.1
+Version: 2.0.2
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.1/README.md` & `pyweatherfr-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.1/pyweatherfr/args.py` & `pyweatherfr-2.0.2/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.1/pyweatherfr/pyweatherfr.py` & `pyweatherfr-2.0.2/pyweatherfr/pyweatherfr.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,32 +331,32 @@
     print_generic_data_town(infos, city, gps, elevation)
     # Utilisation d'une expression régulière pour extraire les nombres
     matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
 
     # Récupération des deux nombres extraits
     latitude = float(matches[0])
     longitude = float(matches[1])
-    hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m,surface_pressure,current_weather_code=specific_day(latitude,longitude,compute_args().jour)
+    hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m,surface_pressure,current_weather_code,snowfall,relative_humidity_2m=specific_day(latitude,longitude,compute_args().jour)
     data = []
     for h in range(0, 24):
         warning=""
         if compute_args().jour==0 and 0<h-int(datetime.datetime.now().strftime('%H'))<=1:
             warning=warning+CLOCK
         temp = f"{hourly_temperature_2m[h]:.1f}° ({hourly_apparent_temperature[h]:.1f}°)"
         if float(hourly_temperature_2m[h])<0 or float(hourly_apparent_temperature[h])<0:
             warning=warning+" "+print_emoji(COLD)
         if hourly_temperature_2m[h]>30 or hourly_apparent_temperature[h]>30:           
             warning=warning+" "+print_emoji(WARM)            
         pluie = f"{hourly_precipitation[h]:.1f}mm"
-        if hourly_precipitation[h]>0:
-            warning=warning+" "+print_emoji(RAIN) 
-        vent = f"{hourly_wind_speed_10m[h]:.1f}km/h ({hourly_wind_gusts_10m[h]:.1f}km/h)"  
-
-
+        if snowfall[h]>0:
+            warning=warning+" "+print_emoji(FLOCON)
+        elif hourly_precipitation[h]>0:
+            warning=warning+" "+print_emoji(DROPLET) 
 
+        vent = f"{hourly_wind_speed_10m[h]:.1f}km/h ({hourly_wind_gusts_10m[h]:.1f}km/h)"  
         if hourly_wind_direction_10m[h]<=22.5 or hourly_wind_direction_10m[h]>=360-22.5:
             direction="N"
         if hourly_wind_direction_10m[h]<=360-22.5 and hourly_wind_direction_10m[h]>360-22.5-45:
             direction="NO"
         if hourly_wind_direction_10m[h]<=360-22.5-45 and hourly_wind_direction_10m[h]>360-22.5-90:
             direction="W"
         if hourly_wind_direction_10m[h]<=360-22.5-90 and hourly_wind_direction_10m[h]>360-22.5-135:
@@ -375,24 +375,25 @@
             warning=warning+" "+print_emoji(WIND)
 
         pression=f"{surface_pressure[h]:.1f}Hpa"
         if surface_pressure[h]>1030:
             warning=warning+" "+print_emoji(ELEPHANT)     
         if surface_pressure[h]<990:
             warning=warning+" "+print_emoji(PLUME)
-        weather,emojiweather=traduction(current_weather_code[h])                     
+        weather,emojiweather=traduction(current_weather_code[h])
+        humidity=f"{relative_humidity_2m[h]:.0f}%"                     
         if compute_args().nocolor:
-            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),weather,temp,pluie,vent,direction,pression])    
+            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),weather,temp,pluie,vent,direction,pression,humidity])    
         else:
-            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),emojiweather + " " + weather,temp,pluie,vent,direction,pression,warning])
+            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),emojiweather + " " + weather,temp,pluie,vent,direction,pression,humidity,warning])
     
     if compute_args().nocolor:
-        headers = ["date", "temps", "température (ressenties)", "précipitations", "vent (rafales)","direction","pression"]
+        headers = ["date", "temps", "température (ressenties)", "précipitations", "vent (rafales)","direction","pression","humidité"]
     else:
-        headers = ["date", "temps", "température (ressenties)", "précipitations", "vent (rafales)","direction","pression","warnings"]
+        headers = ["date", "temps", "température (ressenties)", "précipitations", "vent (rafales)","direction","pression","humidité","warnings"]
 
     if data != []:
         if compute_args().condensate:
             table = columnar(data, no_borders=True, wrap_max=0)
         else:
             print("")
             table = columnar(
@@ -496,35 +497,60 @@
 
     print_generic_data_town(infos, city, gps, elevation)
 
     matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
     latitude = float(matches[0])
     longitude = float(matches[1])
     
-    date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant,weather_code=resume(latitude,longitude)
+    date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant,weather_code,snowfall=resume(latitude,longitude)
     data2 = []
     for i in [0, 1, 2, 3]:
         warning=""
         if i==0:
             warning=warning+CLOCK
         pluie = f"{daily_precipitation_sum[i]:.1f}mm"
-        if daily_precipitation_sum[i]>0:
-            warning = warning + print_emoji(RAIN)
+        if snowfall[i]>0:
+            warning = warning + print_emoji(FLOCON)
+        elif daily_precipitation_sum[i]>0:
+            warning = warning + print_emoji(DROPLET)
         temp = f"{daily_temperature_2m_min[i]:.1f}° ({daily_apparent_temperature_min[i]:.1f}°) -> {daily_temperature_2m_max[i]:.1f}° ({daily_apparent_temperature_max[i]:.1f}°)"
         if daily_temperature_2m_min[i] <0 or daily_apparent_temperature_min[i] < 0 or daily_temperature_2m_max[i] <0 or daily_apparent_temperature_max[i] <0:
             warning = warning + print_emoji(COLD)
         if daily_temperature_2m_min[i] >30 or daily_apparent_temperature_min[i] >30 or daily_temperature_2m_max[i] >30 or daily_apparent_temperature_max[i] >30:
             warning = warning + print_emoji(WARM) 
-        weather,emojiweather=traduction(weather_code[i])          
+        weather,emojiweather=traduction(weather_code[i]) 
+
+        vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"  
+        if daily_wind_direction_10m_dominant[i]<=22.5 or daily_wind_direction_10m_dominant[i]>=360-22.5:
+            direction="N"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5 and daily_wind_direction_10m_dominant[i]>360-22.5-45:
+            direction="NO"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5-45 and daily_wind_direction_10m_dominant[i]>360-22.5-90:
+            direction="W"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5-90 and daily_wind_direction_10m_dominant[i]>360-22.5-135:
+            direction="SO"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5-135 and daily_wind_direction_10m_dominant[i]>360-22.5-180:
+            direction="S"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5-180 and daily_wind_direction_10m_dominant[i]>360-22.5-225:
+            direction="SE"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5-225 and daily_wind_direction_10m_dominant[i]>360-22.5-270:
+            direction="E"
+        if daily_wind_direction_10m_dominant[i]<=360-22.5-270 and daily_wind_direction_10m_dominant[i]>360-22.5-315:
+            direction="NE"
+
+        vent=vent
+        if daily_wind_speed_10m_max[i]>30 or daily_wind_gusts_10m_max[i]>50:
+            warning=warning+" "+print_emoji(WIND)        
+
         if compute_args().nocolor:
-            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),weather,temp,pluie])
-            headers = ["date", "temps", "température", "précipitations"]
+            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),weather,temp,pluie,vent,direction])
+            headers = ["date", "temps", "température", "précipitations","vent (rafales)","direction"]
         else:
-            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),emojiweather + " " + weather,temp,pluie,warning])
-            headers = ["date", "temps", "température", "précipitations","warning"]    
+            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),emojiweather + " " + weather,temp,pluie,vent,direction,warning])
+            headers = ["date", "temps", "température", "précipitations","vent (rafales)","direction","warning"]    
 
 
     if data2 != []:
         if compute_args().condensate:
             table = columnar(data2, no_borders=True, wrap_max=0)
         else:
             print("")
@@ -890,15 +916,15 @@
     # Make sure all required weather variables are listed here
     # The order of variables in hourly or daily is important to assign them correctly below
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "timezone": "Europe/Paris",
         "latitude": latitude,
         "longitude": longitude,
-        "daily": ["temperature_2m_max", "temperature_2m_min", "apparent_temperature_max", "apparent_temperature_min", "precipitation_sum", "wind_speed_10m_max", "wind_gusts_10m_max", "wind_direction_10m_dominant","weather_code"]
+        "daily": ["temperature_2m_max", "temperature_2m_min", "apparent_temperature_max", "apparent_temperature_min", "precipitation_sum", "wind_speed_10m_max", "wind_gusts_10m_max", "wind_direction_10m_dominant","weather_code","snowfall_sum"]
     }
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
 
     # Process daily data. The order of variables needs to be the same as requested.
@@ -908,28 +934,29 @@
     daily_apparent_temperature_max = daily.Variables(2).ValuesAsNumpy()
     daily_apparent_temperature_min = daily.Variables(3).ValuesAsNumpy()
     daily_precipitation_sum = daily.Variables(4).ValuesAsNumpy()
     daily_wind_speed_10m_max = daily.Variables(5).ValuesAsNumpy()
     daily_wind_gusts_10m_max = daily.Variables(6).ValuesAsNumpy()
     daily_wind_direction_10m_dominant = daily.Variables(7).ValuesAsNumpy()
     weather_code= daily.Variables(8).ValuesAsNumpy()
+    snowfall=daily.Variables(9).ValuesAsNumpy()
     date_debut= pd.to_datetime(daily.Time(), unit = "s", utc = True)
-    return date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant,weather_code
+    return date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant,weather_code,snowfall
 
 
 def specific_day(latitude,longitude,day):
     cache_session = requests_cache.CachedSession(get_user_config_directory_pyweather()+ '.cache', expire_after = 3600)
     retry_session = retry(cache_session, retries = 5, backoff_factor = 0.2)
     openmeteo = openmeteo_requests.Client(session = retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "timezone": "Europe/Paris",
         "latitude": latitude,
         "longitude": longitude,
-        "hourly": ["temperature_2m", "apparent_temperature", "precipitation", "wind_speed_10m", "wind_gusts_10m", "wind_direction_10m", "pressure_msl","weather_code"],
+        "hourly": ["temperature_2m", "apparent_temperature", "precipitation", "wind_speed_10m", "wind_gusts_10m", "wind_direction_10m", "pressure_msl","weather_code","snowfall","relative_humidity_2m"],
         "start_date": (datetime.datetime.now()+ datetime.timedelta(days=day)).strftime('%Y-%m-%d'),
         "end_date": (datetime.datetime.now()+ datetime.timedelta(days=day+1)).strftime('%Y-%m-%d'),
     }
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
@@ -940,15 +967,17 @@
     hourly_apparent_temperature = hourly.Variables(1).ValuesAsNumpy()
     hourly_precipitation = hourly.Variables(2).ValuesAsNumpy()
     hourly_wind_speed_10m = hourly.Variables(3).ValuesAsNumpy()
     hourly_wind_gusts_10m = hourly.Variables(4).ValuesAsNumpy()
     hourly_wind_direction_10m = hourly.Variables(5).ValuesAsNumpy()
     surface_pressure = hourly.Variables(6).ValuesAsNumpy()
     weather_code = hourly.Variables(7).ValuesAsNumpy()
-    return hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m, surface_pressure, weather_code
+    snowfall = hourly.Variables(8).ValuesAsNumpy()
+    relative_humidity_2m = hourly.Variables(9).ValuesAsNumpy()
+    return hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m, surface_pressure, weather_code, snowfall, relative_humidity_2m
 
 
 
 def current(latitude,longitude):
     cache_session = requests_cache.CachedSession(get_user_config_directory_pyweather() + '.cache', expire_after = 3600)
     retry_session = retry(cache_session, retries = 5, backoff_factor = 0.2)
     openmeteo = openmeteo_requests.Client(session = retry_session)
```

### Comparing `pyweatherfr-2.0.1/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-2.0.2/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.1
+Version: 2.0.2
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.1/setup.py` & `pyweatherfr-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="2.0.1",
+    version="2.0.2",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

