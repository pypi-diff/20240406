# Comparing `tmp/pyweatherfr-2.0.0.tar.gz` & `tmp/pyweatherfr-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-2.0.0.tar", last modified: Thu Apr  4 19:42:12 2024, max compression
+gzip compressed data, was "pyweatherfr-2.0.1.tar", last modified: Sat Apr  6 10:42:40 2024, max compression
```

## Comparing `pyweatherfr-2.0.0.tar` & `pyweatherfr-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    31075 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 19:42:12.000000 pyweatherfr-2.0.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:42:12.691089 pyweatherfr-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-04 19:42:08.000000 pyweatherfr-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:40.763970 pyweatherfr-2.0.1/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35192 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 10:42:40.000000 pyweatherfr-2.0.1/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:42:40.767970 pyweatherfr-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 10:42:36.000000 pyweatherfr-2.0.1/setup.py
```

### Comparing `pyweatherfr-2.0.0/LICENSE.txt` & `pyweatherfr-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.0/PKG-INFO` & `pyweatherfr-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.0
+Version: 2.0.1
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.0/README.md` & `pyweatherfr-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.0/pyweatherfr/args.py` & `pyweatherfr-2.0.1/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-2.0.1/pyweatherfr/pyweatherfr.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 
 FLECHE_SE ="\U0000FE0F"
 
 FLECHE_E ="\U0000FE0F"
 
 FLECHE_NE ="\U0000FE0F"
 
+ELEPHANT= "\U0001F418"
+PLUME= "\U0001FAB6"
+
 
 
 def emoji_rain(key, isSnow):
     return emoji_rain_allign(key, isSnow, True)
 
 
 def emoji_rain_allign(key, isSnow, allign):
@@ -328,35 +331,28 @@
     print_generic_data_town(infos, city, gps, elevation)
     # Utilisation d'une expression régulière pour extraire les nombres
     matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
 
     # Récupération des deux nombres extraits
     latitude = float(matches[0])
     longitude = float(matches[1])
-    hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m=specific_day(latitude,longitude,compute_args().jour)
-    headers = [
-        "heure",
-        "température",
-        "humidité",
-        "précipitations",
-        "vent",
-        "direction",
-        "warning"
-    ]
+    hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m,surface_pressure,current_weather_code=specific_day(latitude,longitude,compute_args().jour)
     data = []
     for h in range(0, 24):
         warning=""
+        if compute_args().jour==0 and 0<h-int(datetime.datetime.now().strftime('%H'))<=1:
+            warning=warning+CLOCK
         temp = f"{hourly_temperature_2m[h]:.1f}° ({hourly_apparent_temperature[h]:.1f}°)"
         if float(hourly_temperature_2m[h])<0 or float(hourly_apparent_temperature[h])<0:
             warning=warning+" "+print_emoji(COLD)
         if hourly_temperature_2m[h]>30 or hourly_apparent_temperature[h]>30:           
             warning=warning+" "+print_emoji(WARM)            
         pluie = f"{hourly_precipitation[h]:.1f}mm"
         if hourly_precipitation[h]>0:
-            warning=warning+" "+print_emoji(DROPLET) 
+            warning=warning+" "+print_emoji(RAIN) 
         vent = f"{hourly_wind_speed_10m[h]:.1f}km/h ({hourly_wind_gusts_10m[h]:.1f}km/h)"  
 
 
 
         if hourly_wind_direction_10m[h]<=22.5 or hourly_wind_direction_10m[h]>=360-22.5:
             direction="N"
         if hourly_wind_direction_10m[h]<=360-22.5 and hourly_wind_direction_10m[h]>360-22.5-45:
@@ -374,62 +370,122 @@
         if hourly_wind_direction_10m[h]<=360-22.5-270 and hourly_wind_direction_10m[h]>360-22.5-315:
             direction="NE"
 
         vent=vent
         if hourly_wind_speed_10m[h]>30 or hourly_wind_gusts_10m[h]>50:
             warning=warning+" "+print_emoji(WIND)
 
