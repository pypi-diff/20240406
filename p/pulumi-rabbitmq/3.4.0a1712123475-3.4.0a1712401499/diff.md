# Comparing `tmp/pulumi_rabbitmq-3.4.0a1712123475.tar.gz` & `tmp/pulumi_rabbitmq-3.4.0a1712401499.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rabbitmq-3.4.0a1712123475.tar", last modified: Wed Apr  3 05:53:15 2024, max compression
+gzip compressed data, was "pulumi_rabbitmq-3.4.0a1712401499.tar", last modified: Sat Apr  6 11:23:36 2024, max compression
```

## Comparing `pulumi_rabbitmq-3.4.0a1712123475.tar` & `pulumi_rabbitmq-3.4.0a1712401499.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:53:15.449871 pulumi_rabbitmq-3.4.0a1712123475/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-03 05:53:15.449871 pulumi_rabbitmq-3.4.0a1712123475/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:53:15.449871 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:53:15.449871 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/federation_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/get_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/get_v_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/operator_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37993 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/shovel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/topic_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/v_host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:53:15.449871 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-03 05:53:15.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-03 05:53:15.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:53:15.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 05:53:15.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 05:53:15.000000 pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-03 05:53:09.000000 pulumi_rabbitmq-3.4.0a1712123475/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:53:15.449871 pulumi_rabbitmq-3.4.0a1712123475/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:23:36.991965 pulumi_rabbitmq-3.4.0a1712401499/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-06 11:23:36.991965 pulumi_rabbitmq-3.4.0a1712401499/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:23:36.987965 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20719 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:23:36.991965 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/federation_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/get_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/get_v_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/operator_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37993 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/shovel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/topic_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/v_host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:23:36.991965 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-06 11:23:36.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-06 11:23:36.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:23:36.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 11:23:36.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 11:23:36.000000 pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-06 11:23:30.000000 pulumi_rabbitmq-3.4.0a1712401499/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:23:36.991965 pulumi_rabbitmq-3.4.0a1712401499/setup.cfg
```

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1712401499/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1712123475
+Version: 3.4.0a1712401499
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/README.md` & `pulumi_rabbitmq-3.4.0a1712401499/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/__init__.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/_inputs.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/_utilities.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/binding.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,15 @@
 
         ## Import
 
         Bindings can be imported using the `id` which is composed of
           `vhost/source/destination/destination_type/properties_key`. E.g.
 
         ```sh
-        $ pulumi import rabbitmq:index/binding:Binding test test/test/test/queue/%!
-        (MISSING)```
+        $ pulumi import rabbitmq:index/binding:Binding test test/test/test/queue/%23
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] arguments: Additional key/value arguments for the binding.
         :param pulumi.Input[str] destination: The destination queue or exchange.
         :param pulumi.Input[str] destination_type: The type of destination (queue or exchange).
@@ -379,16 +378,15 @@
 
         ## Import
 
         Bindings can be imported using the `id` which is composed of
           `vhost/source/destination/destination_type/properties_key`. E.g.
 
         ```sh
-        $ pulumi import rabbitmq:index/binding:Binding test test/test/test/queue/%!
-        (MISSING)```
+        $ pulumi import rabbitmq:index/binding:Binding test test/test/test/queue/%23
         ```
 
         :param str resource_name: The name of the resource.
         :param BindingArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/config/__init__.pyi` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/config/vars.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/exchange.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/federation_upstream.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/federation_upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/get_exchange.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/get_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/get_user.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/get_v_host.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/get_v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/operator_policy.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/operator_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/outputs.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/permissions.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/policy.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/provider.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/queue.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/shovel.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/shovel.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/topic_permissions.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/topic_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/user.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq/v_host.py` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq/v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1712123475
+Version: 3.4.0a1712401499
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pulumi_rabbitmq.egg-info/SOURCES.txt` & `pulumi_rabbitmq-3.4.0a1712401499/pulumi_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1712123475/pyproject.toml` & `pulumi_rabbitmq-3.4.0a1712401499/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rabbitmq"
   description = "A Pulumi package for creating and managing RabbitMQ resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rabbitmq"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1712123475"
+  version = "3.4.0a1712401499"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rabbitmq"
 
 [build-system]
```

