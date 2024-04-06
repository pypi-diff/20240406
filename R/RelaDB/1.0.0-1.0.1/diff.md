# Comparing `tmp/RelaDB-1.0.0.tar.gz` & `tmp/RelaDB-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RelaDB-1.0.0.tar", last modified: Sat Apr  6 02:14:01 2024, max compression
+gzip compressed data, was "RelaDB-1.0.1.tar", last modified: Sat Apr  6 02:46:44 2024, max compression
```

## Comparing `RelaDB-1.0.0.tar` & `RelaDB-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:14:01.140565 RelaDB-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 02:14:01.140565 RelaDB-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-06 02:13:55.000000 RelaDB-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:14:01.140565 RelaDB-1.0.0/RelaDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 02:14:01.000000 RelaDB-1.0.0/RelaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 02:14:01.000000 RelaDB-1.0.0/RelaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:14:01.000000 RelaDB-1.0.0/RelaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:14:01.000000 RelaDB-1.0.0/RelaDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:14:01.140565 RelaDB-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-06 02:13:55.000000 RelaDB-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:46:44.629441 RelaDB-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-06 02:46:44.629441 RelaDB-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-06 02:46:40.000000 RelaDB-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:46:44.625441 RelaDB-1.0.1/RelaDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-06 02:46:44.000000 RelaDB-1.0.1/RelaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 02:46:44.000000 RelaDB-1.0.1/RelaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:46:44.000000 RelaDB-1.0.1/RelaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:46:44.000000 RelaDB-1.0.1/RelaDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:46:44.629441 RelaDB-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-06 02:46:40.000000 RelaDB-1.0.1/setup.py
```

### Comparing `RelaDB-1.0.0/README.md` & `RelaDB-1.0.1/README.md`

 * *Files identical despite different names*

