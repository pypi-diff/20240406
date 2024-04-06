# Comparing `tmp/pyshv-0.5.0.tar.gz` & `tmp/pyshv-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshv-0.5.0.tar", last modified: Thu Jan 18 17:55:59 2024, max compression
+gzip compressed data, was "pyshv-0.6.0.tar", last modified: Sat Apr  6 19:04:33 2024, max compression
```

## Comparing `pyshv-0.5.0.tar` & `pyshv-0.6.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-01-18 17:55:59.661444 pyshv-0.5.0/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1078 2023-10-11 09:25:34.000000 pyshv-0.5.0/LICENSE
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4135 2024-01-18 17:55:59.660443 pyshv-0.5.0/PKG-INFO
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1356 2023-11-10 14:08:07.000000 pyshv-0.5.0/README.rst
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2262 2024-01-18 17:24:57.000000 pyshv-0.5.0/pyproject.toml
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-01-18 17:55:59.659443 pyshv-0.5.0/pyshv.egg-info/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4135 2024-01-18 17:55:59.000000 pyshv-0.5.0/pyshv.egg-info/PKG-INFO
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1067 2024-01-18 17:55:59.000000 pyshv-0.5.0/pyshv.egg-info/SOURCES.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        1 2024-01-18 17:55:59.000000 pyshv-0.5.0/pyshv.egg-info/dependency_links.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       91 2024-01-18 17:55:59.000000 pyshv-0.5.0/pyshv.egg-info/entry_points.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      221 2024-01-18 17:55:59.000000 pyshv-0.5.0/pyshv.egg-info/requires.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       14 2024-01-18 17:55:59.000000 pyshv-0.5.0/pyshv.egg-info/top_level.txt
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)       38 2024-01-18 17:55:59.661444 pyshv-0.5.0/setup.cfg
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-01-18 17:55:59.655443 pyshv-0.5.0/shv/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3623 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/__init__.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-01-18 17:55:59.656443 pyshv-0.5.0/shv/broker/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      173 2023-06-16 08:04:39.000000 pyshv-0.5.0/shv/broker/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1844 2023-11-10 13:13:10.000000 pyshv-0.5.0/shv/broker/__main__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    29363 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/broker/rpcbroker.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12102 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/broker/rpcbrokerconfig.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14860 2023-11-10 09:49:24.000000 pyshv-0.5.0/shv/chainpack.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7654 2023-11-10 09:49:24.000000 pyshv-0.5.0/shv/commonpack.py
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-01-18 17:55:59.656443 pyshv-0.5.0/shv/cp2cp/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      135 2023-04-20 12:01:13.000000 pyshv-0.5.0/shv/cp2cp/__init__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2282 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/cp2cp/__main__.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2099 2023-10-13 20:09:09.000000 pyshv-0.5.0/shv/cp2cp/cp2cp.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    16088 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/cpon.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-07 07:26:23.000000 pyshv-0.5.0/shv/py.typed
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    13157 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/rpcclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3258 2023-11-07 14:42:36.000000 pyshv-0.5.0/shv/rpcerrors.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2957 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/rpclogin.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    11529 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/rpcmessage.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6165 2023-10-13 12:53:59.000000 pyshv-0.5.0/shv/rpcmethod.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5593 2023-11-10 09:49:24.000000 pyshv-0.5.0/shv/rpcprotocol.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    10644 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/rpcserver.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5578 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/rpcsubscription.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8307 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/rpcurl.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      117 2023-10-11 09:25:34.000000 pyshv-0.5.0/shv/shvversion.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    17871 2024-01-18 17:24:57.000000 pyshv-0.5.0/shv/simpleclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1766 2024-01-09 20:44:21.000000 pyshv-0.5.0/shv/simpledevice.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      392 2023-10-13 12:53:59.000000 pyshv-0.5.0/shv/tools.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7842 2023-10-13 20:09:09.000000 pyshv-0.5.0/shv/value.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1807 2023-10-13 12:53:59.000000 pyshv-0.5.0/shv/value_tools.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12520 2023-11-10 12:39:07.000000 pyshv-0.5.0/shv/valueclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)        6 2024-01-18 17:52:34.000000 pyshv-0.5.0/shv/version
-drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-01-18 17:55:59.659443 pyshv-0.5.0/tests/
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3142 2023-05-22 19:59:41.000000 pyshv-0.5.0/tests/test_chainpack.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      535 2023-05-22 19:59:41.000000 pyshv-0.5.0/tests/test_cp2cp.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4675 2023-07-18 12:02:43.000000 pyshv-0.5.0/tests/test_cpon.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      377 2023-11-10 09:49:24.000000 pyshv-0.5.0/tests/test_crc32.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1011 2023-05-22 19:59:41.000000 pyshv-0.5.0/tests/test_errors.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3133 2024-01-09 16:31:34.000000 pyshv-0.5.0/tests/test_example.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6139 2024-01-18 17:24:57.000000 pyshv-0.5.0/tests/test_rpcclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2453 2024-01-18 17:24:57.000000 pyshv-0.5.0/tests/test_rpcsubscription.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3551 2024-01-18 17:24:57.000000 pyshv-0.5.0/tests/test_rpcurl.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3531 2023-11-10 09:49:24.000000 pyshv-0.5.0/tests/test_simpleclient.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2142 2023-11-10 09:49:24.000000 pyshv-0.5.0/tests/test_simpledevice.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4755 2023-10-13 20:09:09.000000 pyshv-0.5.0/tests/test_value.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)      678 2023-10-13 12:53:59.000000 pyshv-0.5.0/tests/test_value_tools.py
--rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5492 2023-10-11 09:25:34.000000 pyshv-0.5.0/tests/test_valueclient.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.682715 pyshv-0.6.0/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1078 2023-10-11 09:25:34.000000 pyshv-0.6.0/LICENSE
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3776 2024-04-06 19:04:33.681715 pyshv-0.6.0/PKG-INFO
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1332 2024-04-06 18:44:22.000000 pyshv-0.6.0/README.rst
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3077 2024-04-06 18:44:22.000000 pyshv-0.6.0/pyproject.toml
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.681715 pyshv-0.6.0/pyshv.egg-info/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3776 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/PKG-INFO
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1080 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/SOURCES.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        1 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/dependency_links.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       93 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/entry_points.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      153 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/requires.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       14 2024-04-06 19:04:33.000000 pyshv-0.6.0/pyshv.egg-info/top_level.txt
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)       38 2024-04-06 19:04:33.682715 pyshv-0.6.0/setup.cfg
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.677715 pyshv-0.6.0/shv/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3919 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      782 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/__version__.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.677715 pyshv-0.6.0/shv/broker/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      162 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1829 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/__main__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    30962 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/broker.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12306 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/broker/config.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14153 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/chainpack.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7573 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/commonpack.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.678715 pyshv-0.6.0/shv/cpconv/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      137 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpconv/__init__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2365 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpconv/__main__.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2100 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpconv/cpconv.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    16319 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/cpon.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)        0 2023-04-07 07:26:23.000000 pyshv-0.6.0/shv/py.typed
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    13972 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4181 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcerrors.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5580 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpclogin.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    14516 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcmessage.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6877 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcmethod.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5873 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcparams.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6118 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcprotocol.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    11841 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcserver.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5898 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcsubscription.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7318 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/rpcurl.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      117 2023-10-11 09:25:34.000000 pyshv-0.6.0/shv/shvversion.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    19508 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/simplebase.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     8646 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/simpleclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2637 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/simpledevice.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      393 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/tools.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7912 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/value.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)    12299 2024-04-06 18:39:22.000000 pyshv-0.6.0/shv/valueclient.py
+drwxr-xr-x   0 cynerd    (1000) cynerd    (1000)        0 2024-04-06 19:04:33.680715 pyshv-0.6.0/tests/
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3321 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_chainpack.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      536 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_cpconv.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5066 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_cpon.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)      387 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_crc32.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1012 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_errors.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5954 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_example.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     6818 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     1115 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcparam.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     2423 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcsubscription.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4117 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_rpcurl.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     7424 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_simpleclient.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     3034 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_simpledevice.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     4744 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_value.py
+-rw-r--r--   0 cynerd    (1000) cynerd    (1000)     5647 2024-04-06 18:39:22.000000 pyshv-0.6.0/tests/test_valueclient.py
```

### Comparing `pyshv-0.5.0/LICENSE` & `pyshv-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshv-0.5.0/PKG-INFO` & `pyshv-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshv
-Version: 0.5.0
+Version: 0.6.0
 Summary: Pure Python SHV implementation
 Author: Elektroline a.s.
 License: MIT License
         
         Copyright (c) 2022-2023 Elektroline a.s.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,64 +21,55 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://gitlab.com/elektroline-predator/pyshv
-Project-URL: Bug Tracker, https://gitlab.com/elektroline-predator/pyshv/-/issues
+Project-URL: Homepage, https://gitlab.com/silicon-heaven/pyshv
+Project-URL: Bug Tracker, https://gitlab.com/silicon-heaven/pyshv/-/issues
 Project-URL: Github, https://github.com/silicon-heaven/libshv-py
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: python-dateutil
 Requires-Dist: pyserial
 Requires-Dist: aioserial
-Requires-Dist: asyncinotify
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: sphinx-multiversion; extra == "docs"
+Requires-Dist: asyncinotify; sys_platform == "linux"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: pydocstyle; extra == "lint"
-Requires-Dist: pylint; extra == "lint"
-Requires-Dist: mypy; extra == "lint"
-Requires-Dist: types-pyserial; extra == "lint"
-Requires-Dist: types-python-dateutil; extra == "lint"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx-multiversion; extra == "docs"
 
 ============================================
 Pure Python implementation of Silicon Heaven
 ============================================
-.. image:: https://gitlab.com/elektroline-predator/pyshv/-/raw/master/docs/_static/logo.svg
+.. image:: https://gitlab.com/silicon-heaven/pyshv/-/raw/master/docs/_static/logo.svg
    :align: right
    :height: 128px
 
 The implementation of serialized and deserializer for CPON and Chainpack as well
 as implementation of `Silicon Heaven RPC
 <https://silicon-heaven.github.io/shv-doc/>`__.
 
-* `📃 Sources <https://gitlab.com/elektroline-predator/pyshv>`__
-* `⁉️ Issue tracker <https://gitlab.com/elektroline-predator/pyshv/-/issues>`__
-* `📕 Documentation <https://elektroline-predator.gitlab.io/pyshv/>`__
+* `📃 Sources <https://gitlab.com/silicon-heaven/pyshv>`__
+* `⁉️ Issue tracker <https://gitlab.com/silicon-heaven/pyshv/-/issues>`__
+* `📕 Documentation <https://silicon-heaven.gitlab.io/pyshv/>`__
 
 
 Installation
 ------------
 
 The installation can be done with package manager ``pip``.
```

### Comparing `pyshv-0.5.0/pyproject.toml` & `pyshv-0.6.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pyshv"
+version = "0.6.0"
 description = "Pure Python SHV implementation"
 readme = "README.rst"
-dynamic = ["version"]
 license = {file = "LICENSE"}
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: MIT License",
@@ -16,85 +16,105 @@
   "Intended Audience :: Developers",
   "Topic :: Home Automation",
   "Topic :: System :: Networking",
   "Typing :: Typed",
 ]
 requires-python = ">=3.11"
 dependencies = [
-  "python-dateutil",
   "pyserial",
   "aioserial",
-  "asyncinotify",
+  "asyncinotify; sys_platform == \"linux\"",
 ]
 
 [project.urls]
-"Homepage" = "https://gitlab.com/elektroline-predator/pyshv"
-"Bug Tracker" = "https://gitlab.com/elektroline-predator/pyshv/-/issues"
+"Homepage" = "https://gitlab.com/silicon-heaven/pyshv"
+"Bug Tracker" = "https://gitlab.com/silicon-heaven/pyshv/-/issues"
 "Github" = "https://github.com/silicon-heaven/libshv-py"
 
 [project.optional-dependencies]
-docs = [
-  "sphinx",
-  "sphinx_rtd_theme",
-  "sphinx-multiversion",
-]
 test = [
   "pytest",
   "pytest-asyncio",
   "pytest-cov",
 ]
-lint = [
-  "black",
-  "isort",
-  "pydocstyle",
-  "pylint",
-  "mypy",
-  "types-pyserial",
-  "types-python-dateutil",
+docs = [
+  "sphinx",
+  "sphinx_rtd_theme",
+  "sphinx-multiversion",
 ]
 
 [project.scripts]
-pycp2cp = "shv.cp2cp.__main__:main"
+pycpconv = "shv.cpconv.__main__:main"
 pyshvbroker = "shv.broker.__main__:main"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools.dynamic]
-version = {file = "shv/version"}
 [tool.setuptools.packages.find]
 exclude = ["docs", "tests*"]
 [tool.setuptools.package-data]
-"*" = ["version", "py.typed"]
+"*" = ["py.typed"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.coverage.run]
 branch = true
 omit = ["tests/*"]
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "if typing.TYPE_CHECKING:"
 ]
 
-[tool.isort]
-profile = 'black'
-
-[tool.pylint.main]
-recursive = "y"
-ignore = ["tests", "docs"]
-fail-under = 9.5
-[tool.pylint.format]
-disable = [
-  # Exception can be safely caught because there is BaseException for unsafe
-  # ones (such as SystemExit) and there are reasons to catch all exceptions.
-  "W0718",
-  # Prevent usage of module name in documentation (seems unreasonable)
-  "C0104",
-  # We have pydocstyle for the following ones
-  "C0103", "C0114", "C0115", "C0116",
-]
-# https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html
-max-line-length = 88
+[tool.ruff]
+target-version = "py311"
+[tool.ruff.lint]
+select = [
+  "F", "E", "W", "I", "N", "D", "UP", "YTT", "ANN", "ASYNC", "TRIO", "S", "BLE",
+  "B", "A", "COM", "PL", "RUF"
+]
+ignore = [
+  # Magic methods have defined behavior so what is there to document. __init__
+  # should be documented in class docstring.
+  "D105", "D107",
+  # These have conflicting rules.
+  "D203", "D213",
+  # Ignore too long lines (format tackles that)
+  "E501",
+  # It is nice that assert should not be used for input checking but it can be
+  # also used for internal consistency checking.
+  "S101", "B011",
+  # subprocess can be insecurely used but not is insecure by design
+  "S404", "S603", "S607",
+  # Catching Exception is valid and safe in some cases and thus should be allowed
+  "BLE001",
+  # Conflict with formatter
+  "COM812",
+  # Remove too-many limit for more complex code.
+  "PLR0904", "PLR0911", "PLR0912", "PLR0913", "PLR0917", "PLR2004", "PLR1702",
+  # This seems like a wrong rule
+  "PLW1641",
+]
+preview = true
+[tool.ruff.lint.per-file-ignores]
+"tests/**" = [
+  "D100", "D101", "D102", "D103", "D104", "S101", "S106", "ANN001", "ANN002",
+  "ANN003", "ANN201", "ANN202", "ANN204", "ANN205", "PLR6301",
+]
+"docs/conf.py" = ["D100", "D103", "A001", "ANN201", "ANN001"]
+[tool.ruff.format]
+docstring-code-format = true
+preview = true
+
+[tool.mypy]
+python_version = "3.11"
+ignore_missing_imports = true
+disallow_untyped_defs = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+warn_return_any = true
+warn_unreachable = true
+[[tool.mypy.overrides]]
+module = "tests.*"
+allow_untyped_defs = true
```

### Comparing `pyshv-0.5.0/pyshv.egg-info/PKG-INFO` & `pyshv-0.6.0/pyshv.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshv
-Version: 0.5.0
+Version: 0.6.0
 Summary: Pure Python SHV implementation
 Author: Elektroline a.s.
 License: MIT License
         
         Copyright (c) 2022-2023 Elektroline a.s.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,64 +21,55 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://gitlab.com/elektroline-predator/pyshv
-Project-URL: Bug Tracker, https://gitlab.com/elektroline-predator/pyshv/-/issues
+Project-URL: Homepage, https://gitlab.com/silicon-heaven/pyshv
+Project-URL: Bug Tracker, https://gitlab.com/silicon-heaven/pyshv/-/issues
 Project-URL: Github, https://github.com/silicon-heaven/libshv-py
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: Topic :: System :: Networking
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: python-dateutil
 Requires-Dist: pyserial
 Requires-Dist: aioserial
-Requires-Dist: asyncinotify
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx_rtd_theme; extra == "docs"
-Requires-Dist: sphinx-multiversion; extra == "docs"
+Requires-Dist: asyncinotify; sys_platform == "linux"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: pydocstyle; extra == "lint"
-Requires-Dist: pylint; extra == "lint"
-Requires-Dist: mypy; extra == "lint"
-Requires-Dist: types-pyserial; extra == "lint"
-Requires-Dist: types-python-dateutil; extra == "lint"
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx-multiversion; extra == "docs"
 
 ============================================
 Pure Python implementation of Silicon Heaven
 ============================================
-.. image:: https://gitlab.com/elektroline-predator/pyshv/-/raw/master/docs/_static/logo.svg
+.. image:: https://gitlab.com/silicon-heaven/pyshv/-/raw/master/docs/_static/logo.svg
    :align: right
    :height: 128px
 
 The implementation of serialized and deserializer for CPON and Chainpack as well
 as implementation of `Silicon Heaven RPC
 <https://silicon-heaven.github.io/shv-doc/>`__.
 
-* `📃 Sources <https://gitlab.com/elektroline-predator/pyshv>`__
-* `⁉️ Issue tracker <https://gitlab.com/elektroline-predator/pyshv/-/issues>`__
-* `📕 Documentation <https://elektroline-predator.gitlab.io/pyshv/>`__
+* `📃 Sources <https://gitlab.com/silicon-heaven/pyshv>`__
+* `⁉️ Issue tracker <https://gitlab.com/silicon-heaven/pyshv/-/issues>`__
+* `📕 Documentation <https://silicon-heaven.gitlab.io/pyshv/>`__
 
 
 Installation
 ------------
 
 The installation can be done with package manager ``pip``.
```

### Comparing `pyshv-0.5.0/shv/__init__.py` & `pyshv-0.6.0/shv/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 """Python implementation of Silicon Heaven."""
+
+from .__version__ import VERSION
 from .chainpack import ChainPack, ChainPackReader, ChainPackWriter
 from .cpon import Cpon, CponReader, CponWriter
 from .rpcclient import (
     RpcClient,
     RpcClientPipe,
     RpcClientTCP,
     RpcClientTTY,
     RpcClientUnix,
     connect_rpc_client,
+    init_rpc_client,
 )
 from .rpcerrors import (
     RpcError,
     RpcErrorCode,
     RpcInternalError,
     RpcInvalidParamsError,
     RpcInvalidRequestError,
+    RpcLoginRequiredError,
     RpcMethodCallCancelledError,
     RpcMethodCallExceptionError,
     RpcMethodCallTimeoutError,
     RpcMethodNotFoundError,
     RpcParseError,
+    RpcUserIDRequiredError,
 )
-from .rpclogin import rpclogin, rpclogin_url
+from .rpclogin import RpcLogin, RpcLoginType
 from .rpcmessage import RpcMessage
 from .rpcmethod import RpcMethodAccess, RpcMethodDesc, RpcMethodFlags
+from .rpcparams import SHVGetKey, shvarg, shvargt, shvget, shvgett, shvt
 from .rpcprotocol import (
     RpcProtocolSerial,
     RpcProtocolSerialCRC,
     RpcProtocolStream,
     RpcTransportProtocol,
 )
 from .rpcserver import (
     RpcServer,
     RpcServerTCP,
     RpcServerTTY,
     RpcServerUnix,
     create_rpc_server,
 )
-from .rpcsubscription import RpcSubscription
-from .rpcurl import RpcLoginType, RpcProtocol, RpcUrl
+from .rpcsubscription import DefaultRpcSubscription, RpcSubscription
+from .rpcurl import RpcProtocol, RpcUrl
 from .shvversion import SHV_VERSION_MAJOR, SHV_VERSION_MINOR
+from .simplebase import SimpleBase
 from .simpleclient import SimpleClient
 from .simpledevice import SimpleDevice
 from .value import (
     SHVBool,
     SHVBoolType,
     SHVBytes,
     SHVDatetime,
@@ -67,109 +74,114 @@
     is_shvbool,
     is_shvimap,
     is_shvmap,
     is_shvnull,
     shvmeta,
     shvmeta_eq,
 )
-from .value_tools import SHVGetKey, shvget
 from .valueclient import ValueClient
 
-VERSION = (
-    (__import__("pathlib").Path(__file__).parent / "version").read_text("utf-8").strip()
-)
-
-
 __all__ = [
-    # cpon
-    "Cpon",
-    "CponReader",
-    "CponWriter",
+    # shvversion
+    "SHV_VERSION_MAJOR",
+    "SHV_VERSION_MINOR",
+    "VERSION",
     # chainpack
     "ChainPack",
     "ChainPackReader",
     "ChainPackWriter",
-    # rpcclient
-    "connect_rpc_client",
+    # cpon
+    "Cpon",
+    "CponReader",
+    "CponWriter",
+    "DefaultRpcSubscription",
     "RpcClient",
-    "RpcClientTCP",
-    "RpcClientUnix",
     "RpcClientPipe",
+    "RpcClientTCP",
     "RpcClientTTY",
-    # rpcprotocol
-    "RpcTransportProtocol",
-    "RpcProtocolStream",
-    "RpcProtocolSerial",
-    "RpcProtocolSerialCRC",
-    # rpcserver
-    "create_rpc_server",
-    "RpcServer",
-    "RpcServerTCP",
-    "RpcServerUnix",
-    "RpcServerTTY",
-    # rpcurl
-    "RpcProtocol",
-    "RpcLoginType",
-    "RpcUrl",
-    # rpcmessage
-    "RpcMessage",
-    # rpcmethod
-    "RpcMethodFlags",
-    "RpcMethodAccess",
-    "RpcMethodDesc",
+    "RpcClientUnix",
+    "RpcError",
     # rpcerror
     "RpcErrorCode",
-    "RpcError",
     "RpcInternalError",
     "RpcInvalidParamsError",
     "RpcInvalidRequestError",
+    # rpclogin
+    "RpcLogin",
+    "RpcLoginRequiredError",
+    "RpcLoginType",
+    "RpcLoginType",
+    # rpcmessage
+    "RpcMessage",
+    "RpcMethodAccess",
     "RpcMethodCallCancelledError",
     "RpcMethodCallExceptionError",
     "RpcMethodCallTimeoutError",
+    "RpcMethodDesc",
+    # rpcmethod
+    "RpcMethodFlags",
     "RpcMethodNotFoundError",
     "RpcParseError",
-    # rpclogin
-    "rpclogin",
-    "rpclogin_url",
+    # rpcurl
+    "RpcProtocol",
+    "RpcProtocolSerial",
+    "RpcProtocolSerialCRC",
+    "RpcProtocolStream",
+    "RpcServer",
+    "RpcServerTCP",
+    "RpcServerTTY",
+    "RpcServerUnix",
     # rpcsubscription
     "RpcSubscription",
+    # rpcprotocol
+    "RpcTransportProtocol",
+    "RpcUrl",
+    "RpcUserIDRequiredError",
+    "SHVBool",
+    "SHVBoolType",
+    "SHVBytes",
+    "SHVDatetime",
+    "SHVDecimal",
+    "SHVFloat",
+    "SHVGetKey",
+    "SHVIMap",
+    "SHVIMapType",
+    "SHVInt",
+    "SHVList",
+    "SHVListType",
+    "SHVMap",
+    "SHVMapType",
+    # value
+    "SHVMeta",
+    "SHVMetaType",
+    "SHVNull",
+    "SHVNullType",
+    "SHVStr",
+    "SHVType",
+    "SHVUInt",
+    # simplebase
+    "SimpleBase",
     # simpleclient
     "SimpleClient",
     # simpledevice
     "SimpleDevice",
     # valueclient
     "ValueClient",
-    # value
-    "SHVMeta",
-    "shvmeta",
-    "shvmeta_eq",
-    "SHVNull",
-    "is_shvnull",
-    "SHVBool",
-    "is_shvbool",
-    "SHVInt",
-    "SHVUInt",
-    "SHVFloat",
-    "SHVDecimal",
+    "connect_rpc_client",
+    # rpcserver
+    "create_rpc_server",
     "decimal_rexp",
-    "SHVStr",
-    "SHVBytes",
-    "SHVDatetime",
-    "SHVList",
-    "SHVMap",
-    "SHVIMap",
-    "is_shvmap",
+    # rpcclient
+    "init_rpc_client",
+    "is_shvbool",
     "is_shvimap",
-    "SHVType",
-    "SHVNullType",
-    "SHVBoolType",
-    "SHVListType",
-    "SHVMapType",
-    "SHVIMapType",
-    "SHVMetaType",
-    # value_tools
+    "is_shvmap",
+    "is_shvnull",
+    "shvarg",
+    "shvargt",
     "shvget",
-    "SHVGetKey",
-    # shvversion
-    "SHV_VERSION_MAJOR",
-    "SHV_VERSION_MINOR",
+    "shvgett",
+    "shvmeta",
+    "shvmeta_eq",
+    # rpcparams
+    "shvt",
 ]
```

### Comparing `pyshv-0.5.0/shv/broker/__main__.py` & `pyshv-0.6.0/shv/broker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Implementation of generic SHV RPC broker."""
+
 import argparse
 import asyncio
 import configparser
 import logging
 
-from .rpcbroker import RpcBroker
-from .rpcbrokerconfig import RpcBrokerConfig
+from .broker import RpcBroker
+from .config import RpcBrokerConfig
 
 logger = logging.getLogger(__name__)
 log_levels = (
     logging.DEBUG,
     logging.INFO,
     logging.WARNING,
     logging.ERROR,
@@ -37,15 +38,15 @@
         default=0,
         help="Decrease verbosity level of logging",
     )
     parser.add_argument(
         "-c",
         "--config",
         action="store",
-        default="",
+        default="/etc/pyshvbroker.ini",
         help="Configuration file",
     )
     return parser.parse_args()
 
 
 async def _broker_main(config: RpcBrokerConfig) -> None:
     broker = RpcBroker(config)
@@ -61,16 +62,15 @@
 
     logging.basicConfig(
         level=log_levels[sorted([1 - args.v + args.q, 0, len(log_levels) - 1])[1]],
         format="[%(asctime)s] [%(levelname)s] - %(message)s",
     )
 
     config = configparser.ConfigParser()
-    if args.config:
-        config.read(args.config)
+    config.read(args.config)
     brokerconf = RpcBrokerConfig.load(config)
     try:
         asyncio.run(_broker_main(brokerconf))
     except KeyboardInterrupt:
         pass
```

### Comparing `pyshv-0.5.0/shv/broker/rpcbroker.py` & `pyshv-0.6.0/shv/broker/broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,67 @@
 """Common state for the RPC broker that works as server in the SHV network."""
+
 from __future__ import annotations
 
 import asyncio
+import collections
 import collections.abc
-import importlib.metadata
-import itertools
+import contextlib
 import logging
 import random
+import string
 import time
 import typing
 
-from .. import VERSION
-from ..rpcclient import RpcClient
+from ..rpcclient import RpcClient, init_rpc_client
 from ..rpcerrors import (
     RpcError,
     RpcErrorCode,
     RpcInvalidParamsError,
+    RpcLoginRequiredError,
     RpcMethodCallExceptionError,
 )
 from ..rpcmessage import RpcMessage
 from ..rpcmethod import RpcMethodAccess, RpcMethodDesc
+from ..rpcparams import shvgett
 from ..rpcserver import RpcServer, create_rpc_server
 from ..rpcsubscription import RpcSubscription
 from ..rpcurl import RpcLoginType
+from ..simplebase import SimpleBase
 from ..simpleclient import SimpleClient
-from ..value import SHVType
-from ..value_tools import shvget
-from .rpcbrokerconfig import RpcBrokerConfig
+from ..value import SHVType, is_shvmap
+from .config import RpcBrokerConfig
 
 logger = logging.getLogger(__name__)
 
 
 class RpcBroker:
     """SHV RPC broker.
 
     The broker manages multiple RpcClient instances and exchanges messages
     between them.
     """
 
-    class Client(SimpleClient):
+    class Client(SimpleBase):
         """Single client connected to the broker."""
 
-        APP_NAME = "pyshvbroker"
-        """Name reported as application name for pySHVBroker."""
-        APP_VERSION = VERSION
-        """pySHVBroker version."""
-
-        IDLE_TIMEOUT_LOGIN: float = 5
-        """:param:`IDLE_TIMEOUT` set for clients without user.
-
-        This is intentionally shorter to quickly disconnect inactive clients
-        that are not participating in SHV RPC.
-        """
-
         def __init__(
             self,
             client: RpcClient,
             broker: RpcBroker,
+            *args: typing.Any,  # noqa ANN401
             user: RpcBrokerConfig.User | None = None,
-            **kwargs: typing.Any,
-        ):
-            super().__init__(client, **kwargs)
-            self.idle_disconnect = True
-            self.subscriptions: set[RpcSubscription] = set()
-            """Set of all subscriptions."""
-            self.user = user
-            """User used to login to the broker."""
-            if user is not None:
-                self.IDLE_TIMEOUT = self.IDLE_TIMEOUT_LOGIN
-            self._nonce: str | None = None
+            **kwargs: typing.Any,  # noqa ANN401
+        ) -> None:
+            super().__init__(client, *args, **kwargs)
+            self.user: RpcBrokerConfig.User | None = user
+            """Local user used to deduce access rights."""
             self.__broker = broker
-            self.__broker_client_id = broker.next_caller_id()
-            self.__mount_point: str | None = None
+            self.__broker_client_id = broker._register_client(self)
             self.__peer_is_broker: bool | None = None
-            self.__maintain_subscriptions_lock = asyncio.Lock()
-            broker.clients[self.__broker_client_id] = self
             logger.info(
                 "Client registered to broker with ID %d", self.__broker_client_id
             )
 
         @property
         def broker(self) -> RpcBroker:
             """Broker this client is part of."""
@@ -86,236 +69,114 @@
 
         @property
         def broker_client_id(self) -> int:
             """Identifier assigned to the client in the broker."""
             return self.__broker_client_id
 
         @property
-        def mount_point(self) -> str | None:
-            """Mount point of this client, if any."""
-            return self.__mount_point
-
-        def _lschng_path(self, path: str) -> tuple[str, str]:
-            pth = path.split("/")
-            valid_level = 0
-            for c in self.__broker.clients.values():
-                if c.mount_point is None or c.mount_point == path:
-                    continue
-                valid_level = max(
-                    valid_level,
-                    sum(
-                        1
-                        for _ in itertools.takewhile(
-                            lambda v: v[0] == v[1], zip(pth, c.mount_point.split("/"))
-                        )
-                    ),
-                )
-            return "/".join(pth[:valid_level]), pth[valid_level]
+        def active(self) -> bool:
+            """Check if given client is actively communicating.
 
