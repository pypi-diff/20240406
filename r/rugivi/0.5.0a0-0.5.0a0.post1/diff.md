# Comparing `tmp/rugivi-0.5.0a0.tar.gz` & `tmp/rugivi-0.5.0a0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rugivi-0.5.0a0.tar", last modified: Fri Apr  5 21:52:25 2024, max compression
+gzip compressed data, was "rugivi-0.5.0a0.post1.tar", last modified: Fri Apr  5 22:03:12 2024, max compression
```

## Comparing `rugivi-0.5.0a0.tar` & `rugivi-0.5.0a0.post1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.249709 rugivi-0.5.0a0/
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    35149 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/LICENSE
--rw-r--r--   0 deskuser  (1000) deskuser  (1000)      497 2024-04-05 21:52:25.249709 rugivi-0.5.0a0/PKG-INFO
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    32138 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/README.md
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.241709 rugivi-0.5.0a0/rugivi/
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     3807 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/config_file_handler.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.233709 rugivi-0.5.0a0/rugivi/crawlers/
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.241709 rugivi-0.5.0a0/rugivi/crawlers/first_organic/
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)    24249 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/crawlers/first_organic/organic_crawler_first_edition.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     5018 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/dialogs.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2340 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/dir_helper.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.245709 rugivi-0.5.0a0/rugivi/exports/
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     5614 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/exports/world_overlook.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.245709 rugivi-0.5.0a0/rugivi/fap_table/
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2395 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/fap_table/fap_table.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     7219 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/fap_table/fap_table_manager.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     4481 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/fap_table/fap_table_view.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     3271 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/fap_table/fap_tables.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    51262 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/icon.ico
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    18461 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/icon.png
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.245709 rugivi-0.5.0a0/rugivi/image_database_service/
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     4882 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_database_service/image_server_database.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.245709 rugivi-0.5.0a0/rugivi/image_service/
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1329 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/abstract_cache_filename_generator.py
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     4625 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/abstract_streamed_media.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2531 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/image_cache.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    21758 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/image_server.py
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     3706 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/streamed_image.py
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1753 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/streamed_mockup.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     7760 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/image_service/video_still_generator.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     1220 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/print_module_dir.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)      741 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/rugivi.conf
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    31699 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/rugivi.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    20668 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/rugivi_configurator.py
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     6228 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/rugivi_image_cache_maintenance.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)      813 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/rugivi_windows.conf
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2235 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/selection.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2255 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/status.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     1600 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/thread_safe_list.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    13258 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/view.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.245709 rugivi-0.5.0a0/rugivi/world_database_service/
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1356 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/world_database_service/abstract_world_database.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     6392 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/world_database_service/world_database.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.249709 rugivi-0.5.0a0/rugivi/world_things/
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1557 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/world_things/abstract_world.py
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     2671 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/world_things/chunk.py
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1488 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/world_things/frame.py
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     3623 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/rugivi/world_things/world.py
-drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 21:52:25.249709 rugivi-0.5.0a0/rugivi.egg-info/
--rw-r--r--   0 deskuser  (1000) deskuser  (1000)      497 2024-04-05 21:52:25.000000 rugivi-0.5.0a0/rugivi.egg-info/PKG-INFO
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1397 2024-04-05 21:52:25.000000 rugivi-0.5.0a0/rugivi.egg-info/SOURCES.txt
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)        1 2024-04-05 21:52:25.000000 rugivi-0.5.0a0/rugivi.egg-info/dependency_links.txt
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)      254 2024-04-05 21:52:25.000000 rugivi-0.5.0a0/rugivi.egg-info/entry_points.txt
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)        1 2024-04-05 21:52:24.000000 rugivi-0.5.0a0/rugivi.egg-info/not-zip-safe
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)      126 2024-04-05 21:52:25.000000 rugivi-0.5.0a0/rugivi.egg-info/requires.txt
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)        7 2024-04-05 21:52:25.000000 rugivi-0.5.0a0/rugivi.egg-info/top_level.txt
--rw-rw-r--   0 deskuser  (1000) deskuser  (1000)       38 2024-04-05 21:52:25.249709 rugivi-0.5.0a0/setup.cfg
--rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2184 2024-04-05 21:40:55.000000 rugivi-0.5.0a0/setup.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.321727 rugivi-0.5.0a0.post1/
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    35149 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/LICENSE
+-rw-r--r--   0 deskuser  (1000) deskuser  (1000)      850 2024-04-05 22:03:12.321727 rugivi-0.5.0a0.post1/PKG-INFO
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    32138 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/README.md
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.309727 rugivi-0.5.0a0.post1/rugivi/
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     3807 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/config_file_handler.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.297727 rugivi-0.5.0a0.post1/rugivi/crawlers/
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.313727 rugivi-0.5.0a0.post1/rugivi/crawlers/first_organic/
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)    24249 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/crawlers/first_organic/organic_crawler_first_edition.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     5018 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/dialogs.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2340 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/dir_helper.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.313727 rugivi-0.5.0a0.post1/rugivi/exports/
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     5614 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/exports/world_overlook.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.313727 rugivi-0.5.0a0.post1/rugivi/fap_table/
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2395 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/fap_table/fap_table.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     7219 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/fap_table/fap_table_manager.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     4481 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/fap_table/fap_table_view.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     3271 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/fap_table/fap_tables.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    51262 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/icon.ico
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    18461 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/icon.png
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.313727 rugivi-0.5.0a0.post1/rugivi/image_database_service/
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     4882 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_database_service/image_server_database.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.317727 rugivi-0.5.0a0.post1/rugivi/image_service/
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1329 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/abstract_cache_filename_generator.py
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     4625 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/abstract_streamed_media.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2531 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/image_cache.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    21758 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/image_server.py
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     3706 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/streamed_image.py
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1753 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/streamed_mockup.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     7760 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/image_service/video_still_generator.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     1220 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/print_module_dir.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)      741 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/rugivi.conf
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    31699 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/rugivi.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    20668 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/rugivi_configurator.py
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     6228 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/rugivi_image_cache_maintenance.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)      813 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/rugivi_windows.conf
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2235 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/selection.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2255 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/status.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     1600 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/thread_safe_list.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)    13258 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/view.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.317727 rugivi-0.5.0a0.post1/rugivi/world_database_service/
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1356 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/world_database_service/abstract_world_database.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     6392 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/world_database_service/world_database.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.317727 rugivi-0.5.0a0.post1/rugivi/world_things/
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1557 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/world_things/abstract_world.py
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     2671 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/world_things/chunk.py
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1488 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/world_things/frame.py
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     3623 2024-04-05 21:40:55.000000 rugivi-0.5.0a0.post1/rugivi/world_things/world.py
+drwxrwxr-x   0 deskuser  (1000) deskuser  (1000)        0 2024-04-05 22:03:12.317727 rugivi-0.5.0a0.post1/rugivi.egg-info/
+-rw-r--r--   0 deskuser  (1000) deskuser  (1000)      850 2024-04-05 22:03:12.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/PKG-INFO
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)     1397 2024-04-05 22:03:12.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/SOURCES.txt
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)        1 2024-04-05 22:03:12.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/dependency_links.txt
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)      254 2024-04-05 22:03:12.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/entry_points.txt
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)        1 2024-04-05 21:52:24.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/not-zip-safe
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)      126 2024-04-05 22:03:12.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/requires.txt
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)        7 2024-04-05 22:03:12.000000 rugivi-0.5.0a0.post1/rugivi.egg-info/top_level.txt
+-rw-rw-r--   0 deskuser  (1000) deskuser  (1000)       38 2024-04-05 22:03:12.321727 rugivi-0.5.0a0.post1/setup.cfg
+-rwxr-xr-x   0 deskuser  (1000) deskuser  (1000)     2557 2024-04-05 22:03:05.000000 rugivi-0.5.0a0.post1/setup.py
```

### Comparing `rugivi-0.5.0a0/LICENSE` & `rugivi-0.5.0a0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/README.md` & `rugivi-0.5.0a0.post1/README.md`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/config_file_handler.py` & `rugivi-0.5.0a0.post1/rugivi/config_file_handler.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/crawlers/first_organic/organic_crawler_first_edition.py` & `rugivi-0.5.0a0.post1/rugivi/crawlers/first_organic/organic_crawler_first_edition.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/dialogs.py` & `rugivi-0.5.0a0.post1/rugivi/dialogs.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/dir_helper.py` & `rugivi-0.5.0a0.post1/rugivi/dir_helper.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/exports/world_overlook.py` & `rugivi-0.5.0a0.post1/rugivi/exports/world_overlook.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/fap_table/fap_table.py` & `rugivi-0.5.0a0.post1/rugivi/fap_table/fap_table.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/fap_table/fap_table_manager.py` & `rugivi-0.5.0a0.post1/rugivi/fap_table/fap_table_manager.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/fap_table/fap_table_view.py` & `rugivi-0.5.0a0.post1/rugivi/fap_table/fap_table_view.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/fap_table/fap_tables.py` & `rugivi-0.5.0a0.post1/rugivi/fap_table/fap_tables.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/icon.ico` & `rugivi-0.5.0a0.post1/rugivi/icon.ico`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/icon.png` & `rugivi-0.5.0a0.post1/rugivi/icon.png`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_database_service/image_server_database.py` & `rugivi-0.5.0a0.post1/rugivi/image_database_service/image_server_database.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/abstract_cache_filename_generator.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/abstract_cache_filename_generator.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/abstract_streamed_media.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/abstract_streamed_media.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/image_cache.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/image_cache.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/image_server.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/image_server.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/streamed_image.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/streamed_image.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/streamed_mockup.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/streamed_mockup.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/image_service/video_still_generator.py` & `rugivi-0.5.0a0.post1/rugivi/image_service/video_still_generator.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/print_module_dir.py` & `rugivi-0.5.0a0.post1/rugivi/print_module_dir.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/rugivi.conf` & `rugivi-0.5.0a0.post1/rugivi/rugivi.conf`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/rugivi.py` & `rugivi-0.5.0a0.post1/rugivi/rugivi.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/rugivi_configurator.py` & `rugivi-0.5.0a0.post1/rugivi/rugivi_configurator.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/rugivi_image_cache_maintenance.py` & `rugivi-0.5.0a0.post1/rugivi/rugivi_image_cache_maintenance.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/rugivi_windows.conf` & `rugivi-0.5.0a0.post1/rugivi/rugivi_windows.conf`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/selection.py` & `rugivi-0.5.0a0.post1/rugivi/selection.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/status.py` & `rugivi-0.5.0a0.post1/rugivi/status.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/thread_safe_list.py` & `rugivi-0.5.0a0.post1/rugivi/thread_safe_list.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/view.py` & `rugivi-0.5.0a0.post1/rugivi/view.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/world_database_service/abstract_world_database.py` & `rugivi-0.5.0a0.post1/rugivi/world_database_service/abstract_world_database.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/world_database_service/world_database.py` & `rugivi-0.5.0a0.post1/rugivi/world_database_service/world_database.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/world_things/abstract_world.py` & `rugivi-0.5.0a0.post1/rugivi/world_things/abstract_world.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/world_things/chunk.py` & `rugivi-0.5.0a0.post1/rugivi/world_things/chunk.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/world_things/frame.py` & `rugivi-0.5.0a0.post1/rugivi/world_things/frame.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi/world_things/world.py` & `rugivi-0.5.0a0.post1/rugivi/world_things/world.py`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/rugivi.egg-info/SOURCES.txt` & `rugivi-0.5.0a0.post1/rugivi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rugivi-0.5.0a0/setup.py` & `rugivi-0.5.0a0.post1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 ##############################################################################################
 
 from setuptools import setup
 
 setup(name='rugivi',
-	version='0.5.0-alpha',
+	version='0.5.0-alpha.post1',
 	description='RuGiVi - Adult Media Landscape Browser',
+	long_description='RuGiVi enables you to fly over your image and video collection and view thousands of images and video frames at once. Zoom in and out from one image to small thumbnails with your mousewheel in seconds. All images are grouped as you have them on your disk and arranged in a huge landscape. RuGiVi can work with hundred thousand of images at once.',
 	url='https://github.com/pronopython/rugivi',
 	author='pronopython',
 	author_email='pronopython@proton.me',
 	license='GNU GENERAL PUBLIC LICENSE V3',
 	packages=['rugivi','rugivi.crawlers.first_organic','rugivi.fap_table','rugivi.image_database_service','rugivi.image_service','rugivi.world_database_service','rugivi.world_things','rugivi.exports'],
 	package_data={'rugivi':['*']},
 	include_package_data=True,
```

