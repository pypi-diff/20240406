# Comparing `tmp/xia-module-gcp-bigquery-0.0.5.tar.gz` & `tmp/xia-module-gcp-bigquery-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-gcp-bigquery-0.0.5.tar", last modified: Sat Apr  6 15:43:57 2024, max compression
+gzip compressed data, was "xia-module-gcp-bigquery-0.0.6.tar", last modified: Sat Apr  6 16:37:21 2024, max compression
```

## Comparing `xia-module-gcp-bigquery-0.0.5.tar` & `xia-module-gcp-bigquery-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 15:43:56.000000 xia-module-gcp-bigquery-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.040198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.040198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.040198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.040198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.040198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/base/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 15:43:34.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:43:57.044198 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 15:43:56.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-06 15:43:57.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:43:56.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:43:56.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 15:43:56.000000 xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 16:37:20.000000 xia-module-gcp-bigquery-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.191261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 16:36:52.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:37:21.187261 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 16:37:21.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-06 16:37:21.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:37:21.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 16:37:21.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 16:37:21.000000 xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/top_level.txt
```

### Comparing `xia-module-gcp-bigquery-0.0.5/LICENSE` & `xia-module-gcp-bigquery-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.5/setup.py` & `xia-module-gcp-bigquery-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 locals {
   project = yamldecode(file(var.project_file))
-  module_name = replace(substr(basename(path.module), 9, length(basename(path.module)) - 9), "-", "_")
+  module_name = substr(basename(path.module), 9, length(basename(path.module)) - 9)
   landscape = yamldecode(file(var.landscape_file))
   applications = yamldecode(file(var.applications_file))
   project_prefix = local.project["project_prefix"]
   environment_dict = local.landscape["environments"]
   application_list = lookup(lookup(local.landscape["modules"], local.module_name, {}), "applications", [])
 }
```

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 locals {
   project = yamldecode(file(var.project_file))
-  module_name = replace(substr(basename(path.module), 9, length(basename(path.module)) - 9), "-", "_")
+  module_name = substr(basename(path.module), 9, length(basename(path.module)) - 9)
   landscape = yamldecode(file(var.landscape_file))
   applications = yamldecode(file(var.applications_file))
   project_prefix = local.project["project_prefix"]
   environment_dict = local.landscape["environments"]
   application_list = lookup(lookup(local.landscape["modules"], local.module_name, {}), "applications", [])
 }
```

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.5/xia_module_gcp_bigquery.egg-info/SOURCES.txt` & `xia-module-gcp-bigquery-0.0.6/xia_module_gcp_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