-        async def set_mount_point(self, value: str | None) -> None:
-            if value is not None:
-                # We remove trailing slash because otherwise we could fail when we
-                # compare this string against path of exactly this node.
-                value = value.rstrip("/")
-            if self.__mount_point == value:
-                return
-            # Prepare lschng signal with old path
-            lschng: RpcMessage | None = None
-            if self.__mount_point is not None:
-                path, node = self._lschng_path(self.__mount_point)
-                lschng = RpcMessage.signal(
-                    path, "lschng", {node: False}, RpcMethodAccess.BROWSE
-                )
-            was_mounted = self.__mount_point is not None
-            # Perform mount point change
-            self.__mount_point = value
-            if value is not None:
-                # Prepare lschng for new path. We need to tackle here root change and
-                # thus we might need to send it first before we generate the one with
-                # correct root.
-                path, node = self._lschng_path(value)
-                if lschng is not None and lschng.path == path:
-                    lschng.param[node] = True  # type: ignore
-                else:
-                    if lschng is not None:
-                        await self.__broker.signal(lschng)
-                    lschng = RpcMessage.signal(
-                        path, "lschng", {node: True}, RpcMethodAccess.BROWSE
-                    )
-            # Send lschng signal
-            assert lschng is not None
-            await self.__broker.signal(lschng)
-            # Now remove old subscriptions and add new ones
-            await self.maintain_subscriptions(cleanup=was_mounted)
-            if value:
-                logger.info(
-                    "Client with ID %d is now mounted on: %s",
-                    self.__broker_client_id,
-                    value,
-                )
+            Client can be inactive for example due to being disconnected, or in
+            the middle of reset, or waiting for login.
+            """
+            return self.user is not None and self.client.connected
 
         async def peer_is_broker(self) -> bool:
             """Identify if peer this client is handle for is broker."""
             if self.__peer_is_broker is None:
-                try:
-                    lsr = await self.call(".app", "ls", "broker")
+                self.__peer_is_broker = False
+                with contextlib.suppress(RpcError):
+                    lsr = await self.call("", "ls", ".broker")
                     self.__peer_is_broker = lsr if isinstance(lsr, bool) else False
-                except RpcError:
-                    self.__peer_is_broker = False
             return self.__peer_is_broker
 
-        async def _loop(self) -> None:
-            await super()._loop()
-            self.__broker.clients.pop(self.__broker_client_id, None)
-            if self.__mount_point is not None:
-                path, node = self._lschng_path(self.__mount_point)
-                await self.__broker.signal(
-                    RpcMessage.signal(
-                        path, "lschng", {node: False}, RpcMethodAccess.BROWSE
-                    )
-                )
-            self.client.disconnect()
-            await self.client.wait_disconnect()
-            logger.info("Client with ID %d disconnected", self.__broker_client_id)
+        async def send(self, msg: RpcMessage) -> None:
+            """Propagate given message to this peer.
+
+            This is only wrapper around standard :meth:`_send`. We need to make
+            it public because in Broker peers are propagating messages from one
+            to another.
+
+            :param msg: Message to be sent.
+            """
+            await self._send(msg)
 
         async def _message(self, msg: RpcMessage) -> None:
-            if self.user is None:
-                if self._nonce is None:
-                    return await self.client.send(self._message_hello(msg))
-                return await self.client.send(self._message_login(msg))
+            assert self.user is not None
 
             if msg.is_request:
                 # Set access granted to the level allowed by user
                 access = self.user.access_level(msg.path, msg.method)
                 if access is None:
-                    resp = msg.make_response()
-                    resp.rpc_error = RpcError(
-                        "No access", RpcErrorCode.METHOD_NOT_FOUND
-                    )
-                    await self.client.send(resp)
-                    return
-                if access is not RpcMethodAccess.ADMIN or msg.rpc_access is None:
-                    msg.rpc_access = access
+                    return await self._send(
+                        msg.make_response(
+                            error=RpcError("No access", RpcErrorCode.METHOD_NOT_FOUND)
+                        )
+                    )
+                msg.rpc_access = (
+                    access
+                    if msg.rpc_access is None or msg.rpc_access > access
+                    else msg.rpc_access
+                )
+                # Append user ID
+                if msg.user_id is not None:
+                    bname = self.broker.config.name
+                    msg.user_id += (
+                        "," if msg.user_id else ""
+                    ) + f"{bname}{':' if bname else ''}{self.user.name}"
                 # Check if we should delegate it or handle it ourself
                 if (cpath := self.__broker.client_on_path(msg.path)) is None:
                     return await super()._message(msg)
                 # Propagate to some peer
-                msg.caller_ids = list(msg.caller_ids) + [self.__broker_client_id]
+                msg.caller_ids = [*msg.caller_ids, self.__broker_client_id]
                 msg.path = cpath[1]
-                await cpath[0].client.send(msg)
+                await cpath[0].send(msg)
 
-            if msg.is_response:
+            elif msg.is_response:
                 cids = list(msg.caller_ids)
                 if not cids:  # no caller IDs means this is message for us
                     return await super()._message(msg)
                 cid = cids.pop()
                 msg.caller_ids = cids
-                try:
-                    peer = self.__broker.clients[cid]
-                except KeyError:
-                    return
-                await peer.client.send(msg)
-
-            if msg.is_signal and self.mount_point is not None:
-                msg.path = self.mount_point + "/" + msg.path
-                await self.__broker.signal(msg)
-
-        def _message_hello(self, msg: RpcMessage) -> RpcMessage:
-            resp = msg.make_response()
-            if msg.is_request and msg.method == "hello":
-                self._nonce = "".join(
-                    random.choice("0123456789abcdef") for _ in range(8)
-                )
-                resp = msg.make_response()
-                resp.result = {"nonce": self._nonce}
-            else:
-                resp.rpc_error = RpcError(
-                    "Only 'hello' is allowed", RpcErrorCode.INVALID_REQUEST
-                )
-            return resp
+                if (peer := self.__broker.get_client(cid)) is not None:
+                    await peer.send(msg)
 
-        def _message_login(self, msg: RpcMessage) -> RpcMessage:
-            assert self._nonce is not None
-            resp = msg.make_response()
-            if not msg.is_request or msg.method != "login":
-                resp.rpc_error = RpcError(
-                    "Only 'login' is allowed", RpcErrorCode.INVALID_REQUEST
-                )
-                return resp
-            param = msg.param
-            resp = msg.make_response()
-            if isinstance(param, collections.abc.Mapping):
-                self.user = self.broker.config.login(
-                    shvget(param, ("login", "user"), str, ""),
-                    shvget(param, ("login", "password"), str, ""),
-                    self._nonce,
-                    RpcLoginType(
-                        shvget(param, ("login", "type"), str, RpcLoginType.SHA1.value)
-                    ),
-                )
-                if self.user is None:
-                    resp.rpc_error = RpcError(
-                        "Invalid login", RpcErrorCode.METHOD_CALL_EXCEPTION
-                    )
-                    return resp
-                logger.info(
-                    "Client with ID %d logged in as user: %s",
-                    self.__broker_client_id,
-                    self.user.name,
-                )
-                mount_point = shvget(
-                    param, ("options", "device", "mountPoint"), str, ""
-                )
-                if self.broker.client_on_path(mount_point) is not None:
-                    resp.rpc_error = RpcError(
-                        "Mount point already mounted",
-                        RpcErrorCode.METHOD_CALL_EXCEPTION,
-                    )
-                    return resp
-                if mount_point:
-                    asyncio.create_task(self.set_mount_point(mount_point))
-                self.IDLE_TIMEOUT = float(
-                    shvget(
-                        param,
-                        ("options", "idleWatchDogTimeOut"),
-                        int,
-                        type(self).IDLE_TIMEOUT,
-                    )
-                )
-                resp.result = {"clientId": self.broker_client_id}
-            else:
-                resp.rpc_error = RpcError(
-                    "Invalid type of parameters", RpcErrorCode.INVALID_PARAMS
-                )
-            return resp
+            elif msg.is_signal:
+                await self.__broker.signal_from(msg, self)
+
+        def _reset(self) -> None:
+            self.__broker._unregister_client(self)  # pylint: disable=protected-access
+            self.__peer_is_broker = None
+            # pylint: disable=protected-access
+            self.__broker_client_id = self.__broker._register_client(self)
 
         def _ls(self, path: str) -> typing.Iterator[str]:
             yield from super()._ls(path)
+            if not path:
+                yield ".broker"
             match path:
-                case ".app":
-                    yield "broker"
-                case ".app/broker":
+                case ".broker":
                     yield "currentClient"
                     yield "client"
-                    yield "clientInfo"
-                case ".app/broker/clientInfo" | ".app/broker/client":
-                    yield from map(str, self.broker.clients.keys())
+                case ".broker/client":
+                    yield from (
+                        str(c.broker_client_id) for c in self.__broker.clients()
+                    )
                 case _:
-                    for client in self.broker.clients.values():
-                        mnt = client.mount_point
-                        if mnt is not None:
-                            if path == "":
-                                yield mnt.split("/", maxsplit=1)[0]
-                            elif mnt.startswith(path + "/"):
-                                yield mnt[len(path) + 1 :].split("/", maxsplit=1)[0]
+                    for mnt, _ in self.broker.mounted_clients():
+                        if not path:
+                            yield mnt.split("/", maxsplit=1)[0]
+                        elif mnt.startswith(path + "/"):
+                            yield mnt[len(path) + 1 :].split("/", maxsplit=1)[0]
 
         def _dir(self, path: str) -> typing.Iterator[RpcMethodDesc]:
             yield from super()._dir(path)
             match path:
-                case ".app/broker":
+                case ".broker":
                     yield RpcMethodDesc(
                         "clientInfo", access=RpcMethodAccess.SUPER_SERVICE
                     )
                     yield RpcMethodDesc(
                         "mountedClientInfo", access=RpcMethodAccess.SUPER_SERVICE
                     )
                     yield RpcMethodDesc.getter(
@@ -323,325 +184,525 @@
                     )
                     yield RpcMethodDesc.getter(
                         "mounts", access=RpcMethodAccess.SUPER_SERVICE
                     )
                     yield RpcMethodDesc(
                         "disconnectClient", access=RpcMethodAccess.SUPER_SERVICE
                     )
-                case ".app/broker/currentClient":
+                case ".broker/currentClient":
                     yield RpcMethodDesc.getter("info", access=RpcMethodAccess.BROWSE)
                     yield RpcMethodDesc("subscribe", access=RpcMethodAccess.BROWSE)
                     yield RpcMethodDesc("unsubscribe", access=RpcMethodAccess.BROWSE)
-                    yield RpcMethodDesc(
-                        "rejectNotSubscribed", access=RpcMethodAccess.BROWSE
-                    )
                     yield RpcMethodDesc.getter(
                         "subscriptions", access=RpcMethodAccess.BROWSE
                     )
-                case _ if (
-                    path.startswith(".app/broker/clientInfo/")
-                    and self.broker.get_client(path[23:]) is not None
-                ):
-                    yield RpcMethodDesc.getter("userName", "String")
-                    yield RpcMethodDesc.getter("mountPoint", "String")
-                    yield RpcMethodDesc.getter("subscriptions")
-                    yield RpcMethodDesc(
-                        "dropClient", access=RpcMethodAccess.SUPER_SERVICE
-                    )
-                    yield RpcMethodDesc.getter("idleTime")
-                    yield RpcMethodDesc.getter("idleTimeMax")
 
         async def _method_call(
-            self, path: str, method: str, access: RpcMethodAccess, param: SHVType
+            self,
+            path: str,
+            method: str,
+            param: SHVType,
+            access: RpcMethodAccess,
+            user_id: str | None,
         ) -> SHVType:
             assert self.user is not None  # Otherwise handled in _message
-            if path == ".app/broker" and access >= RpcMethodAccess.SUPER_SERVICE:
-                match method:
-                    case "clientInfo":
-                        if not isinstance(param, int):
-                            raise RpcInvalidParamsError("Use Int")
-                        client = self.broker.get_client(param)
-                        return client.infomap() if client is not None else None
-                    case "mountedClientInfo":
-                        if not isinstance(param, str):
-                            raise RpcInvalidParamsError("Use String with SHV path")
-                        client_pth = self.broker.client_on_path(param)
-                        if client_pth is not None:
-                            return client_pth[0].infomap()
-                        return None
-                    case "clients":
-                        return list(self.broker.clients.keys())
-                    case "mounts":
-                        return [
-                            "/".join(c.mount_point)
-                            for c in self.broker.clients.values()
-                            if c.mount_point
-                        ]
-                    case "disconnectClient":
-                        if not isinstance(param, int):
-                            raise RpcInvalidParamsError("Use Int")
-                        client = self.broker.get_client(param)
-                        if client is None:
-                            raise RpcMethodCallExceptionError(
-                                f"No such client with ID: {param}"
+            match path.split("/"):
+                case [".broker"] if access >= RpcMethodAccess.SUPER_SERVICE:
+                    match method:
+                        case "clientInfo":
+                            if not isinstance(param, int):
+                                raise RpcInvalidParamsError("Use Int")
+                            client = self.broker.get_client(param)
+                            return client.infomap() if client is not None else None
+                        case "mountedClientInfo":
+                            if not isinstance(param, str):
+                                raise RpcInvalidParamsError("Use String with SHV path")
+                            client_pth = self.broker.client_on_path(param)
+                            if client_pth is not None:
+                                return client_pth[0].infomap()
+                            return None
+                        case "clients":
+                            return list(
+                                c.broker_client_id for c in self.broker.clients()
                             )
-                        await client.disconnect()
-                        return None
-            elif path == ".app/broker/currentClient":
-                match method:
-                    case "info":
-                        return self.infomap()
-                    case "subscriptions":
-                        return self.subslist()
-                    case "subscribe":
-                        sub = RpcSubscription.fromSHV(param)
-                        self.subscriptions.add(sub)
-                        async for subb in self.broker.subbrokers():
-                            assert subb.mount_point is not None
-                            if self.user.could_receive_signal(sub, subb.mount_point):
-                                if subsub := sub.relative_to(subb.mount_point):
-                                    await subb.subscribe(subsub)
-                        return None
-                    case "unsubscribe":
-                        sub = RpcSubscription.fromSHV(param)
-                        try:
-                            self.subscriptions.remove(sub)
-                        except KeyError:
-                            return False
-                        async for subb in self.broker.subbrokers():
-                            await subb.maintain_subscriptions()
-                        return True
-                    case "rejectNotSubscribed":
-                        method = shvget(param, "method", str, "chng")
-                        path = shvget(param, "path", str, "")
-                        match = {
-                            sub
-                            for sub in self.subscriptions
-                            if sub.applies(path, method)
-                        }
-                        self.subscriptions -= match
-                        return [
-                            {"method": sub.method, "path": sub.path} for sub in match
-                        ]
-            elif (
-                path.startswith(".app/broker/clientInfo/")
-                and (client := self.broker.get_client(path[23:])) is not None
-                and access >= RpcMethodAccess.SUPER_SERVICE
-            ):
-                match method:
-                    case "userName":
-                        return client.user.name if client.user is not None else None
-                    case "mountPoint":
-                        return "/".join(self.mount_point) if self.mount_point else None
-                    case "subscriptions":
-                        return client.subslist()
-                    case "dropClient":
-                        await client.disconnect()
-                        return None
-                    case "idleTime":
-                        return int(
-                            (time.monotonic() - client.client.last_receive) * 1000
-                        )
-                    case "idleTimeMax":
-                        return int(self.IDLE_TIMEOUT * 1000)
-            return await super()._method_call(path, method, access, param)
+                        case "mounts":
+                            return [mnt for mnt, _ in self.broker.mounted_clients()]
+                        case "disconnectClient":
+                            if not isinstance(param, int):
+                                raise RpcInvalidParamsError("Use Int")
+                            client = self.broker.get_client(param)
+                            if client is None:
+                                raise RpcMethodCallExceptionError(
+                                    f"No such client with ID: {param}"
+                                )
+                            await client.disconnect()
+                            return None
+                case [".broker", "currentClient"]:
+                    match method:
+                        case "info":
+                            return self.infomap()
+                        case "subscriptions":
+                            return [
+                                s.to_shv() for s in self.__broker.subscriptions(self)
+                            ]
+                        case "subscribe":
+                            sub = RpcSubscription.from_shv(param)
+                            return await self.__broker.subscribe(sub, self)
+                        case "unsubscribe":
+                            sub = RpcSubscription.from_shv(param)
+                            return await self.__broker.unsubscribe(sub, self)
+            return await super()._method_call(path, method, param, access, user_id)
 
         def infomap(self) -> SHVType:
             """Produce Map with client's info.
 
-            This is primarilly used internally by SVH Broker. You most likely won't have
-            use for it outside of SHV Broker context.
+            This is info provided to administator to inform it about this
+            client.
             """
             return {
                 "clientId": self.broker_client_id,
                 "userName": self.user.name if self.user is not None else None,
-                "mountPoint": self.mount_point,
-                "subscriptions": self.subslist(),
+                "mountPoint": self.__broker.client_mountpoint(self),
+                "subscriptions": [
+                    s.to_shv() for s in self.__broker.subscriptions(self)
+                ],
+                "idleTime": int((time.monotonic() - self.client.last_receive) * 1000),
+                "idleTimeMax": int(self.IDLE_TIMEOUT * 1000),
             }
 
-        def subslist(self) -> SHVType:
-            """Produce List of all client's subscriptions.
+        async def disconnect(self) -> None:  # noqa: D102
+            logger.info("Disconnecting client with ID %d", self.broker_client_id)
+            self.__broker._unregister_client(self)  # pylint: disable=protected-access
+            await super().disconnect()
 
-            This is primarilly used internally by SVH Broker. You most likely won't have
-            use for it outside of SHV Broker context.
-            """
-            return [{"method": s.method, "path": s.path} for s in self.subscriptions]
+    class LoginClient(Client):
+        """Broker's client that expects login from client."""
+
+        APP_NAME = "pyshvbroker"
+        """Name reported as application name for pyshvbroker."""
+
+        IDLE_TIMEOUT_LOGIN: float = 5
+        """:attr:`IDLE_TIMEOUT` set for clients without user.
+
+        This is intentionally shorter to quickly disconnect inactive clients
+        that are not participating in SHV RPC.
+        """
+
+        def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:  # noqa ANN204
+            super().__init__(*args, **kwargs)
+            self.IDLE_TIMEOUT = self.IDLE_TIMEOUT_LOGIN
+            self._nonce: str = ""
 
-        async def maintain_subscriptions(self, cleanup: bool = True) -> None:
-            """Remove no longer valid subscriptions and add missing ones.
+        async def _loop(self) -> None:
+            activity_task = asyncio.create_task(self._activity_loop())
+            await super()._loop()
+            activity_task.cancel()
+            with contextlib.suppress(asyncio.exceptions.CancelledError):
+                await activity_task
 
-            This does nothing if peer of this client is not sub-broker.
+            self.broker._unregister_client(self)  # pylint: disable=protected-access
+            self.client.disconnect()
+            await self.client.wait_disconnect()
+            logger.info("Client with ID %d disconnected", self.broker_client_id)
 
-            :param cleanup: If cleanup should be performed or if it is enough to
-            just push all subscriptions.
+        async def _activity_loop(self) -> None:
+            """Loop run alongside with :meth:`_loop`.
+
+            It disconnects this client if it is idling.
             """
-            assert self.user is not None
-            if not await self.peer_is_broker():
+            while self.client.connected:
+                t = time.monotonic() - self.client.last_receive
+                if t < self.IDLE_TIMEOUT:
+                    await asyncio.sleep(self.IDLE_TIMEOUT - t)
+                else:
+                    await self.disconnect()
+
+        async def _message(self, msg: RpcMessage) -> None:
+            # Login is required before we start handling messages as we would.
+            if self.user is None:
+                if msg.is_request:
+                    await self._send(self._message_login(msg))
                 return
-            # We lock here because we do multiple calls and we must be sure that nobody
-            # is going to be doing the same as us.
-            async with self.__maintain_subscriptions_lock:
-                present: set[RpcSubscription] = set()
-                required: set[RpcSubscription] = set()
-                if cleanup:
-                    rsubs = await self.call(
-                        ".app/broker/currentClient", "subscriptions"
-                    )
-                    # TODO error instead of assert
-                    assert isinstance(rsubs, collections.abc.Sequence)
-                    present = {RpcSubscription.fromSHV(sub) for sub in rsubs}
-                if self.mount_point is not None:
-                    for client in self.broker.clients.values():
-                        if client.user is None:
-                            continue
-                        for sub in client.subscriptions:
-                            if client.user.could_receive_signal(sub, self.mount_point):
-                                if subsub := sub.relative_to(self.mount_point):
-                                    required.add(subsub)
-                for sub in present - required:
-                    await self.unsubscribe(sub)
-                for sub in required - present:
-                    await self.subscribe(sub)
+            await super()._message(msg)
 
-        async def disconnect(self) -> None:
-            logger.info("Disconnecting client with ID %d", self.broker_client_id)
-            self.broker.clients.pop(self.broker_client_id, None)
-            await super().disconnect()
+        def _message_login(self, msg: RpcMessage) -> RpcMessage:
+            if not msg.path:
+                if msg.method == "hello":
+                    self._nonce = "".join(random.choices(string.hexdigits, k=10))  # noqa S311
+                    return msg.make_response({"nonce": self._nonce})
+                if self._nonce and msg.method == "login":
+                    param = msg.param
+                    if not is_shvmap(param):
+                        return msg.make_response(
+                            error=RpcInvalidParamsError("Invalid type of parameters")
+                        )
+                    self.user = self.broker.config.login(
+                        shvgett(param, ("login", "user"), str, ""),
+                        shvgett(param, ("login", "password"), str, ""),
+                        self._nonce,
+                        RpcLoginType(
+                            shvgett(
+                                param, ("login", "type"), str, RpcLoginType.SHA1.value
+                            )
+                        ),
+                    )
+                    if self.user is None:
+                        return msg.make_response(
+                            error=RpcMethodCallExceptionError("Invalid login")
+                        )
+                    logger.info(
+                        "Client with ID %d logged in as user: %s",
+                        self.broker_client_id,
+                        self.user.name,
+                    )
+                    mount_point = shvgett(
+                        param, ("options", "device", "mountPoint"), str, ""
+                    )
+                    if self.broker.client_on_path(mount_point) is not None:
+                        return msg.make_response(
+                            error=RpcError(
+                                "Mount point already mounted",
+                                RpcErrorCode.METHOD_CALL_EXCEPTION,
+                            )
+                        )
+                    if mount_point:
+                        self.broker.mount_client(self, mount_point)
+                    self.IDLE_TIMEOUT = float(
+                        shvgett(
+                            param,
+                            ("options", "idleWatchDogTimeOut"),
+                            int,
+                            type(self).IDLE_TIMEOUT,
+                        )
+                    )
+                    return msg.make_response({"clientId": self.broker_client_id})
+            return msg.make_response(
+                error=RpcLoginRequiredError(
+                    "Use hello and login methods" if self._nonce else "Use hello method"
+                )
+            )
+
+        def _reset(self) -> None:
+            self._nonce = ""
+            self.user = None
+            super()._reset()
+
+    class ConnectClient(SimpleClient, Client):
+        """Broker client that activelly connects to some other peer."""
+
+        APP_NAME = "pyshvbroker-client"
+        """Name reported as application name for pyshvbroker connection."""
+
+        def __init__(
+            self,
+            *args: typing.Any,  # noqa ANN204
+            target_mount_point: str | None = None,
+            **kwargs: typing.Any,  # noqa ANN204
+        ) -> None:
+            super().__init__(*args, **kwargs)
+            self.target_mount_point = target_mount_point
+
+        async def _login(self) -> None:
+            await super()._login()
+            self.broker.mount_client(self, self.target_mount_point)
+
+        # TODO possibly add info about where it is connect to the infomap but we
+        # must not disclouse login information
 
     def __init__(self, config: RpcBrokerConfig) -> None:
-        self.clients: dict[int, RpcBroker.Client] = {}
-        """Mapping from client IDs to client objects."""
         self.config = config
         """Configuration of the RPC Broker."""
         self.servers: dict[str, RpcServer] = {}
         """All servers managed by Broker where keys are their configured names."""
-        self.__connection_tasks: dict[str, asyncio.Task] = {}
-        self.__next_caller_id = 0
-
-    def next_caller_id(self) -> int:
-        """Allocate new caller ID."""
-        # TODO try to reuse older caller IDs to send smaller messages but we need to do
-        # it only after some given delay. We can safe time of client disconnect to the
-        # self.clients and use that to identify when we can reuse caller id.
-        self.__next_caller_id += 1
-        return self.__next_caller_id - 1
-
-    def add_client(
-        self,
-        client: RpcClient,
-        user: RpcBrokerConfig.User | None = None,
-    ) -> Client:
-        """Add a new client to be handled by the broker.
-
-        :param client: RPC client instance to be handled by broker.
-        :param user: The user this client is logged in. Use ``None`` if you
-          require login from this client.
-        :return: The client instance in the broker.
-        """
-        return self.Client(client, self, user, idle_disconnect=True)
+        self._clients: dict[int, RpcBroker.Client] = {}
+        self._subs: dict[RpcSubscription, set[int]] = {}
+        self._mounts: dict[str, int] = {}
+        self._subsubs: dict[str, collections.Counter[RpcSubscription]] = {}
+        self.__last_caller_id = -1
+
+    def _register_client(self, client: Client) -> int:
+        """Register client that is called by :class:`Client` initialization."""
+        # TODO try to reuse older caller IDs to send smaller messages but we
+        # need to do it only after some given delay. We can safe time of client
+        # disconnect to the self.clients and use that to identify when we can
+        # reuse caller id.
+        self.__last_caller_id += 1
+        self._clients[self.__last_caller_id] = client
+        return self.__last_caller_id
+
+    def _unregister_client(self, client: Client) -> None:
+        """Unregister client that is called by :class:`Client` reset and teardown."""
+        self.mount_client(client, None)
+        for subs in self._subs.values():
+            subs.discard(client.broker_client_id)
+        self._clients.pop(client.broker_client_id, None)
 
-    def get_client(self, cid: int | str) -> typing.Union[Client, None]:
+    def get_client(self, cid: int | str) -> Client | None:
         """Lookup client with given ID.
 
         :param cid: ID of the client either as string or as integer.
         :return: :class:`RpcBroker.Client` when such client is located and ``None``
             otherwise.
         """
         try:
-            return self.clients[cid if isinstance(cid, int) else int(cid, 10)]
+            return self._clients[cid if isinstance(cid, int) else int(cid, 10)]
         except (ValueError, KeyError):
             return None
 
     def client_on_path(self, path: str) -> tuple[Client, str] | None:
         """Locate client mounted on given path.
 
         :return: client associated with this mount point and path relative to
             the client or None if there is no such client.
         """
-        if path.startswith(".app/broker/client/"):
+        if path.startswith(".broker/client/"):
             pth = path.split("/")
-            client = self.get_client(pth[3])
-            return (client, "/".join(pth[4:])) if client else None
+            client = self.get_client(pth[2])
+            return (client, "/".join(pth[3:])) if client else None
 
         # Note: we do not allow recursive mount points and thus first match is the
         # correct and the only client.
-        for c in self.clients.values():
-            mp = c.mount_point
-            if (
-                mp
-                and path.startswith(mp)
-                and (len(path) == len(mp) or path[len(mp)] == "/")
-            ):
-                return c, path[len(c.mount_point or "") + 1 :]
+        for mnt, cid in self._mounts.items():
+            if path.startswith(mnt + "/") or path == mnt:
+                return self._clients[cid], path[len(mnt) + 1 :]
         return None
 
-    async def subbrokers(self) -> collections.abc.AsyncIterator[Client]:
-        """Iterate over all mounted clients that are brokers."""
-        for client in self.clients.values():
-            if client.user is None:
-                continue  # Ignore unlogged clients
-            if client.mount_point is not None and await client.peer_is_broker():
-                yield client
+    def clients(self) -> collections.abc.Iterator[Client]:
+        """Iterate over all clients of the broker."""
+        yield from self._clients.values()
+
+    def mounted_clients(self) -> collections.abc.Iterator[tuple[str, Client]]:
+        """Goes through all clients and provides those active and mounted."""
+        return (
+            (mnt, self._clients[cid])
+            for mnt, cid in self._mounts.items()
+            if self._clients[cid].active
+        )
+
+    def mount_client(self, client: Client, mount_point: str | None) -> asyncio.Task:
+        """Mount given client on given mount point.
+
+        :param client: The client ID or object that should be mounted.
+        :param mount_point: The mount point where client should be mounted.
+        :return: Asyncio task you can await to make sure that mount is fully
+          propagated.
+        """
+        cid = client.broker_client_id
+        if mount_point is not None:
+            mount_point = mount_point.rstrip("/")
+        if mount_point and any(
+            mnt.startswith(mount_point + "/")
+            for mnt, mntcid in self._mounts.items()
+            if mntcid != cid
+        ):
+            raise ValueError("Path already mounted")
+        oldmnt = self.client_mountpoint(client)
+        if oldmnt:
+            self._mounts.pop(oldmnt, None)
+            logger.info("Client with ID %d is no longer mounted on: %s", cid, oldmnt)
+        if mount_point:
+            self._mounts[mount_point] = cid
+            logger.info("Client with ID %d is now mounted on: %s", cid, mount_point)
+        return asyncio.create_task(self.__mount_client(client, oldmnt, mount_point))
+
+    async def __mount_client(
+        self, client: Client, oldmnt: str | None, newmnt: str | None
+    ) -> None:
+        prev = set(self._subsubs.pop(oldmnt, {}).keys()) if oldmnt else set()
+        if client.active and await client.peer_is_broker():
+            if newmnt:
+                self._subsubs[newmnt] = collections.Counter(
+                    s for sub in self._subs if (s := sub.relative_to(newmnt))
+                )
+                for s in self._subsubs[newmnt]:
+                    if s in prev:
+                        prev.discard(s)
+                    else:
+                        await client.call(
+                            ".broker/currentClient"
+                            if await client.peer_is_shv3()
+                            else ".broker/app",
+                            "subscribe",
+                            s.to_shv(not await client.peer_is_shv3()),
+                        )
+            for s in prev:
+                await client.call(
+                    ".broker/currentClient"
+                    if await client.peer_is_shv3()
+                    else ".broker/app",
+                    "unsubscribe",
+                    s.to_shv(not await client.peer_is_shv3()),
+                )
+
+        await self._signal_mount_point_change(*(mnt for mnt in (oldmnt, newmnt) if mnt))
+
+    def client_mountpoint(self, client: Client) -> str | None:
+        """Get mount point for this client.
+
+        :param client: The client ID or object that mount point should be
+          received for.
+        :return: The mount point of the client or ``None`` in case there is
+          none.
+        """
+        try:
+            return next(
+                mnt
+                for mnt, cid in self._mounts.items()
+                if cid == client.broker_client_id
+            )
+        except StopIteration:
+            return None
+
+    def subscriptions(
+        self, client: Client | None = None
+    ) -> collections.abc.Iterator[RpcSubscription]:
+        """Iterate over subscriptions this broker manages.
+
+        :param client: The optional filtering over client's subscriptions.
+        :return: Iterator over subscriptions.
+        """
+        yield from (
+            s
+            for s, v in self._subs.items()
+            if client is None or client.broker_client_id in v
+        )
+
+    async def subscribe(self, subscription: RpcSubscription, client: Client) -> bool:
+        """Add given subscription as being requested by given client."""
+        assert client.user is not None
+        if subscription in self._subs:
+            self._subs[subscription].add(client.broker_client_id)
+            return False
+        self._subs[subscription] = {client.broker_client_id}
+        # Propagate subscription to the sub-brokers
+        for mnt, subc in self.mounted_clients():
+            if not await subc.peer_is_broker():
+                continue
+            if sub := subscription.relative_to(mnt):
+                if mnt not in self._subsubs:
+                    self._subsubs[mnt] = collections.Counter()
+                self._subsubs[mnt][sub] += 1
+                if self._subsubs[mnt][sub] == 1:
+                    await subc.call(
+                        ".broker/currentClient"
+                        if await subc.peer_is_shv3()
+                        else ".broker/app",
+                        "subscribe",
+                        sub.to_shv(),
+                    )
+        return True
+
+    async def unsubscribe(self, subscription: RpcSubscription, client: Client) -> bool:
+        """Remove given subscription as being requested by given client."""
+        if subscription not in self._subs:
+            return False
+        self._subs[subscription].discard(client.broker_client_id)
+        if self._subs[subscription]:
+            return True
+        del self._subs[subscription]
+        # Propagate unsubscribe to the sub-brokers
+        for mnt, subc in self.mounted_clients():
+            if not await subc.peer_is_broker():
+                continue
+            if sub := subscription.relative_to(mnt):
+                self._subsubs[mnt][sub] -= 1
+                if self._subsubs[mnt][sub] == 0:
+                    del self._subsubs[mnt][sub]
+                    await subc.call(
+                        ".broker/currentClient"
+                        if await subc.peer_is_shv3()
+                        else ".broker/app",
+                        "unsubscribe",
+                        sub.to_shv(),
+                    )
+        return True
 
     async def signal(self, msg: RpcMessage) -> None:
         """Send signal to the broker's clients.
 
         :param msg: Signal message to be sent.
         """
         msgaccess = msg.rpc_access or RpcMethodAccess.READ
-        for client in self.clients.values():
-            if client.user is None:
+        for sub, clients in self._subs.items():
+            if not sub.applies(msg.path, msg.signal_name, msg.source):
                 continue
-            access = client.user.access_level(msg.path, msg.method)
-            if (
-                access is not None
-                and access >= msgaccess
-                and any(s.applies(msg.path, msg.method) for s in client.subscriptions)
-            ):
-                await client.client.send(msg)
+            for cid in clients:
+                client = self._clients[cid]
+                if not client.active:
+                    continue
+                assert client.user is not None
+                access = client.user.access_level(msg.path, msg.method)
+                if access is None or access < msgaccess:
+                    continue
+                await client.send(msg)
 
-    async def start_serving(self) -> None:
-        """Start accepting connectons on all configured servers."""
+    async def signal_from(self, msg: RpcMessage, client: Client) -> None:
+        """Send signal to the broker's client as comming from given client.
+
+        :param msg: Signal message to be sent.
+        :param client: Client ID or object signal should be propagated from.
+        """
+        if mnt := self.client_mountpoint(client):
+            msg.path = mnt + ("/" if msg.path else "") + msg.path
+            await self.signal(msg)
+
+    async def _signal_mount_point_change(self, *path: str) -> None:
+        """Send lsmod signal for node changes for given mount points.
+
+        The state of the mount point can be deduced from the current list of
+        them.
+
+        You most likely do not want to call this if you are just a Broker user.
+        It is used by broker's clients to inform all peers about mount point
+        changes. Think about before you use this in your application!
+        """
+        mounts = set(self._mounts)
+        constmounts = mounts.difference(path)
+        changes: dict[str, dict[str, bool]] = {}
+        for mp in path:
+            ggi = enumerate(zip(mp, *constmounts, strict=False))
+            gi = (i for i, ch in ggi if ch[0] not in ch[1:])
+            i = mp.find("/", next(gi, 0))
+            pth, _, name = mp[: i if i >= 0 else None].rpartition("/")
+            if pth not in changes:
+                changes[pth] = {}
+            changes[pth][name] = mp in mounts
+        for pth, value in changes.items():
+            await self.signal(
+                RpcMessage.signal(pth, "lsmod", "ls", value, RpcMethodAccess.BROWSE)
+            )
+
+    async def start_serving(self, connect_timeout: float = 1.0) -> None:
+        """Start accepting connections on all configured servers.
+
+        :param connect_timeout: The timeout before we stop waiting for
+           connections to be established.
+        """
 
         def add(client: RpcClient) -> None:
-            self.add_client(client)
+            self.LoginClient(client, self)
 
         for name, url in self.config.listen.items():
             if name not in self.servers:
                 self.servers[name] = await create_rpc_server(add, url)
-        for connection in self.config.connections():
-            if connection.name not in self.__connection_tasks:
-                self.__connection_tasks[connection.name] = asyncio.create_task(
-                    self._connection_task(connection)
-                )
 
-    async def _connection_task(self, connection: RpcBrokerConfig.Connection) -> None:
-        """Loop that connects client."""
-        timeout = 1
-        while True:
-            client = None
-            try:
-                client = await self.Client.connect(
-                    connection.url, self, connection.user
-                )
-                await client.client.wait_disconnect()
-            except Exception as exc:
-                logger.error(
-                    "Client connection '%s' failure (waiting %d secs): %s",
-                    connection.name,
-                    timeout,
-                    exc.message if isinstance(exc, RpcError) else exc,
-                )
-                await asyncio.sleep(timeout)
-                timeout = (timeout * 2) % 512
-            else:
-                timeout = 1
-            finally:
-                if client is not None:
-                    await client.disconnect()
+        async with asyncio.timeout(connect_timeout):
+            await asyncio.gather(
+                *(
+                    self.ConnectClient(
+                        init_rpc_client(connection.url),
+                        connection.url.login,
+                        self,
+                        user=connection.user,
+                        reconnects=-1,
+                    ).wait_for_login()
+                    for connection in self.config.connections()
+                ),
+                return_exceptions=True,
+            )
 
     async def serve_forever(self) -> None:
         """Serve all configured servers and block.
 
         This is a convenient coroutine that you can use to block main task until broker
         termination. You do not have to await this coroutine to run broker, awaiting on
         :meth:`start_serving` and keeping the loop running is enough to get broker
