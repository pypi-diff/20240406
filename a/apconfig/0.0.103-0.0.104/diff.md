# Comparing `tmp/apconfig-0.0.103.tar.gz` & `tmp/apconfig-0.0.104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.103.tar", max compression
+gzip compressed data, was "apconfig-0.0.104.tar", max compression
```

## Comparing `apconfig-0.0.103.tar` & `apconfig-0.0.104.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.103/README.md
--rw-r--r--   0        0        0     2792 2024-04-05 10:45:32.404147 apconfig-0.0.103/apconfig/__init__.py
--rw-r--r--   0        0        0      112 2024-04-05 06:25:39.273690 apconfig-0.0.103/apconfig/utilities.py
--rw-r--r--   0        0        0      305 2024-04-05 10:45:32.416147 apconfig-0.0.103/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.103/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.104/README.md
+-rw-r--r--   0        0        0     2849 2024-04-05 16:44:50.307577 apconfig-0.0.104/apconfig/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.104/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-04-05 16:45:07.967656 apconfig-0.0.104/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.104/PKG-INFO
```

### Comparing `apconfig-0.0.103/apconfig/__init__.py` & `apconfig-0.0.104/apconfig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 for chain in chains:
     try:
         ftso_reward_offers_manager_addresses[chain] \
             = setup_data["chains"][chain]["ftso_reward_offers_manager_address"]
     except Exception as e:
         print(e)
 
+
+print(f"froma {ftso_reward_offers_manager_addresses}")
+
 # Database Configuration
 environment = os.getenv("ENVIRONMENT")
 
 assert environment is not None, "Environment not set. "
 assert environment in ['development', 'production'], f"Environment has invalid value. Must be 'development' or 'production'."
 assert environment in setup_data["environments"], f"Environment {environment} not found in setup data. "
```

