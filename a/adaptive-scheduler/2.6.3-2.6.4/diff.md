# Comparing `tmp/adaptive_scheduler-2.6.3.tar.gz` & `tmp/adaptive_scheduler-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_scheduler-2.6.3.tar", last modified: Fri Mar 22 17:32:13 2024, max compression
+gzip compressed data, was "adaptive_scheduler-2.6.4.tar", last modified: Sat Apr  6 08:09:59 2024, max compression
```

## Comparing `adaptive_scheduler-2.6.3.tar` & `adaptive_scheduler-2.6.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:13.298566 adaptive_scheduler-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-22 17:32:13.298566 adaptive_scheduler-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:13.302566 adaptive_scheduler-2.6.3/adaptive_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7996 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_mock_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:13.294566 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:13.294566 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/base_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    14217 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/run_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-22 17:32:13.302566 adaptive_scheduler-2.6.3/adaptive_scheduler/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/client_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/server_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    42831 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32917 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/adaptive_scheduler/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:13.298566 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-22 17:32:13.000000 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-22 17:32:13.000000 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:32:13.000000 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-22 17:32:13.000000 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-22 17:32:13.000000 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-22 17:32:13.000000 adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:32:13.298566 adaptive_scheduler-2.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:13.298566 adaptive_scheduler-2.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_client_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    13837 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_log_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_log_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_run_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_server_support_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_slurm_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_utils_file_creation_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-03-22 17:32:00.000000 adaptive_scheduler-2.6.3/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:59.825352 adaptive_scheduler-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-06 08:09:59.825352 adaptive_scheduler-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:59.829352 adaptive_scheduler-2.6.4/adaptive_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7996 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_mock_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:59.821352 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:59.821352 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-06 08:09:59.829352 adaptive_scheduler-2.6.4/adaptive_scheduler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/client_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/server_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42831 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32917 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/adaptive_scheduler/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:59.825352 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-06 08:09:59.000000 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-06 08:09:59.000000 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:09:59.000000 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-06 08:09:59.000000 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-06 08:09:59.000000 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 08:09:59.000000 adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:09:59.825352 adaptive_scheduler-2.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:09:59.825352 adaptive_scheduler-2.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_client_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17884 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_log_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_log_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_server_support_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_slurm_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_utils_file_creation_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-04-06 08:09:43.000000 adaptive_scheduler-2.6.4/tests/test_widgets.py
```

### Comparing `adaptive_scheduler-2.6.3/LICENSE` & `adaptive_scheduler-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/PKG-INFO` & `adaptive_scheduler-2.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 2.6.3
+Version: 2.6.4
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.6.3/README.md` & `adaptive_scheduler-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_mock_scheduler.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_mock_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/base_scheduler.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/common.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/local.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/local.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/pbs.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_scheduler/slurm.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/base_manager.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/base_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/common.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/database_manager.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/database_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,16 +196,17 @@
 
     def update(self, queue: dict[str, dict[str, str]] | None = None) -> None:
         """If the ``job_id`` isn't running anymore, replace it with None."""
         if self._db is None:
             return
         if queue is None:
             queue = self.scheduler.queue(me_only=True)
+        job_names_in_queue = [x["job_name"] for x in queue.values()]
         failed = self._db.get_all(
-            lambda e: (e.job_id is not None) and (e.job_id not in queue),  # type: ignore[operator]
+            lambda e: e.job_name is not None and e.job_name not in job_names_in_queue,  # type: ignore[operator]
         )
         self.failed.extend([asdict(entry) for _, entry in failed])
         indices = [index for index, _ in failed]
         self._db.update(
             {"job_id": None, "job_name": None, "is_pending": False},
             indices,
         )
@@ -247,32 +248,35 @@
         job_id = self.scheduler.sanatize_job_id(job_id)
         output_fnames = self.scheduler.output_fnames(job_name)
         return [
             f.with_name(f.name.replace(self.scheduler._JOB_ID_VARIABLE, job_id))
             for f in output_fnames
         ]
 
