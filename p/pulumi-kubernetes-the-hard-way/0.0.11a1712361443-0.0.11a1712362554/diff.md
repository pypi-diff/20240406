# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1712361443.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1712362554.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1712361443.tar", last modified: Fri Apr  5 23:59:34 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1712362554.tar", last modified: Sat Apr  6 00:17:29 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443.tar` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554.tar`

### file list

```diff
@@ -1,47 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.230387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-05 23:59:34.230387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.222387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     2355 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.226387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      318 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      463 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)     4567 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     2843 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.226387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      421 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)      952 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    10044 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8177 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    21579 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)     6927 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9732 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)     9878 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.226387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      403 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)      942 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1401 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    18602 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    14904 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4166 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)    15417 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.230387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      369 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8252 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    10335 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    19738 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    10561 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    11452 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    12663 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:59:34.230387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-05 23:59:34.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-05 23:59:34.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:59:34.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 23:59:34.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 23:59:34.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      860 2024-04-05 23:59:28.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:59:34.230387 pulumi_kubernetes_the_hard_way-0.0.11a1712361443/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.941998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-06 00:17:29.941998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.933998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     2778 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.937998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      318 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      463 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     4567 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     2843 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.937998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      545 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      952 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    10044 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8177 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    22322 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)     6927 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     8028 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     8232 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     8016 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9732 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    12168 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.941998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      403 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      942 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1401 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    18785 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    14904 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4166 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)    15417 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.941998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      458 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      752 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     9202 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)     9983 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    13042 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    20833 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    12292 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)     8325 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    12221 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14109 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    13586 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:17:29.941998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-06 00:17:29.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-06 00:17:29.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:17:29.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 00:17:29.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 00:17:29.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      860 2024-04-06 00:17:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:17:29.941998 pulumi_kubernetes_the_hard_way-0.0.11a1712362554/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1712361443
+Version: 0.0.11a1712362554
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/README.md` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,17 @@
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
    "kubernetes-the-hard-way:remote:Download": "Download",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:File": "File",
+   "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
+   "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
+   "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tls",
   "fqn": "pulumi_kubernetes_the_hard_way.tls",