@@ -671,18 +732,17 @@
         )
 
     async def terminate(self) -> None:
         """Request termination of the broker.
 
         This closes broker as well as disconnects all established clients.
         """
-        self.close()
-        for connection in self.__connection_tasks.values():
-            connection.cancel()
+
+        async def client_disconnect(client: RpcBroker.Client) -> None:
             try:
-                await connection
-            except asyncio.CancelledError:
-                pass
+                await client.disconnect()
             except Exception as exc:
-                logger.error("Connection task failure: %s", exc)
+                logger.error("Disconnect failed", exc_info=exc)
+
+        self.close()
         await self.wait_closed()
-        await asyncio.gather(*(client.disconnect() for client in self.clients.values()))
+        await asyncio.gather(*(client_disconnect(c) for c in self._clients.values()))
```

### Comparing `pyshv-0.5.0/shv/broker/rpcbrokerconfig.py` & `pyshv-0.6.0/shv/broker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """Configuration of the broker."""
+
 from __future__ import annotations
 
 import collections.abc
 import configparser
 import dataclasses
 import hashlib
 import typing
 
 from ..rpcmethod import RpcMethodAccess
 from ..rpcsubscription import RpcSubscription
 from ..rpcurl import RpcLoginType, RpcUrl
 
 
 class RpcBrokerConfig:
-    """Generic store of broker configuration."""
+    """SHV RPC Broker configuration."""
 
     @dataclasses.dataclass(frozen=True)
     class Method:
         """Combination of method and SHV path."""
 
         path: str = ""
         """Path prefix that need to match for this to apply."""
         method: str = ""
         """Method name that should be matched. Empty matches all methods."""
 
         @classmethod
-        def fromstr(cls, string: str) -> "RpcBrokerConfig.Method":
+        def fromstr(cls, string: str) -> RpcBrokerConfig.Method:
             """Parse :class:`RpcBrokerConfig.Method` from string."""
             if ":" not in string:
                 raise ValueError(f"Invalid specification of method: {string}")
             return cls(*string.split(":", maxsplit=1))
 
         def applies(self, path: str, method: str) -> bool:
             """Check if this method applies to this combination of path and method."""
@@ -41,19 +42,19 @@
     class Role:
         """Generic roles assigned to the users."""
 
         name: str
         """Name of the role."""
         access: RpcMethodAccess = RpcMethodAccess.BROWSE
         """Access level granted to the user by this role."""
