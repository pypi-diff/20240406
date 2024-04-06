# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1712367286.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1712430472.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1712367286.tar", last modified: Sat Apr  6 01:36:43 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1712430472.tar", last modified: Sat Apr  6 19:10:12 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286.tar` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.598878 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-06 01:36:43.598878 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.590879 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     2778 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.594879 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      318 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      463 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)     4567 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     2843 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.594879 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      545 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)      952 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    10044 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8177 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    22322 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)     6927 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     8028 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     8232 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     8016 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9732 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    12168 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.598878 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      403 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)      942 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1401 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    18785 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    14904 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4166 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)    15417 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.598878 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      458 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)      752 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)     9202 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)     9983 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    13042 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    20833 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    12292 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)     8325 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    12221 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14109 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    13586 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:36:43.598878 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-06 01:36:43.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-06 01:36:43.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:36:43.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 01:36:43.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 01:36:43.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      860 2024-04-06 01:36:37.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 01:36:43.598878 pulumi_kubernetes_the_hard_way-0.0.11a1712367286/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.295215 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-06 19:10:12.295215 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.287215 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     3352 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.287215 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      318 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      463 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     4567 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     2843 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.291216 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      802 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      952 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    10044 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    12657 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)     9219 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)     9163 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8177 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    14444 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10810 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)     6927 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     8399 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     8747 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     8844 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9147 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     8814 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8814 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)     9732 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     8772 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)    12168 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.291216 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      403 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      942 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1401 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    18785 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    14904 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4166 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)    15417 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.291216 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      458 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      752 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     9202 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)     9983 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    13042 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    20833 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    12292 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)     8325 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    12221 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14109 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    13586 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:10:12.295215 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-06 19:10:12.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-06 19:10:12.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:10:12.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-06 19:10:12.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 19:10:12.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      860 2024-04-06 19:09:58.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:10:12.295215 pulumi_kubernetes_the_hard_way-0.0.11a1712430472/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1712367286
+Version: 0.0.11a1712430472
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/README.md` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,20 +27,28 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
+   "kubernetes-the-hard-way:remote:CniPluginsInstall": "CniPluginsInstall",
+   "kubernetes-the-hard-way:remote:ContainerdInstall": "ContainerdInstall",
+   "kubernetes-the-hard-way:remote:CrictlInstall": "CrictlInstall",
    "kubernetes-the-hard-way:remote:Download": "Download",
+   "kubernetes-the-hard-way:remote:EtcdConfiguration": "EtcdConfiguration",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:File": "File",
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
+   "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
    "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
+   "kubernetes-the-hard-way:remote:KubectlInstall": "KubectlInstall",
+   "kubernetes-the-hard-way:remote:KubeletInstall": "KubeletInstall",
+   "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tls",
   "fqn": "pulumi_kubernetes_the_hard_way.tls",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 # *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
 from ._enums import *
+from .cni_plugins_install import *
+from .containerd_install import *
+from .crictl_install import *
 from .download import *
+from .etcd_configuration import *
 from .etcd_install import *
 from .file import *
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
+from .kube_proxy_install import *
 from .kube_scheduler_install import *
+from .kubectl_install import *
+from .kubelet_install import *
+from .runc_install import *
 from .systemd_service import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,79 +5,61 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import tools as _tools
-from ._enums import *
-from .download import Download
 from .file import File
 from .systemd_service import SystemdService
 import pulumi_command
 
-__all__ = ['EtcdInstallArgs', 'EtcdInstall']
+__all__ = ['EtcdConfigurationArgs', 'EtcdConfiguration']
 
 @pulumi.input_type
-class EtcdInstallArgs:
+class EtcdConfigurationArgs:
     def __init__(__self__, *,
                  ca_pem: pulumi.Input[str],
                  cert_pem: pulumi.Input[str],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
+                 etcd_path: pulumi.Input[str],
                  internal_ip: pulumi.Input[str],
                  key_pem: pulumi.Input[str],
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 download_directory: Optional[pulumi.Input[str]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
-                 systemd_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
+                 systemd_directory: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a EtcdInstall resource.
+        The set of arguments for constructing a EtcdConfiguration resource.
         :param pulumi.Input[str] ca_pem: The PEM encoded CA data.
         :param pulumi.Input[str] cert_pem: The PEM encoded certificate data.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details.
         :param pulumi.Input[str] internal_ip: IP used to serve client requests and communicate with etcd peers.
         :param pulumi.Input[str] key_pem: The PEM encoded key data.
-        :param pulumi.Input['Architecture'] architecture: The etcd CPU architecture.
         :param pulumi.Input[str] configuration_directory: The directory to store etcd configuration.
         :param pulumi.Input[str] data_directory: The directory etcd will use.
-        :param pulumi.Input[str] download_directory: Temporary directory to download files to. Defaults to `/tmp/<random string>`.
-        :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
         :param pulumi.Input[str] systemd_directory: The systemd service file dirctory.
-        :param pulumi.Input[str] version: The version of etcd to install.
         """
         pulumi.set(__self__, "ca_pem", ca_pem)
         pulumi.set(__self__, "cert_pem", cert_pem)
         pulumi.set(__self__, "connection", connection)
+        pulumi.set(__self__, "etcd_path", etcd_path)
         pulumi.set(__self__, "internal_ip", internal_ip)
         pulumi.set(__self__, "key_pem", key_pem)
-        if architecture is not None:
-            pulumi.set(__self__, "architecture", architecture)
         if configuration_directory is None:
             configuration_directory = '/etc/etcd'
         if configuration_directory is not None:
             pulumi.set(__self__, "configuration_directory", configuration_directory)
         if data_directory is None:
             data_directory = '/var/lib/etcd'
         if data_directory is not None:
             pulumi.set(__self__, "data_directory", data_directory)
-        if download_directory is not None:
-            pulumi.set(__self__, "download_directory", download_directory)
-        if install_directory is None:
-            install_directory = '/usr/local/bin'
-        if install_directory is not None:
-            pulumi.set(__self__, "install_directory", install_directory)
         if systemd_directory is None:
             systemd_directory = '/etc/system/systemd'
         if systemd_directory is not None:
             pulumi.set(__self__, "systemd_directory", systemd_directory)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="caPem")
     def ca_pem(self) -> pulumi.Input[str]:
         """
         The PEM encoded CA data.
         """
@@ -108,14 +90,23 @@
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
+    @pulumi.getter(name="etcdPath")
+    def etcd_path(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "etcd_path")
+
+    @etcd_path.setter
+    def etcd_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "etcd_path", value)
+
+    @property
     @pulumi.getter(name="internalIp")
     def internal_ip(self) -> pulumi.Input[str]:
         """
         IP used to serve client requests and communicate with etcd peers.
         """
         return pulumi.get(self, "internal_ip")
 
@@ -132,26 +123,14 @@
         return pulumi.get(self, "key_pem")
 
     @key_pem.setter
     def key_pem(self, value: pulumi.Input[str]):
         pulumi.set(self, "key_pem", value)
 
     @property
-    @pulumi.getter
-    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
-        """
-        The etcd CPU architecture.
-        """
-        return pulumi.get(self, "architecture")
-
-    @architecture.setter
-    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
-        pulumi.set(self, "architecture", value)
-
-    @property
     @pulumi.getter(name="configurationDirectory")
     def configuration_directory(self) -> Optional[pulumi.Input[str]]:
         """
         The directory to store etcd configuration.
         """
         return pulumi.get(self, "configuration_directory")
 
@@ -168,146 +147,97 @@
         return pulumi.get(self, "data_directory")
 
     @data_directory.setter
     def data_directory(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "data_directory", value)
 
     @property
-    @pulumi.getter(name="downloadDirectory")
-    def download_directory(self) -> Optional[pulumi.Input[str]]:
-        """
-        Temporary directory to download files to. Defaults to `/tmp/<random string>`.
-        """
-        return pulumi.get(self, "download_directory")
-
-    @download_directory.setter
-    def download_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "download_directory", value)
-
-    @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> Optional[pulumi.Input[str]]:
-        """
-        Directory to install the `etcd` and `etcdctl` binaries.
-        """
-        return pulumi.get(self, "install_directory")
-
-    @install_directory.setter
-    def install_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "install_directory", value)
-
-    @property
     @pulumi.getter(name="systemdDirectory")
     def systemd_directory(self) -> Optional[pulumi.Input[str]]:
         """
         The systemd service file dirctory.
         """
         return pulumi.get(self, "systemd_directory")
 
     @systemd_directory.setter
     def systemd_directory(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "systemd_directory", value)
 
-    @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
-        """
-        The version of etcd to install.
-        """
-        return pulumi.get(self, "version")
-
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
 
-
-class EtcdInstall(pulumi.ComponentResource):
+class EtcdConfiguration(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
                  ca_pem: Optional[pulumi.Input[str]] = None,
                  cert_pem: Optional[pulumi.Input[str]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 download_directory: Optional[pulumi.Input[str]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 etcd_path: Optional[pulumi.Input[str]] = None,
                  internal_ip: Optional[pulumi.Input[str]] = None,
                  key_pem: Optional[pulumi.Input[str]] = None,
                  systemd_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Represents an etcd binary on a remote system.
-
+        Create a EtcdConfiguration resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['Architecture'] architecture: The etcd CPU architecture.
         :param pulumi.Input[str] ca_pem: The PEM encoded CA data.
         :param pulumi.Input[str] cert_pem: The PEM encoded certificate data.
         :param pulumi.Input[str] configuration_directory: The directory to store etcd configuration.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details.
         :param pulumi.Input[str] data_directory: The directory etcd will use.
-        :param pulumi.Input[str] download_directory: Temporary directory to download files to. Defaults to `/tmp/<random string>`.
-        :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
         :param pulumi.Input[str] internal_ip: IP used to serve client requests and communicate with etcd peers.
         :param pulumi.Input[str] key_pem: The PEM encoded key data.
         :param pulumi.Input[str] systemd_directory: The systemd service file dirctory.
-        :param pulumi.Input[str] version: The version of etcd to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EtcdInstallArgs,
+                 args: EtcdConfigurationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Represents an etcd binary on a remote system.
-
+        Create a EtcdConfiguration resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param EtcdInstallArgs args: The arguments to use to populate this resource's properties.
+        :param EtcdConfigurationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EtcdInstallArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EtcdConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
                  ca_pem: Optional[pulumi.Input[str]] = None,
                  cert_pem: Optional[pulumi.Input[str]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 download_directory: Optional[pulumi.Input[str]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 etcd_path: Optional[pulumi.Input[str]] = None,
                  internal_ip: Optional[pulumi.Input[str]] = None,
                  key_pem: Optional[pulumi.Input[str]] = None,
                  systemd_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EtcdInstallArgs.__new__(EtcdInstallArgs)
+            __props__ = EtcdConfigurationArgs.__new__(EtcdConfigurationArgs)
 
-            __props__.__dict__["architecture"] = architecture
             if ca_pem is None and not opts.urn:
                 raise TypeError("Missing required property 'ca_pem'")
             __props__.__dict__["ca_pem"] = ca_pem
             if cert_pem is None and not opts.urn:
                 raise TypeError("Missing required property 'cert_pem'")
             __props__.__dict__["cert_pem"] = cert_pem
             if configuration_directory is None:
@@ -315,69 +245,40 @@
             __props__.__dict__["configuration_directory"] = configuration_directory
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             if data_directory is None:
                 data_directory = '/var/lib/etcd'
             __props__.__dict__["data_directory"] = data_directory
-            __props__.__dict__["download_directory"] = download_directory
-            if install_directory is None:
-                install_directory = '/usr/local/bin'
-            __props__.__dict__["install_directory"] = install_directory
+            if etcd_path is None and not opts.urn:
+                raise TypeError("Missing required property 'etcd_path'")
+            __props__.__dict__["etcd_path"] = etcd_path
             if internal_ip is None and not opts.urn:
                 raise TypeError("Missing required property 'internal_ip'")
             __props__.__dict__["internal_ip"] = internal_ip
             if key_pem is None and not opts.urn:
                 raise TypeError("Missing required property 'key_pem'")
             __props__.__dict__["key_pem"] = key_pem
             if systemd_directory is None:
                 systemd_directory = '/etc/system/systemd'
             __props__.__dict__["systemd_directory"] = systemd_directory
-            __props__.__dict__["version"] = version
-            __props__.__dict__["archive_name"] = None
             __props__.__dict__["ca_file"] = None
             __props__.__dict__["cert_file"] = None
             __props__.__dict__["configuration_mkdir"] = None
             __props__.__dict__["data_mkdir"] = None
-            __props__.__dict__["download"] = None
-            __props__.__dict__["download_mkdir"] = None
-            __props__.__dict__["etcd_path"] = None
-            __props__.__dict__["etcdctl_path"] = None
-            __props__.__dict__["install_mkdir"] = None
             __props__.__dict__["key_file"] = None
-            __props__.__dict__["mv_etcd"] = None
-            __props__.__dict__["mv_etcdctl"] = None
-            __props__.__dict__["name"] = None
             __props__.__dict__["systemd_service"] = None
-            __props__.__dict__["tar"] = None
-            __props__.__dict__["url"] = None
-        super(EtcdInstall, __self__).__init__(
-            'kubernetes-the-hard-way:remote:EtcdInstall',
+        super(EtcdConfiguration, __self__).__init__(
+            'kubernetes-the-hard-way:remote:EtcdConfiguration',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter
-    def architecture(self) -> pulumi.Output['Architecture']:
-        """
-        The etcd CPU architecture.
-        """
-        return pulumi.get(self, "architecture")
-
-    @property
-    @pulumi.getter(name="archiveName")
-    def archive_name(self) -> pulumi.Output[str]:
-        """
-        The name of the etcd release archive.
-        """
-        return pulumi.get(self, "archive_name")
-
-    @property
     @pulumi.getter(name="caFile")
     def ca_file(self) -> pulumi.Output[Optional['File']]:
         """
         The remote certificate authority file.
         """
         return pulumi.get(self, "ca_file")
 
@@ -418,70 +319,14 @@
     def data_mkdir(self) -> pulumi.Output['_tools.Mkdir']:
         """
         The command used to create the data directory.
         """
         return pulumi.get(self, "data_mkdir")
 
     @property
-    @pulumi.getter
-    def download(self) -> pulumi.Output['Download']:
-        """
-        The etcd download operation.
-        """
-        return pulumi.get(self, "download")
-
-    @property
-    @pulumi.getter(name="downloadDirectory")
-    def download_directory(self) -> pulumi.Output[str]:
-        """
-        The directory where the etcd binary was downloaded to.
-        """
-        return pulumi.get(self, "download_directory")
-
-    @property
-    @pulumi.getter(name="downloadMkdir")
-    def download_mkdir(self) -> pulumi.Output['_tools.Mkdir']:
-        """
-        The operation to create the download directory.
-        """
-        return pulumi.get(self, "download_mkdir")
-
-    @property
-    @pulumi.getter(name="etcdPath")
-    def etcd_path(self) -> pulumi.Output[str]:
-        """
-        The path to the etcd binary on the remote system.
-        """
-        return pulumi.get(self, "etcd_path")
-
-    @property
-    @pulumi.getter(name="etcdctlPath")
-    def etcdctl_path(self) -> pulumi.Output[str]:
-        """
-        The path to the etcdctl binary on the remote system.
-        """
-        return pulumi.get(self, "etcdctl_path")
-
-    @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> pulumi.Output[str]:
-        """
-        Directory to install the `etcd` and `etcdctl` binaries.
-        """
-        return pulumi.get(self, "install_directory")
-
-    @property
-    @pulumi.getter(name="installMkdir")
-    def install_mkdir(self) -> pulumi.Output['_tools.Mkdir']:
-        """
-        The operation to create the install directory.
-        """
-        return pulumi.get(self, "install_mkdir")
-
-    @property
     @pulumi.getter(name="internalIp")
     def internal_ip(self) -> pulumi.Output[str]:
         """
         IP used to serve client requests and communicate with etcd peers.
         """
         return pulumi.get(self, "internal_ip")
 
@@ -490,80 +335,14 @@
     def key_file(self) -> pulumi.Output[Optional['File']]:
         """
         The remote key file.
         """
         return pulumi.get(self, "key_file")
 
     @property
-    @pulumi.getter(name="mvEtcd")
-    def mv_etcd(self) -> pulumi.Output['_tools.Mv']:
-        """
-        The operation to move the etcd binary to the install directory.
-        """
-        return pulumi.get(self, "mv_etcd")
-
-    @property
-    @pulumi.getter(name="mvEtcdctl")
-    def mv_etcdctl(self) -> pulumi.Output['_tools.Mv']:
-        """
-        The operation to move the etcdctl binary to the install directory.
-        """
-        return pulumi.get(self, "mv_etcdctl")
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
-        """
-        The name of the resource.
-        """
-        return pulumi.get(self, "name")
-
-    @property
     @pulumi.getter(name="systemdService")
     def systemd_service(self) -> pulumi.Output['SystemdService']:
         """
         The remote systemd service.
         """
         return pulumi.get(self, "systemd_service")
 
-    @property
-    @pulumi.getter
-    def tar(self) -> pulumi.Output['_tools.Tar']:
-        """
-        The tar operation.
-        """
-        return pulumi.get(self, "tar")
-
-    @property
-    @pulumi.getter
-    def url(self) -> pulumi.Output[str]:
-        """
-        The url used to download etcd.
-        """
-        return pulumi.get(self, "url")
-
-    @property
-    @pulumi.getter
-    def version(self) -> pulumi.Output[str]:
-        """
-        The version of etcd downloaded.
-        """
-        return pulumi.get(self, "version")
-
-    @pulumi.output_type
-    class EtcdctlResult:
-        def __init__(__self__, result=None):
-            if result and not isinstance(result, _tools.Etcdctl):
-                raise TypeError("Expected argument 'result' to be a _tools.Etcdctl")
-            pulumi.set(__self__, "result", result)
-
-        @property
-        @pulumi.getter
-        def result(self) -> '_tools.Etcdctl':
-            return pulumi.get(self, "result")
-
-    def etcdctl(__self__) -> pulumi.Output['_tools.Etcdctl']:
-        __args__ = dict()
-        __args__['__self__'] = __self__
-        __result__ = pulumi.runtime.call('kubernetes-the-hard-way:remote:EtcdInstall/etcdctl', __args__, res=__self__, typ=EtcdInstall.EtcdctlResult)
-        return __result__.result
-
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from .. import tools as _tools
 from ._enums import *
 import pulumi_command
 
 __all__ = ['KubeApiServerInstallArgs', 'KubeApiServerInstall']
 
 @pulumi.input_type
 class KubeApiServerInstallArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  architecture: Optional[pulumi.Input['Architecture']] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a KubeApiServerInstall resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details.
         :param pulumi.Input['Architecture'] architecture: The kube-apiserver CPU architecture.
-        :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
+        :param pulumi.Input[str] directory: Directory to install the `etcd` and `etcdctl` binaries.
         :param pulumi.Input[str] version: The version of kube-apiserver to install.
         """
         pulumi.set(__self__, "connection", connection)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
-        if install_directory is None:
-            install_directory = '/usr/local/bin'
-        if install_directory is not None:
-            pulumi.set(__self__, "install_directory", install_directory)
+        if directory is None:
+            directory = '/usr/local/bin'
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
@@ -58,24 +59,24 @@
         return pulumi.get(self, "architecture")
 
     @architecture.setter
     def architecture(self, value: Optional[pulumi.Input['Architecture']]):
         pulumi.set(self, "architecture", value)
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
         Directory to install the `etcd` and `etcdctl` binaries.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
 
-    @install_directory.setter
-    def install_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "install_directory", value)
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
         The version of kube-apiserver to install.
         """
@@ -89,25 +90,25 @@
 class KubeApiServerInstall(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Installs kube-apiserver on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input['Architecture'] architecture: The kube-apiserver CPU architecture.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details.
-        :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
+        :param pulumi.Input[str] directory: Directory to install the `etcd` and `etcdctl` binaries.
         :param pulumi.Input[str] version: The version of kube-apiserver to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: KubeApiServerInstallArgs,
@@ -128,15 +129,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
@@ -145,18 +146,21 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KubeApiServerInstallArgs.__new__(KubeApiServerInstallArgs)
 
             __props__.__dict__["architecture"] = architecture
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if install_directory is None:
-                install_directory = '/usr/local/bin'
-            __props__.__dict__["install_directory"] = install_directory
+            if directory is None:
+                directory = '/usr/local/bin'
+            __props__.__dict__["directory"] = directory
             __props__.__dict__["version"] = version
+            __props__.__dict__["bin_name"] = None
+            __props__.__dict__["mkdir"] = None
+            __props__.__dict__["path"] = None
         super(KubeApiServerInstall, __self__).__init__(
             'kubernetes-the-hard-way:remote:KubeApiServerInstall',
             resource_name,
             __props__,
             opts,
             remote=True)
 
@@ -165,28 +169,43 @@
     def architecture(self) -> pulumi.Output['Architecture']:
         """
         The kube-apiserver CPU architecture.
         """
         return pulumi.get(self, "architecture")
 
     @property
+    @pulumi.getter(name="binName")
+    def bin_name(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "bin_name")
+
+    @property
     @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The connection details.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def directory(self) -> pulumi.Output[str]:
         """
         Directory to install the `kube-apiserver` binary.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
+
+    @property
+    @pulumi.getter
+    def mkdir(self) -> pulumi.Output[Optional['_tools.Mkdir']]:
+        return pulumi.get(self, "mkdir")
+
+    @property
+    @pulumi.getter
+    def path(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
         The version of kube-apiserver to install.
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from .. import tools as _tools
 from ._enums import *
 import pulumi_command
 
 __all__ = ['KubeControllerManagerInstallArgs', 'KubeControllerManagerInstall']
 
 @pulumi.input_type
 class KubeControllerManagerInstallArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  architecture: Optional[pulumi.Input['Architecture']] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a KubeControllerManagerInstall resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details.
         :param pulumi.Input['Architecture'] architecture: The kube-controller-manager CPU architecture.
-        :param pulumi.Input[str] install_directory: Directory to install the `kube-controller-manager` binary.
+        :param pulumi.Input[str] directory: Directory to install the `kube-controller-manager` binary.
         :param pulumi.Input[str] version: The version of kube-controller-manager to install.
         """
         pulumi.set(__self__, "connection", connection)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
-        if install_directory is None:
-            install_directory = '/usr/local/bin'
-        if install_directory is not None:
-            pulumi.set(__self__, "install_directory", install_directory)
+        if directory is None:
+            directory = '/usr/local/bin'
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
@@ -58,24 +59,24 @@
         return pulumi.get(self, "architecture")
 
     @architecture.setter
     def architecture(self, value: Optional[pulumi.Input['Architecture']]):
         pulumi.set(self, "architecture", value)
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
         Directory to install the `kube-controller-manager` binary.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
 
-    @install_directory.setter
-    def install_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "install_directory", value)
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
         The version of kube-controller-manager to install.
         """
@@ -89,25 +90,25 @@
 class KubeControllerManagerInstall(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Installs kube-controller-manager on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input['Architecture'] architecture: The kube-controller-manager CPU architecture.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details.
-        :param pulumi.Input[str] install_directory: Directory to install the `kube-controller-manager` binary.
+        :param pulumi.Input[str] directory: Directory to install the `kube-controller-manager` binary.
         :param pulumi.Input[str] version: The version of kube-controller-manager to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: KubeControllerManagerInstallArgs,
@@ -128,15 +129,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
@@ -145,18 +146,22 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KubeControllerManagerInstallArgs.__new__(KubeControllerManagerInstallArgs)
 
             __props__.__dict__["architecture"] = architecture
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if install_directory is None:
-                install_directory = '/usr/local/bin'
-            __props__.__dict__["install_directory"] = install_directory
+            if directory is None:
+                directory = '/usr/local/bin'
+            __props__.__dict__["directory"] = directory
             __props__.__dict__["version"] = version
+            __props__.__dict__["bin_name"] = None
+            __props__.__dict__["mkdir"] = None
+            __props__.__dict__["mv"] = None
+            __props__.__dict__["path"] = None
         super(KubeControllerManagerInstall, __self__).__init__(
             'kubernetes-the-hard-way:remote:KubeControllerManagerInstall',
             resource_name,
             __props__,
             opts,
             remote=True)
 
@@ -165,28 +170,48 @@
     def architecture(self) -> pulumi.Output['Architecture']:
         """
         The kube-controller-manager CPU architecture.
         """
         return pulumi.get(self, "architecture")
 
     @property
+    @pulumi.getter(name="binName")
+    def bin_name(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "bin_name")
+
+    @property
     @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The connection details.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def directory(self) -> pulumi.Output[str]:
         """
         Directory to install the `kube-controller-manager` binary.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
+
+    @property
+    @pulumi.getter
+    def mkdir(self) -> pulumi.Output['_tools.Mkdir']:
+        return pulumi.get(self, "mkdir")
+
+    @property
+    @pulumi.getter
+    def mv(self) -> pulumi.Output['_tools.Mv']:
+        return pulumi.get(self, "mv")
+
+    @property
+    @pulumi.getter
+    def path(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
         The version of kube-controller-manager to install.
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,40 +4,42 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from .. import tools as _tools
 from ._enums import *
+from .download import Download
 import pulumi_command
 
-__all__ = ['KubeSchedulerInstallArgs', 'KubeSchedulerInstall']
+__all__ = ['KubectlInstallArgs', 'KubectlInstall']
 
 @pulumi.input_type
-class KubeSchedulerInstallArgs:
+class KubectlInstallArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  architecture: Optional[pulumi.Input['Architecture']] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a KubeSchedulerInstall resource.
+        The set of arguments for constructing a KubectlInstall resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details.
-        :param pulumi.Input['Architecture'] architecture: The kube-scheduler CPU architecture.
-        :param pulumi.Input[str] install_directory: Directory to install the `kube-scheduler` binary.
-        :param pulumi.Input[str] version: The version of kube-scheduler to install.
+        :param pulumi.Input['Architecture'] architecture: The CPU architecture.
+        :param pulumi.Input[str] directory: Directory to install the binary.
+        :param pulumi.Input[str] version: The version of to install.
         """
         pulumi.set(__self__, "connection", connection)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
-        if install_directory is None:
-            install_directory = '/usr/local/bin'
-        if install_directory is not None:
-            pulumi.set(__self__, "install_directory", install_directory)
+        if directory is None:
+            directory = '/usr/local/bin'
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
@@ -49,146 +51,188 @@
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
     def architecture(self) -> Optional[pulumi.Input['Architecture']]:
         """
-        The kube-scheduler CPU architecture.
+        The CPU architecture.
         """
         return pulumi.get(self, "architecture")
 
     @architecture.setter
     def architecture(self, value: Optional[pulumi.Input['Architecture']]):
         pulumi.set(self, "architecture", value)
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
-        Directory to install the `kube-scheduler` binary.
+        Directory to install the binary.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
 
-    @install_directory.setter
-    def install_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "install_directory", value)
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
-        The version of kube-scheduler to install.
+        The version of to install.
         """
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class KubeSchedulerInstall(pulumi.ComponentResource):
+class KubectlInstall(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Installs kube-scheduler on a remote system.
+        Installs kubectl on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['Architecture'] architecture: The kube-scheduler CPU architecture.
+        :param pulumi.Input['Architecture'] architecture: The CPU architecture.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details.
-        :param pulumi.Input[str] install_directory: Directory to install the `kube-scheduler` binary.
-        :param pulumi.Input[str] version: The version of kube-scheduler to install.
+        :param pulumi.Input[str] directory: Directory to install the binary.
+        :param pulumi.Input[str] version: The version of to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: KubeSchedulerInstallArgs,
+                 args: KubectlInstallArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Installs kube-scheduler on a remote system.
+        Installs kubectl on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param KubeSchedulerInstallArgs args: The arguments to use to populate this resource's properties.
+        :param KubectlInstallArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(KubeSchedulerInstallArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(KubectlInstallArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = KubeSchedulerInstallArgs.__new__(KubeSchedulerInstallArgs)
+            __props__ = KubectlInstallArgs.__new__(KubectlInstallArgs)
 
             __props__.__dict__["architecture"] = architecture
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if install_directory is None:
-                install_directory = '/usr/local/bin'
-            __props__.__dict__["install_directory"] = install_directory
+            if directory is None:
+                directory = '/usr/local/bin'
+            __props__.__dict__["directory"] = directory
             __props__.__dict__["version"] = version
-        super(KubeSchedulerInstall, __self__).__init__(
-            'kubernetes-the-hard-way:remote:KubeSchedulerInstall',
+            __props__.__dict__["bin_name"] = None
+            __props__.__dict__["download"] = None
+            __props__.__dict__["mkdir"] = None
+            __props__.__dict__["mktemp"] = None
+            __props__.__dict__["mv"] = None
+            __props__.__dict__["path"] = None
+            __props__.__dict__["rm"] = None
+        super(KubectlInstall, __self__).__init__(
+            'kubernetes-the-hard-way:remote:KubectlInstall',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
     def architecture(self) -> pulumi.Output['Architecture']:
         """
-        The kube-scheduler CPU architecture.
+        The CPU architecture.
         """
         return pulumi.get(self, "architecture")
 
     @property
+    @pulumi.getter(name="binName")
+    def bin_name(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "bin_name")
+
+    @property
     @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The connection details.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def directory(self) -> pulumi.Output[str]:
         """
-        Directory to install the `etcd` and `etcdctl` binaries.
+        Directory to install the binary.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
+
+    @property
+    @pulumi.getter
+    def download(self) -> pulumi.Output['Download']:
+        return pulumi.get(self, "download")
+
+    @property
+    @pulumi.getter
+    def mkdir(self) -> pulumi.Output[Optional['_tools.Mkdir']]:
+        return pulumi.get(self, "mkdir")
+
+    @property
+    @pulumi.getter
+    def mktemp(self) -> pulumi.Output['_tools.Mktemp']:
+        return pulumi.get(self, "mktemp")
+
+    @property
+    @pulumi.getter
+    def mv(self) -> pulumi.Output['_tools.Mv']:
+        return pulumi.get(self, "mv")
+
+    @property
+    @pulumi.getter
+    def path(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "path")
+
+    @property
+    @pulumi.getter
+    def rm(self) -> pulumi.Output['_tools.Rm']:
+        return pulumi.get(self, "rm")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
-        The version of kube-scheduler to install.
+        The version to install.
         """
         return pulumi.get(self, "version")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1712367286
+Version: 0.0.11a1712430472
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,21 +13,29 @@
 pulumi_kubernetes_the_hard_way/config/__init__.py
 pulumi_kubernetes_the_hard_way/config/_enums.py
 pulumi_kubernetes_the_hard_way/config/_inputs.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
+pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+pulumi_kubernetes_the_hard_way/remote/crictl_install.py
 pulumi_kubernetes_the_hard_way/remote/download.py
+pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
+pulumi_kubernetes_the_hard_way/remote/runc_install.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
 pulumi_kubernetes_the_hard_way/tls/encryption_key.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712367286/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.11a1712430472/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-command>=0.9.0,<1.0.0", "pulumi-random>=4.0.0,<5.0.0", "pulumi-tls>=5.0.0,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.11a1712367286"
+  version = "0.0.11a1712430472"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