@@ -49,19 +52,22 @@
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tools",
   "fqn": "pulumi_kubernetes_the_hard_way.tools",
   "classes": {
+   "kubernetes-the-hard-way:tools:Etcdctl": "Etcdctl",
    "kubernetes-the-hard-way:tools:Mkdir": "Mkdir",
    "kubernetes-the-hard-way:tools:Mktemp": "Mktemp",
    "kubernetes-the-hard-way:tools:Mv": "Mv",
    "kubernetes-the-hard-way:tools:Rm": "Rm",
+   "kubernetes-the-hard-way:tools:Systemctl": "Systemctl",
    "kubernetes-the-hard-way:tools:Tar": "Tar",
+   "kubernetes-the-hard-way:tools:Tee": "Tee",
    "kubernetes-the-hard-way:tools:Wget": "Wget"
   }
  }
 ]
 """,
     resource_packages="""
 [
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -545,7 +545,25 @@
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
         The version of etcd downloaded.
         """
         return pulumi.get(self, "version")
 
+    @pulumi.output_type
+    class EtcdctlResult:
+        def __init__(__self__, result=None):
+            if result and not isinstance(result, _tools.Etcdctl):
+                raise TypeError("Expected argument 'result' to be a _tools.Etcdctl")
+            pulumi.set(__self__, "result", result)
+
+        @property
+        @pulumi.getter
+        def result(self) -> '_tools.Etcdctl':
+            return pulumi.get(self, "result")
+
+    def etcdctl(__self__) -> pulumi.Output['_tools.Etcdctl']:
+        __args__ = dict()
+        __args__['__self__'] = __self__
+        __result__ = pulumi.runtime.call('kubernetes-the-hard-way:remote:EtcdInstall/etcdctl', __args__, res=__self__, typ=EtcdInstall.EtcdctlResult)
+        return __result__.result
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from .. import tools as _tools
 from ._enums import *
 from ._inputs import *
 from .file import File
 import pulumi_command
 
 __all__ = ['SystemdServiceArgs', 'SystemdService']
 
@@ -227,7 +228,61 @@
     @pulumi.getter
     def unit(self) -> pulumi.Output[Optional['outputs.SystemdUnitSection']]:
         """
         Describes the [Unit] section of a systemd service file.
         """
         return pulumi.get(self, "unit")
 
+    @pulumi.output_type
+    class DisableResult:
+        def __init__(__self__, result=None):
+            if result and not isinstance(result, _tools.Systemctl):
+                raise TypeError("Expected argument 'result' to be a _tools.Systemctl")
+            pulumi.set(__self__, "result", result)
+
+        @property
+        @pulumi.getter
+        def result(self) -> '_tools.Systemctl':
+            return pulumi.get(self, "result")
+
+    def disable(__self__) -> pulumi.Output['_tools.Systemctl']:
+        __args__ = dict()
+        __args__['__self__'] = __self__
+        __result__ = pulumi.runtime.call('kubernetes-the-hard-way:remote:SystemdService/disable', __args__, res=__self__, typ=SystemdService.DisableResult)
+        return __result__.result
+
+    @pulumi.output_type
+    class EnableResult:
+        def __init__(__self__, result=None):
+            if result and not isinstance(result, _tools.Systemctl):
+                raise TypeError("Expected argument 'result' to be a _tools.Systemctl")
+            pulumi.set(__self__, "result", result)
+
+        @property
+        @pulumi.getter
+        def result(self) -> '_tools.Systemctl':
+            return pulumi.get(self, "result")
+
+    def enable(__self__) -> pulumi.Output['_tools.Systemctl']:
+        __args__ = dict()
+        __args__['__self__'] = __self__
+        __result__ = pulumi.runtime.call('kubernetes-the-hard-way:remote:SystemdService/enable', __args__, res=__self__, typ=SystemdService.EnableResult)
+        return __result__.result
+
+    @pulumi.output_type
+    class StartResult:
+        def __init__(__self__, result=None):
+            if result and not isinstance(result, _tools.Systemctl):
+                raise TypeError("Expected argument 'result' to be a _tools.Systemctl")
+            pulumi.set(__self__, "result", result)
+
+        @property
+        @pulumi.getter
+        def result(self) -> '_tools.Systemctl':
+            return pulumi.get(self, "result")
+
+    def start(__self__) -> pulumi.Output['_tools.Systemctl']:
+        __args__ = dict()
+        __args__['__self__'] = __self__
+        __result__ = pulumi.runtime.call('kubernetes-the-hard-way:remote:SystemdService/start', __args__, res=__self__, typ=SystemdService.StartResult)
+        return __result__.result
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,19 @@
             'kubernetes-the-hard-way:tls:Certificate',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
+    @pulumi.getter(name="allowedUses")
+    def allowed_uses(self) -> pulumi.Output[Optional[Sequence['AllowedUsage']]]:
+        return pulumi.get(self, "allowed_uses")
+
+    @property
     @pulumi.getter
     def cert(self) -> pulumi.Output['pulumi_tls.LocallySignedCert']:
         return pulumi.get(self, "cert")
 
     @property
     @pulumi.getter(name="certPem")
     def cert_pem(self) -> pulumi.Output[str]:
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,206 +4,201 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from ._enums import *
 import pulumi_command
 
-__all__ = ['MkdirArgs', 'Mkdir']
+__all__ = ['SystemctlArgs', 'Systemctl']
 
 @pulumi.input_type
-class MkdirArgs:
+class SystemctlArgs:
     def __init__(__self__, *,
+                 commands: pulumi.Input[Sequence[pulumi.Input['SystemctlCommand']]],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 directory: pulumi.Input[str],
-                 parents: Optional[pulumi.Input[bool]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None):
-        """
-        The set of arguments for constructing a Mkdir resource.
-        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details for the remote system.
-        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
-        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
-        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
+                 service_name: Optional[pulumi.Input[str]] = None):
         """
+        The set of arguments for constructing a Systemctl resource.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system.
+        """
+        pulumi.set(__self__, "commands", commands)
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "directory", directory)
-        if parents is not None:
-            pulumi.set(__self__, "parents", parents)
-        if remove_on_delete is not None:
-            pulumi.set(__self__, "remove_on_delete", remove_on_delete)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
+        if lifecycle is not None:
+            pulumi.set(__self__, "lifecycle", lifecycle)
+        if service_name is not None:
+            pulumi.set(__self__, "service_name", service_name)
+
+    @property
+    @pulumi.getter
+    def commands(self) -> pulumi.Input[Sequence[pulumi.Input['SystemctlCommand']]]:
+        return pulumi.get(self, "commands")
+
+    @commands.setter
+    def commands(self, value: pulumi.Input[Sequence[pulumi.Input['SystemctlCommand']]]):
+        pulumi.set(self, "commands", value)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
-        The connection details for the remote system.
+        Connection details for the remote system.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Input[str]:
-        """
-        The fully qualified path of the directory on the remote system.
-        """
-        return pulumi.get(self, "directory")
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "environment")
 
