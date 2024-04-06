# Comparing `tmp/dekpkglock-0.1.2.tar.gz` & `tmp/dekpkglock-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekpkglock-0.1.2.tar", last modified: Sat Apr  6 15:32:35 2024, max compression
+gzip compressed data, was "dekpkglock-0.1.4.tar", last modified: Sat Apr  6 19:51:19 2024, max compression
```

## Comparing `dekpkglock-0.1.2.tar` & `dekpkglock-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      123 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/__init__.py
--rw-r--r--   0        0        0       42 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/click/__entry__.py
--rw-r--r--   0        0        0      359 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/click/__init__.py
--rw-r--r--   0        0        0      223 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/core/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/core/base/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/core/pdm.py
--rw-r--r--   0        0        0   140317 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
--rw-r--r--   0        0        0   140317 2024-04-06 15:32:34.496592 dekpkglock-0.1.2/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
--rw-r--r--   0        0        0   101191 2024-04-06 15:32:34.500592 dekpkglock-0.1.2/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock
--rw-r--r--   0        0        0    31259 2024-04-06 15:32:34.500592 dekpkglock-0.1.2/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
--rw-r--r--   0        0        0   123953 2024-04-06 15:32:34.500592 dekpkglock-0.1.2/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
--rw-r--r--   0        0        0      476 2024-04-06 15:32:35.796589 dekpkglock-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/click/__entry__.py
+-rw-r--r--   0        0        0      361 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/click/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/core/__init__.py
+-rw-r--r--   0        0        0     2047 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/core/base/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/core/pdm.py
+-rw-r--r--   0        0        0   140317 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
+-rw-r--r--   0        0        0   140317 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
+-rw-r--r--   0        0        0   101191 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock
+-rw-r--r--   0        0        0   101213 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0    31259 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0   123953 2024-04-06 19:51:18.159023 dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
+-rw-r--r--   0        0        0      476 2024-04-06 19:51:19.583017 dekpkglock-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.4/PKG-INFO
```

### Comparing `dekpkglock-0.1.2/dekpkglock/core/base/__init__.py` & `dekpkglock-0.1.4/dekpkglock/core/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.2/dekpkglock/core/pdm.py` & `dekpkglock-0.1.4/dekpkglock/core/pdm.py`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.2/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock` & `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.2/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock` & `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.2/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock` & `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.2/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock` & `dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.2/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock` & `dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock`

 * *Files identical despite different names*

