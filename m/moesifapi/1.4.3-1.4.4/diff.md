# Comparing `tmp/moesifapi-1.4.3.tar.gz` & `tmp/moesifapi-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifapi-1.4.3.tar", last modified: Thu Feb 29 20:34:46 2024, max compression
+gzip compressed data, was "moesifapi-1.4.4.tar", last modified: Sat Apr  6 01:06:13 2024, max compression
```

## Comparing `moesifapi-1.4.3.tar` & `moesifapi-1.4.4.tar`

### file list

```diff
@@ -1,58 +1,65 @@
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.213595 moesifapi-1.4.3/
--rwxr-xr-x   0 praveen    (501) staff       (20)    11918 2023-11-09 16:30:27.000000 moesifapi-1.4.3/LICENSE
--rw-rw-r--   0 praveen    (501) staff       (20)       61 2022-08-18 23:33:42.000000 moesifapi-1.4.3/MANIFEST.in
--rw-r--r--   0 praveen    (501) staff       (20)    13889 2024-02-29 20:34:46.213467 moesifapi-1.4.3/PKG-INFO
--rwxr-xr-x   0 praveen    (501) staff       (20)    12654 2024-02-29 20:25:49.000000 moesifapi-1.4.3/README.md
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.178496 moesifapi-1.4.3/moesifapi/
--rwxr-xr-x   0 praveen    (501) staff       (20)      209 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     5538 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/api_helper.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      294 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/configuration.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.185913 moesifapi-1.4.3/moesifapi/controllers/
--rwxr-xr-x   0 praveen    (501) staff       (20)       94 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/controllers/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)    19397 2024-02-29 20:25:49.000000 moesifapi-1.4.3/moesifapi/controllers/api_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1493 2024-01-10 04:21:31.000000 moesifapi-1.4.3/moesifapi/controllers/base_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2342 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/controllers/health_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      409 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/decorators.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.186384 moesifapi-1.4.3/moesifapi/exceptions/
--rwxr-xr-x   0 praveen    (501) staff       (20)       29 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/exceptions/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      827 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/exceptions/api_exception.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.189617 moesifapi-1.4.3/moesifapi/http/
--rwxr-xr-x   0 praveen    (501) staff       (20)      205 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1117 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/http_call_back.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     7690 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/http_client.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      962 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/http_context.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      791 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/http_method_enum.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2343 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/http_request.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1004 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/http_response.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2815 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/http/requests_client.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.203024 moesifapi-1.4.3/moesifapi/models/
--rwxr-xr-x   0 praveen    (501) staff       (20)      245 2024-02-29 20:25:49.000000 moesifapi-1.4.3/moesifapi/models/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1836 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/models/base_model.py
--rw-rw-r--   0 praveen    (501) staff       (20)     3002 2022-08-18 23:33:42.000000 moesifapi-1.4.3/moesifapi/models/campaign_model.py
--rw-rw-r--   0 praveen    (501) staff       (20)     3182 2022-08-18 23:33:42.000000 moesifapi-1.4.3/moesifapi/models/company_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     4135 2024-01-10 04:21:31.000000 moesifapi-1.4.3/moesifapi/models/event_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     3141 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/models/event_request_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     2638 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/models/event_response_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     1525 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/models/status_model.py
--rw-r--r--   0 praveen    (501) staff       (20)     3047 2024-02-29 20:25:49.000000 moesifapi-1.4.3/moesifapi/models/subscription_model.py
--rw-rw-r--   0 praveen    (501) staff       (20)     3470 2022-08-18 23:33:42.000000 moesifapi-1.4.3/moesifapi/models/user_model.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      461 2023-11-09 16:30:27.000000 moesifapi-1.4.3/moesifapi/moesif_api_client.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.209602 moesifapi-1.4.3/moesifapi/utils/
--rw-r--r--   0 praveen    (501) staff       (20)       65 2023-11-09 16:38:22.000000 moesifapi-1.4.3/moesifapi/utils/__init__.py
--rw-r--r--   0 praveen    (501) staff       (20)     8027 2023-11-10 03:46:36.000000 moesifapi-1.4.3/moesifapi/utils/governance_manager.py
--rw-r--r--   0 praveen    (501) staff       (20)     5016 2023-11-10 03:38:02.000000 moesifapi-1.4.3/moesifapi/utils/governance_util.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.213066 moesifapi-1.4.3/moesifapi.egg-info/
--rw-r--r--   0 praveen    (501) staff       (20)    13889 2024-02-29 20:34:46.000000 moesifapi-1.4.3/moesifapi.egg-info/PKG-INFO
--rw-rw-r--   0 praveen    (501) staff       (20)     1438 2024-02-29 20:34:46.000000 moesifapi-1.4.3/moesifapi.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen    (501) staff       (20)        1 2024-02-29 20:34:46.000000 moesifapi-1.4.3/moesifapi.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       45 2024-02-29 20:34:46.000000 moesifapi-1.4.3/moesifapi.egg-info/entry_points.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       75 2024-02-29 20:34:46.000000 moesifapi-1.4.3/moesifapi.egg-info/requires.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       16 2024-02-29 20:34:46.000000 moesifapi-1.4.3/moesifapi.egg-info/top_level.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       67 2024-02-29 20:34:46.213894 moesifapi-1.4.3/setup.cfg
--rw-r--r--   0 praveen    (501) staff       (20)     3607 2024-02-29 20:34:30.000000 moesifapi-1.4.3/setup.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.211093 moesifapi-1.4.3/tests/
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-02-29 20:34:46.212710 moesifapi-1.4.3/tests/controllers/
--rwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-11-09 16:30:27.000000 moesifapi-1.4.3/tests/controllers/__init__.py
--rwxr-xr-x   0 praveen    (501) staff       (20)      887 2023-11-09 16:30:27.000000 moesifapi-1.4.3/tests/controllers/controller_test_base.py
--rwxr-xr-x   0 praveen    (501) staff       (20)    17361 2024-02-29 20:25:49.000000 moesifapi-1.4.3/tests/controllers/test_api_controller.py
--rwxr-xr-x   0 praveen    (501) staff       (20)     4922 2023-11-09 16:30:27.000000 moesifapi-1.4.3/tests/test_helper.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.125795 moesifapi-1.4.4/
+-rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-05-11 16:17:23.000000 moesifapi-1.4.4/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-11 16:17:23.000000 moesifapi-1.4.4/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-04-06 01:06:13.126288 moesifapi-1.4.4/PKG-INFO
+-rwxr-xr-x   0 keyur      (501) staff       (20)    12654 2024-03-29 18:28:28.000000 moesifapi-1.4.4/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.099363 moesifapi-1.4.4/moesifapi/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      209 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     5538 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/api_helper.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.106331 moesifapi-1.4.4/moesifapi/app_config/
+-rw-r--r--   0 keyur      (501) staff       (20)       25 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/app_config/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2688 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/app_config/app_config.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4028 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/app_config/regex_config_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     5064 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/config_manager.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      294 2023-07-01 00:47:27.000000 moesifapi-1.4.4/moesifapi/configuration.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.109903 moesifapi-1.4.4/moesifapi/controllers/
+-rwxr-xr-x   0 keyur      (501) staff       (20)       94 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/controllers/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)    19397 2024-03-29 18:28:28.000000 moesifapi-1.4.4/moesifapi/controllers/api_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1493 2024-03-29 18:28:28.000000 moesifapi-1.4.4/moesifapi/controllers/base_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2342 2021-02-17 05:27:26.000000 moesifapi-1.4.4/moesifapi/controllers/health_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      409 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/decorators.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.111656 moesifapi-1.4.4/moesifapi/exceptions/
+-rwxr-xr-x   0 keyur      (501) staff       (20)       29 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/exceptions/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      827 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/exceptions/api_exception.py
+-rw-r--r--   0 keyur      (501) staff       (20)    11182 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/governance_manager.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.116516 moesifapi-1.4.4/moesifapi/http/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      205 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1117 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/http_call_back.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     7690 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/http_client.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      962 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/http_context.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      791 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/http_method_enum.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2343 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/http_request.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1004 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/http_response.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2815 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/http/requests_client.py
+-rw-r--r--   0 keyur      (501) staff       (20)      148 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/logger_helper.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.122293 moesifapi-1.4.4/moesifapi/models/
+-rwxr-xr-x   0 keyur      (501) staff       (20)      245 2024-03-29 18:28:28.000000 moesifapi-1.4.4/moesifapi/models/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1836 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/base_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3002 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/campaign_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3182 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/company_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     4135 2024-03-29 18:28:28.000000 moesifapi-1.4.4/moesifapi/models/event_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     3141 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/event_request_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     2638 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/event_response_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     1525 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/status_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3047 2024-03-29 18:28:28.000000 moesifapi-1.4.4/moesifapi/models/subscription_model.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3470 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/models/user_model.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      461 2020-05-11 16:17:23.000000 moesifapi-1.4.4/moesifapi/moesif_api_client.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2344 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/parse_body.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8043 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/update_companies.py
+-rw-r--r--   0 keyur      (501) staff       (20)     7784 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/update_users.py
+-rw-r--r--   0 keyur      (501) staff       (20)     8502 2024-04-06 01:03:24.000000 moesifapi-1.4.4/moesifapi/workers.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.103564 moesifapi-1.4.4/moesifapi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    13737 2024-04-06 01:06:12.000000 moesifapi-1.4.4/moesifapi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)     1637 2024-04-06 01:06:12.000000 moesifapi-1.4.4/moesifapi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2024-04-06 01:06:12.000000 moesifapi-1.4.4/moesifapi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       45 2024-04-06 01:06:12.000000 moesifapi-1.4.4/moesifapi.egg-info/entry_points.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       75 2024-04-06 01:06:12.000000 moesifapi-1.4.4/moesifapi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       16 2024-04-06 01:06:12.000000 moesifapi-1.4.4/moesifapi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2024-04-06 01:06:13.127975 moesifapi-1.4.4/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3607 2024-04-06 01:03:24.000000 moesifapi-1.4.4/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.122929 moesifapi-1.4.4/tests/
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-06 01:06:13.124670 moesifapi-1.4.4/tests/controllers/
+-rwxr-xr-x   0 keyur      (501) staff       (20)        0 2020-05-11 16:17:23.000000 moesifapi-1.4.4/tests/controllers/__init__.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)      887 2024-04-06 01:04:20.000000 moesifapi-1.4.4/tests/controllers/controller_test_base.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)    17361 2024-03-29 18:28:28.000000 moesifapi-1.4.4/tests/controllers/test_api_controller.py
+-rwxr-xr-x   0 keyur      (501) staff       (20)     4922 2020-05-11 16:17:23.000000 moesifapi-1.4.4/tests/test_helper.py
```

### Comparing `moesifapi-1.4.3/LICENSE` & `moesifapi-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/PKG-INFO` & `moesifapi-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.3
+Version: 1.4.4
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
@@ -18,22 +18,17 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: jsonpickle
-Requires-Dist: python-dateutil
-Requires-Dist: isodatetimehandler
 Provides-Extra: dev
 Provides-Extra: test