-    def _choose_fname(self, job_name: str) -> tuple[int, str | list[str] | None]:
+    def _choose_fname(self) -> tuple[int, str | list[str] | None]:
         assert self._db is not None
         entry = self._db.get(
             lambda e: e.job_id is None and not e.is_done and not e.is_pending,
         )
         if entry is None:
             msg = "Requested a new job but no more learners to run in the database."
             raise RuntimeError(msg)
         log.debug("choose fname", entry=entry)
         index = self._db.all().index(entry)
+        return index, _ensure_str(entry.fname)  # type: ignore[return-value]
+
+    def _confirm_submitted(self, index: int, job_name: str) -> None:
+        assert self._db is not None
         self._db.update(
             {
                 "job_name": job_name,
                 "is_pending": True,
             },
             indices=[index],
         )
-        return index, _ensure_str(entry.fname)  # type: ignore[return-value]
 
     def _start_request(
         self,
         job_id: str,
         log_fname: str,
         job_name: str,
     ) -> str | list[str] | None:
```

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/job_manager.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/job_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,22 +239,25 @@
         num_jobs_to_start = min(
             len(not_queued),
             self.max_simultaneous_jobs - len(queued),
         )
         for _ in range(num_jobs_to_start):
             job_name = not_queued.pop()
             queued.add(job_name)
-            index, fname = self.database_manager._choose_fname(job_name)
+
+            index, fname = self.database_manager._choose_fname()
             log.debug(
                 f"Starting `job_name={job_name}` with `index={index}` and `fname={fname}`",
             )
             await loop.run_in_executor(
                 ex,
                 partial(self.scheduler.start_job, name=job_name, index=index),
             )
+            self.database_manager._confirm_submitted(index, job_name)
+
             self.n_started += 1
             self._request_times[job_name] = _now()
 
     async def _manage(self) -> None:
         loop = asyncio.get_event_loop()
         with ThreadPoolExecutor() as ex:  # TODO: use asyncio.to_thread when Python≥3.9
             while True:
```

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/kill_manager.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/launcher.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/parse_logs.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/parse_logs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/run_manager.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/run_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/_server_support/slurm_run.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/_server_support/slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/client_support.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/scheduler.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/server_support.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/server_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/utils.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler/widgets.py` & `adaptive_scheduler-2.6.4/adaptive_scheduler/widgets.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/PKG-INFO` & `adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 2.6.3
+Version: 2.6.4
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.6.3/adaptive_scheduler.egg-info/SOURCES.txt` & `adaptive_scheduler-2.6.4/adaptive_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/pyproject.toml` & `adaptive_scheduler-2.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     "TD002",   # Missing author in TODO; try: `# TODO(<author_name>): ...`
     "TD003",   # Missing issue link on the line following this TODO
     "FIX002",  # Line contains TODO"
     "E501",    # Line too long
 ]
 
 [tool.ruff.lint.per-file-ignores]
-"tests/*" = ["SLF001", "PLR2004"]
+"tests/*" = ["SLF001", "PLR2004", "PLR0915"]
 "tests/test_examples.py" = ["E501"]
 ".github/*" = ["INP001"]
 
 [tool.ruff.lint.mccabe]
 max-complexity = 18
 
 [tool.mypy]
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_base_scheduler.py` & `adaptive_scheduler-2.6.4/tests/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_client_support.py` & `adaptive_scheduler-2.6.4/tests/test_client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_database_manager.py` & `adaptive_scheduler-2.6.4/tests/test_database_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -177,15 +177,16 @@
     | list[adaptive.BalancingLearner]
     | list[adaptive.SequenceLearner],
     fnames: list[str] | list[Path],
 ) -> None:
     """Test starting and stopping jobs using the dispatch method."""
     db_manager.learners, db_manager.fnames = learners, fnames
     db_manager.create_empty_db()
-    index, _fname = db_manager._choose_fname("test_job")
+    index, _fname = db_manager._choose_fname()
+    db_manager._confirm_submitted(index, "test_job")
     assert index == 0  # The first learner is chosen
     start_request = ("start", "1000", "log_1000.txt", "test_job")
     fname = db_manager._dispatch(start_request)  # type: ignore[arg-type]
     assert fname == _fname
     assert fname in _ensure_str(db_manager.fnames)
     if isinstance(learners[0], adaptive.BalancingLearner):
         assert isinstance(fname, list)
