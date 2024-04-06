# Comparing `tmp/herepy-3.6.1.tar.gz` & `tmp/herepy-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herepy-3.6.1.tar", last modified: Sun Mar 31 18:01:09 2024, max compression
+gzip compressed data, was "herepy-3.6.2.tar", last modified: Sat Apr  6 19:03:19 2024, max compression
```

## Comparing `herepy-3.6.1.tar` & `herepy-3.6.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-03-31 18:01:09.825099 herepy-3.6.1/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.1/COPYING
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.1/LICENSE
--rw-r--r--   0 abdullahselek   (501) staff       (20)      118 2023-09-13 13:06:01.000000 herepy-3.6.1/MANIFEST.in
--rw-r--r--   0 abdullahselek   (501) staff       (20)       91 2023-09-13 13:06:01.000000 herepy-3.6.1/NOTICE
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-03-31 18:01:09.825034 herepy-3.6.1/PKG-INFO
--rw-r--r--   0 abdullahselek   (501) staff       (20)     5574 2023-09-13 13:06:01.000000 herepy-3.6.1/README.rst
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-03-31 18:01:09.821531 herepy-3.6.1/herepy/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     3420 2024-03-31 17:52:34.000000 herepy-3.6.1/herepy/__init__.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     5846 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/destination_weather_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      754 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/error.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    10908 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/ev_charging_stations_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     8642 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/fleet_telematics_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4792 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/geocoder_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2905 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/geocoder_autocomplete_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2537 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/geocoder_reverse_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      730 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/here_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    12999 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/here_enum.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    13901 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/isoline_routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     8695 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/map_image_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4861 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/map_tile_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      734 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/mercator_projection.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    10149 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/models.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     3816 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/objects.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4273 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/places_api.py
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-03-31 18:01:09.822301 herepy-3.6.1/herepy/platform/
--rw-r--r--   0 abdullahselek   (501) staff       (20)       47 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/platform/__init__.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      544 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/platform/tour_planning_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     5819 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/polling.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    15370 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/public_transit_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)        0 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/py.typed
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2531 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/rme_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    40100 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    12825 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/traffic_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2047 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/utils.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4021 2023-09-13 13:06:01.000000 herepy-3.6.1/herepy/vector_tile_api.py
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-03-31 18:01:09.824846 herepy-3.6.1/herepy.egg-info/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-03-31 18:01:09.000000 herepy-3.6.1/herepy.egg-info/PKG-INFO
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1447 2024-03-31 18:01:09.000000 herepy-3.6.1/herepy.egg-info/SOURCES.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)        1 2024-03-31 18:01:09.000000 herepy-3.6.1/herepy.egg-info/dependency_links.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-03-31 18:01:09.000000 herepy-3.6.1/herepy.egg-info/requires.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)        7 2024-03-31 18:01:09.000000 herepy-3.6.1/herepy.egg-info/top_level.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-03-31 17:22:24.000000 herepy-3.6.1/requirements.txt
--rw-r--r--   0 abdullahselek   (501) staff       (20)      235 2024-03-31 18:01:09.825321 herepy-3.6.1/setup.cfg
--rwxr-xr-x   0 abdullahselek   (501) staff       (20)     2072 2024-03-31 17:36:07.000000 herepy-3.6.1/setup.py
-drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-03-31 18:01:09.824698 herepy-3.6.1/tests/
--rw-r--r--   0 abdullahselek   (501) staff       (20)     7759 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_destination_weather_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    29190 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_enum.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6286 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_ev_charging_stations_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     7156 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_fleet_telematics_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     4614 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_geocoder_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2690 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_geocoder_autocomplete_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1556 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_geocoder_reverse_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    14367 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_isoline_routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6013 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_map_image_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    14479 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_map_tile_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      366 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_mercator_projection.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     6811 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_models.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     3559 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_places_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    14931 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_publictransit_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     1616 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_rme_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    44334 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_routing_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)    16597 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_traffic_api.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)      957 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_utils.py
--rw-r--r--   0 abdullahselek   (501) staff       (20)     2718 2023-09-13 13:06:01.000000 herepy-3.6.1/tests/test_vector_tile_api.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.662596 herepy-3.6.2/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.2/COPYING
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1071 2023-09-13 13:06:01.000000 herepy-3.6.2/LICENSE
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      118 2023-09-13 13:06:01.000000 herepy-3.6.2/MANIFEST.in
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       91 2023-09-13 13:06:01.000000 herepy-3.6.2/NOTICE
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-04-06 19:03:19.662527 herepy-3.6.2/PKG-INFO
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5574 2023-09-13 13:06:01.000000 herepy-3.6.2/README.rst
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.658762 herepy-3.6.2/herepy/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     3420 2024-04-06 19:00:51.000000 herepy-3.6.2/herepy/__init__.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5846 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/destination_weather_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      754 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/error.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    10908 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/ev_charging_stations_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     8642 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/fleet_telematics_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4792 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/geocoder_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2905 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/geocoder_autocomplete_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2537 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/geocoder_reverse_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      730 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/here_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    12999 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/here_enum.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    13901 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/isoline_routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     8695 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/map_image_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4861 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/map_tile_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      734 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/mercator_projection.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    10149 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/models.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     3816 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/objects.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4273 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/places_api.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.659555 herepy-3.6.2/herepy/platform/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       47 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/platform/__init__.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      544 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/platform/tour_planning_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     5819 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/polling.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    15370 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/public_transit_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)        0 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/py.typed
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2531 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/rme_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    40099 2024-04-06 18:43:16.000000 herepy-3.6.2/herepy/routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    12825 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/traffic_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2047 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/utils.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4021 2023-09-13 13:06:01.000000 herepy-3.6.2/herepy/vector_tile_api.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.662303 herepy-3.6.2/herepy.egg-info/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6756 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/PKG-INFO
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1447 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/SOURCES.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)        1 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/dependency_links.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/requires.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)        7 2024-04-06 19:03:19.000000 herepy-3.6.2/herepy.egg-info/top_level.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)       20 2024-03-31 17:22:24.000000 herepy-3.6.2/requirements.txt
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      235 2024-04-06 19:03:19.662836 herepy-3.6.2/setup.cfg
+-rwxr-xr-x   0 abdullahselek   (501) staff       (20)     2072 2024-03-31 17:36:07.000000 herepy-3.6.2/setup.py
+drwxr-xr-x   0 abdullahselek   (501) staff       (20)        0 2024-04-06 19:03:19.662121 herepy-3.6.2/tests/
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     7759 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_destination_weather_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    29190 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_enum.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6286 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_ev_charging_stations_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     7156 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_fleet_telematics_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     4614 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_geocoder_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2690 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_geocoder_autocomplete_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1556 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_geocoder_reverse_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    14367 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_isoline_routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6013 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_map_image_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    14479 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_map_tile_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      366 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_mercator_projection.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     6811 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_models.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     3559 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_places_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    14931 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_publictransit_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     1616 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_rme_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    45084 2024-04-06 18:44:02.000000 herepy-3.6.2/tests/test_routing_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)    16597 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_traffic_api.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)      957 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_utils.py
+-rw-r--r--   0 abdullahselek   (501) staff       (20)     2718 2023-09-13 13:06:01.000000 herepy-3.6.2/tests/test_vector_tile_api.py
```

### Comparing `herepy-3.6.1/COPYING` & `herepy-3.6.2/COPYING`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/LICENSE` & `herepy-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/PKG-INFO` & `herepy-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herepy
-Version: 3.6.1
+Version: 3.6.2
 Summary: A library that provides a Python interface to the HERE APIs
 Home-page: https://github.com/abdullahselek/HerePy
 Download-URL: https://pypi.org/pypi/herepy
 Author: Abdullah Selek
 Author-email: abdullahselek.os@gmail.com
 Maintainer: Abdullah Selek
 Maintainer-email: abdullahselek.os@gmail.com
```