-Requires-Dist: nose; extra == "test"
+License-File: LICENSE
 
 # MoesifApi Lib for Python
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
```

### Comparing `moesifapi-1.4.3/README.md` & `moesifapi-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/api_helper.py` & `moesifapi-1.4.4/moesifapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/controllers/api_controller.py` & `moesifapi-1.4.4/moesifapi/controllers/api_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/controllers/base_controller.py` & `moesifapi-1.4.4/moesifapi/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/controllers/health_controller.py` & `moesifapi-1.4.4/moesifapi/controllers/health_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/exceptions/api_exception.py` & `moesifapi-1.4.4/moesifapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/http_call_back.py` & `moesifapi-1.4.4/moesifapi/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/http_client.py` & `moesifapi-1.4.4/moesifapi/http/http_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/http_context.py` & `moesifapi-1.4.4/moesifapi/http/http_context.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/http_method_enum.py` & `moesifapi-1.4.4/moesifapi/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/http_request.py` & `moesifapi-1.4.4/moesifapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/http_response.py` & `moesifapi-1.4.4/moesifapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/http/requests_client.py` & `moesifapi-1.4.4/moesifapi/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/base_model.py` & `moesifapi-1.4.4/moesifapi/models/base_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/campaign_model.py` & `moesifapi-1.4.4/moesifapi/models/campaign_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/company_model.py` & `moesifapi-1.4.4/moesifapi/models/company_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/event_model.py` & `moesifapi-1.4.4/moesifapi/models/event_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/event_request_model.py` & `moesifapi-1.4.4/moesifapi/models/event_request_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/event_response_model.py` & `moesifapi-1.4.4/moesifapi/models/event_response_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/status_model.py` & `moesifapi-1.4.4/moesifapi/models/status_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/subscription_model.py` & `moesifapi-1.4.4/moesifapi/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi/models/user_model.py` & `moesifapi-1.4.4/moesifapi/models/user_model.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/moesifapi.egg-info/PKG-INFO` & `moesifapi-1.4.4/moesifapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifapi
-Version: 1.4.3
+Version: 1.4.4
 Summary: Moesif API Lib for Python
 Home-page: https://www.moesif.com/docs/api?python#api-libs
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
@@ -18,22 +18,17 @@
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: jsonpickle
-Requires-Dist: python-dateutil
-Requires-Dist: isodatetimehandler
 Provides-Extra: dev
 Provides-Extra: test
