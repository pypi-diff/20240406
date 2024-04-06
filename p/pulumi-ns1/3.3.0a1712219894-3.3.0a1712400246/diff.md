# Comparing `tmp/pulumi_ns1-3.3.0a1712219894.tar.gz` & `tmp/pulumi_ns1-3.3.0a1712400246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.3.0a1712219894.tar", last modified: Thu Apr  4 08:41:43 2024, max compression
+gzip compressed data, was "pulumi_ns1-3.3.0a1712400246.tar", last modified: Sat Apr  6 10:56:05 2024, max compression
```

## Comparing `pulumi_ns1-3.3.0a1712219894.tar` & `pulumi_ns1-3.3.0a1712400246.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:41:43.530917 pulumi_ns1-3.3.0a1712219894/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-04 08:41:43.530917 pulumi_ns1-3.3.0a1712219894/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:41:43.526917 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/account_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    87352 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:41:43.530917 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/dnsview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_monitoring_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    45856 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/monitoring_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/notify_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/pulsar_job.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    81738 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/tsigkey.py
--rw-r--r--   0 runner    (1001) docker     (127)    89294 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:41:43.530917 pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-04 08:41:43.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 08:41:43.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:41:43.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 08:41:43.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 08:41:43.000000 pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-04 08:41:36.000000 pulumi_ns1-3.3.0a1712219894/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:41:43.530917 pulumi_ns1-3.3.0a1712219894/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:56:05.596532 pulumi_ns1-3.3.0a1712400246/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-06 10:56:05.596532 pulumi_ns1-3.3.0a1712400246/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:56:05.596532 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/account_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87352 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:56:05.596532 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/dnsview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_monitoring_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45856 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/monitoring_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/notify_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/pulsar_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81738 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/tsigkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89294 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 10:56:05.596532 pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-06 10:56:05.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-06 10:56:05.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 10:56:05.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 10:56:05.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 10:56:05.000000 pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-06 10:55:59.000000 pulumi_ns1-3.3.0a1712400246/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 10:56:05.600532 pulumi_ns1-3.3.0a1712400246/setup.cfg
```

### Comparing `pulumi_ns1-3.3.0a1712219894/PKG-INFO` & `pulumi_ns1-3.3.0a1712400246/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1712219894
+Version: 3.3.0a1712400246
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1712219894/README.md` & `pulumi_ns1-3.3.0a1712400246/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/__init__.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/_inputs.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/_utilities.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/account_whitelist.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/account_whitelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/api_key.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/application.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/config/__init__.pyi` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/config/vars.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/data_feed.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/data_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/data_source.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/dataset.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/dnsview.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/dnsview.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_dns_sec.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_dns_sec.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_monitoring_regions.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_monitoring_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_networks.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_record.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/get_zone.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/monitoring_job.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/monitoring_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/notify_list.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/notify_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/outputs.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/provider.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/pulsar_job.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/pulsar_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/record.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/subnet.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/team.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/tsigkey.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/tsigkey.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/user.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1/zone.py` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/PKG-INFO` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1712219894
+Version: 3.3.0a1712400246
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1712219894/pulumi_ns1.egg-info/SOURCES.txt` & `pulumi_ns1-3.3.0a1712400246/pulumi_ns1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1712219894/pyproject.toml` & `pulumi_ns1-3.3.0a1712400246/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_ns1"
   description = "A Pulumi package for creating and managing ns1 cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "ns1"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1712219894"
+  version = "3.3.0a1712400246"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-ns1"
 
 [build-system]
```