-        methods: frozenset["RpcBrokerConfig.Method"] = dataclasses.field(
+        methods: frozenset[RpcBrokerConfig.Method] = dataclasses.field(
             default_factory=frozenset
         )
         """Methods used to check if this role should apply."""
-        roles: frozenset["RpcBrokerConfig.Role"] = dataclasses.field(
+        roles: frozenset[RpcBrokerConfig.Role] = dataclasses.field(
             default_factory=frozenset
         )
         """Additional roles to applied after this role."""
 
         def applies(self, path: str, method: str) -> bool:
             """Check if this role applies on any method."""
             return any(rule.applies(path, method) for rule in self.methods)
@@ -61,39 +62,39 @@
     @dataclasses.dataclass(frozen=True)
     class User:
         """User's login information."""
 
         name: str
         password: str
         login_type: RpcLoginType | None = RpcLoginType.SHA1
-        roles: frozenset["RpcBrokerConfig.Role"] = dataclasses.field(
+        roles: frozenset[RpcBrokerConfig.Role] = dataclasses.field(
             default_factory=frozenset
         )
 
-        def all_roles(self) -> typing.Iterator["RpcBrokerConfig.Role"]:
+        def all_roles(self) -> typing.Iterator[RpcBrokerConfig.Role]:
             """Iterate over all roles assigned to this user."""
             rlst = list(self.roles)
             while rlst:
                 role = rlst.pop()
                 yield role
                 rlst.extend(role.roles)
 
         def access_level(self, path: str, method: str) -> RpcMethodAccess | None:
             """Deduce access level (if any) for this user on given path and method."""
             for role in self.all_roles():
                 if role.applies(path, method):
                     return role.access
             # These are defined paths we need to allow all users to access
-            if path == ".app/broker/currentClient":
+            if path == ".broker/currentClient":
                 return RpcMethodAccess.READ
-            if path in (".app", ".app/broker"):
+            if path in {".app", ".broker"}:
                 return RpcMethodAccess.BROWSE
             return None
 
-        def could_receive_signal(
+        def could_receive_signal(  # noqa PLR6301
             self, subscription: RpcSubscription, path: str = ""
         ) -> bool:
             """Check if this user could even receive signal based on this subscription.
 
             This is used to optimize subscriptions for sub-brokers. There is no
             need to propagate subscription if it couldn't be received by the
             user anyway.
@@ -112,33 +113,33 @@
             return True  # TODO
 
         @property
         def shapass(self) -> str:
             """Password in SHA1 format."""
             if self.login_type is RpcLoginType.SHA1:
                 return self.password
-            m = hashlib.sha1()
+            m = hashlib.sha1()  # noqa S324
             m.update(self.password.encode("utf-8"))
             return m.hexdigest()
 
         def validate_password(
             self,
             password: str,
             nonce: str,
             login_type: RpcLoginType = RpcLoginType.SHA1,
         ) -> bool:
             """Check if given password is correct."""
             if login_type is RpcLoginType.PLAIN:
                 if self.login_type is RpcLoginType.PLAIN:
                     return self.password == password
                 if self.login_type is RpcLoginType.SHA1:
-                    hpass = hashlib.sha1(password.encode("utf-8")).hexdigest()
+                    hpass = hashlib.sha1(password.encode("utf-8")).hexdigest()  # noqa PLR6301
                     return self.shapass == hpass
             if login_type is RpcLoginType.SHA1:
-                m = hashlib.sha1()
+                m = hashlib.sha1()  # noqa PLR6301
                 m.update(nonce.encode("utf-8"))
                 m.update(self.shapass.encode("utf-8"))
                 return m.hexdigest() == password
             return False
 
     @dataclasses.dataclass(frozen=True)
     class Connection:
@@ -147,14 +148,16 @@
         name: str
         url: RpcUrl
         user: RpcBrokerConfig.User
 
     def __init__(self) -> None:
         self.listen: dict[str, RpcUrl] = {}
         """URLs the broker should listen on."""
+        self.name: str = ""
+        """Name of the broker used to identify broker in UserID."""
         self._connect: dict[str, RpcBrokerConfig.Connection] = {}
         self._users: dict[str, RpcBrokerConfig.User] = {}
         self._roles: dict[str, RpcBrokerConfig.Role] = {}
 
     def add_connection(self, connection: Connection) -> None:
         """Add or replace connection.
 
@@ -233,36 +236,38 @@
 
     def roles(self) -> collections.abc.Iterator[Role]:
         """Iterate over all roles."""
         yield from self._roles.values()
 
     def login(
         self, user: str, password: str, nonce: str, login_type: RpcLoginType
-    ) -> typing.Optional["RpcBrokerConfig.User"]:
+    ) -> RpcBrokerConfig.User | None:
         """Check the login and provide user if login is correct."""
         try:
             u = self.user(user)
         except KeyError:
             pass
         else:
             if u.validate_password(password, nonce, login_type):
                 return u
         return None
 
     @classmethod
-    def load(cls, config: configparser.ConfigParser) -> "RpcBrokerConfig":
+    def load(cls, config: configparser.ConfigParser) -> RpcBrokerConfig:
         """Load configuration from ConfigParser.
 
         :param config: Configuration to be loaded.
         :return: Broker configuration instance.
         :raise ValueError: When there is an issue in the configuration.
         :raise KeyError: When referencing non-existent user or role.
         """
         # TODO do not ignore uknown options and sections
         res = cls()
+        if "config" in config:
+            res.name = config["config"].get("name", "")
         if "listen" in config:
             for name, url in config["listen"].items():
                 res.listen[name] = RpcUrl.parse(url)
         for secname, sec in filter(lambda v: v[0].startswith("roles."), config.items()):
             res.add_role(
                 cls.Role(
                     secname[6:],
```

### Comparing `pyshv-0.5.0/shv/chainpack.py` & `pyshv-0.6.0/shv/chainpack.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Chainpack data format reader and writer."""
-import collections.abc
+
 import datetime
 import decimal
 import io
 import struct
 import typing
 
 from . import commonpack
@@ -91,21 +91,21 @@
         writer.write_uint_data(value)
         return bio.getvalue()
 
 
 class ChainPackReader(commonpack.CommonReader):
     """Read data in ChainPack format."""
 
-    def read_meta(self) -> SHVMetaType | None:
+    def read_meta(self) -> SHVMetaType | None:  # noqa: D102
         if self._peek_byte() != ChainPack.CP_MetaMap:
             return None
         self._peek_drop()
         return self._read_map()
 
-    def read(self) -> SHVType:
+    def read(self) -> SHVType:  # noqa: D102
         meta = self.read_meta()
 
         value: SHVType
         packing_schema = self._read_byte()
         if packing_schema < 128:
             # tiny Int or UInt
             value = packing_schema & 63
@@ -141,15 +141,15 @@
             value = self._read_cstring()
         else:
             raise ValueError(f"ChainPack - Invalid type: {packing_schema}")
         if meta is not None:
             value = SHVMeta.new(value, meta)
         return value
 
-    def _read_uint_dataHelper(self) -> tuple[int, int]:
+    def _read_uint_data_helper(self) -> tuple[int, int]:
         num = 0
         bitlen = 0
         head = self._read_byte()
         if (head & 128) == 0:
             bytes_to_read_cnt = 0
             num = head & 127
             bitlen = 7
@@ -170,20 +170,20 @@
             bitlen = bytes_to_read_cnt * 8
 
         for _ in range(bytes_to_read_cnt):
             r = self._read_byte()
             num = (num << 8) + r
         return num, bitlen
 
-    def read_uint_data(self) -> int:
-        num, _ = self._read_uint_dataHelper()
+    def read_uint_data(self) -> int:  # noqa: D102
+        num, _ = self._read_uint_data_helper()
         return num
 
     def _read_int_data(self) -> int:
-        num, bitlen = self._read_uint_dataHelper()
+        num, bitlen = self._read_uint_data_helper()
         sign_bit_mask = 1 << (bitlen - 1)
         neg = num & sign_bit_mask
         snum = num
         if neg:
             snum &= ~sign_bit_mask
             snum = -snum
         return snum
@@ -255,15 +255,15 @@
         mmap: dict[str | int, SHVType] = {}
         while True:
             b = self._peek_byte()
             if b == ChainPack.CP_TERM:
                 self._read_byte()
                 break
             key = self.read()
-            if not isinstance(key, (str, int)):
+            if not isinstance(key, str | int):
                 raise ValueError(f"Invalid Map key: {type(key)}")
             val = self.read()
             mmap[key] = val
         return mmap
 
 
 class ChainPackWriter(commonpack.CommonWriter):
@@ -276,175 +276,145 @@
     # 22 ... 28 bits  4  bytes |1|1|1|0|s|x|x|x| |x|x|x|x|x|x|x|x| |x|x|x|x|x|x|x|x| |x|x|x|x|x|x|x|x|<-- LSB
     # 29+       bits  5+ bytes |1|1|1|1|n|n|n|n| |s|x|x|x|x|x|x|x| |x|x|x|x|x|x|x|x| |x|x|x|x|x|x|x|x| ... <-- LSB
     #                                         n ==  0 ->  4 bytes number (32 bit number)
     #                                         n ==  1 ->  5 bytes number
     #                                         n == 14 -> 18 bytes number
     #                                         n == 15 -> for future (number of bytes will be specified in next byte)
 
-    @staticmethod
-    def _significant_bits_part_length(num: int) -> int:
-        length = 0
-        if num & 0xFFFFFFFF00000000:
-            length += 32
-            num >>= 32
-        if num & 0xFFFF0000:
-            length += 16
-            num >>= 16
-        if num & 0xFF00:
-            length += 8
-            num >>= 8
-        if num & 0xF0:
-            length += 4
-            num >>= 4
-        # see https://en.wikipedia.org/wiki/Find_first_set#CLZ
-        sig_table_4bit = [0, 1, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 4, 4, 4]
-        length += sig_table_4bit[num]
-        return max(length, 1)
-
     @classmethod
     def _bytes_needed(cls, bit_len: int) -> int:
         """Calculate needed maximum number of bytes.
 
         Return max bit length >= bit_len, which can be encoded by same number of
         bytes number of bytes needed to encode bit_len.
         """
         if bit_len <= 28:
             cnt = ((bit_len - 1) // 7) + 1
         else:
             cnt = ((bit_len - 1) // 8) + 2
-        return cnt
+        return cnt or 1  # Always at least one byte is needed
 
     @classmethod
     def _expand_bit_len(cls, bit_len: int) -> int:
         byte_cnt = cls._bytes_needed(bit_len)
         if bit_len <= 28:
             ret = byte_cnt * (8 - 1) - 1
         else:
             ret = (byte_cnt - 1) * 8 - 1
         return ret
 
     def _write_uint_data_helper(self, num: int, bit_len: int) -> None:
         byte_cnt = self._bytes_needed(bit_len)
         data = bytearray(byte_cnt)
         for i in range(byte_cnt - 1, -1, -1):
-            r = num & 255
-            data[i] = r
+            data[i] = num & 0xFF
             num = num >> 8
 
         if bit_len <= 28:
             mask = 0xF0 << (4 - byte_cnt)
             data[0] = data[0] & ~mask
             mask = (mask << 1) & 0xFF
             data[0] = data[0] | mask
         else:
             data[0] = 0xF0 | (byte_cnt - 5)
 
         for i in range(0, byte_cnt):
-            r = data[i]
-            self._write(r)
+            self._write(data[i])
 
-    def write_meta(self, meta: SHVMetaType) -> None:
+    def write_meta(self, meta: SHVMetaType) -> None:  # noqa: D102
         self._write(ChainPack.CP_MetaMap)
         for k, v in meta.items():
             self.write(k)
             self.write(v)
         self._write(ChainPack.CP_TERM)
 
-    def write_null(self) -> None:
+    def write_null(self) -> None:  # noqa: D102
         self._write(ChainPack.CP_Null)
 
-    def write_bool(self, value: bool) -> None:
+    def write_bool(self, value: bool) -> None:  # noqa: D102
         self._write(ChainPack.CP_TRUE if value else ChainPack.CP_FALSE)
 
-    def write_blob(self, value: bytes | bytearray) -> None:
+    def write_blob(self, value: bytes | bytearray) -> None:  # noqa: D102
         self._write(ChainPack.CP_Blob)
         self.write_uint_data(len(value))
         self._write(value)
 
-    def write_string(self, value: str) -> None:
+    def write_string(self, value: str) -> None:  # noqa: D102
         bstring = value.encode("utf-8")
         self._write(ChainPack.CP_String)
         self.write_uint_data(len(bstring))
         self._write(bstring)
 
-    def write_cstring(self, value: str) -> None:
+    def write_cstring(self, value: str) -> None:  # noqa: D102
         bstring = value.encode("utf-8")
         self._write(ChainPack.CP_CString)
         self._write(bstring)
         self._write(b"\0")
 
-    def write_uint(self, value: int) -> None:
+    def write_uint(self, value: int) -> None:  # noqa: D102
         if value < 64:
             self._write(value % 64)
         else:
             self._write(ChainPack.CP_UInt)
             self.write_uint_data(value)
 
-    def write_uint_data(self, value: int) -> None:
-        bitcnt = self._significant_bits_part_length(value)
+    def write_uint_data(self, value: int) -> None:  # noqa: D102
+        bitcnt = value.bit_length()
         self._write_uint_data_helper(value, bitcnt)
 
-    def write_int(self, value: int) -> None:
+    def write_int(self, value: int) -> None:  # noqa: D102
         if 0 <= value < 64:
             self._write((value % 64) + 64)
         else:
             self._write(ChainPack.CP_Int)
             self.write_int_data(value)
 
-    def write_int_data(self, value: int) -> None:
-        num = -value if value < 0 else value
-        neg = value < 0
+    def write_int_data(self, value: int) -> None:  # noqa: D102
+        num: int = abs(value)
+        neg: bool = value < 0
 
-        bitlen = self._significant_bits_part_length(num)
+        bitlen = num.bit_length()
         bitlen += 1  # add sign bit
         if neg:
             sign_pos = self._expand_bit_len(bitlen)
             sign_bit_mask = 1 << sign_pos
             num |= sign_bit_mask
         self._write_uint_data_helper(num, bitlen)
 
-    def write_double(self, value: float) -> None:
+    def write_double(self, value: float) -> None:  # noqa: D102
         self._write(ChainPack.CP_Double)
         self._write(struct.pack("<d", value))  # little endian
 
-    def write_decimal(self, value: decimal.Decimal) -> None:
+    def write_decimal(self, value: decimal.Decimal) -> None:  # noqa: D102
         mantissa, exponent = decimal_rexp(value)
         self._write(ChainPack.CP_Decimal)
         self.write_int_data(mantissa)
         self.write_int_data(exponent)
 
-    def write_list(self, value: collections.abc.Iterable[SHVType]) -> None:
+    def write_list(self, value: SHVListType) -> None:  # noqa: D102
         self._write(ChainPack.CP_List)
         for val in value:
             self.write(val)
         self._write(ChainPack.CP_TERM)
 
-    def _write_map_data(
-        self, mmap: collections.abc.Mapping[str | int, SHVType]
-    ) -> None:
-        for k, v in mmap.items():
-            self.write(k)
-            self.write(v)
-        self._write(ChainPack.CP_TERM)
-
-    def write_map(self, value: collections.abc.Mapping[str, SHVType]) -> None:
+    def write_map(self, value: SHVMapType) -> None:  # noqa: D102
         self._write(ChainPack.CP_Map)
         for k, v in value.items():
             self.write(k)
             self.write(v)
         self._write(ChainPack.CP_TERM)
 
-    def write_imap(self, value: collections.abc.Mapping[int, SHVType]) -> None:
+    def write_imap(self, value: SHVIMapType) -> None:  # noqa: D102
         self._write(ChainPack.CP_IMap)
         for k, v in value.items():
             self.write(k)
             self.write(v)
         self._write(ChainPack.CP_TERM)
 
-    def write_datetime(self, value: datetime.datetime) -> None:
+    def write_datetime(self, value: datetime.datetime) -> None:  # noqa: D102
         self._write(ChainPack.CP_DateTime)
         res = int(value.timestamp() * 1000) - (ChainPack.SHV_EPOCH_SEC * 1000)
         tzdelta = value.utcoffset()
         tzoff = int(tzdelta.total_seconds() // 60 // 15) if tzdelta is not None else 0
         if not -63 <= tzoff <= 63:
             raise ValueError(f"Invalid UTC offset value: {tzoff}")
         ms = res % 1000 == 0
```

### Comparing `pyshv-0.5.0/shv/commonpack.py` & `pyshv-0.6.0/shv/commonpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Common base for SHV writers and readers."""
+
 import abc
 import asyncio
 import collections.abc
 import datetime
 import decimal
 import io
 import typing
 
 from .value import (
+    SHVIMapType,
+    SHVListType,
+    SHVMapType,
     SHVMetaType,
     SHVType,
     SHVUInt,
     is_shvbool,
     is_shvimap,
     is_shvmap,
     is_shvnull,
@@ -21,23 +25,23 @@
 
 class CommonReader(abc.ABC):
     """Common reader base."""
 
     def __init__(
         self, stream: typing.Union[bytes, bytearray, typing.IO, "CommonReader"]
     ) -> None:
-        if isinstance(stream, (bytes, bytearray)):
+        if isinstance(stream, bytes | bytearray):
             stream = io.BytesIO(stream)
         if isinstance(stream, CommonReader):
             orig = stream
             stream = stream.stream
 
         self.stream: typing.IO = stream
         """Stream used to receive bytes from."""
-        self.peek_bytes = bytes()
+        self.peek_bytes = b""
         """Peeked bytes so far."""
         self.bytes_cnt = 0
         """Number of bytes read so far."""
 
         if isinstance(stream, CommonReader):
             self.peek_bytes = orig.peek_bytes
             self.bytes_cnt = orig.bytes_cnt
@@ -48,15 +52,15 @@
         Compared to regular read this reads always given number of bytes.
 
         :param size: Number of bytes to read.
         :return: Read bytes.
         :raise EOFError: in case EOF is encountered.
         """
         assert size > 0
-        res = bytes()
+        res = b""
         while len(res) < size:
             read = self.read_raw(size - len(res))
             if len(read) == 0:
                 raise EOFError("End of message or file encountered.")
             res += read
         self.bytes_cnt += size
         return res
@@ -85,26 +89,26 @@
             except EOFError:
                 return 0
         return self.peek_bytes[0]
 
     def _peek_drop(self) -> None:
         """Drop peeked data."""
         self.bytes_cnt += len(self.peek_bytes)
-        self.peek_bytes = bytes()
+        self.peek_bytes = b""
 
     def _read_check(self, data: bytes) -> None:
         """Read bytes and check that it is what we expected.
 
         :param data: Expected bytes.
         :raise ValueError: when unexpected byte was received.
         :raise EOFError: in case EOF is encountered.
         """
         b = self._read(len(data))
         if data != b:
-            raise ValueError(f"Expected {repr(data)} but got {repr(b)}")
+            raise ValueError(f"Expected {data!r} but got {b!r}")
 
     def read_raw(self, size: int) -> bytes:
         """Read raw bytes from the stream."""
         res = self.peek_bytes[:size]
         self.peek_bytes = self.peek_bytes[size:]
         if len(res) < size:
             res = res + self.stream.read(size - len(res))
@@ -171,19 +175,19 @@
         elif isinstance(value, str):
             self.write_string(value)
         elif isinstance(value, datetime.datetime):
             self.write_datetime(value)
         elif isinstance(value, collections.abc.Sequence):
             self.write_list(value)
         elif is_shvimap(value):
-            self.write_imap(value)  # type: ignore
+            self.write_imap(value)
         elif is_shvmap(value):
-            self.write_map(value)  # type: ignore
+            self.write_map(value)
         else:
-            raise ValueError(f"Invalid value for SHV: {repr(value)}")
+            raise ValueError(f"Invalid value for SHV: {value!r}")
 
     @abc.abstractmethod
     def write_meta(self, meta: SHVMetaType) -> None:
         """Write given meta to the stream."""
 
     @abc.abstractmethod
     def write_null(self) -> None:
@@ -218,23 +222,23 @@
         """Write floating point number to the stream."""
 
     @abc.abstractmethod
     def write_decimal(self, value: decimal.Decimal) -> None:
         """Write decimal number to the stream."""
 
     @abc.abstractmethod
-    def write_list(self, value: collections.abc.Sequence[SHVType]) -> None:
+    def write_list(self, value: SHVListType) -> None:
         """Write list of other types to the stream."""
 
     @abc.abstractmethod
-    def write_map(self, value: collections.abc.Mapping[str, SHVType]) -> None:
+    def write_map(self, value: SHVMapType) -> None:
         """Write map of other types to the stream."""
 
     @abc.abstractmethod
-    def write_imap(self, value: collections.abc.Mapping[int, SHVType]) -> None:
+    def write_imap(self, value: SHVIMapType) -> None:
         """Write integer map of other types to the stream."""
 
     @abc.abstractmethod
     def write_datetime(self, value: datetime.datetime) -> None:
         """Write date and time to the stream."""
 
     @classmethod
```

### Comparing `pyshv-0.5.0/shv/cp2cp/__main__.py` & `pyshv-0.6.0/shv/cpconv/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Implementation of CPON ChainPack conversion tool."""
+
 import argparse
 import functools
 import sys
 
-from .. import VERSION, cpon
-from .cp2cp import CPFormat, convert
+from .. import cpon
+from ..__version__ import VERSION
+from .cpconv import CPFormat, convert
 
 
 def parse_args() -> argparse.Namespace:
     """Parse passed arguments and return result."""
     parser = argparse.ArgumentParser(
         "pycp2cp2", description="Chainpack to Cpon and vice versa converter"
     )
```

### Comparing `pyshv-0.5.0/shv/cp2cp/cp2cp.py` & `pyshv-0.6.0/shv/cpconv/cpconv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The implementation of conversion."""
+
 import enum
 import io
 import pathlib
 import typing
 
 from ..chainpack import ChainPackReader, ChainPackWriter
 from ..commonpack import CommonReader, CommonWriter
```

### Comparing `pyshv-0.5.0/shv/cpon.py` & `pyshv-0.6.0/shv/cpon.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Cpon data format reader and writer."""
+
 import collections.abc
 import dataclasses
 import datetime
 import decimal
 import io
 import typing
 
-import dateutil.parser
-
 from . import commonpack
 from .value import (
     SHVIMapType,
     SHVListType,
     SHVMapType,
     SHVMeta,
     SHVMetaType,
@@ -65,30 +64,30 @@
                         # to end of line comment entered
                         while True:
                             b = self._read_byte()
                             if b == ord("\n"):
                                 break
                     else:
                         raise ValueError("Malformed comment")
-                elif b in (ord(":"), ord(",")):
+                elif b in {ord(":"), ord(",")}:
                     self._peek_drop()
                     continue
                 else:
                     break
             else:
                 self._peek_drop()
 
-    def read_meta(self) -> SHVMetaType | None:
+    def read_meta(self) -> SHVMetaType | None:  # noqa: D102
         self._skip_white_insignificant()
         b = self._peek_byte()
         if b != ord("<"):
             return None
         return self._read_map(">")
 
-    def read(self) -> SHVType:
+    def read(self) -> SHVType:  # noqa: D102
         meta = self.read_meta()
 
         value: SHVType
         self._skip_white_insignificant()
         b = self._peek_byte()
         if ord("0") <= b <= ord("9") or b == ord("+") or b == ord("-"):
             value = self._new_read_number()
@@ -141,15 +140,15 @@
         self._peek_drop()  # eat '"'
         date = ""
         while True:
             c = chr(self._read_byte())
             if c == '"':
                 break
             date += c
-        return dateutil.parser.isoparse(date)
+        return datetime.datetime.fromisoformat(date)
 
     @staticmethod
     def _hexdigit_to_int(b: int) -> int:
         if ord("0") <= b <= ord("9"):
             val = b - 48
         elif ord("a") <= b <= ord("f"):
             val = b - ord("a") + 10
@@ -255,15 +254,15 @@
         while True:
             self._skip_white_insignificant()
             b = self._peek_byte()
             if b == ord(terminator):
                 self._peek_drop()
                 break
             key = self.read()
-            if not isinstance(key, (str, int)):
+            if not isinstance(key, str | int):
                 raise ValueError(f"Invalid Map key: {type(key)}")
             self._skip_white_insignificant()
             val = self.read()
             res[key] = val
         return res
 
     def _new_read_number(self) -> int | SHVUInt | decimal.Decimal:
@@ -272,15 +271,15 @@
         def accept(possib: bytes) -> int | None:
             b = self._peek_byte()
             if b not in possib:
                 return None
             bval.append(self._read_byte())
             return b
 
-        tp: typing.Type = int
+        tp: type = int
         parsed = False
         nonempty = False
         accept(b"-+")
         if accept(b"0") is not None:
             if accept(b"x") is not None:
                 while accept(b"0123456789AaBbCcDdEeFf") is not None:
                     nonempty = True
@@ -290,36 +289,36 @@
                     nonempty = True
                 parsed = True
         if not parsed:
             exp = False
             while True:
                 lb = accept(
                     b"0123456789.ueE"
-                    if tp == int
+                    if tp is int
                     else b"0123456789"
                     if exp
                     else b"0123456789eE"
                 )
                 if lb == ord("."):
                     tp = decimal.Decimal
-                elif lb in (ord("e"), ord("E")):
+                elif lb in {ord("e"), ord("E")}:
                     tp = decimal.Decimal
                     accept(b"-+")
                     exp = True
                 elif lb == ord("u"):
                     tp = SHVUInt
                     bval.pop()  # remove "u" from bytes
                     break
                 elif lb is None:
                     break
                 nonempty = True
         if not nonempty:
             bval.append(ord("0"))
 
-        if tp in (int, SHVUInt):
+        if tp in {int, SHVUInt}:
             return tp(bval, 0)  # type: ignore
         if tp == decimal.Decimal:
             return tp(bval.decode("ascii"))  # type: ignore
         assert False  # should be unreachable
 
 
 class CponWriter(commonpack.CommonWriter):
@@ -328,41 +327,43 @@
     @dataclasses.dataclass
     class Options:
         """Options for the CponWriter."""
 
         indent: bytes = b""
         """Bytes or string used to indent the code."""
 
-    def __init__(self, stream: typing.IO | None = None, options: Options | None = None):
+    def __init__(
+        self, stream: typing.IO | None = None, options: Options | None = None
+    ) -> None:
         super().__init__(stream)
         self.options = options if options is not None else self.Options()
         self._nest_level = 0
 
     def _indent_item(self, is_online_container: bool, item_index: int) -> None:
         if not self.options.indent:
             return
         if is_online_container:
             if item_index > 0:
                 self._writestr(" ")
         else:
             self._writestr("\n")
             self._write(self.options.indent * self._nest_level)
 
-    def write_meta(self, meta: SHVMetaType) -> None:
+    def write_meta(self, meta: SHVMetaType) -> None:  # noqa: D102
         self._writestr("<")
         self._write_map_content(meta)
         self._writestr(">")
 
-    def write_null(self) -> None:
+    def write_null(self) -> None:  # noqa: D102
         self._writestr("null")
 
-    def write_bool(self, value: bool) -> None:
+    def write_bool(self, value: bool) -> None:  # noqa: D102
         self._writestr("true" if value else "false")
 
-    def write_blob(self, value: bytes | bytearray) -> None:
+    def write_blob(self, value: bytes | bytearray) -> None:  # noqa: D102
         self._writestr('b"')
         for d in value:
             if d >= 0x7F:
                 self._writestr("\\")
                 self._writestr(self._nibble_to_hexdigit(d // 16))
                 self._writestr(self._nibble_to_hexdigit(d % 16))
             else:
@@ -384,18 +385,18 @@
         if b >= 0:
             if b < 10:
                 return chr(b + ord("0"))
             if b < 16:
                 return chr(b - 10 + ord("a"))
         raise ValueError(f"Invalid nibble value: {b}")
 
-    def write_string(self, value: str) -> None:
+    def write_string(self, value: str) -> None:  # noqa: D102
         self.write_cstring(value)
 
-    def write_cstring(self, value: str) -> None:
+    def write_cstring(self, value: str) -> None:  # noqa: D102
         self._writestr('"')
         for d in value:
             self._writestr(
                 {
                     "\0": "\\0",
                     "\\": "\\\\",
                     "\t": "\\t",
@@ -403,81 +404,81 @@
                     "\r": "\\r",
                     "\n": "\\n",
                     '"': '\\"',
                 }.get(d, d)
             )
         self._writestr('"')
 
-    def write_int(self, value: int) -> None:
+    def write_int(self, value: int) -> None:  # noqa: D102
         self._writestr(str(value))
 
-    def write_uint(self, value: int) -> None:
+    def write_uint(self, value: int) -> None:  # noqa: D102
         self._writestr(f"{value}u")
 
-    def write_double(self, value: float) -> None:
+    def write_double(self, value: float) -> None:  # noqa: D102
         self._writestr(str(value))
 
-    def write_decimal(self, value: decimal.Decimal) -> None:
+    def write_decimal(self, value: decimal.Decimal) -> None:  # noqa: D102
         sval = str(value)
         if not any(c in ".eE" for c in sval):
             sval = sval + ".0"
         self._writestr(sval)
 
-    def write_datetime(self, value: datetime.datetime) -> None:
-        # TODO possibly just use datetime iso format
+    def write_datetime(self, value: datetime.datetime) -> None:  # noqa: D102
+        # We perform here some modification to make the format more compact in
+        # some cases. This is not essentailly required but makes it more
+        # compatible with other implementations.
         self._writestr('d"')
-        DT_LEN = 19
-        dt_str = value.isoformat()
-        self._writestr(dt_str[:DT_LEN])
-        dt_str = dt_str[DT_LEN:]
-        if len(dt_str) > 0 and dt_str[0] == ".":
-            self._writestr(dt_str[:4])
-            dt_str = dt_str[7:]
-        if dt_str[:6] == "+00:00":
+        rstr = value.isoformat(
+            timespec="milliseconds" if value.microsecond else "seconds"
+        )
+        rlen = 23 if value.microsecond else 19
+        self._writestr(rstr[:rlen])
+        rstr = rstr[rlen:]
+        if rstr[:6] == "+00:00":
             self._writestr("Z")
-        elif dt_str[:1] == "Z":
-            self._writestr(dt_str)
-        elif dt_str[:1] == "+" or dt_str[:1] == "-":
-            self._writestr(dt_str[:3])
-            min_part = dt_str[4:6]
-            if min_part != "00":
-                self._writestr(min_part)
+        elif rstr[:1] == "Z":
+            self._writestr(rstr)
+        elif rstr[:1] == "+" or rstr[:1] == "-":
+            self._writestr(rstr[:3])
+            if (mpart := rstr[4:6]) != "00":
+                self._writestr(mpart)
         self._writestr('"')
 
-    def write_list(self, value: collections.abc.Sequence[SHVType]) -> None:
+    def write_list(self, value: SHVListType) -> None:  # noqa: D102
         self._nest_level += 1
         is_oneliner = self._is_oneline_list(value)
         self._writestr("[")
         for i, v in enumerate(value):
             if i > 0:
                 self._writestr(",")
             self._indent_item(is_oneliner, i)
             self.write(v)
         self._nest_level -= 1
         self._indent_item(is_oneliner, 0)
         self._writestr("]")
 
     @staticmethod
     def _is_oneline_list(lst: collections.abc.Sequence[SHVType]) -> bool:
-        return len(lst) <= 10 and all(not isinstance(v, (list, dict)) for v in lst)
+        return len(lst) <= 10 and all(not isinstance(v, list | dict) for v in lst)
 
-    def write_imap(self, value: collections.abc.Mapping[int, SHVType]) -> None:
+    def write_imap(self, value: SHVIMapType) -> None:  # noqa: D102
         self._writestr("i{")
         self._write_map_content(value)
         self._writestr("}")
 
-    def write_map(self, value: collections.abc.Mapping[str, SHVType]) -> None:
+    def write_map(self, value: SHVMapType) -> None:  # noqa: D102
         self._writestr("{")
         self._write_map_content(value)
         self._writestr("}")
 
     @staticmethod
     def _is_oneline_map(mmap: collections.abc.Mapping) -> bool:
         return len(mmap) <= 10 and all(
-            not isinstance(v, (list, dict)) for v in mmap.values()
+            not isinstance(v, list | dict) for v in mmap.values()
         )
 
     def _write_map_content(self, mmap: collections.abc.Mapping) -> None:
         self._nest_level += 1
         is_oneliner = self._is_oneline_map(mmap)
         i = -1
         for ikey in sorted(k for k in mmap.keys() if isinstance(k, int)):
```

### Comparing `pyshv-0.5.0/shv/rpcclient.py` & `pyshv-0.6.0/shv/rpcserver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,399 +1,351 @@
-"""RPC connection, that includes client and specific server connection."""
+"""RPC server that waits for clients connection."""
+
 from __future__ import annotations
 
 import abc
 import asyncio
+import collections.abc
+import contextlib
 import logging
-import os
-import time
+import pathlib
 import typing
 
-import aioserial
+try:
+    import asyncinotify
+except (ImportError, TypeError):  # pragma: no cover
+    asyncinotify = None  # type: ignore
 
-from . import rpcprotocol
-from .chainpack import ChainPack
-from .rpcmessage import RpcMessage
+from .rpcclient import RpcClient, RpcClientTTY
 from .rpcprotocol import (
     RpcProtocolSerial,
     RpcProtocolSerialCRC,
     RpcProtocolStream,
     RpcTransportProtocol,
 )
 from .rpcurl import RpcProtocol, RpcUrl
-from .value import SHVIMap, SHVType
 
 logger = logging.getLogger(__name__)
 
 
-class RpcClient(abc.ABC):
-    """RPC connection to some SHV peer."""
-
-    def __init__(self) -> None:
-        self.last_send = time.monotonic()
-        """Monotonic time when last message was sent on this connection.
-
-        The initial value is time of the RpcClient creation.
-        """
-        self.last_receive = time.monotonic()
-        """Monotonic time when last message was received on this connection.
-
-        The initial value is time of the RpcClient creation.
-        """
-
-    async def send(self, msg: RpcMessage) -> None:
-        """Send the given SHV RPC Message.
-
-        :param msg: Message to be sent
-        """
-        await self._send(bytearray((ChainPack.ProtocolType,)) + msg.to_chainpack())
-        self.last_send = time.monotonic()
-        logger.debug("<== SND: %s", msg.to_string())
+class RpcServer(abc.ABC):
+    """RPC server listening for new SHV connections."""
 
     @abc.abstractmethod
-    async def _send(self, msg: bytes) -> None:
-        """Implementation of message sending."""
-
-    async def receive(self, raise_error: bool = True) -> RpcMessage:
-        """Read next received RPC message or wait for next to be received.
-
-        :param raise_error: If RpcError should be raised or not.
-        :return: Next RPC message is returned or `None` in case of EOF.
-        :raise RpcError: When mesasge is error and ``raise_error`` is `True`.
-        :raise EOFError: in case EOF is encountered.
-        """
-        shvdata: SHVType = None
-        while True:
-            data = await self._receive()
-            self.last_receive = time.monotonic()
-            if len(data) > 1 and data[0] == ChainPack.ProtocolType:
-                try:
-                    shvdata = ChainPack.unpack(data[1:])
-                except ValueError:
-                    pass
-                else:
-                    if isinstance(shvdata, SHVIMap):
-                        break
-            logger.debug("==> Invalid message received: %s", data)
-
-        msg = RpcMessage(shvdata)
-        logger.debug("==> REC: %s", msg.to_string())
-        if raise_error and msg.is_error:
-            raise msg.rpc_error
-        return msg
+    def is_serving(self) -> bool:
+        """Check if server is accepting new SHV connections."""
 
     @abc.abstractmethod
-    async def _receive(self) -> bytes:
-        """Implementation of message receive.
-
-        :return: bytes of received message (complete valid message).
-        :raise EOFError: if end of the connection is encountered.
-        """
+    async def listen(self) -> None:
+        """Start accepting new SHV connections."""
 
-    @property
     @abc.abstractmethod
-    def connected(self) -> bool:
-        """Check if client is still connected.
-
-        This is only local check. There is no communication done and thus depending on
-        the transport layer this can be pretty much a lie. The only reliable tests is
-        sending request and receiving respond to it.
+    async def listen_forewer(self) -> None:
+        """Listen and block the calling coroutine until cancelation."""
 
-        :return: ``True`` if client might still connected and ``False`` if we know that
-            it is not.
-        """
-
-    async def reset(self) -> bool:
-        """Reset the connection.
+    @abc.abstractmethod
+    def close(self) -> None:
+        """Stop accepting new SHV connections."""
 
-        Attempt to reset the connection.
+    @abc.abstractmethod
+    async def wait_closed(self) -> None:
+        """Stop accepting new SHV connections and for that to make effect."""
 
-        This might just close the link without opening it again!
 
-        It is common that we use connection tracking native to the link layer and reset
-        is performed by really closing the connection and establishing a new one but
-        that might not be available for all implementations and especially not for
-        servers.
+class _RpcServerStream(RpcServer):
+    """RPC server listenting for SHV connections for streams."""
 
-        :return: ``True`` if client is connected after reset and ``False`` otherwise.
-        """
-        self.disconnect()
-        return False
+    def __init__(
+        self,
+        client_connected_cb: typing.Callable[
+            [RpcClient], None | collections.abc.Awaitable[None]
+        ],
+        protocol: type[RpcTransportProtocol] = RpcProtocolStream,
+    ) -> None:
+        self.client_connected_cb = client_connected_cb
+        """Callbact that is called when new client is connected."""
+        self.protocol = protocol
+        """Stream communication protocol."""
+        self.clients: list[_RpcServerStream.Client] = []
+        """List of clients used for termination of the server."""
+        self._server: asyncio.Server | None = None
 
     @abc.abstractmethod
-    def disconnect(self) -> None:
-        """Close the connection."""
+    async def _create_server(self) -> asyncio.Server:
+        """Create the server instance."""
 
-    async def wait_disconnect(self) -> None:
-        """Close the connection."""
+    def is_serving(self) -> bool:
+        return self._server is not None and self._server.is_serving()
 
+    async def listen(self) -> None:
+        if self._server is None:
+            self._server = await self._create_server()
+        await self._server.start_serving()
+
+    async def listen_forewer(self) -> None:
+        if self._server is None:
+            self._server = await self._create_server()
+        await self._server.serve_forever()
 
-class _RpcClientStream(RpcClient):
-    """RPC connection to some SHV peer over data stream."""
-
-    def __init__(
-        self,
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolStream,
+    async def _client_connect(
+        self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
     ) -> None:
-        super().__init__()
-        self._reader: None | asyncio.StreamReader = None
-        self._writer: None | asyncio.StreamWriter = None
-        self._protocol: RpcTransportProtocol | None = None
-        self.protocol_factory = protocol_factory
-
-    async def _send(self, msg: bytes) -> None:
-        if self._protocol is not None:
-            await self._protocol.send(msg)
-        # Drop message if not connected
-
-    async def _receive(self) -> bytes:
-        if self._protocol is None:
-            raise EOFError("Not connected")
-        return await self._protocol.receive()
-
-    @property
-    def connected(self) -> bool:
-        return self._writer is not None and not self._writer.is_closing()
+        client = self.Client(reader, writer, self)
+        self.clients.append(client)
+        res = self.client_connected_cb(client)
+        if isinstance(res, collections.abc.Awaitable):
+            await res
+
+    def close(self) -> None:
+        if self._server is not None:
+            self._server.close()
+
+    async def wait_closed(self) -> None:
+        if self._server is not None:
+            await self._server.wait_closed()
+
+    class Client(RpcClient):
+        """RPC client for Asyncio's stream server connection."""
+
+        def __init__(
+            self,
+            reader: asyncio.StreamReader,
+            writer: asyncio.StreamWriter,
+            server: _RpcServerStream,
+        ) -> None:
+            super().__init__()
+            self._reader = reader
+            self._writer = writer
+            self.protocol = server.protocol
+            """Stream communication protocol."""
+
+        async def _send(self, msg: bytes) -> None:
+            try:
+                await self.protocol.asyncio_send(self._writer, msg)
+            except ConnectionError as exc:
+                raise EOFError from exc
 
-    def disconnect(self) -> None:
-        if self._writer is not None:
+        async def _receive(self) -> bytes:
+            try:
+                return await self.protocol.asyncio_receive(self._reader)
+            except EOFError:
+                self._writer.close()
+                raise
+
+        @property
+        def connected(self) -> bool:
+            return not self._writer.is_closing()
+
+        def _disconnect(self) -> None:
             self._writer.close()
 
-    async def wait_disconnect(self) -> None:
-        if self._writer is not None:
-            await self._writer.wait_closed()
+        async def wait_disconnect(self) -> None:
+            with contextlib.suppress(ConnectionError):
+                await self._writer.wait_closed()
 
 
-class RpcClientTCP(_RpcClientStream):
-    """RPC connection to some SHV peer over TCP/IP."""
+class RpcServerTCP(_RpcServerStream):
+    """RPC server listenting for SHV connections in TCP/IP."""
 
     def __init__(
         self,
-        location: str,
-        port: int,
-        protocol_factory: typing.Type[RpcTransportProtocol],
+        client_connected_cb: typing.Callable[
+            [RpcClient], None | collections.abc.Awaitable[None]
+        ],
+        location: str | None = None,
+        port: int = 3755,
+        protocol: type[RpcTransportProtocol] = RpcProtocolStream,
     ) -> None:
-        super().__init__(protocol_factory)
+        super().__init__(client_connected_cb, protocol)
         self.location = location
         self.port = port
 
-    async def reset(self) -> bool:
-        await super().reset()
-        self.disconnect()
-        self._reader, self._writer = await asyncio.open_connection(
-            self.location, self.port
+    def __str__(self) -> str:
+        location = (
+            "locahost"
+            if self.location is None
+            else f"[{self.location}]"
+            if ":" in self.location
+            else self.location
         )
-        self._protocol = rpcprotocol.protocol_for_asyncio_stream(
-            self.protocol_factory, self._reader, self._writer
+        return f"server.tcp:{location}:{self.port}"
+
+    async def _create_server(self) -> asyncio.Server:
+        return await asyncio.start_server(
+            self._client_connect, host=self.location, port=self.port
         )
-        logger.debug("Connected to: (TCP) %s:%d", self.location, self.port)
-        return True
 
-    def disconnect(self) -> None:
-        if self.connected:
-            logger.debug("Disconnecting from: (TCP) %s:%d", self.location, self.port)
-        super().disconnect()
-
-    @classmethod
-    async def connect(
-        cls,
-        location: str = "localhost",
-        port: int = 3755,
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolStream,
-    ) -> RpcClientTCP:
-        res = cls(location, port, protocol_factory)
-        await res.reset()
-        return res
+    async def listen(self) -> None:  # noqa: D102
+        was_listening = self.is_serving()
+        await super().listen()
+        if not was_listening:
+            logger.debug("%s: Listening for clients", self)
+
+    def close(self) -> None:  # noqa: D102
+        was_listening = self.is_serving()
+        super().close()
+        if was_listening and (self._server is None or not self._server.is_serving()):
+            logger.debug("%s: No longer listening for clients", self)
+
+    async def _client_connect(
+        self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
+    ) -> None:
+        peername = writer.get_extra_info("peername")
+        location = f"[{peername[0]}]" if ":" in peername[0] else peername[0]
+        logger.debug("%s: New client %s:%d", self, location, peername[1])
+        await super()._client_connect(reader, writer)
+
+    class Client(_RpcServerStream.Client):
+        """RPC client for TCP server connection."""
+
+        def __str__(self) -> str:
+            peername = self._writer.get_extra_info("peername")
+            location = f"[{peername[0]}]" if ":" in peername[0] else peername[0]
+            return f"tcp:{location}:{peername[1]}"
 
 
-class RpcClientUnix(_RpcClientStream):
-    """RPC connection to some SHV peer over Unix domain named socket."""
+class RpcServerUnix(_RpcServerStream):
+    """RPC server listenting for SHV connections on Unix domain named socket."""
 
     def __init__(
         self,
-        location: str,
-        protocol_factory: typing.Type[RpcTransportProtocol],
+        client_connected_cb: typing.Callable[
+            [RpcClient], None | collections.abc.Awaitable[None]
+        ],
+        location: str = "shv.sock",
+        protocol: type[RpcTransportProtocol] = RpcProtocolSerial,
     ) -> None:
-        super().__init__(protocol_factory)
+        super().__init__(client_connected_cb, protocol)
         self.location = location
 
-    async def reset(self) -> bool:
-        await super().reset()
-        self._reader, self._writer = await asyncio.open_unix_connection(self.location)
-        self._protocol = rpcprotocol.protocol_for_asyncio_stream(
-            self.protocol_factory, self._reader, self._writer
-        )
-        logger.debug("Connected to: (Unix) %s", self.location)
-        return True
+    def __str__(self) -> str:
+        return f"server.unix:{self.location}"
 
-    def disconnect(self) -> None:
-        if self.connected:
-            logger.debug("Disconnecting from: (Unix) %s", self.location)
-        super().disconnect()
-
-    @classmethod
-    async def connect(
-        cls,
-        location: str = "shv.sock",
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolStream,
-    ) -> RpcClientUnix:
-        res = cls(location, protocol_factory)
-        await res.reset()
-        return res
+    async def _create_server(self) -> asyncio.Server:
+        return await asyncio.start_unix_server(self._client_connect, path=self.location)
 
+    async def listen(self) -> None:  # noqa: D102
+        was_listening = self.is_serving()
+        await super().listen()
+        if not was_listening:
+            logger.debug("%s: Listening for clients", self)
+
+    def close(self) -> None:  # noqa: D102
+        was_listening = self.is_serving()
+        super().close()
+        if was_listening and (self._server is None or self._server.is_serving()):
+            logger.debug("%s: No longer listening for clients", self)
 
-class RpcClientPipe(_RpcClientStream):
-    """RPC connection to some SHV peer over Unix pipes."""
-
-    def __init__(
-        self,
-        reader: asyncio.StreamReader,
-        writer: asyncio.StreamWriter,
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolSerial,
+    async def _client_connect(
+        self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
     ) -> None:
-        super().__init__(protocol_factory)
-        self._reader = reader
-        self._writer = writer
-        self._protocol = rpcprotocol.protocol_for_asyncio_stream(
-            protocol_factory, reader, writer
-        )
+        logger.debug("%s: New client %s", self, writer.get_extra_info("peername"))
+        await super()._client_connect(reader, writer)
 
-    @classmethod
-    async def fdopen(
-        cls,
-        rpipe: int | typing.IO,
-        wpipe: int | typing.IO,
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolSerial,
-    ) -> RpcClientPipe:
-        """Create RPC client from existing Unix pipes."""
-        if isinstance(rpipe, int):
-            rpipe = os.fdopen(rpipe, mode="r")
-        reader = asyncio.StreamReader()
-        protocol = asyncio.StreamReaderProtocol(reader)
-        await asyncio.get_running_loop().connect_read_pipe(lambda: protocol, rpipe)
-
-        if isinstance(wpipe, int):
-            wpipe = os.fdopen(wpipe, mode="w")
-        wtransport, _ = await asyncio.get_running_loop().connect_write_pipe(
-            lambda: protocol, wpipe
-        )
-        writer = asyncio.StreamWriter(
-            wtransport, protocol, None, asyncio.get_running_loop()
-        )
+    class Client(_RpcServerStream.Client):
+        """RPC client for Unix server connection."""
 
-        return cls(reader, writer, protocol_factory)
+        def __str__(self) -> str:
+            return f"unix:{self._writer.get_extra_info('peername')}"
 
-    @classmethod
-    async def open_pair(
-        cls,
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolSerial,
-        flags: int = 0,
-    ) -> tuple[RpcClientPipe, RpcClientPipe]:
-        """Create pair of clients that are interconnected over the pipe.
-
-        :param protocol_factory: The protocol factory to be used.
-        :param flags: Flags passed to :meth:`os.pipe2`.
-        :return: Pair of clients that are interconnected over Unix pipes.
-        """
-        pr1, pw1 = os.pipe2(flags)
-        pr2, pw2 = os.pipe2(flags)
-        client1 = await cls.fdopen(pr1, pw2, protocol_factory)
-        client2 = await cls.fdopen(pr2, pw1, protocol_factory)
-        return client1, client2
 
+class RpcServerTTY(RpcServer):
+    """RPC server waiting for TTY to appear.
 
-class RpcClientTTY(RpcClient):
-    """RPC connection to some SHV peer over Unix domain named socket."""
+    This actually only maintains a single client as there can't be more than one
+    client on single TTY.
+    """
 
     def __init__(
         self,
-        port: str,
-        baudrate: int,
-        protocol_factory: typing.Type[RpcTransportProtocol],
-    ) -> None:
-        super().__init__()
-        self.port = port
-        self.baudrate = baudrate
-        self.protocol_factory = protocol_factory
-        self.serial: None | aioserial.AioSerial = None
-        self._protocol: None | RpcTransportProtocol = None
-        self._eof = asyncio.Event()
-        self._eof.set()
-
-    async def _send(self, msg: bytes) -> None:
-        if self._protocol is not None:
-            await self._protocol.send(msg)
-
-    async def _receive(self) -> bytes:
-        if self._protocol is None:
-            raise EOFError
-        return await self._protocol.receive()
-
-    @property
-    def connected(self) -> bool:
-        return self.serial is not None and self.serial.is_open
-
-    async def reset(self) -> bool:
-        await super().reset()
-        self.serial = aioserial.AioSerial(
-            port=self.port,
-            baudrate=self.baudrate,
-            rtscts=True,
-            dsrdtr=True,
-            exclusive=True,
-        )
-        self._protocol = self.protocol_factory(
-            self._read_exactly, self.serial.write_async
-        )
-        self._eof.clear()
-        logger.debug("Connected to: (TTY) %s", self.port)
-        return True
-
-    async def _read_exactly(self, n: int) -> bytes:
-        assert self.serial is not None
-        res = bytearray()
-        while len(res) < n:
-            try:
-                res += await self.serial.read_async(n - len(res))
-            except aioserial.SerialException as exc:
-                self._eof.set()
-                raise EOFError from exc
-        return res
-
-    def disconnect(self) -> None:
-        if self.serial is not None and self.serial.is_open:
-            self.serial.close()
-            self._eof.set()
-            logger.debug("Disconnecting from: (TTY) %s", self.port)
-
-    async def wait_disconnect(self) -> None:
-        await self._eof.wait()
-
-    @classmethod
-    async def open(
-        cls,
+        client_connected_cb: typing.Callable[
+            [RpcClient], None | collections.abc.Awaitable[None]
+        ],
         port: str,
         baudrate: int = 115200,
-        protocol_factory: typing.Type[RpcTransportProtocol] = RpcProtocolSerialCRC,
-    ) -> RpcClientTTY:
-        res = cls(port, baudrate, protocol_factory)
-        await res.reset()
-        return res
+        protocol: type[RpcTransportProtocol] = RpcProtocolSerialCRC,
+    ) -> None:
+        self.client_connected_cb = client_connected_cb
+        """Callbact that is called when new client is connected."""
+        self.client = RpcClientTTY(port, baudrate, protocol)
+        """The :class:`RpcClientTTY` instance."""
+        self._task: asyncio.Task | None = None
 
+    def __str__(self) -> str:
+        return f"tty:{self.client.port}"
 
-async def connect_rpc_client(url: RpcUrl) -> RpcClient:
-    """Connect to the server on given URL.
+    async def _loop(self) -> None:
+        while True:
+            try:
+                await self.client.reset()
+            except OSError as exc:
+                logger.debug("%s: Waiting for accessible TTY device: %s", self, exc)
+            else:
+                res = self.client_connected_cb(self.client)
+                if isinstance(res, collections.abc.Awaitable):
+                    await res
+                await self.client.wait_disconnect()
+                continue
+            if asyncinotify is not None:
+                with asyncinotify.Inotify() as inotify:
+                    pth = pathlib.Path(self.client.port)
+                    inotify.add_watch(
+                        pth.parent, asyncinotify.Mask.CREATE | asyncinotify.Mask.ATTRIB
+                    )
+                    async for event in inotify:
+                        if str(pth.name) == str(event.name):
+                            break
+            else:
+                await asyncio.sleep(5)  # type: ignore
+
+    def is_serving(self) -> bool:  # noqa: D102
+        return self._task is not None and not self._task.done()
+
+    async def listen(self) -> None:  # noqa: D102
+        if not self.is_serving():
+            self._task = asyncio.create_task(self._loop())
+
+    async def listen_forewer(self) -> None:  # noqa: D102
+        await self.listen()
+        await self.wait_closed()
+
+    def close(self) -> None:  # noqa: D102
+        if self._task is not None:
+            self._task.cancel()
+
+    async def wait_closed(self) -> None:  # noqa: D102
+        if self._task is not None:
+            await self._task
+
+
+async def create_rpc_server(
+    client_connected_cb: typing.Callable[
+        [RpcClient], None | collections.abc.Awaitable[None]
+    ],
+    url: RpcUrl,
+) -> RpcServer:
+    """Create server listening on given URL.
 
-    :param url: RPC URL specifying the server location.
+    :param client_connected_cb: function called for every new client connected.
+    :param url: RPC URL specifying where server should listen.
     """
+    res: RpcServer
     if url.protocol is RpcProtocol.TCP:
-        return await RpcClientTCP.connect(url.location, url.port, RpcProtocolStream)
-    if url.protocol is RpcProtocol.TCPS:
-        return await RpcClientTCP.connect(url.location, url.port, RpcProtocolSerial)
-    # TODO SSL and SSLS
-    if url.protocol is RpcProtocol.UNIX:
-        return await RpcClientUnix.connect(url.location, RpcProtocolStream)
-    if url.protocol is RpcProtocol.UNIXS:
-        return await RpcClientUnix.connect(url.location, RpcProtocolSerial)
-    if url.protocol is RpcProtocol.SERIAL:
-        return await RpcClientTTY.open(url.location, url.baudrate, RpcProtocolSerialCRC)
-    raise NotImplementedError(f"Unimplemented protocol: {url.protocol}")
+        res = RpcServerTCP(
+            client_connected_cb, url.location, url.port, RpcProtocolStream
+        )
+    elif url.protocol is RpcProtocol.TCPS:
+        res = RpcServerTCP(
+            client_connected_cb, url.location, url.port, RpcProtocolSerial
+        )
+    elif url.protocol is RpcProtocol.UNIX:
+        res = RpcServerUnix(client_connected_cb, url.location, RpcProtocolStream)
+    elif url.protocol is RpcProtocol.UNIXS:
+        res = RpcServerUnix(client_connected_cb, url.location, RpcProtocolSerial)
+    elif url.protocol is RpcProtocol.SERIAL:
+        res = RpcServerTTY(
+            client_connected_cb, url.location, url.baudrate, RpcProtocolSerialCRC
+        )
+    else:
+        raise NotImplementedError(f"Unimplemented protocol: {url.protocol}")
+    await res.listen()
+    return res
```

### Comparing `pyshv-0.5.0/shv/rpcerrors.py` & `pyshv-0.6.0/shv/rpcerrors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Implementation of Rpc RPC specific errors."""
+
 from __future__ import annotations
 
+import dataclasses
 import enum
-import typing
 
 
 class RpcErrorCode(enum.IntEnum):
     """Number representing an SHV RPC error code."""
 
     NO_ERROR = 0
     INVALID_REQUEST = 1
@@ -14,14 +15,17 @@
     INVALID_PARAMS = 3
     INTERNAL_ERR = 4
     PARSE_ERR = 5
     METHOD_CALL_TIMEOUT = 6
     METHOD_CALL_CANCELLED = 7
     METHOD_CALL_EXCEPTION = 8
     UNKNOWN = 9
+    LOGIN_REQUIRED = 10
+    USER_ID_REQUIRED = 11
+    NOT_IMPLEMENTED = 12
     USER_CODE = 32
 
 
 class RpcError(RuntimeError):
     """Top level for Rpc RPC errors.
 
     This tries to be a bit smart when objects are created. There is class
@@ -30,27 +34,33 @@
     this map to be looked up by their code.
 
     :param msg: Message describing the error circumstances.
     :param code: Error code.
     """
 
     shv_error_code: RpcErrorCode = RpcErrorCode.UNKNOWN
-    shv_error_map: dict[int, typing.Type[RpcError]] = {}
+    shv_error_map: dict[int, type[RpcError]] = dataclasses.field(default_factory=dict)
 
-    def __new__(cls, msg: str, code: RpcErrorCode | None = None) -> "RpcError":
+    def __new__(
+        cls, msg: str | None = None, code: RpcErrorCode | None = None
+    ) -> RpcError:
+        """Create an appropriate exception based on the code."""
         ncls = cls.shv_error_map.get(cls.shv_error_code if code is None else code, cls)
-        return super(RpcError, cls).__new__(ncls)
+        return super(RpcError, cls).__new__(ncls)  # noqa UP008
 
-    def __init__(self, msg: str, code: RpcErrorCode | None = None) -> None:
+    def __init__(
+        self, msg: str | None = None, code: RpcErrorCode | None = None
+    ) -> None:
         super().__init__(str(msg), self.shv_error_code if code is None else code)
 
     @property
-    def message(self) -> str:
+    def message(self) -> str | None:
         """Provides access to the SHV RPC message."""
-        assert isinstance(self.args[0], str)
+        if not isinstance(self.args[0], str) and self.args[0] is not None:
+            raise ValueError(f"Must be string or None but is: {type(self.args[0])}")
         return self.args[0]
 
     @property
     def error_code(self) -> RpcErrorCode:
         """Provides access to the :class:`RpcErrorCode`."""
         assert isinstance(self.args[1], RpcErrorCode)
         return self.args[1]
@@ -100,20 +110,41 @@
 
 class RpcMethodCallExceptionError(RpcError):
     """Method call resulted in exception and not result."""
 
     shv_error_code = RpcErrorCode.METHOD_CALL_EXCEPTION
 
 
+class RpcLoginRequiredError(RpcError):
+    """Login sequence must be performed before anything else."""
+
+    shv_error_code = RpcErrorCode.LOGIN_REQUIRED
+
+
+class RpcUserIDRequiredError(RpcError):
+    """Request must be sent with UserID field."""
+
+    shv_error_code = RpcErrorCode.USER_ID_REQUIRED
+
+
+class RpcNotImplementedError(RpcError):
+    """Called method that is not implemented right now but valid."""
+
+    shv_error_code = RpcErrorCode.NOT_IMPLEMENTED
+
+
 RpcError.shv_error_map = {
     e.shv_error_code: e
     for e in (
         RpcInvalidRequestError,
         RpcMethodNotFoundError,
         RpcInvalidParamsError,
         RpcInternalError,
         RpcParseError,
         RpcMethodCallTimeoutError,
         RpcMethodCallCancelledError,
         RpcMethodCallExceptionError,
+        RpcLoginRequiredError,
+        RpcUserIDRequiredError,
+        RpcNotImplementedError,
     )
 }
```

### Comparing `pyshv-0.5.0/shv/rpcmessage.py` & `pyshv-0.6.0/shv/rpcmessage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implementation of RpcMessage."""
+
 from __future__ import annotations
 
 import collections.abc
 import enum
 import typing
 
 from .chainpack import ChainPackWriter
@@ -31,28 +32,34 @@
     def __init__(self, rpc_val: SHVIMapType | None = None) -> None:
         if rpc_val is None:
             rpc_val = SHVIMap()
         if not isinstance(rpc_val, SHVIMap):
             rpc_val = SHVIMap(rpc_val)
         self.value: SHVIMap = rpc_val
 
-    def __eq__(self, other: typing.Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, RpcMessage) and shvmeta_eq(self.value, other.value)
 
     def __repr__(self) -> str:
         return f"<RpcMessage {self.value.meta!r}: {self.value!r}>"
 
     class Tag(enum.IntEnum):
         """Tags in Meta for RPC message."""
 
         REQUEST_ID = 8
         PATH = 9
         METHOD = 10
+        SIGNAL = 10
         CALLER_IDS = 11
+        RESP_CALLER_IDS = 13
         ACCESS = 14
+        USER_ID = 16
+        ACCESS_LEVEL = 17
+        PART = 18
+        SOURCE = 19
 
     class Key(enum.IntEnum):
         """Keys in the toplevel IMap of the RPC message."""
 
         PARAMS = 1
         RESULT = 2
         ERROR = 3
@@ -61,16 +68,22 @@
         """Keys in the error IMap."""
 
         CODE = 1
         MESSAGE = 2
 
     def is_valid(self) -> bool:
         """Check if message is valid RPC message."""
-        # TODO maybe do more work than just check basic type
-        return isinstance(self.value, SHVIMap)
+        return (
+            isinstance(self.value, SHVIMap)
+            and bool(set(self.value) ^ set(self.Key))
+            and (self.is_request or self.is_response or self.is_signal)
+            and isinstance(self._path, str)
+            and isinstance(self._signal_name, str)
+            and isinstance(self._source, str)
+        )
 
     @property
     def is_request(self) -> bool:
         """Check if message is request."""
         return bool(self.has_request_id and self.has_method)
 
     @property
@@ -86,23 +99,36 @@
             and self.error is not None
             and self.rpc_error.error_code != RpcErrorCode.NO_ERROR
         )
 
     @property
     def is_signal(self) -> bool:
         """Check if message is a signal."""
-        return bool(not self.has_request_id and self.has_method)
+        return not self.has_request_id
 
-    def make_response(self) -> RpcMessage:
-        """Create new message that is response to this one."""
+    def make_response(
+        self, result: SHVType = None, error: RpcError | SHVType = None
+    ) -> RpcMessage:
+        """Create new message that is response to this one.
+
+        :param result: The result value to be set in the response.
+        :param error: The error to be set to the response message. You should
+          use either *result* or *error* not both.
+        :return: The new message that is response to this one.
+        """
         if not self.is_request:
             raise ValueError("Response can be created from request only.")
         resp = RpcMessage()
         resp.request_id = self.request_id
         resp.caller_ids = self.caller_ids
+        resp.result = result
+        if isinstance(error, RpcError):
+            resp.rpc_error = error
+        else:
+            resp.error = error
         return resp
 
     @property
     def has_request_id(self) -> bool:
         """Check if valid request ID was provided in this message."""
         return self.Tag.REQUEST_ID in self.value.meta and isinstance(
             self.value.meta[self.Tag.REQUEST_ID], int
@@ -120,18 +146,30 @@
     def request_id(self, rqid: int | None) -> None:
         """Set given request identicator to this message."""
         if rqid is None:
             self.value.meta.pop(self.Tag.REQUEST_ID, None)
         else:
             self.value.meta[self.Tag.REQUEST_ID] = rqid
 
+    def new_request_id(self) -> int:
+        """Set new request ID.
+
+        :return: The new request ID.
+        """
+        self.request_id = self.next_request_id()
+        return self.request_id
+
+    @property
+    def _path(self) -> SHVType:
+        return self.value.meta.get(self.Tag.PATH, "")
+
     @property
     def path(self) -> str:
         """SHV path specified for this message or empty string."""
-        res = self.value.meta.get(self.Tag.PATH, "")
+        res = self._path
         if not isinstance(res, str):
             raise ValueError(f"Invalid path type: {type(res)}")
         return res
 
     @path.setter
     def path(self, path: str) -> None:
         """Set given path as SHV path for this message."""
@@ -160,23 +198,61 @@
         """Set SHV method name for this message."""
         if method:
             self.value.meta[self.Tag.METHOD] = method
         else:
             self.value.meta.pop(self.Tag.METHOD, None)
 
     @property
+    def _signal_name(self) -> SHVType:
+        return self.value.meta.get(self.Tag.METHOD, "chng")
+
+    @property
+    def signal_name(self) -> str:
+        """SHV signal name for this message."""
+        res = self._signal_name
+        if not isinstance(res, str):
+            raise ValueError(f"Invalid method type: {type(res)}")
+        return res
+
+    @signal_name.setter
+    def signal_name(self, signal: str) -> None:
+        """Set SHV signal name for this message."""
+        # Note: we always set it because old implementations were dropping
+        # messages without method name.
+        self.value.meta[self.Tag.SIGNAL] = signal
+
+    @property
+    def _source(self) -> SHVType:
+        return self.value.meta.get(self.Tag.SOURCE, "get")
+
+    @property
+    def source(self) -> str:
+        """SHV signal source method name for this message."""
+        res = self._source
+        if not isinstance(res, str):
+            raise ValueError(f"Invalid method type: {type(res)}")
+        return res
+
+    @source.setter
+    def source(self, source: str) -> None:
+        """Set SHV signal source method name for this message."""
+        if source and source != "get":
+            self.value.meta[self.Tag.SOURCE] = source
+        else:
+            self.value.meta.pop(self.Tag.SOURCE, None)
+
+    @property
     def caller_ids(self) -> collections.abc.Sequence[int]:
         """Caller idenfieiers associated with this message."""
         res = self.value.meta.get(self.Tag.CALLER_IDS, None)
         if isinstance(res, int):
             return [res]
         if not isinstance(res, list):
             return []
-        filter(lambda v: isinstance(v, int), res)
-        return res
+        return list(filter(lambda v: isinstance(v, int), res))
 
     @caller_ids.setter
     def caller_ids(self, cids: collections.abc.Sequence[int]) -> None:
         """Set caller idenfieiers associated with this message."""
         if not cids:
             self.value.meta.pop(self.Tag.CALLER_IDS, None)
         else:
@@ -212,18 +288,37 @@
         return None
 
     @rpc_access.setter
     def rpc_access(self, access: RpcMethodAccess | None) -> None:
         """Set access level with :class:`shv.RpcMethodAccess`."""
         if access is not None:
             self.value.meta[self.Tag.ACCESS] = RpcMethodAccess.tostr(access)
+            self.value.meta[self.Tag.ACCESS_LEVEL] = access.value
         else:
             self.value.meta.pop(self.Tag.ACCESS, None)
 
     @property
+    def user_id(self) -> str | None:
+        """User's ID caried by message."""
+        res = self.value.meta.get(self.Tag.USER_ID, None)
+        if isinstance(res, dict):  # Note: backward compatibility
+            res = f"{res.get('brokerId')}:{res.get('shvUser')}"
+        if res is not None and not isinstance(res, str):
+            res = str(res)
+        return res
+
+    @user_id.setter
+    def user_id(self, value: str | None) -> None:
+        """Set User's ID."""
+        if value is not None:
+            self.value.meta[self.Tag.USER_ID] = value
+        else:
+            self.value.meta.pop(self.Tag.USER_ID, None)
+
+    @property
     def param(self) -> SHVType:
         """SHV parameters for the method call."""
         return self.value.get(self.Key.PARAMS, None) if is_shvimap(self.value) else None
 
     @param.setter
     def param(self, param: SHVType) -> None:
         """Set SHV parameters for this method call."""
@@ -259,15 +354,14 @@
             self.value[self.Key.ERROR] = error
 
     @property
     def rpc_error(self) -> RpcError:
         """SHV method call error in standard SHV format :class:`RpcError`."""
         res = self.error
         if is_shvimap(res):
-            assert isinstance(res, dict)
             rcode = res.get(self.ErrorKey.CODE)
             code: RpcErrorCode = RpcErrorCode.UNKNOWN
             if isinstance(rcode, int):
                 try:
                     code = RpcErrorCode(rcode)
                 except ValueError:
                     pass
@@ -290,66 +384,63 @@
 
     def to_string(self) -> str:
         """Convert message to CPON and return it as string."""
         return self.to_cpon().decode("utf-8")
 
     def to_cpon(self) -> bytes:
         """Convert message to Cpon."""
-        return CponWriter.pack(self.value) if self.is_valid() else b""
+        return CponWriter.pack(self.value)
 
     def to_chainpack(self) -> bytes:
         """Convert message to Chainpack."""
-        return ChainPackWriter.pack(self.value) if self.is_valid() else b""
+        return ChainPackWriter.pack(self.value)
 
     @classmethod
     def request(
         cls,
         path: str,
         method: str,
         param: SHVType = None,
         rid: int | None = None,
-    ) -> "RpcMessage":
+        user_id: str | None = None,
+    ) -> RpcMessage:
         """Create request message.
 
         :param path: SHV path for signal.
         :param method: method name for signal.
         :param param: Parameters passed to the method.
         :param rid: Request identifier for this message. It is automatically assigned if
           ``None`` is passed.
+        :param user_id: User's ID to be caried with request message.
         """
         res = cls()
         res.request_id = rid or cls.next_request_id()
         res.method = method
         res.path = path
         res.param = param
+        res.user_id = user_id
         return res
 
     @classmethod
     def signal(
         cls,
         path: str,
-        method: str,
+        name: str = "chng",
+        source: str = "get",
         value: SHVType = None,
         access: RpcMethodAccess = RpcMethodAccess.READ,
-    ) -> "RpcMessage":
+    ) -> RpcMessage:
         """Create signal message.
 
         :param path: SHV path for signal.
-        :param method: method name for signal.
+        :param name: Name of the signal.
+        :param source: Name of the method this signal is associated with.
         :param value: Value to be sent in the message.
         :param access: Minimal access level needed to get this signal.
         """
         res = cls()
-        res.method = method
+        res.signal_name = name
+        res.source = source
         res.path = path
         res.param = value
         res.rpc_access = access
         return res
-
-    @classmethod
-    def chng(cls, path: str, value: SHVType) -> "RpcMessage":
-        """Create message for ``chng`` signal.
-
-        :param path: SHV path for signal.
-        :param value: New value to be sent in the message.
-        """
-        return cls.signal(path, "chng", value)
```

### Comparing `pyshv-0.5.0/shv/rpcmethod.py` & `pyshv-0.6.0/tests/test_simpleclient.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,186 +1,244 @@
-"""Types used in SHV RPC method description."""
-import collections.abc
+"""Check implementation of SimpleClient."""
+
+import contextlib
 import dataclasses
-import enum
-import functools
-import typing
-
-from .value import SHVType
-from .value_tools import SHVGetKey, shvget
-
-
-class RpcMethodFlags(enum.IntFlag):
-    """Flags assigned to the SHV RPC methods."""
-
-    SIGNAL = 1 << 0
-    GETTER = 1 << 1
-    SETTER = 1 << 2
-    LARGE_RESULT_HINT = 1 << 3
-
-
-class RpcMethodAccess(enum.IntEnum):
-    """Method access level."""
-
-    BROWSE = enum.auto()
-    READ = enum.auto()
-    WRITE = enum.auto()
-    COMMAND = enum.auto()
-    CONFIG = enum.auto()
-    SERVICE = enum.auto()
-    SUPER_SERVICE = enum.auto()
-    DEVEL = enum.auto()
-    ADMIN = enum.auto()
-
-    @classmethod
-    @functools.cache
-    def strmap(cls) -> dict[str, "RpcMethodAccess"]:
-        return {
-            "bws": cls.BROWSE,
-            "rd": cls.READ,
-            "wr": cls.WRITE,
-            "cmd": cls.COMMAND,
-            "cfg": cls.CONFIG,
-            "srv": cls.SERVICE,
-            "ssrv": cls.SUPER_SERVICE,
-            "dev": cls.DEVEL,
-            "su": cls.ADMIN,
-        }
-
-    @classmethod
-    @functools.cache
-    def strrmap(cls) -> dict[int, str]:
-        return {v.value: k for k, v in cls.strmap().items()}
-
-    def tostr(self) -> str:
-        """Convert to string representation."""
-        return self.strrmap().get(self.value, "bws")
-
-    @classmethod
-    def fromstr(cls, access: str) -> "RpcMethodAccess":
-        """Convert to string representation."""
-        return cls.strmap().get(access, cls.BROWSE)
-
-
-@dataclasses.dataclass
-class RpcMethodDesc:
-    """Description of the SHV RPC method.
-
-    This is implemented as :func:`dataclasses.dataclass`.
-
-    :param name: Name of the method.
-    :param signature: Calling signature for this method.
-    :param flags: Flags assigned to the method.
-    :param access: Minimal granted access level for this method.
-    :param description: Short description of the method.
+
+import pytest
+
+from shv import (
+    RpcLoginType,
+    RpcMessage,
+    RpcMethodAccess,
+    RpcMethodDesc,
+    SimpleClient,
+    shvmeta,
+)
+
+
+@pytest.mark.parametrize(
+    "path,method,params,result",
+    (
+        (".broker/app", "echo", 42, 42),
+        ("", "ls", None, [".broker", "test"]),
+        (
+            "",
+            "dir",
+            None,
+            [
+                {
+                    1: "dir",
+                    3: "DirParam",
+                    4: "DirResult",
+                    5: 1,
+                    6: {},
+                    7: {"description": "", "label": ""},
+                },
+                {
+                    1: "ls",
+                    3: "LsParam",
+                    4: "LsResult",
+                    5: 1,
+                    6: {},
+                    7: {"description": "", "label": ""},
+                },
+            ],
+        ),
+    ),
+)
+async def test_call(client, path, method, params, result):
+    """Check that we can call various methods using blocking call."""
+    res = await client.call(path, method, params)
+    assert res == result
+    assert shvmeta(res) == shvmeta(result)
+
+
+@pytest.mark.parametrize(
+    "path,result",
+    (
+        ("", [".broker", "test"]),
+        (".broker", ["app", "clients", "currentClient", "etc", "masters", "mounts"]),
+        (".broker/app/log", []),
+    ),
+)
+async def test_ls(client, path, result):
+    """Verify that we can use ls method."""
+    assert await client.ls(path) == result
+
+
+@pytest.mark.parametrize(
+    "path,name,result",
+    (
+        ("", ".broker", True),
+        ("", "test", True),
+        ("", "invalid", False),
+        (".broker", "currentClient", True),
+        (".broker", "foo", False),
+        (".broker/app", "log", True),
+    ),
+)
+async def test_ls_has_child(client, path, name, result):
+    """Verify that child existence check works."""
+    assert await client.ls_has_child(path, name) == result
+
+
+@pytest.mark.parametrize(
+    "path,result",
+    (
+        (
+            "",
+            [
+                RpcMethodDesc("dir", param="DirParam", result="DirResult"),
+                RpcMethodDesc("ls", param="LsParam", result="LsResult"),
+            ],
+        ),
+        (
+            ".broker/currentClient",
+            [
+                RpcMethodDesc("dir", param="DirParam", result="DirResult"),
+                RpcMethodDesc("ls", param="LsParam", result="LsResult"),
+                RpcMethodDesc(
+                    name="clientId",
+                    param="void",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                    signals={},
+                    extra={},
+                ),
+                RpcMethodDesc(
+                    name="mountPoint",
+                    param="void",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    name="userRoles",
+                    param="void",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    name="userProfile",
+                    param="void",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    name="accessGrantForMethodCall",
+                    param="param",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    name="accessLevelForMethodCall",
+                    param="param",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    name="accesLevelForMethodCall",
+                    param="param",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    name="changePassword",
+                    param="param",
+                    result="ret",
+                    access=RpcMethodAccess.WRITE,
+                ),
+            ],
+        ),
+        (
+            ".broker/app/log",
+            [
+                RpcMethodDesc("dir", param="DirParam", result="DirResult"),
+                RpcMethodDesc("ls", param="LsParam", result="LsResult"),
+                RpcMethodDesc(
+                    "getSendLogAsSignalEnabled",
+                    param="void",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    "setSendLogAsSignalEnabled",
+                    param="param",
+                    result="ret",
+                    access=RpcMethodAccess.WRITE,
+                ),
+                RpcMethodDesc(
+                    "verbosity",
+                    param="void",
+                    result="ret",
+                    access=RpcMethodAccess.READ,
+                ),
+                RpcMethodDesc(
+                    "setVerbosity",
+                    param="ret",
+                    result="param",
+                    access=RpcMethodAccess.COMMAND,
+                ),
+            ],
+        ),
+    ),
+)
+async def test_dir(client, path, result):
+    """Verify that we can use dir method."""
+    res = await client.dir(path)
+    assert res == result
+
+
+@pytest.mark.parametrize(
+    "path,name,result",
+    (
+        (".broker/app", "ping", True),
+        (".broker/app", "invalid", False),
+        (".broker/currentClient", "clientId", True),
+        (".broker/app/log", "verbosity", True),
+        (".broker/app/log", "verbositys", False),
+    ),
+)
+async def test_dir_exists(client, path, name, result):
+    """Verify that method existence check works."""
+    res = await client.dir_exists(path, name)
+    assert res == result
+
+
+async def test_sha_login(shvbroker, url):
+    """Check that we can login with sha1 password.
+
+    Commonly we login with plain password in tests here but we need to check
+    ability to login with SHA1 hashed password as well.
     """
+    nurl = dataclasses.replace(
+        url,
+        login=dataclasses.replace(
+            url.login,
+            password="57a261a7bcb9e6cf1db80df501cdd89cee82957e",
+            login_type=RpcLoginType.SHA1,
+        ),
+    )
+    client = await SimpleClient.connect(nurl)
+    assert await client.ls("") == [".broker", "test"]
+    await client.disconnect()
+
+
+async def test_disconnect(client):
+    """Tests that multiple calls to disconnect is not an issue."""
+    await client.disconnect()
 
-    name: str
-    flags: RpcMethodFlags = RpcMethodFlags(0)
-    param: str = "Null"
-    result: str = "Null"
-    access: RpcMethodAccess = RpcMethodAccess.BROWSE
-    description: str = ""
-
-    def toshv(self, use_map: bool = False) -> SHVType:
-        """Convert to SHV RPC representation."""
-        res: dict[int | str, SHVType] = {
-            "name" if use_map else 1: self.name,
-            "flags" if use_map else 2: self.flags,
-        }
-        if self.param != "Null":
-            res["param" if use_map else 3] = self.param
-        if self.result != "Null":
-            res["result" if use_map else 4] = self.result
-        res["access" if use_map else 5] = RpcMethodAccess.tostr(self.access)
-        if self.description and use_map:
-            res["description"] = self.description
-        return typing.cast(SHVType, res)
-
-    @classmethod
-    def fromshv(cls, value: SHVType) -> "RpcMethodDesc":
-        """Create from SHV RPC representation."""
-        if not isinstance(value, collections.abc.Mapping):
-            raise ValueError("Expected mapping.")
-        return cls(
-            name=shvget(value, SHVGetKey("name", 1), str, "UNSPECIFIED"),
-            flags=RpcMethodFlags(shvget(value, SHVGetKey("flags", 2), int, cls.flags)),
-            param=shvget(value, SHVGetKey("param", 3), str, cls.param),
-            result=shvget(value, SHVGetKey("result", 4), str, cls.result),
-            access=RpcMethodAccess.fromstr(
-                shvget(value, SHVGetKey("access", 5), str, cls.access.tostr())
-            ),
-            description=shvget(value, "description", str, cls.description),
-        )
 
-    @classmethod
-    def getter(
-        cls,
-        name: str = "get",
-        param: str = "Int",
-        result: str = "Any",
-        access: RpcMethodAccess = RpcMethodAccess.READ,
-        description: str = "",
-    ) -> "RpcMethodDesc":
-        """New getter method description.
-
-        :param name: Name of the method.
-        :param param: Type of the parameter this getter expects.
-        :param result: Type of the result this getter provides.
-        :param access: Minimal granted access level for this getter.
-        :param description: Short description of the value.
-        """
-        return cls(name, RpcMethodFlags.GETTER, param, result, access, description)
-
-    @classmethod
-    def setter(
-        cls,
-        name: str = "set",
-        param: str = "Any",
-        result: str = "Null",
-        access: RpcMethodAccess = RpcMethodAccess.WRITE,
-        description: str = "",
-    ) -> "RpcMethodDesc":
-        """New setter method description.
-
-        :param name: Name of the method.
-        :param param: Type of the parameter this setter expects.
-        :param result: Type of the result this setter provides.
-        :param access: Minimal granted access level for this setter.
-        :param description: Short description of the value.
-        """
-        return cls(name, RpcMethodFlags.SETTER, param, result, access, description)
-
-    @classmethod
-    def signal(
-        cls,
-        name: str = "chng",
-        param: str = "Any",
-        access: RpcMethodAccess = RpcMethodAccess.READ,
-        description: str = "",
-    ) -> "RpcMethodDesc":
-        """New signal method description.
-
-        :param name: Name of the method.
-        :param param: Type of the parameter this signal carries.
-        :param access: Minimal granted access level for this setter.
-        :param description: Short description of the value.
-        """
-        return cls(name, RpcMethodFlags.SIGNAL, "Null", param, access, description)
-
-    @classmethod
-    @functools.lru_cache(maxsize=1)
-    def stddir(cls) -> "RpcMethodDesc":
-        """Get description of standard 'dir' method."""
-        return cls("dir", param="idir", result="odir")
-
-    @classmethod
-    @functools.lru_cache(maxsize=1)
-    def stdls(cls) -> "RpcMethodDesc":
-        """Get description of standard 'ls' method."""
-        return cls("ls", param="ils", result="ols")
-
-    @classmethod
-    @functools.lru_cache(maxsize=1)
-    def stdlschng(cls) -> "RpcMethodDesc":
-        """Get description of standard 'lschng' signal method."""
-        return cls.signal("lschng", "olschng", RpcMethodAccess.BROWSE)
+async def test_reconnect(client):
+    """Checks that client reconnects itself if broker disconnects it.
+
+    This uses broker's API to disconnect itself. Broker will give us a new
+    client ID and that way we will identify that we successfully reconnected.
+    """
+    client.reconnects = 2
+    cid = await client.call(".broker/currentClient", "clientId")
+    # We must use client directly because broker won't respond before it
+    # disconnects us and thus we would attempt resent.
+    with contextlib.suppress(EOFError):
+        await client.client.send(
+            RpcMessage.request(f".broker/clients/{cid}", "dropClient")
+        )
+    assert await client.call(".broker/currentClient", "clientId") != cid
```

### Comparing `pyshv-0.5.0/shv/rpcprotocol.py` & `pyshv-0.6.0/shv/rpcprotocol.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,122 @@
 """Protocols for :class:`RpcClient`."""
+
 import abc
 import asyncio
 import binascii
 import collections.abc
 import logging
+import typing
 
 from .chainpack import ChainPack
 
 logger = logging.getLogger(__name__)
 
 
 class RpcTransportProtocol(abc.ABC):
     """Base for the implementations of RPC transport protocols."""
 
-    def __init__(
-        self,
-        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+    @classmethod
+    @abc.abstractmethod
+    async def send(
+        cls,
         write: collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
+        msg: bytes,
     ) -> None:
-        self.read = read
-        self.write = write
-
-    @abc.abstractmethod
-    async def send(self, msg: bytes) -> None:
         """Send message.
 
         :param msg: Bytes of a complete message to be sent.
         """
 
+    @classmethod
     @abc.abstractmethod
-    async def receive(self) -> bytes:
+    async def receive(
+        cls,
+        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+    ) -> bytes:
         """Receive message.
 
         :return: Bytes of complete message.
         :raise EOFError: when EOF is encountered.
         """
 
+    @classmethod
+    async def asyncio_send(cls, writer: asyncio.StreamWriter, msg: bytes) -> None:
+        """Variation on :meth:`send` that uses :class:`asyncio.StreamWriter`."""
+
+        async def write(d: bytes) -> None:
+            writer.write(d)
+            await writer.drain()
 
-def protocol_for_asyncio_stream(
-    protocol_factory: collections.abc.Callable[
-        [
-            collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
-            collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
-        ],
-        RpcTransportProtocol,
-    ],
-    reader: asyncio.StreamReader,
-    writer: asyncio.StreamWriter,
-) -> RpcTransportProtocol:
-    """Initialize :class:`RpcTransportProtocol` from Asyncio's streams.
-
-    :param protocol_factory: Callable that initializes protocol.
-    :param reader: Asyncio's stream reader.
-    :param writer: Asyncio's stream writer.
-    :return: Transport protocol instance that uses provided streams.
-    """
-
-    async def read(n: int) -> bytes:
-        try:
-            return await reader.readexactly(n)
-        except (asyncio.IncompleteReadError, ConnectionError) as exc:
-            raise EOFError from exc
-
-    async def write(d: bytes) -> None:
-        writer.write(d)
-        await writer.drain()
+        await cls.send(write, msg)
 
-    return protocol_factory(read, write)
+    @classmethod
+    async def asyncio_receive(cls, reader: asyncio.StreamReader) -> bytes:
+        """Variation on :meth:`receive` that uses :class:`asyncio.StreamReader`."""
+
+        async def read(n: int) -> bytes:
+            try:
+                return await reader.readexactly(n)
+            except (asyncio.IncompleteReadError, ConnectionError) as exc:
+                raise EOFError from exc
+
+        return await cls.receive(read)
 
 
 class RpcProtocolStream(RpcTransportProtocol):
     """SHV RPC Stream protocol."""
 
-    async def send(self, msg: bytes) -> None:
-        await self.write(ChainPack.pack_uint_data(len(msg)))
-        await self.write(msg)
+    @classmethod
+    async def send(  # noqa: D102
+        cls,
+        write: collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
+        msg: bytes,
+    ) -> None:
+        await write(ChainPack.pack_uint_data(len(msg)))
+        await write(msg)
 
-    async def receive(self) -> bytes:
+    @classmethod
+    async def receive(  # noqa: D102
+        cls,
+        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+    ) -> bytes:
         sdata = bytearray()
         while True:
-            sdata += await self.read(1)
+            sdata += await read(1)
             try:
                 size = ChainPack.unpack_uint_data(sdata)
             except ValueError:
                 pass
             else:
-                return await self.read(size)
+                return await read(size)
 
 
 class _RpcProtocolSerial(RpcTransportProtocol):
     """SHV RPC Serial protocol."""
 
     STX = 0xA2
     ETX = 0xA3
     ATX = 0xA4
     ESC = 0xAA
-    ESCMAP = {0x02: STX, 0x03: ETX, 0x04: ATX, 0x0A: ESC}
-    ESCRMAP = {v: k for k, v in ESCMAP.items()}
+    ESCMAP: typing.Final = {0x02: STX, 0x03: ETX, 0x04: ATX, 0x0A: ESC}
+    ESCRMAP: typing.Final = {v: k for k, v in ESCMAP.items()}
+
+    @classmethod
+    async def _send(
+        cls,
+        write: collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
+        msg: bytes,
+        use_crc: bool,
+    ) -> None:
+        await write(bytes((cls.STX,)))
+        escmsg = cls.escape(msg)
+        await write(escmsg)
+        await write(bytes((cls.ETX,)))
+        if use_crc:
+            await write(cls.escape(binascii.crc32(escmsg).to_bytes(4, "big")))
 
     @classmethod
     def escape(cls, data: bytes) -> bytes:
         """Escape bytes as defined for serial protocol.
 
         :param data: Data to be escaped (node that you can pass
           :class:`bytearray` to modify in place).
@@ -109,67 +125,78 @@
         # Warning: ESC must be first in the list so we first replace all occurances of
         # ESC before we insert more of them.
         for b in (cls.ESC, cls.STX, cls.ETX, cls.ATX):
             data = data.replace(bytes((b,)), bytes((cls.ESC, cls.ESCRMAP[b])))
         return data
 
     @classmethod
+    async def _receive(
+        cls,
+        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+        use_crc: bool,
+    ) -> bytes:
+        while True:
+            while (await read(1))[0] != cls.STX:
+                pass
+            data = bytearray()
+            while (b := (await read(1))[0]) not in {cls.ETX, cls.ATX}:
+                data += bytes((b,))
+            if b == cls.ATX:
+                continue
+            if use_crc:
+                crc32_br = bytearray()
+                while len(crc32_br) < (siz := 4 + crc32_br.count(bytes((cls.ESC,)))):
+                    crc32_br += await read(siz - len(crc32_br))
+                crc32_b = cls.deescape(crc32_br)
+                if int.from_bytes(crc32_b, "big") != binascii.crc32(data):
+                    continue
+            return cls.deescape(data)
+
+    @classmethod
     def deescape(cls, data: bytes) -> bytes:
         """Reverse escape operation on bytes as defined for serial protocol.
 
         :param data: Escaped data (node that you can pass :class:`bytearray` to
           modify in place).
         :return: The modified data.
         """
         for b in (cls.STX, cls.ETX, cls.ATX, cls.ESC):
             data = data.replace(bytes((cls.ESC, cls.ESCRMAP[b])), bytes((b,)))
         return data
 
-    def __init__(
-        self,
-        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
-        write: collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
-    ) -> None:
-        super().__init__(read, write)
-        self.use_crc = False
-
-    async def send(self, msg: bytes) -> None:
-        await self.write(bytes((self.STX,)))
-        escmsg = self.escape(msg)
-        await self.write(escmsg)
-        await self.write(bytes((self.ETX,)))
-        if self.use_crc:
-            await self.write(self.escape(binascii.crc32(escmsg).to_bytes(4, "big")))
-
-    async def receive(self) -> bytes:
-        while True:
-            while (await self.read(1))[0] != self.STX:
-                pass
-            data = bytearray()
-            while (b := (await self.read(1))[0]) not in (self.ETX, self.ATX):
-                data += bytes((b,))
-            if b != self.ETX:
-                continue
-            if self.use_crc:
-                crc32_br = bytearray()
-                while len(crc32_br) < (siz := 4 + crc32_br.count(bytes((self.ESC,)))):
-                    crc32_br += await self.read(siz - len(crc32_br))
-                crc32_b = self.deescape(crc32_br)
-                if int.from_bytes(crc32_b, "big") != binascii.crc32(data):
-                    continue
-            return self.deescape(data)
-
 
 class RpcProtocolSerial(_RpcProtocolSerial):
     """SHV RPC Serial protocol."""
 
+    @classmethod
+    async def send(  # noqa: D102
+        cls,
+        write: collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
+        msg: bytes,
+    ) -> None:
+        await cls._send(write, msg, False)
+
+    @classmethod
+    async def receive(  # noqa: D102
+        cls,
+        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+    ) -> bytes:
+        return await cls._receive(read, False)
+
 
 class RpcProtocolSerialCRC(_RpcProtocolSerial):
     """SHV RPC Serial protocol with CRC32 message validation."""
 
-    def __init__(
-        self,
-        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+    @classmethod
+    async def send(  # noqa: D102
+        cls,
         write: collections.abc.Callable[[bytes], collections.abc.Awaitable[None]],
+        msg: bytes,
     ) -> None:
-        super().__init__(read, write)
-        self.use_crc = True
+        await cls._send(write, msg, True)
+
+    @classmethod
+    async def receive(  # noqa: D102
+        cls,
+        read: collections.abc.Callable[[int], collections.abc.Awaitable[bytes]],
+    ) -> bytes:
+        return await cls._receive(read, True)
```

### Comparing `pyshv-0.5.0/shv/rpcurl.py` & `pyshv-0.6.0/shv/rpcurl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """SHV RPC URL for RpcClient and RpcServer."""
+
 import dataclasses
 import enum
 import functools
 import getpass
 import urllib.parse
 
-from .value import SHVType
+from .rpclogin import RpcLogin, RpcLoginType
 
 
 @functools.lru_cache
 def _get_user() -> str:
     # getuser fails if there is no account assigned to the UID in the system
     try:
         return getpass.getuser()
@@ -32,27 +33,14 @@
     """Unix local domain named socket using Stream transport layer."""
     UNIXS = enum.auto()
     """Unix local domain named socket using Reliable Serial transport layer."""
     SERIAL = enum.auto()
     """Serial transport layer."""
 
 
-class RpcLoginType(enum.Enum):
-    """Enum specifying which login type should be used.
-
-    The string values are the exact string representation used in SHV RPC
-    protocol identifying these login types.
-    """
-
-    PLAIN = "PLAIN"
-    """Plain login format should be used."""
-    SHA1 = "SHA1"
-    """Use hash algorithm SHA1 (preferred and common default)."""
-
-
 @dataclasses.dataclass
 class RpcUrl:
     """SHV RPC URL specifier.
 
     This is unified locator for SHV RPC connections that is used to specify
     connections. It is implemented as :func:`dataclasses.dataclass` and you
     can set properties directly or you can parse string URL.
@@ -68,48 +56,31 @@
     .. versionchanged:: 0.3.0
        This attribute was named ``host`` in version 0.2.0.
     """
     port: int = -1
     """Port the SHV RPC server is listening on."""
     protocol: RpcProtocol = RpcProtocol.TCP
     """SHV RPC protocol used to communicate (This is scheme in URL therminology)"""
-    username: str = _get_user()
-    """User name used to login to the remote server."""
+    login: RpcLogin = dataclasses.field(default_factory=RpcLogin)
+    """Parameters for RPC Broker login."""
 
-    # Options
-    password: str = ""
-    """Password used to login to the server."""
-    login_type: RpcLoginType = RpcLoginType.PLAIN
-    """Type of the login to be used (specifies format of the password)."""
-    device_id: str | None = None
-    """Device identifier sent to the server with login."""
-    device_mount_point: str | None = None
-    """Request for mounting of connected device to the specified mount point."""
+    # TTY
     baudrate: int = 115200
     """Baudrate used for some of the link protocols."""
 
     def __post_init__(self) -> None:
         """Deduce the correct value for port."""
         if self.port == type(self).port:
             self.port = {
                 RpcProtocol.TCP: 3755,
                 RpcProtocol.TCPS: 3765,
                 RpcProtocol.SSL: 3756,
                 RpcProtocol.SSLS: 3766,
             }.get(self.protocol, self.port)
 
-    def login_options(self) -> dict[str, SHVType]:
-        """Assemble login options for the SHV RPC broker from options here."""
-        res: dict[str, SHVType] = {}
-        if self.device_id:
-            res["deviceId"] = self.device_id
-        if self.device_mount_point:
-            res["mountPoint"] = self.device_mount_point
-        return {"device": res} if res else {}
-
     def __str__(self) -> str:
         return self.to_url()
 
     @classmethod
     def parse(cls, url: str) -> "RpcUrl":
         """Parse string URL to the object representation.
 
@@ -132,47 +103,47 @@
         }
         if sr.scheme not in protocols:
             raise ValueError(f"Invalid scheme: {sr.scheme}")
         protocol = protocols[sr.scheme]
 
         res = cls("", protocol=protocol)
 
-        res.username = sr.username or res.username
-        if protocol in (
+        res.login.username = sr.username or res.login.username
+        if protocol in {
             RpcProtocol.TCP,
             RpcProtocol.TCPS,
             RpcProtocol.SSL,
             RpcProtocol.SSLS,
-        ):
+        }:
             res.location = sr.hostname or ""
             if sr.port is not None:
                 res.port = int(sr.port)
             if sr.path:
                 raise ValueError(f"Path is not supported for {sr.scheme}: {sr.path}")
-        elif protocol in (RpcProtocol.UNIX, RpcProtocol.UNIXS, RpcProtocol.SERIAL):
+        elif protocol in {RpcProtocol.UNIX, RpcProtocol.UNIXS, RpcProtocol.SERIAL}:
             res.location = f"/{sr.netloc}{sr.path}" if sr.netloc else sr.path
         else:
             raise NotImplementedError  # pragma: no cover
 
         if opts := pqs.pop("user", []):
-            res.username = opts[0]
+            res.login.username = opts[0]
         if opts := pqs.pop("shapass", []):
             if len(opts[0]) != 40:
                 raise ValueError("SHA1 password must have 40 characters.")
-            res.password = opts[0]
-            res.login_type = RpcLoginType.SHA1
+            res.login.password = opts[0]
+            res.login.login_type = RpcLoginType.SHA1
             # We prefer SHA1 password and thus discard plain if both are present
             pqs.pop("password", [])
         elif opts := pqs.pop("password", []):
-            res.password = opts[0]
-            res.login_type = RpcLoginType.PLAIN
+            res.login.password = opts[0]
+            res.login.login_type = RpcLoginType.PLAIN
         if opts := pqs.pop("devid", []):
-            res.device_id = opts[0]
+            res.login.device_id = opts[0]
         if opts := pqs.pop("devmount", []):
-            res.device_mount_point = opts[0]
+            res.login.device_mount_point = opts[0]
         if protocol is RpcProtocol.SERIAL:
             if opts := pqs.pop("baudrate", []):
                 res.baudrate = int(opts[0])
 
         if pqs:
             raise ValueError(f"Unsupported URL queries: {', '.join(pqs.keys())}")
 
@@ -185,48 +156,48 @@
             RpcProtocol.TCPS: "tcps",
             RpcProtocol.SSL: "ssl",
             RpcProtocol.SSLS: "ssls",
             RpcProtocol.UNIX: "unix",
             RpcProtocol.UNIXS: "unixs",
             RpcProtocol.SERIAL: "serial",
         }
-        user_added = not self.username or self.username == type(self).username
-        if self.protocol in (
+        user_added = not self.login.username or self.login.username == RpcLogin.username
+        if self.protocol in {
             RpcProtocol.TCP,
             RpcProtocol.TCPS,
             RpcProtocol.SSL,
             RpcProtocol.SSLS,
-        ):
+        }:
             netloc = "//"
             if not user_added:
-                netloc += f"{self.username}@"
+                netloc += f"{self.login.username}@"
                 user_added = True
             if ":" in self.location:
                 netloc += f"[{self.location}]"
             else:
                 netloc += self.location
             netloc += f":{self.port}"
-        elif self.protocol in (RpcProtocol.UNIX, RpcProtocol.UNIXS, RpcProtocol.SERIAL):
+        elif self.protocol in {RpcProtocol.UNIX, RpcProtocol.UNIXS, RpcProtocol.SERIAL}:
             netloc = self.location
         else:
             raise NotImplementedError  # pragma: no cover
 
         opts: list[str] = []
         if not user_added:
-            opts.append(f"user={urllib.parse.quote(self.username)}")
+            opts.append(f"user={urllib.parse.quote(self.login.username)}")
             user_added = True
-        if self.device_id:
-            opts.append(f"devid={urllib.parse.quote(self.device_id)}")
-        if self.device_mount_point:
-            opts.append(f"devmount={urllib.parse.quote(self.device_mount_point)}")
-        if self.password:
-            if self.login_type is RpcLoginType.SHA1:
-                opts.append(f"shapass={self.password}")
-            elif self.login_type is RpcLoginType.PLAIN:
-                opts.append(f"password={urllib.parse.quote(self.password)}")
+        if self.login.device_id:
+            opts.append(f"devid={urllib.parse.quote(self.login.device_id)}")
+        if self.login.device_mount_point:
+            opts.append(f"devmount={urllib.parse.quote(self.login.device_mount_point)}")
+        if self.login.password:
+            if self.login.login_type is RpcLoginType.SHA1:
+                opts.append(f"shapass={self.login.password}")
+            elif self.login.login_type is RpcLoginType.PLAIN:
+                opts.append(f"password={urllib.parse.quote(self.login.password)}")
             else:
                 raise NotImplementedError()  # pragma: no cover
         if self.baudrate != type(self).baudrate:
             opts.append(f"baudrate={self.baudrate}")
 
         return (
             f"{protocols[self.protocol]}:{netloc}{'?' if opts else ''}{'&'.join(opts)}"
```

### Comparing `pyshv-0.5.0/shv/simpleclient.py` & `pyshv-0.6.0/shv/simplebase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,92 @@
-"""RPC client manager that provides facitility to simply connect to the broker."""
+"""The base for the various high level SHV RPC interfaces."""
+
 import asyncio
 import collections.abc
+import contextlib
+import datetime
 import logging
-import time
 import traceback
-import typing
 
-from .rpcclient import RpcClient, connect_rpc_client
+from .__version__ import VERSION
+from .rpcclient import RpcClient
 from .rpcerrors import (
     RpcError,
     RpcInvalidParamsError,
     RpcMethodCallExceptionError,
     RpcMethodNotFoundError,
+    RpcUserIDRequiredError,
 )
-from .rpclogin import rpclogin_url
 from .rpcmessage import RpcMessage
 from .rpcmethod import RpcMethodAccess, RpcMethodDesc
-from .rpcsubscription import RpcSubscription
-from .rpcurl import RpcUrl
 from .shvversion import SHV_VERSION_MAJOR, SHV_VERSION_MINOR
 from .value import SHVType, is_shvbool, is_shvnull
 
 logger = logging.getLogger(__name__)
 
 
-class SimpleClient:
-    """SHV client made simple to use.
+class SimpleBase:
+    """SHV RPC made simple to use.
 
-    You most likely want to use this client instead of using RpcClient directly.
+    You want to use this if you plan to implement your own specific RPC handler
+    but in most cases you might want to use :class:`SimpleClient` or
+    :class:`SimpleDevice` instead.
 
     Messages are handled in an asyncio loop and based on the type of the message
     the different operation is performed.
     """
 
     IDLE_TIMEOUT: float = 180
     """Number of seconds before we are disconnected from the broker automatically."""
 
     APP_NAME: str = "pyshv"
     """Name of the application reported to the SHV.
 
     You can change this value in child class to report a more accurate
     application name.
     """
-    APP_VERSION: str = "unknown"
+    APP_VERSION: str = VERSION
     """Version of the application reported to the SHV.
 
     You should change this value in child class to report a correct number.
+
+    :param client: The RPC client instance to wrap and manage.
+    :param call_attempts: Number of attempts for :meth:`call` when no response
+      is received before call is abandoned. You can use zero (or negative
+      number) for unlimited number of attempts. The default is a single attempt
+      and this only regular one call.
+    :param call_timeout: Timeout in seconds before call is attempted again or
+      abandoned (if there was too much call attempts). This is time before we
+      consider response to be lost.
     """
 
     def __init__(
         self,
         client: RpcClient,
         call_attempts: int = 1,
         call_timeout: float | None = 300.0,
-        idle_disconnect: bool = False,
-    ):
+    ) -> None:
         self.client = client
-        """The underlaying RPC client instance."""
+        """The underlaying RPC client instance.
+
+        **Do not send messages by directly accessing this property. You must use
+        implementations provided by this class!**
+        """
         self.task = asyncio.create_task(self._loop())
-        """Task running the message handling loop."""
+        """Task running the message handling receive loop."""
         self.call_attempts = call_attempts
-        """Number of attempts when no response is received before call is abandoned."""
+        """Number of attempts when no response is received before call is abandoned.
+        You can use zero for no  or negative number to have unlimited attempts.
+        """
         self.call_timeout = call_timeout
         """Timeout in seconds before call is attempted again or abandoned."""
-        self.idle_disconnect = idle_disconnect
-        """If client should be disconnected on IDLE_TIMEOUT instead of ping."""
         self._calls_event: dict[int, asyncio.Event] = {}
         self._calls_msg: dict[int, RpcMessage] = {}
         self.__peer_is_shv3: None | bool = None
 
-    # TODO solve type hinting in this method. It seems that right now it is not
-    # possible to correctly type hint the args and kwargs to copy Self # params.
-    # https://discuss.python.org/t/how-to-properly-hint-a-class-factory-with-paramspec/27941/3
-    @classmethod
-    async def connect(
-        cls: type[typing.Self],
-        url: RpcUrl,
-        *args: typing.Any,
-        **kwargs: typing.Any,
-    ) -> typing.Self:
-        """Connect and login to the SHV broker.
-
-        Any additional parameters after ``url`` are passed to class
-        initialization.
-
-        :param url: SHV RPC URL to the broker
-        :return: Connected instance.
-        """
-        client = await connect_rpc_client(url)
-        await rpclogin_url(client, url, {"idleWatchDogTimeOut": int(cls.IDLE_TIMEOUT)})
-        return cls(client, *args, **kwargs)
-
     async def disconnect(self) -> None:
         """Disconnect an existing connection.
 
         The call to the disconnect when client is not connected is silently
         ignored.
 
         This call blocks until disconnect is completed. You can use
@@ -102,278 +94,315 @@
         for it to take an effect.
         """
         self.client.disconnect()
         await self.task
 
     async def _loop(self) -> None:
         """Loop run in asyncio task to receive messages."""
-        activity_task = asyncio.create_task(self._activity_loop())
-        try:
+        tasks = set()
+        with contextlib.suppress(EOFError):
             while msg := await self.client.receive(raise_error=False):
-                asyncio.create_task(self._message(msg))
-        except EOFError:
-            pass
-        activity_task.cancel()
-        try:
-            await activity_task
-        except asyncio.exceptions.CancelledError:
-            pass
-
-    async def _activity_loop(self) -> None:
-        """Loop run alongside with :meth:`_loop`.
-
-        It either sends pings to the other side or it disconnects other side when
-        idling. The operation is based on :param:`idle_disconnect`.
-        """
-        while self.client.connected:
-            if self.idle_disconnect:
-                t = time.monotonic() - self.client.last_receive
-                if t < self.IDLE_TIMEOUT:
-                    await asyncio.sleep(self.IDLE_TIMEOUT - t)
-                else:
-                    await self.disconnect()
-            else:
-                t = time.monotonic() - self.client.last_send
-                if t < (self.IDLE_TIMEOUT / 2):
-                    await asyncio.sleep(self.IDLE_TIMEOUT / 2 - t)
+                if msg is RpcClient.Control.RESET:
+                    self._reset()
+                elif msg.is_valid():
+                    tasks.add(asyncio.create_task(self._message(msg)))
                 else:
-                    await self.client.send(
-                        RpcMessage.request(
-                            ".app"
-                            if await self._peer_is_shv3()
-                            else ".broker/currentClient",
-                            "ping",
-                        )
-                    )
-
-    async def _message(self, msg: RpcMessage) -> None:
-        """Handle every received message."""
-        if msg.is_request:
-            resp = msg.make_response()
-            method = msg.method
-            assert method  # is ensured by is_request but not detected by mypy
-            try:
-                resp.result = await self._method_call(
-                    msg.path,
-                    method,
-                    msg.rpc_access or RpcMethodAccess.BROWSE,
-                    msg.param,
-                )
-            except RpcError as exp:
-                resp.rpc_error = exp
-            except Exception as exc:
-                resp.rpc_error = RpcMethodCallExceptionError(
-                    "".join(traceback.format_exception(exc))
-                )
-            await self.client.send(resp)
-        elif msg.is_response:
-            rid = msg.request_id
-            assert rid is not None
-            if rid in self._calls_event:
-                self._calls_msg[rid] = msg
-                self._calls_event.pop(rid).set()
-        elif msg.is_signal:
-            if msg.method == "chng":
-                await self._value_update(msg.path, msg.param)
+                    logger.info("%s: Dropped invalid message: %s", self.client, msg)
+                # Drop finished tasks
+                done = {t for t in tasks if t.done()}
+                self.__task_done(done)
+                tasks -= done
+        done, _ = await asyncio.wait(tasks)
+        self.__task_done(done)
+
+    def __task_done(self, tasks: collections.abc.Iterable[asyncio.Task]) -> None:
+        for task in tasks:
+            if exc := task.exception():
+                logger.info("%s: Message handlig failed", self.client, exc_info=exc)
+
+    def _reset(self) -> None:
+        """Handle peer's reset request."""
+        logger.info("%s: Doing reset", self.client)
+        for event in self._calls_event.values():
+            event.set()
+
+    async def reset(self) -> None:
+        """Reset the client and connection.
+
+        This calls :meth:`RpcClient.reset` as well as reset of the internal
+        state.
+        """
+        await self.client.reset()
+        self._reset()
+
+    async def _send(self, msg: RpcMessage) -> None:
+        """Send message.
+
+        Use this only if you want send a generic message (such as when you are
+        passing message along). :meth:`call` or :meth:`_signal` should be
+        prefered when ever possible.
+
+        You should be using this method instead of ``self.client.send`` to
+        ensure that send can be correctly overwritten and optionally postponed
+        or blocked by child implementations.
+        """
+        await self.client.send(msg)
 
-    async def call(self, path: str, method: str, param: SHVType = None) -> SHVType:
+    async def call(
+        self,
+        path: str,
+        method: str,
+        param: SHVType = None,
+        call_attempts: int | None = None,
+        call_timeout: float | None = None,
+        user_id: str | None = None,
+    ) -> SHVType:
         """Call given method on given path with given parameter.
 
-        Note that this is coroutine and this it is up to you if you await it or
+        Note that this is coroutine and thus it is up to you if you await it or
         use asyncio tasks.
 
+        The delivery of the messages is not ensure in SHV network (they can be
+        dropped due to multiple reasons without informing the source of the
+        message) and thus this method can attempt the request sending multiple
+        times if it doesn't receive an appropriate response.
+
         :param path: SHV path method is associated with.
         :param method: SHV method name to be called.
         :param param: Parameter passed to the called method.
+        :param call_attempts: Allows override of the object setting.
+        :param call_timeout: Allows override of the object setting.
+        :param user_id: UserID added to the method call request. This is required
+          by some RPC methods to identify the user and they will respond with
+          :class:`RpcUserIDRequiredError` if it is missing. This is caught by
+          this method and request will be attempted again (not counting in
+          ``call_attempts``) with User ID ``""``. If you know that method needs
+          User ID then you can prevent this round trip by setting this argument
+          to ``""``. On the other hand sending all requests with User ID wastes
+          with bandwidth.
         :return: Return value on successful method call.
         :raise RpcError: The call result in error that is propagated by raising
             `RpcError` or its children based on the failure.
         :raise TimeoutError: when response is not received before timeout with
             all attempts depleted.
+        :raise EOFError: when client disconnected and thus request can't be sent
+          or response received.
         """
-        msg = RpcMessage.request(path, method, param)
-        rid = msg.request_id
+        call_attempts = self.call_attempts if call_attempts is None else call_attempts
+        call_timeout = self.call_timeout if call_timeout is None else call_timeout
+        request = RpcMessage.request(path, method, param, user_id=user_id)
         event = asyncio.Event()
-        self._calls_event[rid] = event
-        for _ in range(self.call_attempts):
-            await self.client.send(msg)
+        self._calls_event[request.request_id] = event
+        attempt = 0
+        while call_attempts < 1 or attempt < call_attempts:
+            attempt += 1
+            await self._send(request)
             try:
-                async with asyncio.timeout(self.call_timeout):
+                async with asyncio.timeout(call_timeout):
                     await event.wait()
             except TimeoutError:
                 continue
-            msg = self._calls_msg.pop(rid)
-            if msg.is_error:
-                raise msg.rpc_error
-            return msg.result
+            if request.request_id not in self._calls_msg:
+                self._calls_event[request.request_id].clear()
+                continue
+            response = self._calls_msg.pop(request.request_id)
+            if response.is_error:
+                rpc_error = response.rpc_error
+                if not isinstance(rpc_error, RpcUserIDRequiredError):
+                    raise response.rpc_error
+                attempt -= 1  # Annul this attempt
+                request.user_id = ""
+                event.clear()
+                self._calls_event[request.new_request_id()] = event
+                continue
+            return response.result
         raise TimeoutError
 
-    async def signal(
-        self,
-        path: str,
-        method: str = "chng",
-        param: SHVType = None,
-        access: RpcMethodAccess = RpcMethodAccess.READ,
-    ) -> None:
-        """Send signal from given path and method and with given parameter.
-
-        Note that this is coroutine and this it is up to you if you await it or
-        use asyncio tasks.
-
-        :param path: SHV path method is associated with.
-        :param method: SHV method name to be called.
-        :param param: Parameter that is the signaled value.
-        :param access: Minimal access level needed to get the signal.
-        """
-        msg = RpcMessage.signal(path, method, param, access)
-        await self.client.send(msg)
+    async def ping(self) -> None:
+        """Ping the peer to check the connection."""
+        await self.call(
+            ".app" if await self.peer_is_shv3() else ".broker/currentClient",
+            "ping",
+        )
 
     async def ls(self, path: str) -> list[str]:
         """List child nodes of the node on the specified path.
 
         :param path: SHV path to the node we want children to be listed for.
         :return: list of child nodes.
         :raise RpcMethodNotFoundError: when there is no such path.
         """
         res = await self.call(path, "ls")
-        if not isinstance(res, list):
-            raise RpcMethodCallExceptionError(f"Invalid result returned: {repr(res)}")
+        if not isinstance(res, list):  # pragma: no cover
+            raise RpcMethodCallExceptionError(f"Invalid result returned: {res!r}")
         return res
 
     async def ls_has_child(self, path: str, name: str) -> bool:
         """Use ``ls`` method to check for child.
 
         :param path: SHV path to the node with possible child of given name.
         :param name: Name of the child node.
         :return: ``True`` if there is such child and ``False`` if not.
         :raise RpcMethodNotFoundError: when there is no such path.
         """
         res = await self.call(path, "ls", name)
-        if not isinstance(res, bool):
-            raise RpcMethodCallExceptionError(f"Invalid result returned: {repr(res)}")
+        if not isinstance(res, bool):  # pragma: no cover
+            raise RpcMethodCallExceptionError(f"Invalid result returned: {res!r}")
         return res
 
     async def dir(self, path: str, details: bool = False) -> list[RpcMethodDesc]:
         """List methods associated with node on the specified path.
 
         :param path: SHV path to the node we want methods to be listed for.
         :param details: If detailed listing should be performed instead of standard one.
         :return: list of the node's methods.
         :raise RpcMethodNotFoundError: when there is no such path.
         """
         res = await self.call(path, "dir", True if details else None)
-        if isinstance(res, list):
-            return [RpcMethodDesc.fromshv(m) for m in res]
-        raise RpcMethodCallExceptionError(f"Invalid result returned: {repr(res)}")
+        if isinstance(res, list):  # pragma: no cover
+            return [RpcMethodDesc.from_shv(m) for m in res]
+        raise RpcMethodCallExceptionError(f"Invalid result returned: {res!r}")
 
-    async def dir_description(self, path: str, name: str) -> RpcMethodDesc | None:
-        """Get method description associated with node on the specified path.
+    async def dir_exists(self, path: str, name: str) -> bool:
+        """Check if method exists using ``dir`` method.
 
         :param path: SHV path to the node we want methods to be listed for.
-        :param name: Name of the method description to be received for.
-        :return: Method description or ``None`` in case there is no such method.
+        :param name: Name of the method which existence should be checked.
+        :return: ``True`` if method exists and ``False`` otherwise.
         :raise RpcMethodNotFoundError: when there is no such path.
         """
         res = await self.call(path, "dir", name)
-        if isinstance(res, list):  # TODO backward compatibility
-            res = res[0] if len(res) == 1 else None
-        if is_shvnull(res):
-            return None
-        return RpcMethodDesc.fromshv(res)
-
-    async def subscribe(self, sub: RpcSubscription) -> None:
-        """Perform subscribe for signals on given path.
+        # list, null and mapping is backward compatibility
+        if not isinstance(
+            res, bool | None | collections.abc.Mapping | collections.abc.Sequence
+        ):  # pragma: no cover
+            raise RpcMethodCallExceptionError(f"Invalid result returned: {res!r}")
+        return bool(res)
 
-        Subscribe is always performed on the node itself as well as all its
-        children.
-
-        :param sub: SHV RPC subscription to be added.
-        """
-        await self.call(
-            ".app/broker/currentClient"
-            if await self._peer_is_shv3()
-            else ".broker/app",
-            "subscribe",
-            sub.toSHV(),
-        )
-
-    async def unsubscribe(self, sub: RpcSubscription) -> bool:
-        """Perform unsubscribe for signals on given path.
-
-        :param sub: SHV RPC subscription to be removed.
-        :return: ``True`` in case such subscribe was located and ``False`` otherwise.
-        """
-        resp = await self.call(
-            ".app/broker/currentClient"
-            if await self._peer_is_shv3()
-            else ".broker/app",
-            "unsubscribe",
-            sub.toSHV(),
-        )
-        assert is_shvbool(resp)
-        return bool(resp)
-
-    async def _peer_is_shv3(self) -> bool:
+    async def peer_is_shv3(self) -> bool:
         """Check if peer supports at least SHV 3.0."""
         if self.__peer_is_shv3 is None:
             try:
                 major = await self.call(".app", "shvVersionMajor")
                 self.__peer_is_shv3 = isinstance(major, int) and major >= 0
             except RpcError:
                 self.__peer_is_shv3 = False
         return self.__peer_is_shv3
 
+    async def _signal(
+        self,
+        path: str,
+        name: str = "chng",
+        source: str = "get",
+        value: SHVType = None,
+        access: RpcMethodAccess = RpcMethodAccess.READ,
+    ) -> None:
+        """Send signal from given path and method source and with given parameter.
+
+        Note that this is coroutine and thus it is up to you if you await it or
+        use asyncio tasks.
+
+        This is intentionally marked as accessible only by class methods because
+        signals must be raised only for valid paths and methods and that is
+        something only class itself can ensure. Your implemntation should
+        provide public methods that protects against call with invalid path or
+        method.
+
+        :param path: SHV path signal is associated with.
+        :param name: Signal name to be raised.
+        :param source: Method name this signal is associated with.
+        :param value: Parameter that is the signaled value.
+        :param access: Minimal access level needed to access the signal.
+        """
+        await self._send(RpcMessage.signal(path, name, source, value, access))
+
+    async def _message(self, msg: RpcMessage) -> None:
+        """Handle every received message."""
+        if msg.is_request:
+            resp = msg.make_response()
+            method = msg.method
+            try:
+                resp.result = await self._method_call(
+                    msg.path,
+                    method,
+                    msg.param,
+                    msg.rpc_access or RpcMethodAccess.BROWSE,
+                    msg.user_id,
+                )
+            except RpcError as exp:
+                resp.rpc_error = exp
+            except Exception as exc:
+                resp.rpc_error = RpcMethodCallExceptionError(
+                    "".join(traceback.format_exception(exc))
+                )
+            await self._send(resp)
+        elif msg.is_response:
+            rid = msg.request_id
+            if rid in self._calls_event:
+                self._calls_msg[rid] = msg
+                self._calls_event.pop(rid).set()
+        elif msg.is_signal:
+            await self._got_signal(msg.path, msg.signal_name, msg.source, msg.param)
+
     async def _method_call(
-        self, path: str, method: str, access: RpcMethodAccess, param: SHVType
+        self,
+        path: str,
+        method: str,
+        param: SHVType,
+        access: RpcMethodAccess,
+        user_id: str | None,
     ) -> SHVType:
-        """Handle request in the provided message.
+        """Handle request.
 
         :param path: SHV path to the node the method is associated with.
         :param method: method requested to be called.
-        :param access: access level of the client specified in the request.
         :param param: Parameter to be passed to the called method.
+        :param access: access level of the client specified in the request.
+        :param client_id: The client's ID collected as message was passed
+          around. This can be ``None`` when request message contained no ID. You
+          can raise :class:`RpcUserIDRequiredError` if you need it.
         :return: result of the method call. To report error you should raise
             :exc:`RpcError`.
         """
-        if method == "ls":
-            return self._method_call_ls(path, param)
-        if method == "dir":
-            return self._method_call_dir(path, param)
-        if path == ".app":
-            match method:
-                case "shvVersionMajor":
-                    return SHV_VERSION_MAJOR
-                case "shvVersionMinor":
-                    return SHV_VERSION_MINOR
-                case "name":
-                    return self.APP_NAME
-                case "version":
-                    return self.APP_VERSION
-                case "ping":
-                    return None
+        match path, method:
+            case _, "ls":
+                return self._method_call_ls(path, param)
+            case _, "dir":
+                return self._method_call_dir(path, param)
+            case ".app", "shvVersionMajor":
+                return SHV_VERSION_MAJOR
+            case ".app", "shvVersionMinor":
+                return SHV_VERSION_MINOR
+            case ".app", "name":
+                return self.APP_NAME
+            case ".app", "version":
+                return self.APP_VERSION
+            case ".app", "date":
+                return datetime.datetime.now().astimezone()
+            case ".app", "ping":
+                return None
         raise RpcMethodNotFoundError(
             f"No such path '{path}' or method '{method}' or access rights."
         )
 
     def _method_call_ls(self, path: str, param: SHVType) -> SHVType:
         """Implement ``ls`` method call functionality."""
-        # TODO list is backward compatibility
-        if is_shvnull(param) or isinstance(param, list):
+        if is_shvnull(param):
             res = []
             for v in self._ls(path):
                 if v not in res:
                     res.append(v)
             if not res and not self._valid_path(path):
                 raise RpcMethodNotFoundError(f"No such node: {path}")
             return res
         if isinstance(param, str):
             return any(v == param for v in self._ls(path))
         raise RpcInvalidParamsError("Use Null or String with node name")
 
-    def _ls(self, path: str) -> typing.Iterator[str]:
+    def _ls(self, path: str) -> collections.abc.Iterator[str]:  # noqa: PLR6301
         """Implement ``ls`` method for all nodes.
 
         The default implementation supports `.app` path. Your implementation
         should yield child nodes.
 
         Always call this as first before you yield your own methods to provide
         users with standard nodes.
@@ -384,69 +413,61 @@
         if not path:
             yield ".app"
 
     def _valid_path(self, path: str) -> bool:
         """Check that :meth:`_ls` reports this path as existing.
 
         :param path: SHV path to be validated.
-        :return: ``True`` if :meth:`_ls` on parent node reports node with this tail
-            piece. ``False`` is returned otherwise.
+        :return: ``True`` if :meth:`_ls` on parent node reports node with this
+          tail piece. ``False`` is returned otherwise.
         """
         if not path:
             return True  # The root path always exists
-        if "/" in path:
-            index = path.rindex("/")
-            return any(path[index + 1 :] == v for v in self._ls(path[:index]))
-        return any(path == v for v in self._ls(""))
-
-    async def _lschng(
-        self, path: str, nodes: collections.abc.Mapping[str, bool]
-    ) -> None:
-        """Report change in the ls method.
-
-        This provides implementation for "lschng" signal that must be used when you are
-        changing the nodes tree to signal clients about that. The argument specifies top
-        level nodes added or removed (based on the mapping value).
-
-        :param path: SHV path to the valid node which children were added or removed.
-        :param nodes: Map where key is node name of the node that is top level node,
-          that was either added (for value ``True``) or removed (for value ``False``).
-        """
-        await self.signal(path, "lschng", nodes, RpcMethodAccess.BROWSE)
+        root, _, name = path.rpartition("/")
+        return any(name == v for v in self._ls(root))
 
     def _method_call_dir(self, path: str, param: SHVType) -> SHVType:
         """Implement ``dir`` method call functionality."""
         if not self._valid_path(path):
             raise RpcMethodNotFoundError(f"No such node: {path}")
-        # TODO the list here is backward compatibility
-        if is_shvnull(param) or is_shvbool(param) or isinstance(param, list):
-            return list(d.toshv(bool(param)) for d in self._dir(path))
+        if is_shvnull(param) or is_shvbool(param):
+            return list(d.to_shv(bool(param)) for d in self._dir(path))
         if isinstance(param, str):
-            for d in self._dir(path):
-                if d.name == param:
-                    return d.toshv()
-            return None
+            return any(v.name == param for v in self._dir(path))
         raise RpcInvalidParamsError("Use Null or Bool or String with node name")
 
-    def _dir(self, path: str) -> typing.Iterator[RpcMethodDesc]:
+    def _dir(self, path: str) -> collections.abc.Iterator[RpcMethodDesc]:  # noqa: PLR6301
         """Implement ``dir`` method for all nodes.
 
         This implementation is called only for valid paths (:meth:`_valid_path`).
 
         Always call this as first before you yield your own methods to provide
         users with standard ones.
 
         :param path: SHV path method should be listed for.
         :return: List of methods associated with given node.
         """
         yield RpcMethodDesc.stddir()
         yield RpcMethodDesc.stdls()
-        yield RpcMethodDesc.stdlschng()
         if path == ".app":
             yield RpcMethodDesc.getter("shvVersionMajor", "Null", "Int")
             yield RpcMethodDesc.getter("shvVersionMinor", "Null", "Int")
             yield RpcMethodDesc.getter("name", "Null", "String")
             yield RpcMethodDesc.getter("version", "Null", "String")
+            yield RpcMethodDesc.getter("date", "Null", "DateTime")
             yield RpcMethodDesc("ping")
 
+    async def _got_signal(
+        self, path: str, signal: str, source: str, value: SHVType
+    ) -> None:
+        """Handle signal.
+
+        :param path: SHV path to the node the signal is associated with.
+        :param signal: Signal name.
+        :param source: Method name signal is associated with.
+        :param value: The value caried by signal.
+        """
+        if signal.endswith("chng") and source == "get":
+            await self._value_update(path, value)
+
     async def _value_update(self, path: str, value: SHVType) -> None:
-        """Handle value change (`chng` method)."""
+        """Handle value change (``*chng`` signal associated with ``get`` method)."""
```

### Comparing `pyshv-0.5.0/shv/value.py` & `pyshv-0.6.0/shv/value.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Values used in SHV communication."""
+
 import abc
 import collections.abc
 import datetime
 import decimal
 import functools
 import itertools
 import typing
 
 SHVNullType: typing.TypeAlias = typing.Union[None, "SHVNull"]
 SHVBoolType: typing.TypeAlias = typing.Union[bool, "SHVBool"]
 SHVListType: typing.TypeAlias = collections.abc.Sequence["SHVType"]
 SHVMapType: typing.TypeAlias = collections.abc.Mapping[str, "SHVType"]
 SHVIMapType: typing.TypeAlias = collections.abc.Mapping[int, "SHVType"]
-SHVType: typing.TypeAlias = typing.Union[
-    SHVNullType,
-    SHVBoolType,
-    int,
-    float,
-    decimal.Decimal,
-    bytes,
-    str,
-    datetime.datetime,
-    SHVListType,
-    SHVMapType,
-    SHVIMapType,
-    SHVIMapType,
-    SHVMapType,
-]
+SHVType: typing.TypeAlias = (
+    SHVNullType
+    | SHVBoolType
+    | int
+    | float
+    | decimal.Decimal
+    | bytes
+    | str
+    | datetime.datetime
+    | SHVListType
+    | SHVMapType
+    | SHVIMapType
+    | SHVIMapType
+    | SHVMapType
+)
 SHVMetaType: typing.TypeAlias = collections.abc.MutableMapping[int | str, SHVType]
 
 
-class SHVMeta(abc.ABC):
+class SHVMeta(abc.ABC):  # noqa B024
     """SHV values can have meta with attributes associated with them.
 
     This provides meta attribute that can be added to other types. Only create
     class that has as parent this class and the class you want to wrap. The
     SHVMeta provides you with meta attribute that you can use to store and
     access meta attributes. Thanks to it being both parent of SHVMeta as well as
     original type you can use isinstance to detect type. For example to check if
@@ -51,19 +52,19 @@
         modifiable. You can use :func:`shvmeta_eq` to compare with meta.
     """
 
     @property
     def meta(self) -> SHVMetaType:
         """Meta attributes for this SHV type."""
         if not hasattr(self, "_meta"):
-            setattr(self, "_meta", {})
-        return typing.cast(SHVMetaType, getattr(self, "_meta"))
+            self._meta: SHVMetaType = {}
+        return typing.cast(SHVMetaType, self._meta)
 
     @staticmethod
-    def new(value: typing.Any, meta: SHVMetaType | None = None) -> SHVType:
+    def new(value: object, meta: SHVMetaType | None = None) -> SHVType:
         """Create new value with given meta.
 
         This select an appropriate class based on the value passed.
 
         You can also use it to set meta value to newly created object because
         when `value` is of `SHVMeta` it returns the same object and only updates
         provided meta.
@@ -90,37 +91,37 @@
         elif isinstance(value, collections.abc.Sequence):
             res = SHVList(value)
         elif is_shvimap(value):
             res = SHVIMap(value)
         elif is_shvmap(value):
             res = SHVMap(value)
         else:
-            raise ValueError(f"Invalid SHV value: {repr(value)}")
+            raise ValueError(f"Invalid SHV value: {value!r}")
         if meta:
             res.meta.update(meta)
         return typing.cast(SHVType, res)
 
 
-def shvmeta(value: SHVType) -> SHVMetaType:
+def shvmeta(value: object) -> SHVMetaType:
     """Get SHV Meta or provide empty dict as a fallback."""
     if isinstance(value, SHVMeta):
         return value.meta
     return {}
 
 
-def shvmeta_eq(v1: typing.Any, v2: typing.Any) -> bool:
+def shvmeta_eq(v1: object, v2: object) -> bool:
     """Perform comparison including the :class:`SHVMeta` not just plain values."""
     if shvmeta(v1) != shvmeta(v2):
         return False
     if isinstance(v1, SHVUInt) != isinstance(v2, SHVUInt):
         return False
     if (
         isinstance(v1, collections.abc.Sequence)
         and isinstance(v2, collections.abc.Sequence)
-        and not (isinstance(v1, (str, bytes)) or isinstance(v2, (str, bytes)))
+        and not (isinstance(v1, str | bytes) or isinstance(v2, str | bytes))
     ):
         return len(v1) == len(v2) and all(
             shvmeta_eq(v1[i], v2[i]) for i in range(len(v1))
         )
     if isinstance(v1, collections.abc.Mapping) and isinstance(
         v2, collections.abc.Mapping
     ):
@@ -133,43 +134,43 @@
 
 class SHVNull(SHVMeta):
     """Null (None) with :class:`SHVMeta`."""
 
     def __bool__(self) -> bool:
         return False
 
-    def __eq__(self, value: typing.Any) -> bool:
+    def __eq__(self, value: object) -> bool:
         return value is None or isinstance(value, SHVNull)
 
     def __hash__(self) -> int:
         return hash(None)
 
 
-def is_shvnull(value: typing.Any) -> bool:
+def is_shvnull(value: object) -> typing.TypeGuard[SHVNullType]:
     """Validate type of the value as either ``None`` or :class:`SHVNull`."""
     return value is None or isinstance(value, SHVNull)
 
 
 class SHVBool(SHVMeta):
     """Boolean with :class:`SHVMeta`."""
 
-    def __init__(self, value: bool):
+    def __init__(self, value: bool) -> None:
         self._value = value
 
     def __bool__(self) -> bool:
         return self._value
 
-    def __eq__(self, value: typing.Any) -> bool:
+    def __eq__(self, value: object) -> bool:
         return bool(value) is self._value
 
     def __hash__(self) -> int:
         return hash(self._value)
 
 
-def is_shvbool(value: typing.Any) -> bool:
+def is_shvbool(value: object) -> typing.TypeGuard[bool | SHVBool]:
     """Validate type of value as either :class:`bool` or :class:`SHVBool`."""
     return isinstance(value, bool | SHVBool)
 
 
 class SHVInt(int, SHVMeta):
     """Integer with class:`SHVMeta`."""
 
@@ -229,19 +230,19 @@
     """Dictionary with :class:`SHVMeta`."""
 
 
 class SHVIMap(dict[int, SHVType], SHVMeta):
     """Dictionary with :class:`SHVMeta`."""
 
 
-def is_shvmap(value: typing.Any) -> bool:
+def is_shvmap(value: object) -> typing.TypeGuard[SHVMapType]:
     """Check if given value can be SHV Map."""
     return isinstance(value, collections.abc.Mapping) and all(
         isinstance(k, str) for k in value.keys()
     )
 
 
-def is_shvimap(value: typing.Any) -> bool:
+def is_shvimap(value: object) -> typing.TypeGuard[SHVIMapType]:
     """Check if given value can be SHV IMap."""
     return isinstance(value, collections.abc.Mapping) and all(
         isinstance(k, int) for k in value.keys()
     )
```

### Comparing `pyshv-0.5.0/shv/valueclient.py` & `pyshv-0.6.0/shv/valueclient.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """Common extension for the SimpleClient."""
+
 import asyncio
 import collections.abc
 import datetime
+import logging
 import time
 import typing
 
-from .rpcclient import RpcClient
 from .rpcerrors import RpcMethodCallExceptionError, RpcMethodNotFoundError
 from .rpcsubscription import RpcSubscription
 from .simpleclient import SimpleClient
 from .value import SHVMapType, SHVType, shvmeta, shvmeta_eq
 
+logger = logging.getLogger(__name__)
+
 
 class ValueClient(SimpleClient, collections.abc.Mapping):
     """SHV client made to track values more easily.
 
     This tailors to the use case of tracking and accessing various values more
     easily. You need to subscribe to specific path and this class automatically
     provides you with cached latest value as received through signals or fetched
     from logs (logs fetching has to be performed explicitly) or with prop_get.
 
     To access subscribed value you can index this object with SHV path to it.
     """
 
-    def __init__(self, client: RpcClient):
-        super().__init__(client)
-        self._subscribes: set[RpcSubscription] = set()
+    def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:  # noqa ANNN401
+        super().__init__(*args, **kwargs)  # notype
         self._cache: dict[str, tuple[float, SHVType]] = {}
         self._handlers: dict[
             str, typing.Callable[[ValueClient, str, SHVType], None]
         ] = {}
         self._futures: dict[str, list[asyncio.Future]] = {}
 
     def __getitem__(self, key: str) -> SHVType:
@@ -76,17 +78,17 @@
         :param max_age: is maximum age in seconds to be specified for the get. Nonzero
           value results in value to be served from cache anywhere along the way (thus not
           just local cache).
         :return: Value of the property node.
         """
         # Serve from cache if cache was updated not before max_age
         if path in self._cache and self._cache[path][0] + max_age >= time.time():
-            return self._cache[path]
+            return self._cache[path][1]
         value = await self.call(path, "get", max_age if int(max_age * 1000) else None)
-        if self.get(path, None) != value:
+        if self.get(path, max_age if max_age else None) != value:
             await self._value_update(path, value)
         return value
 
     async def prop_set(self, path: str, value: SHVType, update: bool = False) -> None:
         """Set value to the property associated with the node on given path.
 
         :param path: SHV path to the property node.
@@ -98,15 +100,15 @@
         if update:
             await self._value_update(path, value)
 
     async def prop_change_wait(
         self,
         path: str,
         value: SHVType = None,
-        timeout: float = 5.0,
+        timeout: float | int | None = 5.0,
         get_period: float = 1.0,
     ) -> SHVType:
         """Wait for property change.
 
         The wait is implemented by combination of pooling and waiting for the change
         signal. Pooling uses :meth:`prop_get` every ``get_period``. If you previously
         subscribed on this path (that includes its parent) then it will wait for signal,
@@ -115,17 +117,16 @@
         note:: This uses :meth:`on_change` internally and thus it might temporally (for
         this method execution time) replace your own callback.
 
         :param path: SHV path to the property node.
         :param value: The value we compare against. It is ignored for if we have this
             path in cache and is ``None``. Otherwise it is used to actually detect the
             change (if returned value is not equal to this one).
-        :param timeout: How long we should wait for change. Pass negative number to wait
-            infinitely. This is only minimal deadline. The check for it is performed
-            only on multiples of ``get_period``.
+        :param timeout: How long we should wait for change. Pass ``None`` to wait
+            infinitely.
         :param get_period: How often the pooling should be performed.
         """
         tasks: set[asyncio.Task] = {
             asyncio.create_task(
                 self._prop_change_wait(
                     path,
                     self.get(path, None) if value is None else value,
@@ -196,48 +197,45 @@
         """
         if path not in self._futures:
             self._futures[path] = []
         future: asyncio.Future[SHVType] = asyncio.get_running_loop().create_future()
         self._futures[path].append(future)
         return await future
 
-    async def subscribe(self, sub: RpcSubscription) -> None:
-        await super().subscribe(sub)
-        self._subscribes.add(sub)
-
     async def unsubscribe(self, sub: RpcSubscription, clean_cache: bool = True) -> bool:
         """Perform unsubscribe for signals on given path.
 
         :param sub: SHV RPC subscription to be removed.
         :param wipe_cache: If no longer subscribed paths should be removed from cache or
             not. The default is to remove them but you can also do multiple unsibscribes
             and then call :meth:`clean_cache` for all of the at once.
         :return: ``True`` in case such subscribe was located and ``False`` otherwise.
         """
         res = await super().unsubscribe(sub)
-        if res:
-            self._subscribes.remove(sub)
-            if clean_cache:
-                self.clean_cache()
+        if res and clean_cache:
+            self.clean_cache()
         return res
 
-    def is_subscribed(self, path: str, method: str = "chng") -> bool:
+    def is_subscribed(
+        self, path: str, signal: str = "chng", source: str = "get"
+    ) -> bool:
         """Check if we are subscribed for given SHV path.
 
         Subscribed paths are cached and thus this also checks if this path would be
         cached.
 
         This is only local check. This won't reach the server to verify that all
         subscriptions are still valid (not removed on the server).
 
         :param path: SHV path
-        :param method: Signal method
+        :param signal: Signal name
+        :param source: Method name signal is associated with.
         :return: ``True`` if subscribed for that path and ``False`` otherwise.
         """
-        return any(sub.applies(path, method) for sub in self._subscribes)
+        return any(sub.applies(path, signal, source) for sub in self._subscribes)
 
     def clean_cache(self) -> None:
         """Remove no longer subscribed paths from cache.
 
         There is commonly no need to call this method unless you call
         :meth:`unsubscribe` with ``wipe_cache=False``.
         """
@@ -275,27 +273,26 @@
 
     async def get_snapshot(self, *paths: str, update: bool = False) -> None:
         """Get snapshot of data on subscribed paths using get methods.
 
         This provides a way for you to initialize cache without logs. It
         iterates over SHV tree and calls any get method it encounters.
 
-        :param paths: Paths to be snapshoted. If none is provide the sunscriptions are
-            used instead.
-        :param update: If already cached values should be updated or just skipped.
+        :param paths: Paths to be snapshoted. If none is provide the
+          subscriptions are used instead.
+        :param update: If already cached values should be updated or just
+          skipped.
         """
         pths: list[str] = list(paths) if paths else [""]
         # TODO we can skip paths that are outside of our subscriptions
         while pths:
             pth = pths.pop()
             try:
                 pths.extend(
-                    (f"{pth}{'/' if pth else ''}{name}" for name in await self.ls(pth))
+                    f"{pth}{'/' if pth else ''}{name}" for name in await self.ls(pth)
                 )
             except (RpcMethodNotFoundError, RpcMethodCallExceptionError):
                 pass  # ls might not be present which is not an issue
             if not self.is_subscribed(pth) or (not update and pth in self._cache):
-                print(f"Ignoring {pth}")
                 continue
-            print(f"Getting {pth}")
-            if await self.dir_description(pth, "get") is not None:
+            if await self.dir_exists(pth, "get"):
                 self._cache[pth] = (time.time(), await self.prop_get(pth))
```

### Comparing `pyshv-0.5.0/tests/test_chainpack.py` & `pyshv-0.6.0/tests/test_chainpack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Check that we can serialize and deserialize Chainpack."""
+
 import datetime
 import decimal
 
-import dateutil.tz
 import pytest
 
-from shv import ChainPackReader, ChainPackWriter, SHVMeta, SHVUInt, shvmeta_eq
+from shv import ChainPackReader, ChainPackWriter, SHVMeta, SHVUInt, shvmeta
 
 # You can get chainpack using this shell command:
 #   echo 'null' | cp2cp --ip --oc \
 #     | python -c "import sys; print(repr(sys.stdin.buffer.read()))"
 DATA: list = [
     (b"\x80", None),
     (b"\xfe", True),
@@ -18,14 +18,15 @@
     (b"\x82A", -1),
     (b"\x82B", -2),
     (b"G", 7),
     (b"j", 42),
     (b"\x01", SHVUInt(1)),
     (b"\x81\xf0\x7f\xff\xff\xff", SHVUInt(2**31 - 1)),
     (b"\x81\xf0\xff\xff\xff\xff", SHVUInt(2**32 - 1)),
+    (b"\x81\xf4\x80\x00\x00\x00\x00\x00\x00\x00", SHVUInt(1 << 63)),
     (b"\x82\xf0\x7f\xff\xff\xff", 2**31 - 1),
     (b"\x82\xf1\x00\xff\xff\xff\xff", 2**32 - 1),
     (b"\x82\xf3\x1f\xff\xff\xff\xff\xff\xff", 2**53 - 1),
     (b"\x82\xf3\x9f\xff\xff\xff\xff\xff\xff", 1 - 2**53),
     (b"\x83\x00\x00\x00\x00\x00\xe0k@", 223.0),
     (b"\x8c\x17A", decimal.Decimal((0, (2, 3), -1))),
     (b"\x86\x00", ""),
@@ -60,45 +61,53 @@
     (
         b"\x8bD\x86\x05svete\xff\x8aB\x8bD\x86\x05svete\xff\x88@A\xff\xff",
         SHVMeta.new({2: SHVMeta.new([0, 1], {4: "svete"})}, {4: "svete"}),
     ),
     (b"\x85\x06ab\xcd\t\r\n", b"ab\xcd\t\r\n"),
     (
         b"\x8d\x04",
-        datetime.datetime(2018, 2, 2, 0, 0, 0, 1000, tzinfo=dateutil.tz.tzutc()),
+        datetime.datetime(2018, 2, 2, 0, 0, 0, 1000, tzinfo=datetime.UTC),
     ),
     (
         b"\x8d\x82\x11",
         datetime.datetime(
-            2018, 2, 2, 1, 0, 0, 1000, tzinfo=dateutil.tz.tzoffset(None, 3600)
+            2018,
+            2,
+            2,
+            1,
+            0,
+            0,
+            1000,
+            tzinfo=datetime.timezone(datetime.timedelta(hours=1)),
         ),
     ),
 ]
 
 
 @pytest.mark.parametrize(
     "chainpack,data",
-    DATA
-    + [
+    [
+        *DATA,
         (b"\x8efoo\x00", "foo"),
     ],
 )
 def test_reader(chainpack, data):
     obj = ChainPackReader.unpack(chainpack)
-    assert shvmeta_eq(obj, data)
+    assert obj == data
+    assert shvmeta(obj) == shvmeta(data)
 
 
 def test_reader_uint():
     assert isinstance(ChainPackReader.unpack(b"\x01"), SHVUInt)
 
 
 @pytest.mark.parametrize(
     "chainpack,data",
-    DATA
-    + [
+    [
+        *DATA,
         (b"A", SHVMeta.new(1)),
     ],
 )
 def test_writer(chainpack, data):
     res = ChainPackWriter.pack(data)
     assert res == chainpack
```

### Comparing `pyshv-0.5.0/tests/test_cp2cp.py` & `pyshv-0.6.0/tests/test_cpconv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Check usability of our stream conversion."""
+
 import pytest
 
-from shv.cp2cp import CPFormat, convert
+from shv.cpconv import CPFormat, convert
 
 DATA = [
     ("true", b"\xfe"),
     ("[1]", b"\x88A\xff"),
 ]
 
 
 @pytest.mark.parametrize("cpon,chainpack", DATA)
-def test_cp2cpon(cpon, chainpack):
+def test_cpconv(cpon, chainpack):
     assert (
         convert(chainpack, CPFormat.CHAINPACK, None, CPFormat.CPON).decode("utf-8")
         == cpon
     )
 
 
 @pytest.mark.parametrize("cpon,chainpack", DATA)
```

### Comparing `pyshv-0.5.0/tests/test_cpon.py` & `pyshv-0.6.0/tests/test_cpon.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Check that we can serialize and deserialize Cpon."""
+
 import datetime
 import decimal
 
-import dateutil.tz
 import pytest
 
-from shv import CponReader, CponWriter, SHVMeta, SHVUInt, shvmeta_eq
+from shv import CponReader, CponWriter, SHVMeta, SHVUInt, shvmeta
 
 DATA: list = [
     ("null", None),
     (b"null", None),
     ("true", True),
     ("false", False),
     ("0", 0),
@@ -56,80 +56,103 @@
     (
         '<4:"svete">i{2:<4:"svete">[0,1]}',
         SHVMeta.new({2: SHVMeta.new([0, 1], {4: "svete"})}, {4: "svete"}),
     ),
     ('b"ab\\cd\\t\\r\\n"', b"ab\xcd\t\r\n"),
     (
         'd"2018-02-02T00:00:00Z"',
-        datetime.datetime(2018, 2, 2, tzinfo=dateutil.tz.tzutc()),
+        datetime.datetime(2018, 2, 2, tzinfo=datetime.UTC),
     ),
     (
         'd"2027-05-03T11:30:12.345+01"',
         datetime.datetime(
-            2027, 5, 3, 11, 30, 12, 345000, tzinfo=dateutil.tz.tzoffset(None, 3600)
+            2027,
+            5,
+            3,
+            11,
+            30,
+            12,
+            345000,
+            tzinfo=datetime.timezone(datetime.timedelta(hours=1)),
         ),
     ),
 ]
 
 
 @pytest.mark.parametrize(
     "cpon,data",
-    DATA
-    + [
+    [
+        *DATA,
         ("0x42", 0x42),
         ("223.", 223.0),
         ("2.30", decimal.Decimal("2.3")),
         ("-1234567890.", decimal.Decimal((1, (1, 2, 3, 4, 5, 6, 7, 8, 9), 1))),
         ("[1, 2, 3]", [1, 2, 3]),
         ("<>1", 1),
         (
             'd"2017-05-03T18:30:00Z"',
-            datetime.datetime(2017, 5, 3, 18, 30, tzinfo=dateutil.tz.tzutc()),
+            datetime.datetime(2017, 5, 3, 18, 30, tzinfo=datetime.UTC),
         ),
         (
             'd"2017-05-03T22:30:00+04"',
             datetime.datetime(
-                2017, 5, 3, 22, 30, tzinfo=dateutil.tz.tzoffset(None, 14400)
+                2017,
+                5,
+                3,
+                22,
+                30,
+                tzinfo=datetime.timezone(datetime.timedelta(seconds=14400)),
             ),
         ),
         (
             'd"2017-05-03T11:30:00-0700"',
             datetime.datetime(
-                2017, 5, 3, 11, 30, tzinfo=dateutil.tz.tzoffset(None, -25200)
+                2017,
+                5,
+                3,
+                11,
+                30,
+                tzinfo=datetime.timezone(datetime.timedelta(seconds=-25200)),
             ),
         ),
         (
             'd"2017-05-03T15:00:00-0330"',
             datetime.datetime(
-                2017, 5, 3, 15, tzinfo=dateutil.tz.tzoffset(None, -12600)
+                2017,
+                5,
+                3,
+                15,
+                tzinfo=datetime.timezone(datetime.timedelta(seconds=-12600)),
             ),
         ),
     ],
 )
 def test_reader(cpon, data):
-    assert shvmeta_eq(CponReader.unpack(cpon), data)
+    res = CponReader.unpack(cpon)
+    assert res == data
+    assert shvmeta(res) == shvmeta(data)
 
 
 def test_reader_uint():
     assert isinstance(CponReader.unpack("1u"), SHVUInt)
 
 
 @pytest.mark.parametrize(
     "cpon,data",
-    DATA
-    + [
+    [
+        *DATA,
         ("1", SHVMeta.new(1, {})),
         ("1.0", decimal.Decimal((0, (1,), 0))),
     ],
 )
 def test_writer(cpon, data):
     res = CponWriter.pack(data)
     if isinstance(cpon, str):
         res = res.decode("utf-8")
-    assert shvmeta_eq(res, cpon)
+    assert res == cpon
 
 
 @pytest.mark.parametrize(
     "cpon,res",
     (
         ("0xab", b"171"),
         ("-0xCD", b"-205"),
```

### Comparing `pyshv-0.5.0/tests/test_errors.py` & `pyshv-0.6.0/tests/test_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Check that errors can be created trough RpcError."""
+
 import pytest
 
 from shv import (
     RpcError,
     RpcInternalError,
     RpcInvalidParamsError,
     RpcInvalidRequestError,
```

### Comparing `pyshv-0.5.0/tests/test_rpcclient.py` & `pyshv-0.6.0/tests/test_rpcclient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-"""Check various clients implementing a different link layers.
-"""
+"""Check various clients implementing a different link layers."""
+
 import asyncio
 import io
 import logging
 import multiprocessing
 import os
 import pty
 import select
 
 import pytest
 
 from shv import (
+    RpcClient,
     RpcClientPipe,
     RpcClientTCP,
     RpcClientTTY,
     RpcClientUnix,
     RpcInvalidRequestError,
     RpcMessage,
     RpcServerTCP,
@@ -29,15 +30,15 @@
 
     async def test_call(self, clients):
         msg = RpcMessage.request(".app", "dir")
         await clients[0].send(msg)
         assert await clients[1].receive() == msg
 
     async def test_notify(self, clients):
-        msg = RpcMessage.chng(".app", None)
+        msg = RpcMessage.signal(".app")
         await clients[1].send(msg)
         assert await clients[0].receive() == msg
 
     async def test_error_receive(self, clients):
         msg = RpcMessage.request(".app", "dir").make_response()
         msg.rpc_error = RpcInvalidRequestError("Fake error")
         await clients[0].send(msg)
@@ -46,38 +47,51 @@
     async def test_error_raise(self, clients):
         msg = RpcMessage.request(".app", "dir").make_response()
         msg.rpc_error = RpcInvalidRequestError("Fake error")
         await clients[0].send(msg)
         with pytest.raises(RpcInvalidRequestError):
             await clients[1].receive(True)
 
+    @pytest.mark.parametrize("a,b", ((0, 1), (1, 0)))
+    async def test_reset(self, clients, a, b):
+        await clients[a].reset()
+        assert await clients[b].receive() == RpcClient.Control.RESET
+
 
 class ServerLink(Link):
     """Additional tests for server-client connections."""
 
-    async def test_reset_client(self, clients, server):
+    @pytest.mark.parametrize("cdisc,crecv", ((0, 1), (1, 0)))
+    async def test_eof_receive(self, clients, cdisc, crecv):
+        clients[cdisc].disconnect()
+        await clients[cdisc].wait_disconnect()
+        assert not clients[cdisc].connected
+        with pytest.raises(EOFError):
+            await clients[crecv].receive()
+        assert not clients[crecv].connected
+
+    @pytest.mark.parametrize("cdisc,crecv", ((0, 1), (1, 0)))
+    async def test_eof_send(self, clients, cdisc, crecv):
+        clients[cdisc].disconnect()
+        await clients[cdisc].wait_disconnect()
+        with pytest.raises(EOFError):
+            await clients[crecv].send(RpcMessage.request(".app", "ping"))
+        assert not clients[crecv].connected
+
+    async def test_reconnect(self, clients, server):
+        clients[1].disconnect()
+        await clients[1].wait_disconnect()
         await clients[1].reset()
         server_client = await server[1].get()
         msg = RpcMessage.request("foo", "ls")
         await clients[1].send(msg)
         assert await server_client.receive() == msg
         server_client.disconnect()
         await server_client.wait_disconnect()
 
-    async def test_reset_server_client(self, clients):
-        assert not await clients[0].reset()
-        assert not clients[0].connected
-
-    @pytest.mark.parametrize("cdisc,crecv", ((0, 1), (1, 0)))
-    async def test_eof(self, clients, cdisc, crecv):
-        clients[cdisc].disconnect()
-        await clients[cdisc].wait_disconnect()
-        with pytest.raises(EOFError):
-            await clients[crecv].receive()
-
 
 class TestTCP(ServerLink):
     """Check that TCP/IP transport protocol works."""
 
     @pytest.fixture(name="server")
     async def fixture_server(self, port):
         queue = asyncio.Queue()
@@ -93,14 +107,23 @@
         server_client = await server[1].get()
         yield server_client, client
         client.disconnect()
         server_client.disconnect()
         await client.wait_disconnect()
         await server_client.wait_disconnect()
 
+    async def test_before_connect(self, port) -> None:
+        client = RpcClientTCP("localhost", port)
+        with pytest.raises(EOFError):
+            await client.receive()
+        with pytest.raises(EOFError):
+            await client.send(RpcMessage.request(".app", "ping"))
+        client.disconnect()
+        await client.wait_disconnect()
+
 
 class TestUnix(ServerLink):
     """Check that Unix transport protocol works."""
 
     @pytest.fixture(name="sockpath")
     def fixture_sockpath(self, tmp_path):
         return tmp_path / "s"
@@ -146,18 +169,20 @@
         pty1_master, pty1_slave = pty.openpty()
         pty2_master, pty2_slave = pty.openpty()
         process = multiprocessing.Process(
             target=self.ptycopy, args=(pty1_master, pty2_master)
         )
         process.start()
 
-        client1 = await RpcClientTTY.open(os.ttyname(pty1_slave))
+        client1 = await RpcClientTTY.connect(os.ttyname(pty1_slave))
         os.close(pty1_slave)
-        client2 = await RpcClientTTY.open(os.ttyname(pty2_slave))
+        client2 = await RpcClientTTY.connect(os.ttyname(pty2_slave))
         os.close(pty2_slave)
+        # Flush reset sent by client2
+        assert await client1.receive() is RpcClient.Control.RESET
 
         yield client1, client2
 
         client1.disconnect()
         client2.disconnect()
         await client1.wait_disconnect()
         await client2.wait_disconnect()
@@ -177,16 +202,7 @@
                     logger.error("Error detected in ptycopy")
                     return
 
     async def test_escapes(self, clients):
         msg = RpcMessage.request("prop", "set", b"1\xa2\xa3\xa4\xa5\xaa2")
         await clients[0].send(msg)
         assert await clients[1].receive() == msg
-
-    async def test_reset_client(self, clients):
-        # Note: both sides are the same so we can test only from one side to the other
-        msg = RpcMessage.request("foo", "ls")
-        await clients[0].send(msg)
-        assert await clients[1].receive() == msg
-        await clients[0].reset()
-        await clients[0].send(msg)
-        assert await clients[1].receive() == msg
```

### Comparing `pyshv-0.5.0/tests/test_rpcsubscription.py` & `pyshv-0.6.0/tests/test_rpcsubscription.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Check our implementation of fnmatch."""
+
 import pytest
 
 from shv.rpcsubscription import RpcSubscription, path_match, tail_pattern
 
 
 @pytest.mark.parametrize(
     "pattern,path",
@@ -36,14 +37,16 @@
     assert not path_match(path, pattern)
 
 
 @pytest.mark.parametrize(
     "pattern,path,result",
     (
         ("", "", None),
+        ("test/some", "test", "some"),
+        ("test/some", "test/some", None),
         ("*/*", "foo", "*"),
         ("*/*", "foo/faa", None),
         ("**", "foo", "**"),
         ("foo/**", "foo", "**"),
         ("some/**", "foo", None),
         ("foo/**", "foo/bar", "**"),
         ("foo/**/some", "foo/bar", "**/some"),
@@ -57,27 +60,20 @@
 @pytest.mark.parametrize(
     "sub,path,res",
     (
         (RpcSubscription(), "", RpcSubscription()),
         (RpcSubscription("test/some"), "", RpcSubscription("test/some")),
         (RpcSubscription("test/some"), "test", RpcSubscription("some")),
         (RpcSubscription("test/some"), "test/", RpcSubscription("some")),
-        (RpcSubscription("test/some"), "test/some", RpcSubscription("")),
-        (RpcSubscription("test/some"), "test/some/", RpcSubscription("")),
+        (RpcSubscription("test/some"), "test/some", None),
+        (RpcSubscription("test/some"), "test/some/", None),
         (RpcSubscription("test/some"), "test/som", None),
-        (RpcSubscription(paths="test/some/*"), "test/some", RpcSubscription(paths="*")),
-        (RpcSubscription(paths="test/some/*"), "test", RpcSubscription(paths="some/*")),
-        (RpcSubscription(paths="test/some/*"), "tes", None),
-        (
-            RpcSubscription(paths="**/some/*"),
-            "test/it/some",
-            RpcSubscription(paths="*"),
-        ),
-        (
-            RpcSubscription(paths="**/some/*"),
-            "test/it",
-            RpcSubscription(paths="**/some/*"),
-        ),
+        (RpcSubscription("test/some/*"), "test/some", RpcSubscription("*")),
+        (RpcSubscription("test/some/*"), "test", RpcSubscription("some/*")),
+        (RpcSubscription("test/some/*"), "tes", None),
+        (RpcSubscription("test/some/*"), "test/some/node", None),
+        (RpcSubscription("**/some/*"), "test/it/some", RpcSubscription("*")),
+        (RpcSubscription("**/some/*"), "test/it", RpcSubscription("**/some/*")),
     ),
 )
 def test_relative_to(sub, path, res):
     assert sub.relative_to(path) == res
```

### Comparing `pyshv-0.5.0/tests/test_rpcurl.py` & `pyshv-0.6.0/tests/test_rpcurl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,78 @@
 """Check that we correctly parse and serialize our URL format."""
+
 import re
 
 import pytest
 
-from shv import RpcLoginType, RpcProtocol, RpcUrl
+from shv import RpcLogin, RpcLoginType, RpcProtocol, RpcUrl
 
 DATA = [
     ("unix:/dev/null", RpcUrl("/dev/null", protocol=RpcProtocol.UNIX)),
     (
         "unixs:/dev/null?user=test&password=foo",
         RpcUrl(
-            "/dev/null", protocol=RpcProtocol.UNIXS, username="test", password="foo"
+            "/dev/null",
+            protocol=RpcProtocol.UNIXS,
+            login=RpcLogin(username="test", password="foo"),
         ),
     ),
     (
         "serial:/dev/null?user=test%40example.com&password=a%C4%8D%C5%A1f",
         RpcUrl(
             "/dev/null",
             protocol=RpcProtocol.SERIAL,
-            username="test@example.com",
-            password="ačšf",
+            login=RpcLogin(username="test@example.com", password="ačšf"),
         ),
     ),
-    ("tcp://test@localhost:4242", RpcUrl("localhost", username="test", port=4242)),
+    (
+        "tcp://test@localhost:4242",
+        RpcUrl("localhost", port=4242, login=RpcLogin(username="test")),
+    ),
     (
         "ssl://test@localhost:4242",
-        RpcUrl("localhost", protocol=RpcProtocol.SSL, username="test", port=4242),
+        RpcUrl(
+            "localhost",
+            protocol=RpcProtocol.SSL,
+            port=4242,
+            login=RpcLogin(username="test"),
+        ),
     ),
     (
         "tcp://localhost:4242?devid=foo&devmount=/dev/null",
-        RpcUrl("localhost", port=4242, device_id="foo", device_mount_point="/dev/null"),
+        RpcUrl(
+            "localhost",
+            port=4242,
+            login=RpcLogin(
+                options={"device": {"deviceId": "foo", "mountPoint": "/dev/null"}}
+            ),
+        ),
     ),
     (
         "tcp://localhost:4242?devid=foo&devmount=/dev/null&password=test",
         RpcUrl(
             "localhost",
             port=4242,
-            password="test",
-            login_type=RpcLoginType.PLAIN,
-            device_id="foo",
-            device_mount_point="/dev/null",
+            login=RpcLogin(
+                password="test",
+                login_type=RpcLoginType.PLAIN,
+                options={"device": {"deviceId": "foo", "mountPoint": "/dev/null"}},
+            ),
         ),
     ),
     (
         "tcp://localhost:4242?devid=foo&devmount=/dev/null&shapass=" + ("x" * 40),
         RpcUrl(
             "localhost",
             port=4242,
-            password="x" * 40,
-            login_type=RpcLoginType.SHA1,
-            device_id="foo",
-            device_mount_point="/dev/null",
+            login=RpcLogin(
+                password="x" * 40,
+                login_type=RpcLoginType.SHA1,
+                options={"device": {"deviceId": "foo", "mountPoint": "/dev/null"}},
+            ),
         ),
     ),
     ("tcp://[::]:4242", RpcUrl("::", port=4242)),
     ("serial:/dev/ttyX", RpcUrl("/dev/ttyX", protocol=RpcProtocol.SERIAL)),
     (
         "serial:/dev/ttyX?baudrate=1152000",
         RpcUrl("/dev/ttyX", protocol=RpcProtocol.SERIAL, baudrate=1152000),
@@ -66,29 +84,37 @@
 def test_to_url(url, rpcurl):
     """Check that we correctly parse these URLs."""
     assert rpcurl.to_url() == url
 
 
 @pytest.mark.parametrize(
     "url,rpcurl",
-    DATA
-    + [
+    [
+        *DATA,
         ("", RpcUrl("", protocol=RpcProtocol.UNIX)),
         ("/dev/null", RpcUrl("/dev/null", protocol=RpcProtocol.UNIX)),
         ("//dev/null", RpcUrl("/dev/null", protocol=RpcProtocol.UNIX)),
         (
             "unix://dev/null",
             RpcUrl("/dev/null", protocol=RpcProtocol.UNIX),
         ),
         ("tcp://localhost", RpcUrl("localhost", port=3755, protocol=RpcProtocol.TCP)),
         ("tcps://localhost", RpcUrl("localhost", port=3765, protocol=RpcProtocol.TCPS)),
         ("ssl://localhost", RpcUrl("localhost", port=3756, protocol=RpcProtocol.SSL)),
         ("ssls://localhost", RpcUrl("localhost", port=3766, protocol=RpcProtocol.SSLS)),
-        ("tcp://test@localhost:4242", RpcUrl("localhost", username="test", port=4242)),
-        ("tcp://localhost?devid=foo", RpcUrl("localhost", device_id="foo")),
+        (
+            "tcp://test@localhost:4242",
+            RpcUrl("localhost", port=4242, login=RpcLogin(username="test")),
+        ),
+        (
+            "tcp://localhost?devid=foo",
+            RpcUrl(
+                "localhost", login=RpcLogin(options={"device": {"deviceId": "foo"}})
+            ),
+        ),
     ],
 )
 def test_parse(url, rpcurl):
     """Check that we correctly parse these URLs."""
     assert RpcUrl.parse(url) == rpcurl
```

### Comparing `pyshv-0.5.0/tests/test_simpledevice.py` & `pyshv-0.6.0/tests/test_simpledevice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 """Check implementation of SimpleDevice."""
+
+import datetime
+
 import pytest
 
-from shv import RpcMethodAccess, RpcMethodDesc, SimpleDevice, shvmeta_eq
+from shv import (
+    SHV_VERSION_MAJOR,
+    SHV_VERSION_MINOR,
+    VERSION,
+    RpcMethodAccess,
+    RpcMethodDesc,
+    RpcMethodNotFoundError,
+    SimpleDevice,
+    shvmeta,
+)
 
 
 class Device(SimpleDevice):
     DEVICE_NAME = "testdev"
     DEVICE_VERSION = "0.0.x"
 
 
@@ -16,48 +28,67 @@
     yield device
     await device.disconnect()
 
 
 @pytest.mark.parametrize(
     "path,method,result",
     (
-        ("test/device/.app/device", "name", "testdev"),
-        ("test/device/.app/device", "version", "0.0.x"),
-        ("test/device/.app/device", "serialNumber", None),
+        ("test/device/.app", "shvVersionMajor", SHV_VERSION_MAJOR),
+        ("test/device/.app", "shvVersionMinor", SHV_VERSION_MINOR),
+        ("test/device/.app", "name", "pyshv-device"),
+        ("test/device/.app", "version", VERSION),
+        ("test/device/.app", "ping", None),
+        ("test/device/.device", "name", "testdev"),
+        ("test/device/.device", "version", "0.0.x"),
+        ("test/device/.device", "serialNumber", None),
     ),
 )
 async def test_call(client, device, path, method, result):
     """Check that we can call various methods using blocking call."""
     res = await client.call(path, method)
-    assert shvmeta_eq(res, result)
+    assert res == result
+    assert shvmeta(res) == shvmeta(result)
+
+
+async def test_call_date(client, device):
+    """Check that we can call various methods using blocking call."""
+    res = await client.call("test/device/.app", "date")
+    assert isinstance(res, datetime.datetime)
+    assert res.tzinfo is not None
+    diff = datetime.datetime.now().astimezone() - res
+    assert datetime.timedelta() <= diff < datetime.timedelta(seconds=1)
+
+
+async def test_invalid_call(client):
+    with pytest.raises(RpcMethodNotFoundError):
+        await client.call(".app", "someInvalid")
 
 
 @pytest.mark.parametrize(
     "path,result",
     (
-        ("test/device", [".app"]),
-        ("test/device/.app", ["device"]),
-        ("test/device/.app/device", []),
+        ("test/device", [".app", ".device"]),
+        ("test/device/.app", []),
+        ("test/device/.device", []),
     ),
 )
 async def test_ls(client, device, path, result):
     """Verify that we can use ls method."""
     res = await client.ls(path)
     assert res == result
 
 
 @pytest.mark.parametrize(
     "path,result",
     (
         (
-            "test/device/.app/device",
+            "test/device/.device",
             [
                 RpcMethodDesc.stddir(),
                 RpcMethodDesc.stdls(),
-                RpcMethodDesc.stdlschng(),
                 RpcMethodDesc.getter(
                     "name", "Null", "String", access=RpcMethodAccess.BROWSE
                 ),
                 RpcMethodDesc.getter(
                     "version", "Null", "String", access=RpcMethodAccess.BROWSE
                 ),
                 RpcMethodDesc.getter(
```

### Comparing `pyshv-0.5.0/tests/test_value.py` & `pyshv-0.6.0/tests/test_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Check our meta value assignment."""
+
 import datetime
 import decimal
 
 import pytest
 
 from shv import (
     SHVBool,
@@ -16,15 +17,14 @@
     SHVMap,
     SHVMeta,
     SHVNull,
     SHVStr,
     SHVUInt,
     is_shvbool,
     is_shvnull,
-    shvget,
     shvmeta_eq,
 )
 
 CLASSES: list = [
     (SHVNull, []),
     (SHVBool, [True]),
     (SHVInt, []),
@@ -106,15 +106,15 @@
     assert obj1 != value2
     assert obj1 != obj2
 
 
 @pytest.mark.parametrize("cls,value1,value2", REPRS)
 def test_hash(cls, value1, value2):
     """Our objects should not modify hash and thus it has to be the same."""
-    if cls in (SHVList, SHVMap, SHVIMap):
+    if cls in {SHVList, SHVMap, SHVIMap}:
         return  # Unhashable types
     assert hash(cls(value1)) == hash(value1)
     assert hash(cls(value2)) == hash(value2)
 
 
 def test_datetime():
     timestamp = 45322
```

### Comparing `pyshv-0.5.0/tests/test_valueclient.py` & `pyshv-0.6.0/tests/test_valueclient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 """Test ValueClient specific tools."""
+
 import asyncio
 
 import pytest
 
 from shv import RpcSubscription
 
 
 async def test_prop_cache(value_client, example_device):
     """Check that we correctly cache values in value client."""
-    await value_client.subscribe(RpcSubscription("test/device/track"))
+    await value_client.subscribe(RpcSubscription("test/device/track/**"))
     assert len(value_client) == 0
     assert not list(iter(value_client))
     assert "test/device/track/1" not in value_client
-    assert await value_client.prop_get("test/device/track/1") == [0]
+    assert await value_client.prop_get("test/device/track/1", 8) == [0]
     assert len(value_client) == 1
     assert value_client["test/device/track/1"] == [0]
+    assert await value_client.prop_get("test/device/track/1", 8) == [0]
     await value_client.prop_set("test/device/track/1", [1, 2])
     assert value_client["test/device/track/1"] == [1, 2]
-    await value_client.unsubscribe(RpcSubscription("test/device/track"))
+    await value_client.unsubscribe(RpcSubscription("test/device/track/**"))
     assert len(value_client) == 0
 
 
 async def test_unsubscribe_keep_cache(value_client, example_device):
     """Check that unsubscribe can keep the cached values."""
-    await value_client.subscribe(RpcSubscription("test/device"))
+    await value_client.subscribe(RpcSubscription("test/device/**"))
     await value_client.prop_get("test/device/track/1")
     assert "test/device/track/1" in value_client
-    await value_client.unsubscribe(RpcSubscription("test/device"), clean_cache=False)
+    await value_client.unsubscribe(RpcSubscription("test/device/**"), clean_cache=False)
     assert "test/device/track/1" in value_client
 
 
 async def test_is_subscribed(value_client, example_device):
     """Check that we correctly trak our own subscriptions."""
-    assert not value_client.is_subscribed("test")
-    await value_client.subscribe(RpcSubscription("test"))
-    assert value_client.is_subscribed("test")
+    assert not value_client.is_subscribed("test/foo")
+    await value_client.subscribe(RpcSubscription("test/**"))
     assert value_client.is_subscribed("test/foo")
     assert value_client.is_subscribed("test/device")
     assert value_client.is_subscribed("test/device/any/other/path/under")
     assert not value_client.is_subscribed(".broker")
     assert not value_client.is_subscribed("tester")  # A different node
-    await value_client.unsubscribe(RpcSubscription("test"))
+    await value_client.unsubscribe(RpcSubscription("test/**"))
     assert not value_client.is_subscribed("test")
 
 
 async def test_get_snapshot(value_client, example_device):
     """Check ability of get_snapshot to cache required properties."""
-    await value_client.subscribe(RpcSubscription("test"))
+    await value_client.subscribe(RpcSubscription("test/**"))
     await value_client.get_snapshot("test/device")
     assert "test/device/track/1" in value_client
 
 
 async def test_get_snapshot_subscribes(value_client, example_device):
     """Check get_snapshot without arguments."""
-    await value_client.subscribe(RpcSubscription("test/device"))
+    await value_client.subscribe(RpcSubscription("test/device/**"))
     await value_client.get_snapshot()
     assert "test/device/track/1" in value_client
     assert len(value_client) == 8
 
 
+@pytest.mark.xfail(reason="libshv doesn't support subscribe to fixed path for now.")
 async def test_get_snapshot_lower_subscribe(value_client, example_device):
     """Check that get_snapshot caches only subscribed paths."""
     await value_client.subscribe(RpcSubscription("test/device/track/2"))
     await value_client.get_snapshot("test")
     assert len(value_client) == 1
     assert "test/device/track/2" in value_client
 
 
 async def test_wait_for_change(value_client, example_device):
     """Check that simple wait for change notification works."""
-    await value_client.subscribe(RpcSubscription("test/device"))
+    await value_client.subscribe(RpcSubscription("test/device/**"))
     task1 = asyncio.create_task(value_client.wait_for_change("test/device/track/1"))
     task2 = asyncio.create_task(value_client.wait_for_change("test/device/track/1"))
     await value_client.prop_set("test/device/track/1", [1, 3])
     assert await task1 == [1, 3]
     assert await task2 == [1, 3]
 
 
@@ -81,15 +83,15 @@
 async def test_prop_change(value_client, example_device, path):
     """Check hook for property change."""
     res = []
 
     def hook(client, path, value):
         res.append((client, path, value))
 
-    await value_client.subscribe(RpcSubscription("test/device"))
+    await value_client.subscribe(RpcSubscription("test/device/**"))
     value_client.on_change(path, hook)
     await value_client.prop_set("test/device/track/1", [1, 2])
     await value_client.prop_set("test/device/track/4", [])
     value_client.on_change(path, None)
     await value_client.prop_set("test/device/track/3", [])
 
     assert res == [
@@ -105,25 +107,25 @@
     await value_client.prop_set("test/device/track/1", [1, 3])
     assert await task1 == [1, 3]
     assert await task2 == [1, 3]
 
 
 async def test_prop_change_subscribed(value_client, example_device):
     """Check that we can wait for property change with prop_change_wait."""
-    await value_client.subscribe(RpcSubscription("test/device"))
+    await value_client.subscribe(RpcSubscription("test/device/**"))
     task1 = asyncio.create_task(value_client.prop_change_wait("test/device/track/1"))
     task2 = asyncio.create_task(value_client.prop_change_wait("test/device/track/1"))
     await value_client.prop_set("test/device/track/1", [1, 3])
     assert await task1 == [1, 3]
     assert await task2 == [1, 3]
 
 
 async def test_prop_change_timeout(value_client, example_device):
     """Check that we can will timeout from prop_change_wait."""
-    await value_client.subscribe(RpcSubscription("test/device"))
+    await value_client.subscribe(RpcSubscription("test/device/**"))
     await value_client.prop_get("test/device/track/1")  # seed cache
     with pytest.raises(TimeoutError):
         print(
             await value_client.prop_change_wait(
                 "test/device/track/1", get_period=0.2, timeout=1
             )
         )
```

