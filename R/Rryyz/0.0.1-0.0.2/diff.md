# Comparing `tmp/Rryyz-0.0.1.tar.gz` & `tmp/Rryyz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Rryyz-0.0.1.tar", last modified: Fri Apr  5 12:00:21 2024, max compression
+gzip compressed data, was "Rryyz-0.0.2.tar", last modified: Sat Apr  6 11:57:25 2024, max compression
```

## Comparing `Rryyz-0.0.1.tar` & `Rryyz-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 12:00:21.910444 Rryyz-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-05 11:53:56.000000 Rryyz-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      436 2024-04-05 12:00:21.910444 Rryyz-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       41 2024-04-05 11:52:45.000000 Rryyz-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 12:00:21.904445 Rryyz-0.0.1/Rryyz/
--rw-rw-rw-   0        0        0      442 2024-04-05 11:41:54.000000 Rryyz-0.0.1/Rryyz/__init__.py
--rw-rw-rw-   0        0        0     6453 2024-04-02 14:03:43.000000 Rryyz-0.0.1/Rryyz/core.py
--rw-rw-rw-   0        0        0     4656 2023-12-09 16:20:04.000000 Rryyz-0.0.1/Rryyz/core_simple.py
--rw-rw-rw-   0        0        0     1421 2024-03-05 14:50:31.000000 Rryyz-0.0.1/Rryyz/cuda.py
--rw-rw-rw-   0        0        0     2152 2024-04-04 14:06:05.000000 Rryyz-0.0.1/Rryyz/dataloaders.py
--rw-rw-rw-   0        0        0    12667 2024-04-05 06:12:16.000000 Rryyz-0.0.1/Rryyz/datasets.py
--rw-rw-rw-   0        0        0     8785 2024-04-05 10:19:49.000000 Rryyz-0.0.1/Rryyz/functions.py
--rw-rw-rw-   0        0        0     2431 2024-03-26 04:21:26.000000 Rryyz-0.0.1/Rryyz/layers.py
--rw-rw-rw-   0        0        0      851 2024-04-01 11:19:24.000000 Rryyz-0.0.1/Rryyz/models.py
--rw-rw-rw-   0        0        0     1531 2024-03-26 09:26:41.000000 Rryyz-0.0.1/Rryyz/optimizers.py
--rw-rw-rw-   0        0        0     4124 2024-04-04 13:00:17.000000 Rryyz-0.0.1/Rryyz/transforms.py
--rw-rw-rw-   0        0        0     3633 2024-04-02 14:17:08.000000 Rryyz-0.0.1/Rryyz/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-05 12:00:21.909444 Rryyz-0.0.1/Rryyz.egg-info/
--rw-rw-rw-   0        0        0      436 2024-04-05 12:00:21.000000 Rryyz-0.0.1/Rryyz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-05 12:00:21.000000 Rryyz-0.0.1/Rryyz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 12:00:21.000000 Rryyz-0.0.1/Rryyz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-05 12:00:21.000000 Rryyz-0.0.1/Rryyz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      399 2024-04-05 12:00:15.000000 Rryyz-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 12:00:21.911444 Rryyz-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 11:57:25.653231 Rryyz-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 11:53:56.000000 Rryyz-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    16046 2024-04-06 11:57:25.653231 Rryyz-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15651 2024-04-06 11:51:40.000000 Rryyz-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 11:57:25.646838 Rryyz-0.0.2/Rryyz/
+-rw-rw-rw-   0        0        0      442 2024-04-05 11:41:54.000000 Rryyz-0.0.2/Rryyz/__init__.py
+-rw-rw-rw-   0        0        0     6453 2024-04-02 14:03:43.000000 Rryyz-0.0.2/Rryyz/core.py
+-rw-rw-rw-   0        0        0     4656 2023-12-09 16:20:04.000000 Rryyz-0.0.2/Rryyz/core_simple.py
+-rw-rw-rw-   0        0        0     1421 2024-03-05 14:50:31.000000 Rryyz-0.0.2/Rryyz/cuda.py
+-rw-rw-rw-   0        0        0     2152 2024-04-04 14:06:05.000000 Rryyz-0.0.2/Rryyz/dataloaders.py
+-rw-rw-rw-   0        0        0    12667 2024-04-05 06:12:16.000000 Rryyz-0.0.2/Rryyz/datasets.py
+-rw-rw-rw-   0        0        0     8785 2024-04-05 10:19:49.000000 Rryyz-0.0.2/Rryyz/functions.py
+-rw-rw-rw-   0        0        0     2431 2024-03-26 04:21:26.000000 Rryyz-0.0.2/Rryyz/layers.py
+-rw-rw-rw-   0        0        0      851 2024-04-01 11:19:24.000000 Rryyz-0.0.2/Rryyz/models.py
+-rw-rw-rw-   0        0        0     1531 2024-03-26 09:26:41.000000 Rryyz-0.0.2/Rryyz/optimizers.py
+-rw-rw-rw-   0        0        0     4124 2024-04-04 13:00:17.000000 Rryyz-0.0.2/Rryyz/transforms.py
+-rw-rw-rw-   0        0        0     3633 2024-04-02 14:17:08.000000 Rryyz-0.0.2/Rryyz/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 11:57:25.652231 Rryyz-0.0.2/Rryyz.egg-info/
+-rw-rw-rw-   0        0        0    16046 2024-04-06 11:57:25.000000 Rryyz-0.0.2/Rryyz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-06 11:57:25.000000 Rryyz-0.0.2/Rryyz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 11:57:25.000000 Rryyz-0.0.2/Rryyz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 11:57:25.000000 Rryyz-0.0.2/Rryyz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      399 2024-04-06 11:53:05.000000 Rryyz-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 11:57:25.653231 Rryyz-0.0.2/setup.cfg
```

### Comparing `Rryyz-0.0.1/LICENSE` & `Rryyz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/core.py` & `Rryyz-0.0.2/Rryyz/core.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/core_simple.py` & `Rryyz-0.0.2/Rryyz/core_simple.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/cuda.py` & `Rryyz-0.0.2/Rryyz/cuda.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/dataloaders.py` & `Rryyz-0.0.2/Rryyz/dataloaders.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/datasets.py` & `Rryyz-0.0.2/Rryyz/datasets.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/functions.py` & `Rryyz-0.0.2/Rryyz/functions.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/layers.py` & `Rryyz-0.0.2/Rryyz/layers.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/models.py` & `Rryyz-0.0.2/Rryyz/models.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/optimizers.py` & `Rryyz-0.0.2/Rryyz/optimizers.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/transforms.py` & `Rryyz-0.0.2/Rryyz/transforms.py`

 * *Files identical despite different names*

### Comparing `Rryyz-0.0.1/Rryyz/utils.py` & `Rryyz-0.0.2/Rryyz/utils.py`

 * *Files identical despite different names*

