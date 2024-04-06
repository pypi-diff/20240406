# Comparing `tmp/xia-module-gcp-bigquery-0.0.3.tar.gz` & `tmp/xia-module-gcp-bigquery-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-gcp-bigquery-0.0.3.tar", last modified: Wed Apr  3 07:12:51 2024, max compression
+gzip compressed data, was "xia-module-gcp-bigquery-0.0.4.tar", last modified: Sat Apr  6 07:28:26 2024, max compression
```

## Comparing `xia-module-gcp-bigquery-0.0.3.tar` & `xia-module-gcp-bigquery-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 07:12:51.000000 xia-module-gcp-bigquery-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.236682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.236682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.236682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.236682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.236682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.236682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/base/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 07:12:27.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:12:51.240682 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 07:12:51.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 07:12:51.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:12:51.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 07:12:51.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 07:12:51.000000 xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-06 07:28:26.000000 xia-module-gcp-bigquery-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.706564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 07:27:59.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:28:26.702564 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-06 07:28:26.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-06 07:28:26.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:28:26.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 07:28:26.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 07:28:26.000000 xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/top_level.txt
```

### Comparing `xia-module-gcp-bigquery-0.0.3/LICENSE` & `xia-module-gcp-bigquery-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/setup.py` & `xia-module-gcp-bigquery-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         project_id        = "${local.project_prefix}${env_name}"
       }
     ]
   ]))
 }
 
 resource "google_project_service" "bigquery_api" {
+  for_each = local.environment_dict
+
+  project     = "${local.project_prefix}${each.key}"
   service = "bigquery.googleapis.com"
   disable_on_destroy = false
 }
 
 resource "google_project_iam_custom_role" "gcp_module_dataset_deployer_role" {
   for_each = local.environment_dict
```

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.3/xia_module_gcp_bigquery.egg-info/SOURCES.txt` & `xia-module-gcp-bigquery-0.0.4/xia_module_gcp_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