-Requires-Dist: nose; extra == "test"
+License-File: LICENSE
 
 # MoesifApi Lib for Python
 
 [![Built For][ico-built-for]][link-built-for]
 [![Latest Version][ico-version]][link-package]
 [![Language Versions][ico-language]][link-language]
 [![Software License][ico-license]][link-license]
```

### Comparing `moesifapi-1.4.3/moesifapi.egg-info/SOURCES.txt` & `moesifapi-1.4.4/moesifapi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 moesifapi/__init__.py
 moesifapi/api_helper.py
+moesifapi/config_manager.py
 moesifapi/configuration.py
 moesifapi/decorators.py
+moesifapi/governance_manager.py
+moesifapi/logger_helper.py
 moesifapi/moesif_api_client.py
+moesifapi/parse_body.py
+moesifapi/update_companies.py
+moesifapi/update_users.py
+moesifapi/workers.py
 moesifapi.egg-info/PKG-INFO
 moesifapi.egg-info/SOURCES.txt
 moesifapi.egg-info/dependency_links.txt
 moesifapi.egg-info/entry_points.txt
 moesifapi.egg-info/requires.txt
 moesifapi.egg-info/top_level.txt
+moesifapi/app_config/__init__.py
+moesifapi/app_config/app_config.py
+moesifapi/app_config/regex_config_helper.py
 moesifapi/controllers/__init__.py
 moesifapi/controllers/api_controller.py
 moesifapi/controllers/base_controller.py
 moesifapi/controllers/health_controller.py
 moesifapi/exceptions/__init__.py
 moesifapi/exceptions/api_exception.py
 moesifapi/http/__init__.py
@@ -34,14 +44,11 @@
 moesifapi/models/company_model.py
 moesifapi/models/event_model.py
 moesifapi/models/event_request_model.py
 moesifapi/models/event_response_model.py
 moesifapi/models/status_model.py
 moesifapi/models/subscription_model.py
 moesifapi/models/user_model.py
-moesifapi/utils/__init__.py
-moesifapi/utils/governance_manager.py
-moesifapi/utils/governance_util.py
 tests/test_helper.py
 tests/controllers/__init__.py
 tests/controllers/controller_test_base.py
 tests/controllers/test_api_controller.py
```

### Comparing `moesifapi-1.4.3/setup.py` & `moesifapi-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifapi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.4.3',
+    version='1.4.4',
 
     description='Moesif API Lib for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/api?python#api-libs',
```

### Comparing `moesifapi-1.4.3/tests/controllers/controller_test_base.py` & `moesifapi-1.4.4/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/tests/controllers/test_api_controller.py` & `moesifapi-1.4.4/tests/controllers/test_api_controller.py`

 * *Files identical despite different names*

### Comparing `moesifapi-1.4.3/tests/test_helper.py` & `moesifapi-1.4.4/tests/test_helper.py`

 * *Files identical despite different names*

