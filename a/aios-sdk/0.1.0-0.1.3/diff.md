# Comparing `tmp/aios_sdk-0.1.0.tar.gz` & `tmp/aios_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aios_sdk-0.1.0.tar", max compression
+gzip compressed data, was "aios_sdk-0.1.3.tar", max compression
```

## Comparing `aios_sdk-0.1.0.tar` & `aios_sdk-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-05 20:00:00.579828 aios_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      660 2024-04-06 00:32:15.446423 aios_sdk-0.1.0/aios_sdk/__init__.py
--rw-r--r--   0        0        0      115 2024-04-06 00:26:38.875127 aios_sdk-0.1.0/aios_sdk/models.py
--rw-r--r--   0        0        0      481 2024-04-05 20:18:42.299528 aios_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      323 1970-01-01 00:00:00.000000 aios_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 20:00:00.579828 aios_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0      660 2024-04-06 00:32:15.446423 aios_sdk-0.1.3/aios_sdk/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-06 00:26:38.875127 aios_sdk-0.1.3/aios_sdk/models.py
+-rw-r--r--   0        0        0      481 2024-04-06 00:36:37.514054 aios_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      323 1970-01-01 00:00:00.000000 aios_sdk-0.1.3/PKG-INFO
```

### Comparing `aios_sdk-0.1.0/aios_sdk/__init__.py` & `aios_sdk-0.1.3/aios_sdk/__init__.py`

 * *Files identical despite different names*

