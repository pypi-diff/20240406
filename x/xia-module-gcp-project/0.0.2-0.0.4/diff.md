# Comparing `tmp/xia-module-gcp-project-0.0.2.tar.gz` & `tmp/xia-module-gcp-project-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-gcp-project-0.0.2.tar", last modified: Sun Feb 25 19:31:00 2024, max compression
+gzip compressed data, was "xia-module-gcp-project-0.0.4.tar", last modified: Sat Apr  6 15:46:18 2024, max compression
```

## Comparing `xia-module-gcp-project-0.0.2.tar` & `xia-module-gcp-project-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 19:30:59.000000 xia-module-gcp-project-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/xia_module_gcp_project/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.092636 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.092636 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/base/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/module/
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-25 19:30:44.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:31:00.096636 xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 19:31:00.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-25 19:31:00.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 19:31:00.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-25 19:31:00.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 19:31:00.000000 xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 15:46:18.000000 xia-module-gcp-project-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/xia_module_gcp_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-06 15:46:09.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:46:18.156769 xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-06 15:46:18.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-06 15:46:18.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:46:18.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:46:18.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 15:46:18.000000 xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/top_level.txt
```

### Comparing `xia-module-gcp-project-0.0.2/LICENSE` & `xia-module-gcp-project-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-project-0.0.2/setup.py` & `xia-module-gcp-project-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-project-0.0.2/xia_module_gcp_project/templates/gcp-module-project/module/main.tf` & `xia-module-gcp-project-0.0.4/xia_module_gcp_project/templates/gcp-module-project/module/main.tf`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,19 @@
   }
 }
 
 locals {
   project = yamldecode(file(var.project_file))
   landscape = yamldecode(file(var.landscape_file))
   applications = yamldecode(file(var.applications_file))
+  settings = lookup(local.landscape, "settings", {})
+  cosmos_name = local.settings["cosmos_name"]
+  realm_name = local.settings["realm_name"]
+  foundation_name = local.settings["foundation_name"]
+  tf_bucket_name = lookup(local.settings, "cosmos_name")
   folder_id = lookup(local.project, "folder_id", null)
   project_prefix = local.project["project_prefix"]
   billing_account = local.project["billing_account"]
   environment_dict = local.landscape["environments"]
   activated_apps = lookup(lookup(local.landscape["modules"], "gcp_module_project", {}), "applications", [])
 }
 
@@ -25,14 +30,15 @@
       for env_name, env in local.environment_dict : {
         app_name          = app_name
         env_name          = env_name
         repository_owner  = app["repository_owner"]
         repository_name   = app["repository_name"]
         project_id        = "${local.project_prefix}${env_name}"
         match_branch      = env["match_branch"]
+        match_event       = lookup(env, "match_event", "push")
       }
     ]
   ]))
 }
 
 resource "google_project" "env_projects" {
   for_each = local.environment_dict
@@ -55,23 +61,14 @@
   for_each = local.environment_dict
 
   project = google_project.env_projects[each.key].project_id
   service = "iam.googleapis.com"
   disable_on_destroy = false
 }
 
-resource "google_storage_bucket" "tfstate-bucket" {
-  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
-
-  project       = local.landscape["settings"]["cosmos_name"]
-  name          = "${local.landscape["settings"]["realm_name"]}_${each.value["app_name"]}_${each.value["env_name"]}"
-  location      = local.landscape["settings"]["foundation_region"]
-  force_destroy = true
-}
-
 resource "google_iam_workload_identity_pool" "github_pool" {
   for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
 
   workload_identity_pool_id = "gh-${each.value["repository_name"]}"
   project  = google_project.env_projects[each.value["env_name"]].project_id
 
   # Workload Identity Pool configuration
@@ -92,19 +89,20 @@
   project  = each.value["project_id"]
 
   # Provider configuration specific to GitHub
   display_name = "ghp-${each.value["repository_name"]}"
   description  = "Provider for GitHub Actions of ${each.value["repository_name"]}"
 
    # Attribute mapping / condition from the OIDC token to Google Cloud attributes
-  attribute_condition = "assertion.sub == 'repo:${each.value["repository_owner"]}/${each.value["repository_name"]}:environment:${each.value["env_name"]}' && assertion.ref.matches('${each.value["match_branch"]}')"
+  attribute_condition = "assertion.sub == 'repo:${each.value["repository_owner"]}/${each.value["repository_name"]}:environment:${each.value["env_name"]}' && assertion.ref.matches('${each.value["match_branch"]}') && assertion.event_name.matches('${each.value["match_event"]}')"
 
   attribute_mapping = {
     "google.subject" = "assertion.sub",
     "attribute.actor" = "assertion.actor",
+    "attribute.event_name" = "assertion.event_name",
     "attribute.repository" = "assertion.repository",
     "attribute.repository_owner" = "assertion.repository_owner"
     "attribute.ref" = "assertion.ref"
   }
 
   oidc {
     issuer_uri = "https://token.actions.githubusercontent.com"
@@ -125,31 +123,88 @@
   service_account_id = google_service_account.github_provider_sa[each.key].id
   role               = "roles/iam.workloadIdentityUser"
   members = [
     "principalSet://iam.googleapis.com/${google_iam_workload_identity_pool.github_pool[each.key].name}/attribute.repository/${each.value["repository_owner"]}/${each.value["repository_name"]}"
   ]
 }
 
-resource "google_storage_bucket_iam_member" "tfstate_bucket_assign" {
+resource "google_storage_bucket_iam_member" "tfstate_bucket_list" {
+  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
+  bucket = local.tf_bucket_name
+  role   = "roles/storage.objectViewer"
+  member = "serviceAccount:${google_service_account.github_provider_sa[each.key].email}"
+}
+
+resource "google_storage_bucket_iam_member" "tfstate_bucket_modify" {
   for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
-  bucket = google_storage_bucket.tfstate-bucket[each.key].id
-  role   = "roles/storage.admin"
+  bucket = local.tf_bucket_name
+  role   = "roles/storage.objectAdmin"
   member = "serviceAccount:${google_service_account.github_provider_sa[each.key].email}"
+
+  condition {
+    title       = "PrefixCondition"
+    description = "Grants access to objects in a specific directory"
+    expression  = "resource.name.startsWith('projects/_/buckets/${local.tf_bucket_name}/objects/${local.realm_name}/_/${local.foundation_name}/${each.value["app_name"]}/${each.value["env_name"]}/')"
+  }
 }
 
+resource "github_actions_environment_variable" "action_var_cosmos_name" {
+  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
+
+  repository       = each.value["repository_name"]
+  environment      = each.value["env_name"]
+  variable_name    = "COSMOS_NAME"
+  value            = local.cosmos_name
+}
+
+resource "github_actions_environment_variable" "action_var_realm_name" {
+  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
+
+  repository       = each.value["repository_name"]
+  environment      = each.value["env_name"]
+  variable_name    = "REALM_NAME"
+  value            = local.realm_name
+}
+
+resource "github_actions_environment_variable" "action_var_foundation_name" {
+  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
+
+  repository       = each.value["repository_name"]
+  environment      = each.value["env_name"]
+  variable_name    = "FOUNDATION_NAME"
+  value            = local.foundation_name
+}
+
+resource "github_actions_environment_variable" "action_var_app_name" {
+  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
+
+  repository       = each.value["repository_name"]
+  environment      = each.value["env_name"]
+  variable_name    = "APP_NAME"
+  value            = each.value["app_name"]
+}
 
 resource "github_actions_environment_variable" "action_var_project_id" {
   for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
 
   repository       = each.value["repository_name"]
   environment      = each.value["env_name"]
   variable_name    = "PROJECT_ID"
   value            = each.value["project_id"]
 }
 
+resource "github_actions_environment_variable" "action_var_env_name" {
+  for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
+
+  repository       = each.value["repository_name"]
+  environment      = each.value["env_name"]
+  variable_name    = "ENV_NAME"
+  value            = each.value["env_name"]
+}
+
 resource "github_actions_environment_variable" "action_var_wip_name" {
   for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
 
   repository       = each.value["repository_name"]
   environment      = each.value["env_name"]
   variable_name    = "SECRET_WIP_NAME"
   value            = google_iam_workload_identity_pool_provider.github_provider[each.key].name
@@ -166,9 +221,9 @@
 
 resource "github_actions_environment_variable" "action_var_tf_bucket" {
   for_each = { for s in local.all_pool_settings : "${s.app_name}-${s.env_name}" => s }
 
   repository       = each.value["repository_name"]
   environment      = each.value["env_name"]
   variable_name    = "TF_BUCKET_NAME"
-  value            = google_storage_bucket.tfstate-bucket[each.key].id
+  value            = local.tf_bucket_name
 }
```

### Comparing `xia-module-gcp-project-0.0.2/xia_module_gcp_project.egg-info/SOURCES.txt` & `xia-module-gcp-project-0.0.4/xia_module_gcp_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