@@ -209,19 +210,21 @@
     fnames: list[str] | list[Path],
 ) -> None:
     """Test starting and updating jobs."""
     db_manager.create_empty_db()
     db_manager.start()
     await asyncio.sleep(0.1)  # Give it some time to start
 
-    # Choose fname for "job_name"
-    _, _fname = db_manager._choose_fname("job_name")
+    job_id, log_fname, job_name = "1000", "log.log", "job_name"
+
+    # Choose fname for "job_name" and tell the DB the job is launched
+    index, _fname = db_manager._choose_fname()
+    db_manager._confirm_submitted(index, job_name)
 
     # Send a start message to the DatabaseManager
-    job_id, log_fname, job_name = "1000", "log.log", "job_name"
     start_message = ("start", job_id, log_fname, job_name)
     fname = await send_message(socket, start_message)
     assert fname == _fname
 
     # Check if the correct fname is returned
     assert fname == _ensure_str(fnames[0]), fname
 
@@ -230,15 +233,15 @@
     entry = db_manager._db.get(lambda entry: entry.fname == fname)
     assert entry is not None
     assert entry.job_id == job_id
     assert entry.log_fname == log_fname
     assert entry.job_name == job_name
 
     # Say that the job is still running
-    queue = {"1000": {"job_id": "1000"}}
+    queue = {"1000": {"job_id": job_id, "job_name": job_name}}
     db_manager.update(queue)
 
     # Check that the database is the same
     entry = db_manager._db.get(lambda entry: entry.fname == fname)
     assert entry is not None
     assert entry.job_id == job_id
     assert entry.log_fname == log_fname
@@ -262,30 +265,29 @@
 ) -> None:
     """Test starting and stopping jobs."""
     db_manager.create_empty_db()
     db_manager.start()
     await asyncio.sleep(0.1)  # Give it some time to start
     assert db_manager.task is not None
 
-    # Choose fname for "job_name"
-    index, _fname = db_manager._choose_fname("job_name")
+    job_id, log_fname, job_name = "1000", "log.log", "job_name"
+
+    # Choose fname for "job_name" and tell the DB the job is launched
+    index, _ = db_manager._choose_fname()
+    db_manager._confirm_submitted(index, job_name)
 
     # Send a start message to the DatabaseManager
-    job_id, log_fname, job_name = "1000", "log.log", "job_name"
     start_message = ("start", job_id, log_fname, job_name)
     fname = await send_message(socket, start_message)
     # Try starting again:
     exception = await send_message(socket, start_message)
-    with pytest.raises(
-        Exception,
-        match="The job_id 1000 already exists in the database and runs",
-    ):
-        raise exception
+    assert "The job_id 1000 already exists in the database and runs" in str(exception)
     assert fname == _ensure_str(fnames[0]), fname
 
+    assert db_manager._db is not None
     # Check that the database is updated correctly
     entry = db_manager._db.get(lambda entry: entry.fname == fname)
     assert entry is not None
     assert entry.job_id == job_id
     assert entry.log_fname == log_fname
     assert entry.job_name == job_name
 
@@ -294,20 +296,22 @@
     assert not db_manager.task.done()
 
     # Send a stop message to the DatabaseManager
     stop_message = ("stop", fname)
     reply = await send_message(socket, stop_message)
     assert reply is None
 
+    assert db_manager._db is not None
     entry = db_manager._db.get(lambda entry: entry.fname == _ensure_str(fnames[0]))
     assert entry is not None
     assert entry.job_id is None
 
     # Start and stop the learner2
-    _index, _fname = db_manager._choose_fname("job_name")
+    index2, _ = db_manager._choose_fname()
+    db_manager._confirm_submitted(index2, job_name)
     fname = await send_message(socket, start_message)
     assert fname == _ensure_str(fnames[1])
 
     # Send a stop message to the DatabaseManager
     stop_message = ("stop", fname)
     reply = await send_message(socket, stop_message)
     assert reply is None
