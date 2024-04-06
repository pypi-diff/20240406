# Comparing `tmp/ehdtd_daemon-0.1.3.tar.gz` & `tmp/ehdtd_daemon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.3.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.1.4.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.3.tar` & `ehdtd_daemon-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.3/LICENSE
--rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.3/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.3/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0    11668 2024-04-05 09:26:03.505231 ehdtd_daemon-0.1.3/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0     7213 2024-04-05 09:26:48.307492 ehdtd_daemon-0.1.3/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.3/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      705 2024-04-05 07:52:49.150202 ehdtd_daemon-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.4/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.4/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0    11727 2024-04-06 14:50:21.411837 ehdtd_daemon-0.1.4/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0     7213 2024-04-05 09:26:48.307492 ehdtd_daemon-0.1.4/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.4/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      705 2024-04-06 14:50:59.602298 ehdtd_daemon-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4017 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.4/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.3/LICENSE` & `ehdtd_daemon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.3/README.md` & `ehdtd_daemon-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.3/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.1.4/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.3/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.1.4/ehdtd_daemon/aux_common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,17 @@
     """
     result = None
     default_log_dir = '/var/log/ehdtd-daemon'
     default_run_dir = '/run/ehdtd-daemon'
 
     home_dir = os.getenv('HOME')
 
+    if home_dir is None:
+        home_dir = '/tmp/.ehdtd'
+
     default_home_log_dir = os.path.join(home_dir, '.ehdtd-daemon/var/log')
     default_home_run_dir = os.path.join(home_dir, '.ehdtd-daemon/var/run')
 
 
     config_data = None
     default_config_file = '/etc/ehdtd-daemon/ehdtd-daemon-config.yaml'
```

### Comparing `ehdtd_daemon-0.1.3/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.1.4/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.3/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml` & `ehdtd_daemon-0.1.4/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.3/pyproject.toml` & `ehdtd_daemon-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.3"
+version = "0.1.4"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
```

### Comparing `ehdtd_daemon-0.1.3/PKG-INFO` & `ehdtd_daemon-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