### Comparing `herepy-3.6.1/README.rst` & `herepy-3.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/__init__.py` & `herepy-3.6.2/herepy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """A library that provides a Python interface to the HERE APIs"""
 
 __author__ = "Abdullah Selek"
 __email__ = "abdullahselek.os@gmail.com"
 __copyright__ = "Copyright (c) 2017 Abdullah Selek"
 __license__ = "MIT License"
-__version__ = "3.6.1"
+__version__ = "3.6.2"
 __url__ = "https://github.com/abdullahselek/HerePy"
 __download_url__ = "https://pypi.org/pypi/herepy"
 __description__ = "A library that provides a Python interface to the HERE APIs"
 
 
 import json
```

### Comparing `herepy-3.6.1/herepy/destination_weather_api.py` & `herepy-3.6.2/herepy/destination_weather_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/error.py` & `herepy-3.6.2/herepy/error.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/ev_charging_stations_api.py` & `herepy-3.6.2/herepy/ev_charging_stations_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/fleet_telematics_api.py` & `herepy-3.6.2/herepy/fleet_telematics_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/geocoder_api.py` & `herepy-3.6.2/herepy/geocoder_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/geocoder_autocomplete_api.py` & `herepy-3.6.2/herepy/geocoder_autocomplete_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/geocoder_reverse_api.py` & `herepy-3.6.2/herepy/geocoder_reverse_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/here_api.py` & `herepy-3.6.2/herepy/here_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/here_enum.py` & `herepy-3.6.2/herepy/here_enum.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/isoline_routing_api.py` & `herepy-3.6.2/herepy/isoline_routing_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/map_image_api.py` & `herepy-3.6.2/herepy/map_image_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/map_tile_api.py` & `herepy-3.6.2/herepy/map_tile_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/mercator_projection.py` & `herepy-3.6.2/herepy/mercator_projection.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/models.py` & `herepy-3.6.2/herepy/models.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/objects.py` & `herepy-3.6.2/herepy/objects.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/places_api.py` & `herepy-3.6.2/herepy/places_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/platform/tour_planning_api.py` & `herepy-3.6.2/herepy/platform/tour_planning_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/polling.py` & `herepy-3.6.2/herepy/polling.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/public_transit_api.py` & `herepy-3.6.2/herepy/public_transit_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/rme_api.py` & `herepy-3.6.2/herepy/rme_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/routing_api.py` & `herepy-3.6.2/herepy/routing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
             "destination": str.format("{0},{1}", destination[0], destination[1]),
             "apiKey": self._api_key,
         }
 
         via_keys = []
         if via:
             for i, v in enumerate(via):