-    @directory.setter
-    def directory(self, value: pulumi.Input[str]):
-        pulumi.set(self, "directory", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
-    def parents(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the `--parents` option.
-        """
-        return pulumi.get(self, "parents")
+    def lifecycle(self) -> Optional['CommandLifecycle']:
+        return pulumi.get(self, "lifecycle")
 
-    @parents.setter
-    def parents(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "parents", value)
+    @lifecycle.setter
+    def lifecycle(self, value: Optional['CommandLifecycle']):
+        pulumi.set(self, "lifecycle", value)
 
     @property
-    @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Remove the created directory when the `Mkdir` resource is deleted or updated.
-        """
-        return pulumi.get(self, "remove_on_delete")
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "service_name")
 
-    @remove_on_delete.setter
-    def remove_on_delete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "remove_on_delete", value)
+    @service_name.setter
+    def service_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "service_name", value)
 
 
-class Mkdir(pulumi.ComponentResource):
+class Systemctl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 commands: Optional[pulumi.Input[Sequence[pulumi.Input['SystemctlCommand']]]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 parents: Optional[pulumi.Input[bool]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Represents the `mkdir` utility.
+        Abstraction over the `systemctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details for the remote system.
-        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
-        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
-        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
+        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MkdirArgs,
+                 args: SystemctlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Represents the `mkdir` utility.
+        Abstraction over the `systemctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MkdirArgs args: The arguments to use to populate this resource's properties.
+        :param SystemctlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MkdirArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SystemctlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 commands: Optional[pulumi.Input[Sequence[pulumi.Input['SystemctlCommand']]]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 parents: Optional[pulumi.Input[bool]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
+                 service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MkdirArgs.__new__(MkdirArgs)
+            __props__ = SystemctlArgs.__new__(SystemctlArgs)
 
+            if commands is None and not opts.urn:
+                raise TypeError("Missing required property 'commands'")
+            __props__.__dict__["commands"] = commands
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if directory is None and not opts.urn:
-                raise TypeError("Missing required property 'directory'")
-            __props__.__dict__["directory"] = directory
-            __props__.__dict__["parents"] = parents
-            __props__.__dict__["remove_on_delete"] = remove_on_delete
+            __props__.__dict__["environment"] = environment
+            __props__.__dict__["lifecycle"] = lifecycle
+            __props__.__dict__["service_name"] = service_name
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
+            __props__.__dict__["stdin"] = None
             __props__.__dict__["stdout"] = None
-        super(Mkdir, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mkdir',
+        super(Systemctl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Systemctl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
     def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
         """
-        The remote command.
+        Represents the command run on the remote system.
         """
         return pulumi.get(self, "command")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[str]:
-        """
-        The fully qualified path of the directory on the remote system.
-        """
-        return pulumi.get(self, "directory")
+    def commands(self) -> pulumi.Output[Sequence['SystemctlCommand']]:
+        return pulumi.get(self, "commands")
 
     @property
     @pulumi.getter
-    def parents(self) -> pulumi.Output[bool]:
+    def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
-        Corresponds to the `--parents` option.
+        Connection details for the remote system.
         """
-        return pulumi.get(self, "parents")
+        return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> pulumi.Output[bool]:
-        """
-        Remove the created directory when the `Mkdir` resource is deleted or updated.
-        """
-        return pulumi.get(self, "remove_on_delete")
+    @pulumi.getter(name="serviceName")
+    def service_name(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
-        """
-        The command's stderr.
-        """
         return pulumi.get(self, "stderr")
 
     @property
     @pulumi.getter
+    def stdin(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "stdin")
+
+    @property
+    @pulumi.getter
     def stdout(self) -> pulumi.Output[str]:
-        """
-        The command's stdout.
-        """
         return pulumi.get(self, "stdout")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,271 +4,242 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from ._enums import *
 import pulumi_command
 
-__all__ = ['MktempArgs', 'Mktemp']
+__all__ = ['MkdirArgs', 'Mkdir']
 
 @pulumi.input_type
-class MktempArgs:
+class MkdirArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 directory: Optional[pulumi.Input[bool]] = None,
-                 dry_run: Optional[pulumi.Input[bool]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
-                 suffix: Optional[pulumi.Input[str]] = None,
-                 template: Optional[pulumi.Input[str]] = None,
-                 tmpdir: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a Mktemp resource.
-        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system.
-        :param pulumi.Input[bool] directory: Corresponds to the --directory option.
-        :param pulumi.Input[bool] dry_run: Corresponds to the --dry-run option.
-        :param pulumi.Input[bool] quiet: Corresponds to the --quiet option.
-        :param pulumi.Input[str] suffix: Corresponds to the --suffix option.
-        :param pulumi.Input[str] template: Corresponds to the [TEMPLATE] arg.
-        :param pulumi.Input[str] tmpdir: Corresponds to the --tmpdir option.
+                 directory: pulumi.Input[str],
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
+                 parents: Optional[pulumi.Input[bool]] = None,
+                 remove_on_delete: Optional[pulumi.Input[bool]] = None):
+        """
+        The set of arguments for constructing a Mkdir resource.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details for the remote system.
+        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
+        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run.
+        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
+        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
         """
         pulumi.set(__self__, "connection", connection)
-        if directory is not None:
-            pulumi.set(__self__, "directory", directory)
-        if dry_run is not None:
-            pulumi.set(__self__, "dry_run", dry_run)
-        if quiet is not None:
-            pulumi.set(__self__, "quiet", quiet)
-        if suffix is not None:
-            pulumi.set(__self__, "suffix", suffix)
-        if template is not None:
-            pulumi.set(__self__, "template", template)
-        if tmpdir is not None:
-            pulumi.set(__self__, "tmpdir", tmpdir)
+        pulumi.set(__self__, "directory", directory)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
+        if lifecycle is not None:
+            pulumi.set(__self__, "lifecycle", lifecycle)
+        if parents is not None:
+            pulumi.set(__self__, "parents", parents)
+        if remove_on_delete is not None:
+            pulumi.set(__self__, "remove_on_delete", remove_on_delete)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
-        Connection details for the remote system.
+        The connection details for the remote system.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def directory(self) -> Optional[pulumi.Input[bool]]:
+    def directory(self) -> pulumi.Input[str]:
         """
-        Corresponds to the --directory option.
+        The fully qualified path of the directory on the remote system.
         """
         return pulumi.get(self, "directory")
 
     @directory.setter
-    def directory(self, value: Optional[pulumi.Input[bool]]):
+    def directory(self, value: pulumi.Input[str]):
         pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="dryRun")
-    def dry_run(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the --dry-run option.
-        """
-        return pulumi.get(self, "dry_run")
-
-    @dry_run.setter
-    def dry_run(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "dry_run", value)
-
-    @property
     @pulumi.getter
-    def quiet(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the --quiet option.
-        """
-        return pulumi.get(self, "quiet")
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "environment")
 
-    @quiet.setter
-    def quiet(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "quiet", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
-    def suffix(self) -> Optional[pulumi.Input[str]]:
+    def lifecycle(self) -> Optional['CommandLifecycle']:
         """
-        Corresponds to the --suffix option.
+        At what stage(s) in the resource lifecycle should the command be run.
         """
-        return pulumi.get(self, "suffix")
+        return pulumi.get(self, "lifecycle")
 
-    @suffix.setter
-    def suffix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "suffix", value)
+    @lifecycle.setter
+    def lifecycle(self, value: Optional['CommandLifecycle']):
+        pulumi.set(self, "lifecycle", value)
 
     @property
     @pulumi.getter
-    def template(self) -> Optional[pulumi.Input[str]]:
+    def parents(self) -> Optional[pulumi.Input[bool]]:
         """
-        Corresponds to the [TEMPLATE] arg.
+        Corresponds to the `--parents` option.
         """
-        return pulumi.get(self, "template")
+        return pulumi.get(self, "parents")
 
-    @template.setter
-    def template(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "template", value)
+    @parents.setter
+    def parents(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "parents", value)
 
     @property
-    @pulumi.getter
-    def tmpdir(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="removeOnDelete")
+    def remove_on_delete(self) -> Optional[pulumi.Input[bool]]:
         """
-        Corresponds to the --tmpdir option.
+        Remove the created directory when the `Mkdir` resource is deleted or updated.
         """
-        return pulumi.get(self, "tmpdir")
+        return pulumi.get(self, "remove_on_delete")
 
-    @tmpdir.setter
-    def tmpdir(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tmpdir", value)
+    @remove_on_delete.setter
+    def remove_on_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "remove_on_delete", value)
 
 
-class Mktemp(pulumi.ComponentResource):
+class Mkdir(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[bool]] = None,
-                 dry_run: Optional[pulumi.Input[bool]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
-                 suffix: Optional[pulumi.Input[str]] = None,
-                 template: Optional[pulumi.Input[str]] = None,
-                 tmpdir: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
+                 parents: Optional[pulumi.Input[bool]] = None,
+                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Abstracion over the `mktemp` utility on a remote system.
+        Represents the `mkdir` utility.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system.
-        :param pulumi.Input[bool] directory: Corresponds to the --directory option.
-        :param pulumi.Input[bool] dry_run: Corresponds to the --dry-run option.
-        :param pulumi.Input[bool] quiet: Corresponds to the --quiet option.
-        :param pulumi.Input[str] suffix: Corresponds to the --suffix option.
-        :param pulumi.Input[str] template: Corresponds to the [TEMPLATE] arg.
-        :param pulumi.Input[str] tmpdir: Corresponds to the --tmpdir option.
+        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details for the remote system.
+        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
+        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run.
+        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
+        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MktempArgs,
+                 args: MkdirArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstracion over the `mktemp` utility on a remote system.
+        Represents the `mkdir` utility.
 
         :param str resource_name: The name of the resource.
-        :param MktempArgs args: The arguments to use to populate this resource's properties.
+        :param MkdirArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MktempArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MkdirArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[bool]] = None,
-                 dry_run: Optional[pulumi.Input[bool]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
-                 suffix: Optional[pulumi.Input[str]] = None,
-                 template: Optional[pulumi.Input[str]] = None,
-                 tmpdir: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
+                 parents: Optional[pulumi.Input[bool]] = None,
+                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MktempArgs.__new__(MktempArgs)
+            __props__ = MkdirArgs.__new__(MkdirArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
+            if directory is None and not opts.urn:
+                raise TypeError("Missing required property 'directory'")
             __props__.__dict__["directory"] = directory
-            __props__.__dict__["dry_run"] = dry_run
-            __props__.__dict__["quiet"] = quiet
-            __props__.__dict__["suffix"] = suffix
-            __props__.__dict__["template"] = template
-            __props__.__dict__["tmpdir"] = tmpdir
+            __props__.__dict__["environment"] = environment
+            __props__.__dict__["lifecycle"] = lifecycle
+            __props__.__dict__["parents"] = parents
+            __props__.__dict__["remove_on_delete"] = remove_on_delete
             __props__.__dict__["command"] = None
-        super(Mktemp, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mktemp',
+            __props__.__dict__["stderr"] = None
+            __props__.__dict__["stdout"] = None
+        super(Mkdir, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mkdir',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
     def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
         """
-        Represents the remote `tar` operation.
+        The remote command.
         """
         return pulumi.get(self, "command")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[bool]:
+    def directory(self) -> pulumi.Output[str]:
         """
-        Corresponds to the --directory option.
+        The fully qualified path of the directory on the remote system.
         """
         return pulumi.get(self, "directory")
 
     @property
-    @pulumi.getter(name="dryRun")
-    def dry_run(self) -> pulumi.Output[bool]:
-        """
-        Corresponds to the --dry-run option.
-        """
-        return pulumi.get(self, "dry_run")
-
-    @property
     @pulumi.getter
-    def quiet(self) -> pulumi.Output[bool]:
+    def parents(self) -> pulumi.Output[bool]:
         """
-        Corresponds to the --quiet option.
+        Corresponds to the `--parents` option.
         """
-        return pulumi.get(self, "quiet")
+        return pulumi.get(self, "parents")
 
     @property
-    @pulumi.getter
-    def suffix(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="removeOnDelete")
+    def remove_on_delete(self) -> pulumi.Output[bool]:
         """
-        Corresponds to the --suffix option.
+        Remove the created directory when the `Mkdir` resource is deleted or updated.
         """
-        return pulumi.get(self, "suffix")
+        return pulumi.get(self, "remove_on_delete")
 
     @property
     @pulumi.getter
-    def template(self) -> pulumi.Output[Optional[str]]:
+    def stderr(self) -> pulumi.Output[str]:
         """
-        Corresponds to the [TEMPLATE] arg.
+        The command's stderr.
         """
-        return pulumi.get(self, "template")
+        return pulumi.get(self, "stderr")
 
     @property
     @pulumi.getter
-    def tmpdir(self) -> pulumi.Output[Optional[str]]:
+    def stdout(self) -> pulumi.Output[str]:
         """
-        Corresponds to the --tmpdir option.
+        The command's stdout.
         """
-        return pulumi.get(self, "tmpdir")
+        return pulumi.get(self, "stdout")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from ._enums import *
 import pulumi_command
 
 __all__ = ['MvArgs', 'Mv']
 
 @pulumi.input_type
 class MvArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  source: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]],
                  backup: Optional[bool] = None,
                  context: Optional[pulumi.Input[bool]] = None,
                  control: Optional[pulumi.Input[str]] = None,
                  dest: Optional[pulumi.Input[str]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
                  no_clobber: Optional[pulumi.Input[bool]] = None,
                  no_target_directory: Optional[pulumi.Input[bool]] = None,
                  strip_trailing_slashes: Optional[pulumi.Input[bool]] = None,
                  suffix: Optional[pulumi.Input[str]] = None,
                  target_directory: Optional[pulumi.Input[str]] = None,
                  update: Optional[pulumi.Input[bool]] = None,
@@ -56,14 +58,16 @@
             pulumi.set(__self__, "context", context)
         if control is not None:
             pulumi.set(__self__, "control", control)
         if dest is not None:
             pulumi.set(__self__, "dest", dest)
         if directory is not None:
             pulumi.set(__self__, "directory", directory)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
         if force is not None:
             pulumi.set(__self__, "force", force)
         if no_clobber is not None:
             pulumi.set(__self__, "no_clobber", no_clobber)
         if no_target_directory is not None:
             pulumi.set(__self__, "no_target_directory", no_target_directory)
         if strip_trailing_slashes is not None:
@@ -159,14 +163,23 @@
 
     @directory.setter
     def directory(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "directory", value)
 
     @property
     @pulumi.getter
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "environment")
+
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
+
+    @property
+    @pulumi.getter
     def force(self) -> Optional[pulumi.Input[bool]]:
         """
         Corresponds to the --force option.
         """
         return pulumi.get(self, "force")
 
     @force.setter
@@ -265,14 +278,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  backup: Optional[bool] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  context: Optional[pulumi.Input[bool]] = None,
                  control: Optional[pulumi.Input[str]] = None,
                  dest: Optional[pulumi.Input[str]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
                  no_clobber: Optional[pulumi.Input[bool]] = None,
                  no_target_directory: Optional[pulumi.Input[bool]] = None,
                  source: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
                  strip_trailing_slashes: Optional[pulumi.Input[bool]] = None,
                  suffix: Optional[pulumi.Input[str]] = None,
                  target_directory: Optional[pulumi.Input[str]] = None,
@@ -326,14 +340,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  backup: Optional[bool] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  context: Optional[pulumi.Input[bool]] = None,
                  control: Optional[pulumi.Input[str]] = None,
                  dest: Optional[pulumi.Input[str]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
                  no_clobber: Optional[pulumi.Input[bool]] = None,
                  no_target_directory: Optional[pulumi.Input[bool]] = None,
                  source: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
                  strip_trailing_slashes: Optional[pulumi.Input[bool]] = None,
                  suffix: Optional[pulumi.Input[str]] = None,
                  target_directory: Optional[pulumi.Input[str]] = None,
@@ -354,26 +369,28 @@
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["context"] = context
             __props__.__dict__["control"] = control
             __props__.__dict__["dest"] = dest
             __props__.__dict__["directory"] = directory
+            __props__.__dict__["environment"] = environment
             __props__.__dict__["force"] = force
             __props__.__dict__["no_clobber"] = no_clobber
             __props__.__dict__["no_target_directory"] = no_target_directory
             if source is None and not opts.urn:
                 raise TypeError("Missing required property 'source'")
             __props__.__dict__["source"] = source
             __props__.__dict__["strip_trailing_slashes"] = strip_trailing_slashes
             __props__.__dict__["suffix"] = suffix
             __props__.__dict__["target_directory"] = target_directory
             __props__.__dict__["update"] = update
             __props__.__dict__["verbose"] = verbose
             __props__.__dict__["command"] = None
+            __props__.__dict__["lifecycle"] = None
         super(Mv, __self__).__init__(
             'kubernetes-the-hard-way:tools:Mv',
             resource_name,
             __props__,
             opts,
             remote=True)
 
@@ -430,14 +447,22 @@
     def force(self) -> pulumi.Output[bool]:
         """
         Corresponds to the --force option.
         """
         return pulumi.get(self, "force")
 
     @property
+    @pulumi.getter
+    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
+        """
+        At what stage(s) in the resource lifecycle should the command be run.
+        """
+        return pulumi.get(self, "lifecycle")
+
+    @property
     @pulumi.getter(name="noClobber")
     def no_clobber(self) -> pulumi.Output[bool]:
         """
         Corresponds to the --no-clobber option.
         """
         return pulumi.get(self, "no_clobber")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,44 +4,52 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from ._enums import *
 import pulumi_command
 
 __all__ = ['RmArgs', 'Rm']
 
 @pulumi.input_type
 class RmArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  files: pulumi.Input[Union[Sequence[pulumi.Input[str]], str]],
                  dir: Optional[pulumi.Input[bool]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
                  on_delete: Optional[bool] = None,
                  recursive: Optional[pulumi.Input[bool]] = None,
                  verbose: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Rm resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system.
         :param pulumi.Input[Union[Sequence[pulumi.Input[str]], str]] files: Corresponds to the [FILE] argument.
         :param pulumi.Input[bool] dir: Corresponds to the --dir option.
         :param pulumi.Input[bool] force: Corresponds to the --force option.
+        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run.
         :param bool on_delete: Whether rm should be run when the resource is created or deleted.
         :param pulumi.Input[bool] recursive: Corresponds to the --recursive option.
         :param pulumi.Input[bool] verbose: Corresponds to the --verbose option.
         """
         pulumi.set(__self__, "connection", connection)
         pulumi.set(__self__, "files", files)
         if dir is not None:
             pulumi.set(__self__, "dir", dir)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
         if force is not None:
             pulumi.set(__self__, "force", force)
+        if lifecycle is not None:
+            pulumi.set(__self__, "lifecycle", lifecycle)
         if on_delete is not None:
             pulumi.set(__self__, "on_delete", on_delete)
         if recursive is not None:
             pulumi.set(__self__, "recursive", recursive)
         if verbose is not None:
             pulumi.set(__self__, "verbose", verbose)
 
@@ -79,25 +87,46 @@
 
     @dir.setter
     def dir(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dir", value)
 
     @property
     @pulumi.getter
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "environment")
+
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
+
+    @property
+    @pulumi.getter
     def force(self) -> Optional[pulumi.Input[bool]]:
         """
         Corresponds to the --force option.
         """
         return pulumi.get(self, "force")
 
     @force.setter
     def force(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force", value)
 
     @property
+    @pulumi.getter
+    def lifecycle(self) -> Optional['CommandLifecycle']:
+        """
+        At what stage(s) in the resource lifecycle should the command be run.
+        """
+        return pulumi.get(self, "lifecycle")
+
+    @lifecycle.setter
+    def lifecycle(self, value: Optional['CommandLifecycle']):
+        pulumi.set(self, "lifecycle", value)
+
+    @property
     @pulumi.getter(name="onDelete")
     def on_delete(self) -> Optional[bool]:
         """
         Whether rm should be run when the resource is created or deleted.
         """
         return pulumi.get(self, "on_delete")
 
@@ -133,29 +162,32 @@
 class Rm(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  dir: Optional[pulumi.Input[bool]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
                  on_delete: Optional[bool] = None,
                  recursive: Optional[pulumi.Input[bool]] = None,
                  verbose: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system.
         :param pulumi.Input[bool] dir: Corresponds to the --dir option.
         :param pulumi.Input[Union[Sequence[pulumi.Input[str]], str]] files: Corresponds to the [FILE] argument.
         :param pulumi.Input[bool] force: Corresponds to the --force option.
+        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run.
         :param bool on_delete: Whether rm should be run when the resource is created or deleted.
         :param pulumi.Input[bool] recursive: Corresponds to the --recursive option.
         :param pulumi.Input[bool] verbose: Corresponds to the --verbose option.
         """
         ...
     @overload
     def __init__(__self__,
@@ -178,16 +210,18 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  dir: Optional[pulumi.Input[bool]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
+                 lifecycle: Optional['CommandLifecycle'] = None,
                  on_delete: Optional[bool] = None,
                  recursive: Optional[pulumi.Input[bool]] = None,
                  verbose: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -198,18 +232,20 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RmArgs.__new__(RmArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["dir"] = dir
+            __props__.__dict__["environment"] = environment
             if files is None and not opts.urn:
                 raise TypeError("Missing required property 'files'")
             __props__.__dict__["files"] = files
             __props__.__dict__["force"] = force
+            __props__.__dict__["lifecycle"] = lifecycle
             __props__.__dict__["on_delete"] = on_delete
             __props__.__dict__["recursive"] = recursive
             __props__.__dict__["verbose"] = verbose
             __props__.__dict__["command"] = None
         super(Rm, __self__).__init__(
             'kubernetes-the-hard-way:tools:Rm',
             resource_name,
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 @pulumi.input_type
 class TarArgs:
     def __init__(__self__, *,
                  archive: pulumi.Input[str],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  extract: Optional[pulumi.Input[bool]] = None,
                  files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
                  gzip: Optional[pulumi.Input[bool]] = None,
                  strip_components: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a Tar resource.
         :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
@@ -32,14 +33,16 @@
         :param pulumi.Input[bool] gzip: Corresponds to the --gzip option.
         :param pulumi.Input[int] strip_components: Corresponds to the --strip-components option.
         """
         pulumi.set(__self__, "archive", archive)
         pulumi.set(__self__, "connection", connection)
         if directory is not None:
             pulumi.set(__self__, "directory", directory)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
         if extract is not None:
             pulumi.set(__self__, "extract", extract)
         if files is not None:
             pulumi.set(__self__, "files", files)
         if gzip is not None:
             pulumi.set(__self__, "gzip", gzip)
         if strip_components is not None:
@@ -79,14 +82,23 @@
 
     @directory.setter
     def directory(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "directory", value)
 
     @property
     @pulumi.getter
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "environment")
+
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
+
+    @property
+    @pulumi.getter
     def extract(self) -> Optional[pulumi.Input[bool]]:
         """
         Corresponds to the --extract option.
         """
         return pulumi.get(self, "extract")
 
     @extract.setter
@@ -134,14 +146,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  archive: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  extract: Optional[pulumi.Input[bool]] = None,
                  files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
                  gzip: Optional[pulumi.Input[bool]] = None,
                  strip_components: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Abstracion over the `tar` utility on a remote system.
@@ -179,14 +192,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  archive: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  directory: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  extract: Optional[pulumi.Input[bool]] = None,
                  files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
                  gzip: Optional[pulumi.Input[bool]] = None,
                  strip_components: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -201,14 +215,15 @@
             if archive is None and not opts.urn:
                 raise TypeError("Missing required property 'archive'")
             __props__.__dict__["archive"] = archive
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["directory"] = directory
+            __props__.__dict__["environment"] = environment
             __props__.__dict__["extract"] = extract
             __props__.__dict__["files"] = files
             __props__.__dict__["gzip"] = gzip
             __props__.__dict__["strip_components"] = strip_components
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdin"] = None
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 @pulumi.input_type
 class WgetArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  url: pulumi.Input[str],
                  directory_prefix: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  https_only: Optional[pulumi.Input[bool]] = None,
                  no_verbose: Optional[pulumi.Input[bool]] = None,
                  output_document: Optional[pulumi.Input[str]] = None,
                  quiet: Optional[pulumi.Input[bool]] = None,
                  timestamping: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Wget resource.
@@ -34,14 +35,16 @@
         :param pulumi.Input[bool] quiet: Corresponds to the --quiet option.
         :param pulumi.Input[bool] timestamping: Corresponds to the --timestamping option.
         """
         pulumi.set(__self__, "connection", connection)
         pulumi.set(__self__, "url", url)
         if directory_prefix is not None:
             pulumi.set(__self__, "directory_prefix", directory_prefix)
+        if environment is not None:
+            pulumi.set(__self__, "environment", environment)
         if https_only is not None:
             pulumi.set(__self__, "https_only", https_only)
         if no_verbose is not None:
             pulumi.set(__self__, "no_verbose", no_verbose)
         if output_document is not None:
             pulumi.set(__self__, "output_document", output_document)
         if quiet is not None:
@@ -82,14 +85,23 @@
         return pulumi.get(self, "directory_prefix")
 
     @directory_prefix.setter
     def directory_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "directory_prefix", value)
 
     @property
+    @pulumi.getter
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        return pulumi.get(self, "environment")
+
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
+
+    @property
     @pulumi.getter(name="httpsOnly")
     def https_only(self) -> Optional[pulumi.Input[bool]]:
         """
         Corresponds to the --https-only option.
         """
         return pulumi.get(self, "https_only")
 
@@ -149,14 +161,15 @@
 class Wget(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  directory_prefix: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  https_only: Optional[pulumi.Input[bool]] = None,
                  no_verbose: Optional[pulumi.Input[bool]] = None,
                  output_document: Optional[pulumi.Input[str]] = None,
                  quiet: Optional[pulumi.Input[bool]] = None,
                  timestamping: Optional[pulumi.Input[bool]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -196,14 +209,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  directory_prefix: Optional[pulumi.Input[str]] = None,
+                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  https_only: Optional[pulumi.Input[bool]] = None,
                  no_verbose: Optional[pulumi.Input[bool]] = None,
                  output_document: Optional[pulumi.Input[str]] = None,
                  quiet: Optional[pulumi.Input[bool]] = None,
                  timestamping: Optional[pulumi.Input[bool]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -217,14 +231,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = WgetArgs.__new__(WgetArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["directory_prefix"] = directory_prefix
+            __props__.__dict__["environment"] = environment
             __props__.__dict__["https_only"] = https_only
             __props__.__dict__["no_verbose"] = no_verbose
             __props__.__dict__["output_document"] = output_document
             __props__.__dict__["quiet"] = quiet
             __props__.__dict__["timestamping"] = timestamping
             if url is None and not opts.urn:
                 raise TypeError("Missing required property 'url'")
@@ -253,14 +268,19 @@
     def directory_prefix(self) -> pulumi.Output[Optional[str]]:
         """
         Corresponds to the --directory-prefix option.
         """
         return pulumi.get(self, "directory_prefix")
 
     @property
+    @pulumi.getter
+    def environment(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
+        return pulumi.get(self, "environment")
+
+    @property
     @pulumi.getter(name="httpsOnly")
     def https_only(self) -> pulumi.Output[bool]:
         """
         Corresponds to the --https-only option.
         """
         return pulumi.get(self, "https_only")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1712361443
+Version: 0.0.11a1712362554
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,30 @@
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/download.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/file.py
+pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
 pulumi_kubernetes_the_hard_way/tls/encryption_key.py
 pulumi_kubernetes_the_hard_way/tls/root_ca.py
 pulumi_kubernetes_the_hard_way/tools/__init__.py
+pulumi_kubernetes_the_hard_way/tools/_enums.py
+pulumi_kubernetes_the_hard_way/tools/etcdctl.py
 pulumi_kubernetes_the_hard_way/tools/mkdir.py
 pulumi_kubernetes_the_hard_way/tools/mktemp.py
 pulumi_kubernetes_the_hard_way/tools/mv.py
 pulumi_kubernetes_the_hard_way/tools/rm.py
+pulumi_kubernetes_the_hard_way/tools/systemctl.py
 pulumi_kubernetes_the_hard_way/tools/tar.py
+pulumi_kubernetes_the_hard_way/tools/tee.py
 pulumi_kubernetes_the_hard_way/tools/wget.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712361443/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.11a1712362554/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-command>=0.9.0,<1.0.0", "pulumi-random>=4.0.0,<5.0.0", "pulumi-tls>=5.0.0,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.11a1712361443"
+  version = "0.0.11a1712362554"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