@@ -328,26 +332,28 @@
     await asyncio.sleep(0.1)  # Give it some time to start
     assert db_manager.task is not None
     assert db_manager._db is not None
 
     # Start a job for learner1
     job_id1, log_fname1, job_name1 = "1000", "log1.log", "job_name1"
     start_message1 = ("start", job_id1, log_fname1, job_name1)
-    _, _fname1 = db_manager._choose_fname(job_name1)
+    _index1, _fname1 = db_manager._choose_fname()
+    db_manager._confirm_submitted(_index1, job_name1)
     fname1 = await send_message(socket, start_message1)
     assert fname1 == _fname1
     assert fname1 == _ensure_str(fnames[0]), fname1
     e = db_manager._db.get(lambda entry: entry.fname == fname1)
     assert isinstance(e, _DBEntry)
     assert e.job_id == job_id1
 
     # Start a job for learner2
     job_id2, log_fname2, job_name2 = "1001", "log2.log", "job_name2"
     start_message2 = ("start", job_id2, log_fname2, job_name2)
-    _, _fname2 = db_manager._choose_fname(job_name2)
+    _index2, _fname2 = db_manager._choose_fname()
+    db_manager._confirm_submitted(_index2, job_name2)
     fname2 = await send_message(socket, start_message2)
     assert fname2 == _fname2
     assert fname2 == _ensure_str(fnames[1]), fname2
     e = db_manager._db.get(lambda entry: entry.fname == fname2)
     assert isinstance(e, _DBEntry)
     assert e.job_id == job_id2
 
@@ -365,14 +371,118 @@
     entry = db_manager._db.get(lambda entry: entry.fname == fname2)
     assert entry is not None
     assert entry.job_id is None, (fname1, fname2)
     assert entry.is_done is True
     assert entry.job_name is None
 
 