+        pression=f"{surface_pressure[h]:.1f}Hpa"
+        if surface_pressure[h]>1030:
+            warning=warning+" "+print_emoji(ELEPHANT)     
+        if surface_pressure[h]<990:
+            warning=warning+" "+print_emoji(PLUME)
+        weather,emojiweather=traduction(current_weather_code[h])                     
         if compute_args().nocolor:
-            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),temp,pluie,vent,direction])    
+            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),weather,temp,pluie,vent,direction,pression])    
         else:
-            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),temp,pluie,vent,direction,warning])
+            data.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(days=compute_args().jour)+ datetime.timedelta(hours=h), "%Y-%m-%d %H:%M"),emojiweather + " " + weather,temp,pluie,vent,direction,pression,warning])
     
     if compute_args().nocolor:
-        headers = ["date", "température (ressenties)", "précipitations", "vent (rafales)","direction"]
+        headers = ["date", "temps", "température (ressenties)", "précipitations", "vent (rafales)","direction","pression"]
     else:
-        headers = ["date", "température (ressenties)", "précipitations", "vent (rafales)","direction","warnings"]
+        headers = ["date", "temps", "température (ressenties)", "précipitations", "vent (rafales)","direction","pression","warnings"]
 
     if data != []:
         if compute_args().condensate:
             table = columnar(data, no_borders=True, wrap_max=0)
         else:
             print("")
             table = columnar(
                 data, headers, no_borders=False, wrap_max=0
             )
         print(table)
 
 
-
-
-    # Affichage des résultats
-
+def traduction(current_weather_code):
+    if current_weather_code==0 or current_weather_code==1 or current_weather_code==2:
+        return ["ciel clair", SUN]
+    if current_weather_code>=3 and current_weather_code<=12:
+        return ["nuageux", CLOUD]    
+    if current_weather_code>=13 and current_weather_code<=19:
+        return ["pluie proche", RAIN] 
+    if current_weather_code>=20 and current_weather_code<=29:
+        return ["fin de pluie" , RAIN]          
+    if current_weather_code>=30 and current_weather_code<=39:
+        return ["tempete de poussière, sable ou neige", FOG]
+    if current_weather_code>=40 and current_weather_code<=49:
+        return ["brouillard", FOG]    
+    if current_weather_code>=50 and current_weather_code<=59:
+        return ["bruine", RAIN]
+    if current_weather_code>=60 and current_weather_code<=69:
+        return ["pluie", RAIN]
+    if current_weather_code>=70 and current_weather_code<=79:
+        return ["neige", SNOW]    
+    if current_weather_code>=80 and current_weather_code<=99:
+        return ["averse / orage", ORAGE_PLUIE]   
+             
 def previsions_courantes(r, infos, city):
     gps, elevation, sunrise, sunset = obtain_data(r)
     print_generic_data_town(infos, city, gps, elevation)
 
     matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
     latitude = float(matches[0])
     longitude = float(matches[1])
     
-    current_temperature_2m,current_apparent_temperature,current_relative_humidity_2m,current_precipitation,current_surface_pressure,current_wind_speed_10m,current_wind_gusts_10m,current_wind_direction_10m=current(latitude,longitude)
+    current_temperature_2m,current_apparent_temperature,current_relative_humidity_2m,current_precipitation,current_surface_pressure,current_wind_speed_10m,current_wind_gusts_10m,current_wind_direction_10m,current_weather_code=current(latitude,longitude)
+    current_weather,emojiweather=traduction(current_weather_code)
     data=[]
