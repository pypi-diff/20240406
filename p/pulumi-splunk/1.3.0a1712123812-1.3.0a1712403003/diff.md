# Comparing `tmp/pulumi_splunk-1.3.0a1712123812.tar.gz` & `tmp/pulumi_splunk-1.3.0a1712403003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1712123812.tar", last modified: Wed Apr  3 05:58:43 2024, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1712403003.tar", last modified: Sat Apr  6 11:33:53 2024, max compression
```

## Comparing `pulumi_splunk-1.3.0a1712123812.tar` & `pulumi_splunk-1.3.0a1712403003.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.110420 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    38756 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    22001 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.110420 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)   154940 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    42158 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    36720 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44131 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    43577 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    32027 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   515197 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:33:53.738839 pulumi_splunk-1.3.0a1712403003/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-06 11:33:53.738839 pulumi_splunk-1.3.0a1712403003/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:33:53.734839 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38756 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22001 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:33:53.738839 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154940 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42158 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36720 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44131 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43577 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32027 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   514567 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:33:53.738839 pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-06 11:33:53.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-06 11:33:53.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:33:53.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 11:33:53.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 11:33:53.000000 pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 11:33:47.000000 pulumi_splunk-1.3.0a1712403003/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:33:53.738839 pulumi_splunk-1.3.0a1712403003/setup.cfg
```

### Comparing `pulumi_splunk-1.3.0a1712123812/PKG-INFO` & `pulumi_splunk-1.3.0a1712403003/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1712123812
+Version: 1.3.0a1712403003
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1712123812/README.md` & `pulumi_splunk-1.3.0a1712403003/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/admin_saml_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/apps_local.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/authentication_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/authorization_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/__init__.pyi` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/configs_conf.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/data_ui_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/generic_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/inputs_udp.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/saved_searches.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,24 +297,24 @@
         :param pulumi.Input[str] alert_condition: Contains a conditional search that is evaluated against the results of the saved search. Defaults to an empty string.
         :param pulumi.Input[bool] alert_digest_mode: Specifies whether alert actions are applied to the entire result set or on each individual result.Defaults to 1 (true).
         :param pulumi.Input[str] alert_expires: Valid values: [number][time-unit]Sets the period of time to show the alert in the dashboard. Defaults to 24h.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
         :param pulumi.Input[int] alert_severity: Valid values: (1 | 2 | 3 | 4 | 5 | 6) Sets the alert severity level.Valid values are:1 DEBUG 2 INFO 3 WARN 4 ERROR 5 SEVERE 6 FATAL Defaults to 3.
         :param pulumi.Input[bool] alert_suppress: Indicates whether alert suppression is enabled for this scheduled search.
         :param pulumi.Input[str] alert_suppress_fields: Comma delimited list of fields to use for suppression when doing per result alerting. Required if suppression is turned on and per result alerting is enabled.
         :param pulumi.Input[str] alert_suppress_period: Valid values: [number][time-unit] Specifies the suppresion period. Only valid if alert.supress is enabled.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
-        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         :param pulumi.Input[bool] alert_track: Valid values: (true | false | auto) Specifies whether to track the actions triggered by this scheduled search.auto - determine whether to track or not based on the tracking setting of each action, do not track scheduled searches that always trigger actions. Default value true - force alert tracking.false - disable alert tracking for this search.
         :param pulumi.Input[str] alert_type: What to base the alert on, overriden by alert_condition if it is specified. Valid values are: always, custom, number of events, number of hosts, number of sources.
         :param pulumi.Input[str] allow_skew: Allows the search scheduler to distribute scheduled searches randomly and more evenly over their specified search periods.
         :param pulumi.Input[bool] auto_summarize: Indicates whether the scheduler should ensure that the data for this search is automatically summarized. Defaults to 0.
         :param pulumi.Input[str] auto_summarize_command: An auto summarization template for this search. See auto summarization options in savedsearches.conf for more details.
         :param pulumi.Input[str] auto_summarize_cron_schedule: Cron schedule that probes and generates the summaries for this saved search.The default value is */10 * * * * and corresponds to \\`every ten hours\\`.
         :param pulumi.Input[str] auto_summarize_dispatch_earliest_time: A time string that specifies the earliest time for summarizing this search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
         :param pulumi.Input[str] auto_summarize_dispatch_latest_time: A time string that specifies the latest time for summarizing this saved search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
-        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] auto_summarize_dispatch_ttl: Valid values: Integer[p]. Defaults to 60.Indicates the time to live (in seconds) for the artifacts of the summarization of the scheduled search.
         :param pulumi.Input[int] auto_summarize_max_disabled_buckets: The maximum number of buckets with the suspended summarization before the summarization search is completely stopped, and the summarization of the search is suspended for auto_summarize.suspend_period. Defaults to 2.
         :param pulumi.Input[float] auto_summarize_max_summary_ratio: The maximum ratio of summary_size/bucket_size, which specifies when to stop summarization and deem it unhelpful for a bucket. Defaults to 0.1 Note: The test is only performed if the summary size is larger than auto_summarize.max_summary_size.
         :param pulumi.Input[int] auto_summarize_max_summary_size: The minimum summary size, in bytes, before testing whether the summarization is helpful.The default value is 52428800 and is equivalent to 5MB.
         :param pulumi.Input[int] auto_summarize_max_time: Maximum time (in seconds) that the summary search is allowed to run. Defaults to 3600.Note: This is an approximate time. The summary search stops at clean bucket boundaries.
         :param pulumi.Input[str] auto_summarize_suspend_period: Time specfier indicating when to suspend summarization of this search if the summarization is deemed unhelpful.Defaults to 24h.
         :param pulumi.Input[str] auto_summarize_timespan: The list of time ranges that each summarized chunk should span. This comprises the list of available granularity levels for which summaries would be available. Specify a comma delimited list of time specifiers.For example a timechart over the last month whose granuality is at the day level should set this to 1d. If you need the same data summarized at the hour level for weekly charts, use: 1h,1d.
@@ -332,15 +332,15 @@
         :param pulumi.Input[bool] dispatch_lookups: Enables or disables the lookups for this search. Defaults to 1.
         :param pulumi.Input[int] dispatch_max_count: The maximum number of results before finalizing the search. Defaults to 500000.
         :param pulumi.Input[int] dispatch_max_time: Indicates the maximum amount of time (in seconds) before finalizing the search. Defaults to 0.
         :param pulumi.Input[int] dispatch_reduce_freq: Specifies, in seconds, how frequently the MapReduce reduce phase runs on accumulated map values. Defaults to 10.
         :param pulumi.Input[bool] dispatch_rt_backfill: Whether to back fill the real time window for this search. Parameter valid only if this is a real time search. Defaults to 0.
         :param pulumi.Input[int] dispatch_rt_maximum_span: Allows for a per-job override of the [search] indexed_realtime_maximum_span setting in limits.conf.
         :param pulumi.Input[bool] dispatch_spawn_process: Specifies whether a new search process spawns when this saved search is executed. Defaults to 1. Searches against indexes must run in a separate process.
-        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] dispatch_ttl: Valid values: Integer[p]. Defaults to 2p.Indicates the time to live (in seconds) for the artifacts of the scheduled search, if no actions are triggered.
         :param pulumi.Input[str] display_view: Defines the default UI view name (not label) in which to load the results. Accessibility is subject to the user having sufficient permissions.
         :param pulumi.Input[bool] is_scheduled: Whether this search is to be run on a schedule
         :param pulumi.Input[bool] is_visible: Specifies whether this saved search should be listed in the visible saved search list. Defaults to 1.
         :param pulumi.Input[int] max_concurrent: The maximum number of concurrent instances of this search the scheduler is allowed to run. Defaults to 1.
         :param pulumi.Input[str] name: A name for the search.
         :param pulumi.Input[bool] realtime_schedule: Defaults to 1. Controls the way the scheduler computes the next execution time of a scheduled search. If this value is set to 1, the scheduler bases its determination of the next scheduled search execution time on the current time. If this value is set to 0, the scheduler bases its determination of the next scheduled search on the last search execution time. This is called continuous scheduling. If set to 0, the scheduler never skips scheduled execution periods. However, the execution of the saved search might fall behind depending on the scheduler load. Use continuous scheduling whenever you enable the summary index option.
@@ -2019,15 +2019,15 @@
     def alert_suppress_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alert_suppress_period", value)
 
     @property
     @pulumi.getter(name="alertThreshold")
     def alert_threshold(self) -> Optional[pulumi.Input[str]]:
         """
-        Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         """
         return pulumi.get(self, "alert_threshold")
 
     @alert_threshold.setter
     def alert_threshold(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alert_threshold", value)
 
@@ -2127,15 +2127,15 @@
     def auto_summarize_dispatch_latest_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "auto_summarize_dispatch_latest_time", value)
 
     @property
     @pulumi.getter(name="autoSummarizeDispatchTimeFormat")
     def auto_summarize_dispatch_time_format(self) -> Optional[pulumi.Input[str]]:
         """
-        Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         """
         return pulumi.get(self, "auto_summarize_dispatch_time_format")
 
     @auto_summarize_dispatch_time_format.setter
     def auto_summarize_dispatch_time_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "auto_summarize_dispatch_time_format", value)
 
@@ -2439,15 +2439,15 @@
     def dispatch_spawn_process(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dispatch_spawn_process", value)
 
     @property
     @pulumi.getter(name="dispatchTimeFormat")
     def dispatch_time_format(self) -> Optional[pulumi.Input[str]]:
         """
-        A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         """
         return pulumi.get(self, "dispatch_time_format")
 
     @dispatch_time_format.setter
     def dispatch_time_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dispatch_time_format", value)
 
@@ -2925,24 +2925,24 @@
         :param pulumi.Input[str] alert_condition: Contains a conditional search that is evaluated against the results of the saved search. Defaults to an empty string.
         :param pulumi.Input[bool] alert_digest_mode: Specifies whether alert actions are applied to the entire result set or on each individual result.Defaults to 1 (true).
         :param pulumi.Input[str] alert_expires: Valid values: [number][time-unit]Sets the period of time to show the alert in the dashboard. Defaults to 24h.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
         :param pulumi.Input[int] alert_severity: Valid values: (1 | 2 | 3 | 4 | 5 | 6) Sets the alert severity level.Valid values are:1 DEBUG 2 INFO 3 WARN 4 ERROR 5 SEVERE 6 FATAL Defaults to 3.
         :param pulumi.Input[bool] alert_suppress: Indicates whether alert suppression is enabled for this scheduled search.
         :param pulumi.Input[str] alert_suppress_fields: Comma delimited list of fields to use for suppression when doing per result alerting. Required if suppression is turned on and per result alerting is enabled.
         :param pulumi.Input[str] alert_suppress_period: Valid values: [number][time-unit] Specifies the suppresion period. Only valid if alert.supress is enabled.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
-        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         :param pulumi.Input[bool] alert_track: Valid values: (true | false | auto) Specifies whether to track the actions triggered by this scheduled search.auto - determine whether to track or not based on the tracking setting of each action, do not track scheduled searches that always trigger actions. Default value true - force alert tracking.false - disable alert tracking for this search.
         :param pulumi.Input[str] alert_type: What to base the alert on, overriden by alert_condition if it is specified. Valid values are: always, custom, number of events, number of hosts, number of sources.
         :param pulumi.Input[str] allow_skew: Allows the search scheduler to distribute scheduled searches randomly and more evenly over their specified search periods.
         :param pulumi.Input[bool] auto_summarize: Indicates whether the scheduler should ensure that the data for this search is automatically summarized. Defaults to 0.
         :param pulumi.Input[str] auto_summarize_command: An auto summarization template for this search. See auto summarization options in savedsearches.conf for more details.
         :param pulumi.Input[str] auto_summarize_cron_schedule: Cron schedule that probes and generates the summaries for this saved search.The default value is */10 * * * * and corresponds to \\`every ten hours\\`.
         :param pulumi.Input[str] auto_summarize_dispatch_earliest_time: A time string that specifies the earliest time for summarizing this search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
         :param pulumi.Input[str] auto_summarize_dispatch_latest_time: A time string that specifies the latest time for summarizing this saved search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
-        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] auto_summarize_dispatch_ttl: Valid values: Integer[p]. Defaults to 60.Indicates the time to live (in seconds) for the artifacts of the summarization of the scheduled search.
         :param pulumi.Input[int] auto_summarize_max_disabled_buckets: The maximum number of buckets with the suspended summarization before the summarization search is completely stopped, and the summarization of the search is suspended for auto_summarize.suspend_period. Defaults to 2.
         :param pulumi.Input[float] auto_summarize_max_summary_ratio: The maximum ratio of summary_size/bucket_size, which specifies when to stop summarization and deem it unhelpful for a bucket. Defaults to 0.1 Note: The test is only performed if the summary size is larger than auto_summarize.max_summary_size.
         :param pulumi.Input[int] auto_summarize_max_summary_size: The minimum summary size, in bytes, before testing whether the summarization is helpful.The default value is 52428800 and is equivalent to 5MB.
         :param pulumi.Input[int] auto_summarize_max_time: Maximum time (in seconds) that the summary search is allowed to run. Defaults to 3600.Note: This is an approximate time. The summary search stops at clean bucket boundaries.
         :param pulumi.Input[str] auto_summarize_suspend_period: Time specfier indicating when to suspend summarization of this search if the summarization is deemed unhelpful.Defaults to 24h.
         :param pulumi.Input[str] auto_summarize_timespan: The list of time ranges that each summarized chunk should span. This comprises the list of available granularity levels for which summaries would be available. Specify a comma delimited list of time specifiers.For example a timechart over the last month whose granuality is at the day level should set this to 1d. If you need the same data summarized at the hour level for weekly charts, use: 1h,1d.
@@ -2960,15 +2960,15 @@
         :param pulumi.Input[bool] dispatch_lookups: Enables or disables the lookups for this search. Defaults to 1.
         :param pulumi.Input[int] dispatch_max_count: The maximum number of results before finalizing the search. Defaults to 500000.
         :param pulumi.Input[int] dispatch_max_time: Indicates the maximum amount of time (in seconds) before finalizing the search. Defaults to 0.
         :param pulumi.Input[int] dispatch_reduce_freq: Specifies, in seconds, how frequently the MapReduce reduce phase runs on accumulated map values. Defaults to 10.
         :param pulumi.Input[bool] dispatch_rt_backfill: Whether to back fill the real time window for this search. Parameter valid only if this is a real time search. Defaults to 0.
         :param pulumi.Input[int] dispatch_rt_maximum_span: Allows for a per-job override of the [search] indexed_realtime_maximum_span setting in limits.conf.
         :param pulumi.Input[bool] dispatch_spawn_process: Specifies whether a new search process spawns when this saved search is executed. Defaults to 1. Searches against indexes must run in a separate process.
-        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] dispatch_ttl: Valid values: Integer[p]. Defaults to 2p.Indicates the time to live (in seconds) for the artifacts of the scheduled search, if no actions are triggered.
         :param pulumi.Input[str] display_view: Defines the default UI view name (not label) in which to load the results. Accessibility is subject to the user having sufficient permissions.
         :param pulumi.Input[bool] is_scheduled: Whether this search is to be run on a schedule
         :param pulumi.Input[bool] is_visible: Specifies whether this saved search should be listed in the visible saved search list. Defaults to 1.
         :param pulumi.Input[int] max_concurrent: The maximum number of concurrent instances of this search the scheduler is allowed to run. Defaults to 1.
         :param pulumi.Input[str] name: A name for the search.
         :param pulumi.Input[bool] realtime_schedule: Defaults to 1. Controls the way the scheduler computes the next execution time of a scheduled search. If this value is set to 1, the scheduler bases its determination of the next scheduled search execution time on the current time. If this value is set to 0, the scheduler bases its determination of the next scheduled search on the last search execution time. This is called continuous scheduling. If set to 0, the scheduler never skips scheduled execution periods. However, the execution of the saved search might fall behind depending on the scheduler load. Use continuous scheduling whenever you enable the summary index option.
@@ -4707,15 +4707,15 @@
     def alert_suppress_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alert_suppress_period", value)
 
     @property
     @pulumi.getter(name="alertThreshold")
     def alert_threshold(self) -> Optional[pulumi.Input[str]]:
         """
-        Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         """
         return pulumi.get(self, "alert_threshold")
 
     @alert_threshold.setter
     def alert_threshold(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alert_threshold", value)
 
@@ -4815,15 +4815,15 @@
     def auto_summarize_dispatch_latest_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "auto_summarize_dispatch_latest_time", value)
 
     @property
     @pulumi.getter(name="autoSummarizeDispatchTimeFormat")
     def auto_summarize_dispatch_time_format(self) -> Optional[pulumi.Input[str]]:
         """
-        Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         """
         return pulumi.get(self, "auto_summarize_dispatch_time_format")
 
     @auto_summarize_dispatch_time_format.setter
     def auto_summarize_dispatch_time_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "auto_summarize_dispatch_time_format", value)
 
@@ -5127,15 +5127,15 @@
     def dispatch_spawn_process(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dispatch_spawn_process", value)
 
     @property
     @pulumi.getter(name="dispatchTimeFormat")
     def dispatch_time_format(self) -> Optional[pulumi.Input[str]]:
         """
-        A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         """
         return pulumi.get(self, "dispatch_time_format")
 
     @dispatch_time_format.setter
     def dispatch_time_format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dispatch_time_format", value)
 
@@ -5651,24 +5651,24 @@
         :param pulumi.Input[str] alert_condition: Contains a conditional search that is evaluated against the results of the saved search. Defaults to an empty string.
         :param pulumi.Input[bool] alert_digest_mode: Specifies whether alert actions are applied to the entire result set or on each individual result.Defaults to 1 (true).
         :param pulumi.Input[str] alert_expires: Valid values: [number][time-unit]Sets the period of time to show the alert in the dashboard. Defaults to 24h.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
         :param pulumi.Input[int] alert_severity: Valid values: (1 | 2 | 3 | 4 | 5 | 6) Sets the alert severity level.Valid values are:1 DEBUG 2 INFO 3 WARN 4 ERROR 5 SEVERE 6 FATAL Defaults to 3.
         :param pulumi.Input[bool] alert_suppress: Indicates whether alert suppression is enabled for this scheduled search.
         :param pulumi.Input[str] alert_suppress_fields: Comma delimited list of fields to use for suppression when doing per result alerting. Required if suppression is turned on and per result alerting is enabled.
         :param pulumi.Input[str] alert_suppress_period: Valid values: [number][time-unit] Specifies the suppresion period. Only valid if alert.supress is enabled.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
-        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         :param pulumi.Input[bool] alert_track: Valid values: (true | false | auto) Specifies whether to track the actions triggered by this scheduled search.auto - determine whether to track or not based on the tracking setting of each action, do not track scheduled searches that always trigger actions. Default value true - force alert tracking.false - disable alert tracking for this search.
         :param pulumi.Input[str] alert_type: What to base the alert on, overriden by alert_condition if it is specified. Valid values are: always, custom, number of events, number of hosts, number of sources.
         :param pulumi.Input[str] allow_skew: Allows the search scheduler to distribute scheduled searches randomly and more evenly over their specified search periods.
         :param pulumi.Input[bool] auto_summarize: Indicates whether the scheduler should ensure that the data for this search is automatically summarized. Defaults to 0.
         :param pulumi.Input[str] auto_summarize_command: An auto summarization template for this search. See auto summarization options in savedsearches.conf for more details.
         :param pulumi.Input[str] auto_summarize_cron_schedule: Cron schedule that probes and generates the summaries for this saved search.The default value is */10 * * * * and corresponds to \\`every ten hours\\`.
         :param pulumi.Input[str] auto_summarize_dispatch_earliest_time: A time string that specifies the earliest time for summarizing this search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
         :param pulumi.Input[str] auto_summarize_dispatch_latest_time: A time string that specifies the latest time for summarizing this saved search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
-        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] auto_summarize_dispatch_ttl: Valid values: Integer[p]. Defaults to 60.Indicates the time to live (in seconds) for the artifacts of the summarization of the scheduled search.
         :param pulumi.Input[int] auto_summarize_max_disabled_buckets: The maximum number of buckets with the suspended summarization before the summarization search is completely stopped, and the summarization of the search is suspended for auto_summarize.suspend_period. Defaults to 2.
         :param pulumi.Input[float] auto_summarize_max_summary_ratio: The maximum ratio of summary_size/bucket_size, which specifies when to stop summarization and deem it unhelpful for a bucket. Defaults to 0.1 Note: The test is only performed if the summary size is larger than auto_summarize.max_summary_size.
         :param pulumi.Input[int] auto_summarize_max_summary_size: The minimum summary size, in bytes, before testing whether the summarization is helpful.The default value is 52428800 and is equivalent to 5MB.
         :param pulumi.Input[int] auto_summarize_max_time: Maximum time (in seconds) that the summary search is allowed to run. Defaults to 3600.Note: This is an approximate time. The summary search stops at clean bucket boundaries.
         :param pulumi.Input[str] auto_summarize_suspend_period: Time specfier indicating when to suspend summarization of this search if the summarization is deemed unhelpful.Defaults to 24h.
         :param pulumi.Input[str] auto_summarize_timespan: The list of time ranges that each summarized chunk should span. This comprises the list of available granularity levels for which summaries would be available. Specify a comma delimited list of time specifiers.For example a timechart over the last month whose granuality is at the day level should set this to 1d. If you need the same data summarized at the hour level for weekly charts, use: 1h,1d.
@@ -5686,15 +5686,15 @@
         :param pulumi.Input[bool] dispatch_lookups: Enables or disables the lookups for this search. Defaults to 1.
         :param pulumi.Input[int] dispatch_max_count: The maximum number of results before finalizing the search. Defaults to 500000.
         :param pulumi.Input[int] dispatch_max_time: Indicates the maximum amount of time (in seconds) before finalizing the search. Defaults to 0.
         :param pulumi.Input[int] dispatch_reduce_freq: Specifies, in seconds, how frequently the MapReduce reduce phase runs on accumulated map values. Defaults to 10.
         :param pulumi.Input[bool] dispatch_rt_backfill: Whether to back fill the real time window for this search. Parameter valid only if this is a real time search. Defaults to 0.
         :param pulumi.Input[int] dispatch_rt_maximum_span: Allows for a per-job override of the [search] indexed_realtime_maximum_span setting in limits.conf.
         :param pulumi.Input[bool] dispatch_spawn_process: Specifies whether a new search process spawns when this saved search is executed. Defaults to 1. Searches against indexes must run in a separate process.
-        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] dispatch_ttl: Valid values: Integer[p]. Defaults to 2p.Indicates the time to live (in seconds) for the artifacts of the scheduled search, if no actions are triggered.
         :param pulumi.Input[str] display_view: Defines the default UI view name (not label) in which to load the results. Accessibility is subject to the user having sufficient permissions.
         :param pulumi.Input[bool] is_scheduled: Whether this search is to be run on a schedule
         :param pulumi.Input[bool] is_visible: Specifies whether this saved search should be listed in the visible saved search list. Defaults to 1.
         :param pulumi.Input[int] max_concurrent: The maximum number of concurrent instances of this search the scheduler is allowed to run. Defaults to 1.
         :param pulumi.Input[str] name: A name for the search.
         :param pulumi.Input[bool] realtime_schedule: Defaults to 1. Controls the way the scheduler computes the next execution time of a scheduled search. If this value is set to 1, the scheduler bases its determination of the next scheduled search execution time on the current time. If this value is set to 0, the scheduler bases its determination of the next scheduled search on the last search execution time. This is called continuous scheduling. If set to 0, the scheduler never skips scheduled execution periods. However, the execution of the saved search might fall behind depending on the scheduler load. Use continuous scheduling whenever you enable the summary index option.
@@ -6407,24 +6407,24 @@
         :param pulumi.Input[str] alert_condition: Contains a conditional search that is evaluated against the results of the saved search. Defaults to an empty string.
         :param pulumi.Input[bool] alert_digest_mode: Specifies whether alert actions are applied to the entire result set or on each individual result.Defaults to 1 (true).
         :param pulumi.Input[str] alert_expires: Valid values: [number][time-unit]Sets the period of time to show the alert in the dashboard. Defaults to 24h.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
         :param pulumi.Input[int] alert_severity: Valid values: (1 | 2 | 3 | 4 | 5 | 6) Sets the alert severity level.Valid values are:1 DEBUG 2 INFO 3 WARN 4 ERROR 5 SEVERE 6 FATAL Defaults to 3.
         :param pulumi.Input[bool] alert_suppress: Indicates whether alert suppression is enabled for this scheduled search.
         :param pulumi.Input[str] alert_suppress_fields: Comma delimited list of fields to use for suppression when doing per result alerting. Required if suppression is turned on and per result alerting is enabled.
         :param pulumi.Input[str] alert_suppress_period: Valid values: [number][time-unit] Specifies the suppresion period. Only valid if alert.supress is enabled.Use [number][time-unit] to specify a time. For example: 60 = 60 seconds, 1m = 1 minute, 1h = 60 minutes = 1 hour.
-        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        :param pulumi.Input[str] alert_threshold: Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         :param pulumi.Input[bool] alert_track: Valid values: (true | false | auto) Specifies whether to track the actions triggered by this scheduled search.auto - determine whether to track or not based on the tracking setting of each action, do not track scheduled searches that always trigger actions. Default value true - force alert tracking.false - disable alert tracking for this search.
         :param pulumi.Input[str] alert_type: What to base the alert on, overriden by alert_condition if it is specified. Valid values are: always, custom, number of events, number of hosts, number of sources.
         :param pulumi.Input[str] allow_skew: Allows the search scheduler to distribute scheduled searches randomly and more evenly over their specified search periods.
         :param pulumi.Input[bool] auto_summarize: Indicates whether the scheduler should ensure that the data for this search is automatically summarized. Defaults to 0.
         :param pulumi.Input[str] auto_summarize_command: An auto summarization template for this search. See auto summarization options in savedsearches.conf for more details.
         :param pulumi.Input[str] auto_summarize_cron_schedule: Cron schedule that probes and generates the summaries for this saved search.The default value is */10 * * * * and corresponds to \\`every ten hours\\`.
         :param pulumi.Input[str] auto_summarize_dispatch_earliest_time: A time string that specifies the earliest time for summarizing this search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
         :param pulumi.Input[str] auto_summarize_dispatch_latest_time: A time string that specifies the latest time for summarizing this saved search. Can be a relative or absolute time.If this value is an absolute time, use the dispatch.time_format to format the value.
-        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] auto_summarize_dispatch_time_format: Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] auto_summarize_dispatch_ttl: Valid values: Integer[p]. Defaults to 60.Indicates the time to live (in seconds) for the artifacts of the summarization of the scheduled search.
         :param pulumi.Input[int] auto_summarize_max_disabled_buckets: The maximum number of buckets with the suspended summarization before the summarization search is completely stopped, and the summarization of the search is suspended for auto_summarize.suspend_period. Defaults to 2.
         :param pulumi.Input[float] auto_summarize_max_summary_ratio: The maximum ratio of summary_size/bucket_size, which specifies when to stop summarization and deem it unhelpful for a bucket. Defaults to 0.1 Note: The test is only performed if the summary size is larger than auto_summarize.max_summary_size.
         :param pulumi.Input[int] auto_summarize_max_summary_size: The minimum summary size, in bytes, before testing whether the summarization is helpful.The default value is 52428800 and is equivalent to 5MB.
         :param pulumi.Input[int] auto_summarize_max_time: Maximum time (in seconds) that the summary search is allowed to run. Defaults to 3600.Note: This is an approximate time. The summary search stops at clean bucket boundaries.
         :param pulumi.Input[str] auto_summarize_suspend_period: Time specfier indicating when to suspend summarization of this search if the summarization is deemed unhelpful.Defaults to 24h.
         :param pulumi.Input[str] auto_summarize_timespan: The list of time ranges that each summarized chunk should span. This comprises the list of available granularity levels for which summaries would be available. Specify a comma delimited list of time specifiers.For example a timechart over the last month whose granuality is at the day level should set this to 1d. If you need the same data summarized at the hour level for weekly charts, use: 1h,1d.
@@ -6442,15 +6442,15 @@
         :param pulumi.Input[bool] dispatch_lookups: Enables or disables the lookups for this search. Defaults to 1.
         :param pulumi.Input[int] dispatch_max_count: The maximum number of results before finalizing the search. Defaults to 500000.
         :param pulumi.Input[int] dispatch_max_time: Indicates the maximum amount of time (in seconds) before finalizing the search. Defaults to 0.
         :param pulumi.Input[int] dispatch_reduce_freq: Specifies, in seconds, how frequently the MapReduce reduce phase runs on accumulated map values. Defaults to 10.
         :param pulumi.Input[bool] dispatch_rt_backfill: Whether to back fill the real time window for this search. Parameter valid only if this is a real time search. Defaults to 0.
         :param pulumi.Input[int] dispatch_rt_maximum_span: Allows for a per-job override of the [search] indexed_realtime_maximum_span setting in limits.conf.
         :param pulumi.Input[bool] dispatch_spawn_process: Specifies whether a new search process spawns when this saved search is executed. Defaults to 1. Searches against indexes must run in a separate process.
-        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        :param pulumi.Input[str] dispatch_time_format: A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         :param pulumi.Input[str] dispatch_ttl: Valid values: Integer[p]. Defaults to 2p.Indicates the time to live (in seconds) for the artifacts of the scheduled search, if no actions are triggered.
         :param pulumi.Input[str] display_view: Defines the default UI view name (not label) in which to load the results. Accessibility is subject to the user having sufficient permissions.
         :param pulumi.Input[bool] is_scheduled: Whether this search is to be run on a schedule
         :param pulumi.Input[bool] is_visible: Specifies whether this saved search should be listed in the visible saved search list. Defaults to 1.
         :param pulumi.Input[int] max_concurrent: The maximum number of concurrent instances of this search the scheduler is allowed to run. Defaults to 1.
         :param pulumi.Input[str] name: A name for the search.
         :param pulumi.Input[bool] realtime_schedule: Defaults to 1. Controls the way the scheduler computes the next execution time of a scheduled search. If this value is set to 1, the scheduler bases its determination of the next scheduled search execution time on the current time. If this value is set to 0, the scheduler bases its determination of the next scheduled search on the last search execution time. This is called continuous scheduling. If set to 0, the scheduler never skips scheduled execution periods. However, the execution of the saved search might fall behind depending on the scheduler load. Use continuous scheduling whenever you enable the summary index option.
@@ -7567,15 +7567,15 @@
         """
         return pulumi.get(self, "alert_suppress_period")
 
     @property
     @pulumi.getter(name="alertThreshold")
     def alert_threshold(self) -> pulumi.Output[str]:
         """
-        Valid values are: Integer[%!](MISSING)Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
+        Valid values are: Integer[%]Specifies the value to compare (see alert_comparator) before triggering the alert actions. If expressed as a percentage, indicates value to use when alert_comparator is set to rises by perc or drops by perc.
         """
         return pulumi.get(self, "alert_threshold")
 
     @property
     @pulumi.getter(name="alertTrack")
     def alert_track(self) -> pulumi.Output[bool]:
         """
@@ -7639,15 +7639,15 @@
         """
         return pulumi.get(self, "auto_summarize_dispatch_latest_time")
 
     @property
     @pulumi.getter(name="autoSummarizeDispatchTimeFormat")
     def auto_summarize_dispatch_time_format(self) -> pulumi.Output[str]:
         """
-        Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        Defines the time format that Splunk software uses to specify the earliest and latest time. Defaults to %FT%T.%Q%:z
         """
         return pulumi.get(self, "auto_summarize_dispatch_time_format")
 
     @property
     @pulumi.getter(name="autoSummarizeDispatchTtl")
     def auto_summarize_dispatch_ttl(self) -> pulumi.Output[str]:
         """
@@ -7847,15 +7847,15 @@
         """
         return pulumi.get(self, "dispatch_spawn_process")
 
     @property
     @pulumi.getter(name="dispatchTimeFormat")
     def dispatch_time_format(self) -> pulumi.Output[str]:
         """
-        A time format string that defines the time format for specifying the earliest and latest time. Defaults to %!F(MISSING)T%!T(MISSING).%!Q(MISSING)%!:(MISSING)z
+        A time format string that defines the time format for specifying the earliest and latest time. Defaults to %FT%T.%Q%:z
         """
         return pulumi.get(self, "dispatch_time_format")
 
     @property
     @pulumi.getter(name="dispatchTtl")
     def dispatch_ttl(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk/sh_indexes_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1712123812
+Version: 1.3.0a1712403003
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1712403003/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1712123812/pyproject.toml` & `pulumi_splunk-1.3.0a1712403003/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_splunk"
   description = "A Pulumi package for creating and managing splunk cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "splunk"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.3.0a1712123812"
+  version = "1.3.0a1712403003"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-splunk"
 
 [build-system]
```