+def test_job_failure_after_start_request(db_manager: DatabaseManager) -> None:
+    """Ensure jobs that fail after they send a start request are updated in the DB."""
+    db_manager.create_empty_db()
+    assert not db_manager.failed
+
+    index, _ = db_manager._choose_fname()
+    db_manager._confirm_submitted(index, "job1")
+    # job is launched and appears in queue
+    db_manager.update({"1": {"job_name": "job1"}})
+    # job reports back that it started
+    db_manager._start_request("1", "log", "job1")
+    # job dies, disappearing from queue
+    db_manager.update({})
+    assert db_manager.failed
+
+
+def test_job_failure_before_start_request(db_manager: DatabaseManager) -> None:
+    """Ensure jobs that fail before they send a start request are updated in the DB.
+
+    This is a regression test against
+    https://github.com/basnijholt/adaptive-scheduler/issues/216
+    """
+    db_manager.create_empty_db()
+    assert not db_manager.failed
+
+    index, _ = db_manager._choose_fname()
+    # Job is launched
+    db_manager._confirm_submitted(index, "job1")
+    # Job appears in queue, and one of our "update" calls sees it
+    db_manager.update({"1": {"job_name": "job1"}})
+    # Job dies, disappearing from queue
+    db_manager.update({})
+    assert db_manager.failed
+
+
+def test_job_failure_before_start_request_slow_update(
+    db_manager: DatabaseManager,
+) -> None:
+    """Ensure jobs that fail before they send a start request are updated in the DB, even if db manager updates slowly.
+
+    This is a regression test against
+    https://github.com/basnijholt/adaptive-scheduler/issues/216
+    """
+    db_manager.create_empty_db()
+    assert not db_manager.failed
+
+    index, _ = db_manager._choose_fname()
+    # Job is launched...
+    db_manager._confirm_submitted(index, "job1")
+    # But dies before the next time our DB updates.
+    db_manager.update({})
+    assert db_manager.failed
+
+
+def test_job_failure_before_start_request_interleaved(
+    db_manager: DatabaseManager,
+) -> None:
+    """Ensure jobs that fail before they send a start request are updated in the DB, even if db manager updates slowly.
+
+    This is a regression test against
+    https://github.com/basnijholt/adaptive-scheduler/issues/216
+    """
+    db_manager.create_empty_db()
+    assert not db_manager.failed
+
+    # fname is chosen...
+    index, _ = db_manager._choose_fname()
+    # Database is updated by another task efore launch is confirmed;
+    # this does not result in the job being marked as failed.
+    db_manager.update({})
+    assert not db_manager.failed
+    # Launch is later confirmed...
+    db_manager._confirm_submitted(index, "job1")
+    # But job is still not in queue...
+    db_manager.update({})
+    # which means that it will be marked as failed
+    assert db_manager.failed
+
+
+def test_job_failure_before_start_request_interleaved2(
+    db_manager: DatabaseManager,
+) -> None:
+    """Ensure jobs that fail before they send a start request are updated in the DB, even if db manager updates slowly.
+
+    This is a regression test against
+    https://github.com/basnijholt/adaptive-scheduler/issues/216
+    """
+    db_manager.create_empty_db()
+    assert not db_manager.failed
+
+    # fname is chosen...
+    index, _ = db_manager._choose_fname()
+    # Database is updated after job is in the queue, but before
+    # launch is confirmed by the job manager
+    db_manager.update({"1": {"job_name": "job1"}})
+    assert not db_manager.failed
+    # launch is confirmed by job manager
+    db_manager._confirm_submitted(index, "job1")
+    # job disappears from queue...
+    db_manager.update({})
+    # which means that it will be marked as failed
+    assert db_manager.failed
+
+
 @pytest.mark.parametrize(
     ("input_list", "expected_output"),
     [
         # Test with a list of strings
         (["path1", "path2", "path3", "path4"], ["path1", "path2", "path3", "path4"]),
         # Test with a list of Path objects
         (
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_job_manager.py` & `adaptive_scheduler-2.6.4/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_kill_manager.py` & `adaptive_scheduler-2.6.4/tests/test_kill_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,16 @@
     with output_file_path.open("w") as f:
         f.write("srun: error: GPU on fire!\n")
 
     kill_manager.database_manager.start()  # creates empty db
     kill_manager.start()
     assert kill_manager.task is not None
     # Marks the job as running, and sets the job_id, job_name, and log_fname
-    kill_manager.database_manager._choose_fname("test_job")
+    index, _ = kill_manager.database_manager._choose_fname()
+    kill_manager.database_manager._confirm_submitted(index, "test_job")
     kill_manager.database_manager._start_request("0", "log_fname.log", "test_job")
     kill_manager.scheduler.start_job("test_job")
     await asyncio.sleep(0.1)  # Give it some time to start and cancel the job
     assert "test_job" in kill_manager.cancelled
     assert str(output_file_path) in kill_manager.deleted
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_launcher.py` & `adaptive_scheduler-2.6.4/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_log_generation.py` & `adaptive_scheduler-2.6.4/tests/test_log_generation.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_log_parsing.py` & `adaptive_scheduler-2.6.4/tests/test_log_parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,16 @@
             f.write(json.dumps(entry) + "\n")
         f.flush()
 
         # Prepare the database manager, scheduler, and job names
         job_name = "test_job"
         db_manager.start()
         # Add an entry in the database manager
-        db_manager._choose_fname(job_name)
+        index, _ = db_manager._choose_fname()
+        db_manager._confirm_submitted(index, job_name)
         db_manager._start_request("0", f.name, job_name)
         db_manager.scheduler.start_job(job_name)
 
         # Test parse_log_files
         df_result = parse_log_files(
             db_manager,
             db_manager.scheduler,
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_run_manager.py` & `adaptive_scheduler-2.6.4/tests/test_run_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test the RunManager class."""
 
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, cast
 from unittest.mock import patch
 
 import adaptive
 import pytest
 from ipywidgets import VBox
 
 from adaptive_scheduler._server_support.run_manager import (
@@ -231,27 +231,31 @@
     | list[adaptive.SequenceLearner],
     fnames: list[str] | list[Path],
 ) -> None:
     """Test starting the RunManager."""
     rm = RunManager(mock_scheduler, learners, fnames, job_manager_interval=0.1)
     rm.start()
     await asyncio.sleep(0.1)
+    assert rm.task is not None
     assert rm.status() == "running"
     q = rm.scheduler.queue()
     assert "0" in q
     assert "1" in q
     # Note: we don't know whether it is:
     # This: "0": {"job_name": "adaptive-scheduler-0"}, "1": {"job_name": "adaptive-scheduler-1"}
     # or:   "1": {"job_name": "adaptive-scheduler-0"}, "0": {"job_name": "adaptive-scheduler-1"}
     job_names = job_name0, job_name1 = "adaptive-scheduler-0", "adaptive-scheduler-1"
     job_id0, job_id1 = rm.scheduler.job_names_to_job_ids(job_name0, job_name1)
     log_fnames = ("log0.log", "log1.log")
 
     db = rm.database_manager.as_dicts()
-    assert db[0]["job_id"] is None  # no jobs are started yet
+    # jobs were all assigned...
+    assert all(x["job_name"] is not None for x in db)
+    # but they have not yet reported that they started.
+    assert all(x["job_id"] is None for x in db)
 
     # Send a start message to the DatabaseManager
     # This is coming from the client
     with get_socket(rm.database_manager) as socket:
         for i, (entry, log_fname) in enumerate(zip(db, log_fnames)):
             job_id = str(i)
             job_name = entry["job_name"]
@@ -271,15 +275,15 @@
         job_id0: {"job_name": job_name0, "status": "C"},
         job_id1: {
             "job_name": "adaptive-scheduler-1",
             "status": "R",
             "state": "RUNNING",
         },
     }
-    rm.scheduler._queue_info.pop(job_id0)
+    cast(MockScheduler, rm.scheduler)._queue_info.pop(job_id0)
     await asyncio.sleep(0.15)
     # Check that the job is restarted automatically with a new job_id:
     q = rm.scheduler.queue()
     assert q["2"] == {"job_name": job_name0, "state": "RUNNING", "status": "R"}
 
     # Start the job "from the client"
     with get_socket(rm.database_manager) as socket:
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_server_support_common.py` & `adaptive_scheduler-2.6.4/tests/test_server_support_common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_slurm_run.py` & `adaptive_scheduler-2.6.4/tests/test_slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_slurm_scheduler.py` & `adaptive_scheduler-2.6.4/tests/test_slurm_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
             --name TEST \\
             --n 23975
         """,
         ).strip()
     )
 
 
-def test_multiple_jobs() -> None:  # noqa: PLR0915
+def test_multiple_jobs() -> None:
     """Test that multiple jobs can be started."""
     cores = (3, 4, 5)
     s = SLURM(cores=cores)
     for i, n in enumerate(cores):
         js = s.job_script(options={}, index=i)
         assert f"#SBATCH --ntasks {n}" in js
         assert js.count("--ntasks") == 1
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_utils.py` & `adaptive_scheduler-2.6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.6.3/tests/test_utils_file_creation_progress.py` & `adaptive_scheduler-2.6.4/tests/test_utils_file_creation_progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     progress = Progress(auto_refresh=False)
     task = asyncio.create_task(
         _track_file_creation_progress(paths_dict, progress, interval=1e-3),
     )
 
     # Allow some time for the task to process
-    await asyncio.sleep(0.05)
+    await asyncio.sleep(0.1)
 
     progress.stop()
     assert "Total" in progress._tasks[0].description
     assert progress._tasks[0].total == 3
     assert progress._tasks[0].completed == 1
 
     assert "category1" in progress._tasks[1].description
@@ -99,15 +99,15 @@
 
     assert "category2" in progress._tasks[2].description
     assert progress._tasks[2].total == 1
     assert progress._tasks[2].completed == 0
 
     # Create one of the files of category2, should still not be completed
     create_test_files(tmp_path, ["file3"])
-    await asyncio.sleep(0.05)
+    await asyncio.sleep(0.1)
 
     assert "category2" in progress._tasks[2].description
     assert progress._tasks[2].total == 1
     assert progress._tasks[2].completed == 0
     assert paths_dict["category2"] == {(tmp_path / "file4",)}
 
     # Create the other file of category2, should now be completed
```

### Comparing `adaptive_scheduler-2.6.3/tests/test_widgets.py` & `adaptive_scheduler-2.6.4/tests/test_widgets.py`

 * *Files identical despite different names*