+    if current_wind_direction_10m>=22.5 or current_wind_direction_10m>=360-22.5:
+        direction="N"
+    if current_wind_direction_10m<=360-22.5 and current_wind_direction_10m>360-22.5-45:
+        direction="NO"
+    if current_wind_direction_10m<=360-22.5-45 and current_wind_direction_10m>360-22.5-90:
+        direction="W"
+    if current_wind_direction_10m<=360-22.5-90 and current_wind_direction_10m>360-22.5-135:
+        direction="SO"
+    if current_wind_direction_10m<=360-22.5-135 and current_wind_direction_10m>360-22.5-180:
+        direction="S"
+    if current_wind_direction_10m<=360-22.5-180 and current_wind_direction_10m>360-22.5-225:
+        direction="SE"
+    if current_wind_direction_10m<=360-22.5-225 and current_wind_direction_10m>360-22.5-270:
+        direction="E"
+    if current_wind_direction_10m<=360-22.5-270 and current_wind_direction_10m>360-22.5-315:
+        direction="NE"    
     if compute_args().nocolor:
         data.append(["température",f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)"])
         data.append(["humidité",f"{current_relative_humidity_2m:.1f}%"])
         data.append(["precipitation",f"{current_precipitation:.1f}mm"])
         data.append(["pression",f"{current_surface_pressure:.1f}Hp"])
-        data.append(["vent",f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - {current_wind_direction_10m:.1f}°"])
+        data.append(["vent",f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "+direction])
+        data.append(["temps",current_weather])
+        
     else:
-        data.append(["température",f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)"])
-        data.append(["humidité",f"{current_relative_humidity_2m:.1f}%"])
-        data.append(["precipitation",f"{current_precipitation:.1f}mm"])
-        data.append(["pression",f"{current_surface_pressure:.1f}Hp"])
-        data.append(["vent",f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - {current_wind_direction_10m:.1f}°"])
-
+        if current_temperature_2m>30 or current_apparent_temperature>30:
+            data.append(["température",f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",WARM])
+        else:
+            data.append(["température",f"{current_temperature_2m:.1f}° ({current_apparent_temperature:.1f}°)",""])    
+        if current_relative_humidity_2m>90:
+            data.append(["humidité",f"{current_relative_humidity_2m:.1f}%",DROPLET])
+        else:
+            data.append(["humidité",f"{current_relative_humidity_2m:.1f}%",""])
+        if current_precipitation>0:
+            data.append(["precipitation",f"{current_precipitation:.1f}mm",RAIN])
+        else:
+            data.append(["precipitation",f"{current_precipitation:.1f}mm",""])
+        if current_surface_pressure>1030:
+            data.append(["pression",f"{current_surface_pressure:.1f}Hp",ELEPHANT])     
+        elif current_surface_pressure<990:
+            data.append(["pression",f"{current_surface_pressure:.1f}Hp",PLUME])
+        else:              
+            data.append(["pression",f"{current_surface_pressure:.1f}Hp",""])
+        if current_wind_speed_10m>30 or current_wind_gusts_10m>50:       
+            data.append(["vent",f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "+direction,WIND])
+        else:
+            data.append(["vent",f"{current_wind_speed_10m:.1f}km/h ({current_wind_gusts_10m:.1f}km/h) - "+direction,""])   
+        data.append(["temps",emojiweather + " "  + current_weather,""])
     if compute_args().condensate:
         table = columnar(data, no_borders=True, wrap_max=0)
     else:
         print("")
         table = columnar(
             data, no_borders=False, wrap_max=0
         )
@@ -440,32 +496,35 @@
 
     print_generic_data_town(infos, city, gps, elevation)
 
     matches = re.findall(r"[-+]?\d*\.\d+|\d+", gps)
     latitude = float(matches[0])
     longitude = float(matches[1])
     
-    date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant=resume(latitude,longitude)
+    date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant,weather_code=resume(latitude,longitude)
     data2 = []
     for i in [0, 1, 2, 3]:
         warning=""
+        if i==0:
+            warning=warning+CLOCK
         pluie = f"{daily_precipitation_sum[i]:.1f}mm"
         if daily_precipitation_sum[i]>0:
-            warning = warning + print_emoji(DROPLET)
+            warning = warning + print_emoji(RAIN)
         temp = f"{daily_temperature_2m_min[i]:.1f}° ({daily_apparent_temperature_min[i]:.1f}°) -> {daily_temperature_2m_max[i]:.1f}° ({daily_apparent_temperature_max[i]:.1f}°)"
         if daily_temperature_2m_min[i] <0 or daily_apparent_temperature_min[i] < 0 or daily_temperature_2m_max[i] <0 or daily_apparent_temperature_max[i] <0:
             warning = warning + print_emoji(COLD)
         if daily_temperature_2m_min[i] >30 or daily_apparent_temperature_min[i] >30 or daily_temperature_2m_max[i] >30 or daily_apparent_temperature_max[i] >30:
-            warning = warning + print_emoji(WARM)        
+            warning = warning + print_emoji(WARM) 
+        weather,emojiweather=traduction(weather_code[i])          
         if compute_args().nocolor:
-            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),temp,pluie])
-            headers = ["date", "température", "précipitations"]
+            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),weather,temp,pluie])
+            headers = ["date", "temps", "température", "précipitations"]
         else:
-            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),temp,pluie,warning])
-            headers = ["date", "température", "précipitations","warning"]    
+            data2.append([datetime.datetime.strftime(datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)+ datetime.timedelta(hours=24*i), "%Y-%m-%d"),emojiweather + " " + weather,temp,pluie,warning])
+            headers = ["date", "temps", "température", "précipitations","warning"]    
 
 
     if data2 != []:
         if compute_args().condensate:
             table = columnar(data2, no_borders=True, wrap_max=0)
         else:
             print("")
@@ -831,15 +890,15 @@
     # Make sure all required weather variables are listed here
     # The order of variables in hourly or daily is important to assign them correctly below
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "timezone": "Europe/Paris",
         "latitude": latitude,
         "longitude": longitude,
-        "daily": ["temperature_2m_max", "temperature_2m_min", "apparent_temperature_max", "apparent_temperature_min", "precipitation_sum", "wind_speed_10m_max", "wind_gusts_10m_max", "wind_direction_10m_dominant"]
+        "daily": ["temperature_2m_max", "temperature_2m_min", "apparent_temperature_max", "apparent_temperature_min", "precipitation_sum", "wind_speed_10m_max", "wind_gusts_10m_max", "wind_direction_10m_dominant","weather_code"]
     }
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
 
     # Process daily data. The order of variables needs to be the same as requested.
@@ -848,28 +907,29 @@
     daily_temperature_2m_min = daily.Variables(1).ValuesAsNumpy()
     daily_apparent_temperature_max = daily.Variables(2).ValuesAsNumpy()
     daily_apparent_temperature_min = daily.Variables(3).ValuesAsNumpy()
     daily_precipitation_sum = daily.Variables(4).ValuesAsNumpy()
     daily_wind_speed_10m_max = daily.Variables(5).ValuesAsNumpy()
     daily_wind_gusts_10m_max = daily.Variables(6).ValuesAsNumpy()
     daily_wind_direction_10m_dominant = daily.Variables(7).ValuesAsNumpy()
+    weather_code= daily.Variables(8).ValuesAsNumpy()
     date_debut= pd.to_datetime(daily.Time(), unit = "s", utc = True)
-    return date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant
+    return date_debut,daily_temperature_2m_min,daily_temperature_2m_max,daily_apparent_temperature_min, daily_apparent_temperature_max, daily_precipitation_sum, daily_wind_speed_10m_max, daily_wind_gusts_10m_max, daily_wind_direction_10m_dominant,weather_code
 
 
 def specific_day(latitude,longitude,day):
     cache_session = requests_cache.CachedSession(get_user_config_directory_pyweather()+ '.cache', expire_after = 3600)
     retry_session = retry(cache_session, retries = 5, backoff_factor = 0.2)
     openmeteo = openmeteo_requests.Client(session = retry_session)
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "timezone": "Europe/Paris",
         "latitude": latitude,
         "longitude": longitude,
-        "hourly": ["temperature_2m", "apparent_temperature", "precipitation", "wind_speed_10m", "wind_gusts_10m", "wind_direction_10m"],
+        "hourly": ["temperature_2m", "apparent_temperature", "precipitation", "wind_speed_10m", "wind_gusts_10m", "wind_direction_10m", "pressure_msl","weather_code"],
         "start_date": (datetime.datetime.now()+ datetime.timedelta(days=day)).strftime('%Y-%m-%d'),
         "end_date": (datetime.datetime.now()+ datetime.timedelta(days=day+1)).strftime('%Y-%m-%d'),
     }
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
@@ -878,41 +938,44 @@
     hourly = response.Hourly()
     hourly_temperature_2m = hourly.Variables(0).ValuesAsNumpy()
     hourly_apparent_temperature = hourly.Variables(1).ValuesAsNumpy()
     hourly_precipitation = hourly.Variables(2).ValuesAsNumpy()
     hourly_wind_speed_10m = hourly.Variables(3).ValuesAsNumpy()
     hourly_wind_gusts_10m = hourly.Variables(4).ValuesAsNumpy()
     hourly_wind_direction_10m = hourly.Variables(5).ValuesAsNumpy()