-                key = str.format("{0}{1}", "via", i)
+                key = str.format("{0}{1}_", "via", i)
                 via_keys.append(key)
                 data[key] = str.format("{0},{1}", v[0], v[1])
         if departure_time:
             data["departureTime"] = departure_time
         data["routingMode"] = routing_mode.__str__()
         if alternatives:
             data["alternatives"] = alternatives
@@ -841,15 +841,15 @@
         """Use the Geocoder API to resolve a location name to a set of coordinates."""
 
         geocoder_api = GeocoderApi(self._api_key)
         try:
             geocoder_response = geocoder_api.free_form(location_name)
             coordinates = geocoder_response.items[0]["position"]
             return [coordinates["lat"], coordinates["lng"]]
-        except (HEREError) as here_error:
+        except HEREError as here_error:
             raise WaypointNotFoundError(here_error.message)
 
     @staticmethod
     def _convert_datetime_to_isoformat(datetime_object):
         """Convert a datetime.datetime object to an ISO8601 string."""
 
         if isinstance(datetime_object, datetime.datetime):
```

### Comparing `herepy-3.6.1/herepy/traffic_api.py` & `herepy-3.6.2/herepy/traffic_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/utils.py` & `herepy-3.6.2/herepy/utils.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy/vector_tile_api.py` & `herepy-3.6.2/herepy/vector_tile_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/herepy.egg-info/PKG-INFO` & `herepy-3.6.2/herepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herepy
-Version: 3.6.1
+Version: 3.6.2
 Summary: A library that provides a Python interface to the HERE APIs
 Home-page: https://github.com/abdullahselek/HerePy
 Download-URL: https://pypi.org/pypi/herepy
 Author: Abdullah Selek
 Author-email: abdullahselek.os@gmail.com
 Maintainer: Abdullah Selek
 Maintainer-email: abdullahselek.os@gmail.com
```

### Comparing `herepy-3.6.1/herepy.egg-info/SOURCES.txt` & `herepy-3.6.2/herepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/setup.py` & `herepy-3.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_destination_weather_api.py` & `herepy-3.6.2/tests/test_destination_weather_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_enum.py` & `herepy-3.6.2/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_ev_charging_stations_api.py` & `herepy-3.6.2/tests/test_ev_charging_stations_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_fleet_telematics_api.py` & `herepy-3.6.2/tests/test_fleet_telematics_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_geocoder_api.py` & `herepy-3.6.2/tests/test_geocoder_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_geocoder_autocomplete_api.py` & `herepy-3.6.2/tests/test_geocoder_autocomplete_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_geocoder_reverse_api.py` & `herepy-3.6.2/tests/test_geocoder_reverse_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_isoline_routing_api.py` & `herepy-3.6.2/tests/test_isoline_routing_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_map_image_api.py` & `herepy-3.6.2/tests/test_map_image_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_map_tile_api.py` & `herepy-3.6.2/tests/test_map_tile_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_models.py` & `herepy-3.6.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_places_api.py` & `herepy-3.6.2/tests/test_places_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_publictransit_api.py` & `herepy-3.6.2/tests/test_publictransit_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_rme_api.py` & `herepy-3.6.2/tests/test_rme_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_routing_api.py` & `herepy-3.6.2/tests/test_routing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1175,7 +1175,29 @@
                 units=herepy.RoutingMetric.metric,
                 lang="tr-TR",
                 return_fields=[herepy.RoutingApiReturnField.polyline],
                 span_fields=[herepy.RoutingApiSpanField.walkAttributes],
                 truck={"shippedHazardousGoods": ["explosive", "gas"]},
                 scooter={"allowHighway": "true"},
             )
+
+    @responses.activate
+    def test_route_v8_multiple_via_points(self):
+        responses.add(
+            responses.GET,
+            "https://router.hereapi.com/v8/routes",
+            "{}",
+            status=200,
+            match=[
+                responses.matchers.query_param_matcher(
+                    {"via": ["41.9339,-87.9021"] * 11}, strict_match=False
+                )
+            ],
+        )
+        response = self._api.route_v8(
+            transport_mode=herepy.RoutingTransportMode.car,
+            origin=[41.9798, -87.8801],
+            destination=[41.9043, -87.9216],
+            via=[[41.9339, -87.9021]] * 11,
+        )
+        self.assertTrue(response)
+        self.assertIsInstance(response, herepy.RoutingResponseV8)
```

### Comparing `herepy-3.6.1/tests/test_traffic_api.py` & `herepy-3.6.2/tests/test_traffic_api.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_utils.py` & `herepy-3.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herepy-3.6.1/tests/test_vector_tile_api.py` & `herepy-3.6.2/tests/test_vector_tile_api.py`

 * *Files identical despite different names*

