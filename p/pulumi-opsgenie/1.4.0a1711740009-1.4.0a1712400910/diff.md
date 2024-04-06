# Comparing `tmp/pulumi_opsgenie-1.4.0a1711740009.tar.gz` & `tmp/pulumi_opsgenie-1.4.0a1712400910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.4.0a1711740009.tar", last modified: Fri Mar 29 19:30:58 2024, max compression
+gzip compressed data, was "pulumi_opsgenie-1.4.0a1712400910.tar", last modified: Sat Apr  6 11:09:24 2024, max compression
```

## Comparing `pulumi_opsgenie-1.4.0a1711740009.tar` & `pulumi_opsgenie-1.4.0a1712400910.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:30:58.419462 pulumi_opsgenie-1.4.0a1711740009/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-29 19:30:58.419462 pulumi_opsgenie-1.4.0a1711740009/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:30:58.419462 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   180603 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58224 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:30:58.419462 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23238 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    23857 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    30636 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)   161038 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25443 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    28130 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:30:58.419462 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-29 19:30:58.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-29 19:30:58.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:30:58.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 19:30:58.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 19:30:58.000000 pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-29 19:30:49.000000 pulumi_opsgenie-1.4.0a1711740009/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:30:58.419462 pulumi_opsgenie-1.4.0a1711740009/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:24.941742 pulumi_opsgenie-1.4.0a1712400910/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-06 11:09:24.941742 pulumi_opsgenie-1.4.0a1712400910/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:24.941742 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   180603 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58224 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:24.941742 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23238 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23857 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30636 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161038 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25443 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28130 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:09:24.941742 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-06 11:09:24.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 11:09:24.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:09:24.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 11:09:24.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 11:09:24.000000 pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 11:09:18.000000 pulumi_opsgenie-1.4.0a1712400910/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:09:24.941742 pulumi_opsgenie-1.4.0a1712400910/setup.cfg
```

### Comparing `pulumi_opsgenie-1.4.0a1711740009/PKG-INFO` & `pulumi_opsgenie-1.4.0a1712400910/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1711740009
+Version: 1.4.0a1712400910
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1711740009/README.md` & `pulumi_opsgenie-1.4.0a1712400910/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/api_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/email_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/incident_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/integration_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/schedule_rotation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1711740009
+Version: 1.4.0a1712400910
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.4.0a1712400910/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1711740009/pyproject.toml` & `pulumi_opsgenie-1.4.0a1712400910/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_opsgenie"
   description = "A Pulumi package for creating and managing opsgenie cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "opsgenie"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.4.0a1711740009"
+  version = "1.4.0a1712400910"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-opsgenie"
 
 [build-system]
```