-    return hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m
+    surface_pressure = hourly.Variables(6).ValuesAsNumpy()
+    weather_code = hourly.Variables(7).ValuesAsNumpy()
+    return hourly_temperature_2m,hourly_apparent_temperature,hourly_precipitation, hourly_wind_speed_10m, hourly_wind_gusts_10m, hourly_wind_direction_10m, surface_pressure, weather_code
 
 
 
 def current(latitude,longitude):
     cache_session = requests_cache.CachedSession(get_user_config_directory_pyweather() + '.cache', expire_after = 3600)
     retry_session = retry(cache_session, retries = 5, backoff_factor = 0.2)
     openmeteo = openmeteo_requests.Client(session = retry_session)
 
     url = "https://api.open-meteo.com/v1/meteofrance"
     params = {
         "latitude": latitude,
         "longitude": longitude,
-        "current": ["temperature_2m", "relative_humidity_2m", "apparent_temperature", "precipitation", "rain", "snowfall", "weather_code", "surface_pressure", "wind_speed_10m", "wind_direction_10m", "wind_gusts_10m"],
+        "current": ["temperature_2m", "relative_humidity_2m", "apparent_temperature", "precipitation", "rain", "snowfall", "weather_code", "pressure_msl", "wind_speed_10m", "wind_direction_10m", "wind_gusts_10m"],
     }
     responses = openmeteo.weather_api(url, params=params)
 
     response = responses[0]
 
     current = response.Current()
     current_temperature_2m = current.Variables(0).Value()
     current_relative_humidity_2m = current.Variables(1).Value()
     current_apparent_temperature = current.Variables(2).Value()
     current_precipitation = current.Variables(3).Value()
+    current_weather_code= current.Variables(6).Value()
     current_surface_pressure = current.Variables(7).Value()
     current_wind_speed_10m = current.Variables(8).Value()
     current_wind_direction_10m = current.Variables(9).Value()
     current_wind_gusts_10m = current.Variables(10).Value()
 
 
-    return current_temperature_2m,current_apparent_temperature,current_relative_humidity_2m,current_precipitation,current_surface_pressure,current_wind_speed_10m,current_wind_gusts_10m,current_wind_direction_10m
+    return current_temperature_2m,current_apparent_temperature,current_relative_humidity_2m,current_precipitation,current_surface_pressure,current_wind_speed_10m,current_wind_gusts_10m,current_wind_direction_10m,current_weather_code
```

### Comparing `pyweatherfr-2.0.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-2.0.1/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.0
+Version: 2.0.1
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.0/setup.py` & `pyweatherfr-2.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="2.0.0",
+    version="2.0.1",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

