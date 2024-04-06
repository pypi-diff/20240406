# Comparing `tmp/apconfig-0.0.104.tar.gz` & `tmp/apconfig-0.0.105.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.104.tar", max compression
+gzip compressed data, was "apconfig-0.0.105.tar", max compression
```

## Comparing `apconfig-0.0.104.tar` & `apconfig-0.0.105.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.104/README.md
--rw-r--r--   0        0        0     2849 2024-04-05 16:44:50.307577 apconfig-0.0.104/apconfig/__init__.py
--rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.104/apconfig/utilities.py
--rw-r--r--   0        0        0      305 2024-04-05 16:45:07.967656 apconfig-0.0.104/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.104/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.105/README.md
+-rw-r--r--   0        0        0     3078 2024-04-06 06:33:06.779236 apconfig-0.0.105/apconfig/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.105/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-04-06 06:33:15.459322 apconfig-0.0.105/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.105/PKG-INFO
```

### Comparing `apconfig-0.0.104/apconfig/__init__.py` & `apconfig-0.0.105/apconfig/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import List
 
 import requests
 
 
 def get_api_setup_data():
     try:
         with requests.Session() as session:
@@ -53,14 +54,19 @@
 for chain in chains:
     try:
         web3_provider_list[chain] = setup_data["chains"][chain]["providers"]["rpc"]
         web3_websocket_list[chain] = setup_data["chains"][chain]["providers"]["ws"]
     except Exception as e:
         print(e)
 
+web3_urls: dict = {}
+for chain in chains:
+    web3_urls[chain] = list(zip(setup_data["chains"][chain]["providers"]["rpc"],
+                                setup_data["chains"][chain]["providers"]["ws"]))
+
 test_web3_provider_list = [os.getenv("WEB3_PROVIDER")]
 test_web3_websocket_list = [os.getenv("WEB3_WEBSOCKETS")]
 
 # Chain Wallet Configuration
 ftso_reward_offers_manager_addresses = {}
 for chain in chains:
     try:
```

