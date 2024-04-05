# Comparing `tmp/swebench-1.0.3.tar.gz` & `tmp/swebench-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.3.tar", last modified: Thu Apr  4 17:24:17 2024, max compression
+gzip compressed data, was "swebench-1.0.4.tar", last modified: Fri Apr  5 23:38:06 2024, max compression
```

## Comparing `swebench-1.0.3.tar` & `swebench-1.0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.756102 swebench-1.0.3/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.3/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-04 17:24:17.756030 swebench-1.0.3/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5270 2024-04-02 05:49:19.000000 swebench-1.0.3/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.745527 swebench-1.0.3/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.746246 swebench-1.0.3/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.748621 swebench-1.0.3/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.3/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.3/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.3/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-04 17:24:17.756307 swebench-1.0.3/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.3/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.748975 swebench-1.0.3/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-04 17:24:01.000000 swebench-1.0.3/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.750956 swebench-1.0.3/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.753171 swebench-1.0.3/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18925 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    30128 2024-04-04 17:22:05.000000 swebench-1.0.3/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.3/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14820 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.754709 swebench-1.0.3/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.3/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     5932 2024-04-04 17:22:14.000000 swebench-1.0.3/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.3/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.755612 swebench-1.0.3/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.755793 swebench-1.0.3/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.956869 swebench-1.0.4/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.4/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-05 23:38:06.956811 swebench-1.0.4/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.4/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.949287 swebench-1.0.4/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.949728 swebench-1.0.4/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.950815 swebench-1.0.4/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.4/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.4/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.4/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-05 23:38:06.957064 swebench-1.0.4/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.4/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.950983 swebench-1.0.4/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-05 23:37:51.000000 swebench-1.0.4/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.952393 swebench-1.0.4/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.953891 swebench-1.0.4/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18858 2024-04-05 22:22:32.000000 swebench-1.0.4/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    30665 2024-04-05 19:15:08.000000 swebench-1.0.4/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.4/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.4/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.955726 swebench-1.0.4/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.4/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5932 2024-04-04 17:22:14.000000 swebench-1.0.4/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.4/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.956405 swebench-1.0.4/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.956564 swebench-1.0.4/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.3/LICENSE` & `swebench-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/PKG-INFO` & `swebench-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.3
+Version: 1.0.4
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -31,15 +31,15 @@
   <a href="https://github.com/princeton-nlp/Llamao">
     <img src="assets/swellama_banner.png" width="50%" alt="Kawi the SWE-Llama" />
   </a>
 </p>
 
 <div align="center">
 
- | [日本語](docs/README_JP.md) | [English](https://github.com/princeton-nlp/SWE-bench) |
+ | [日本語](docs/README_JP.md) | [English](https://github.com/princeton-nlp/SWE-bench) | [中文简体](docs/README_CN.md) | [中文繁體](docs/README_TW.md) |
 
 </div>
 
 
 ---
 <p align="center">
 Code and data for our ICLR 2024 paper <a href="http://swe-bench.github.io/paper.pdf">SWE-bench: Can Language Models Resolve Real-World GitHub Issues?</a>
@@ -52,15 +52,15 @@
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
     <a href="https://badge.fury.io/py/swebench">
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
-Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/master/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
+Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
@@ -72,17 +72,17 @@
 4. Activate the environment with `conda activate swe-bench`
 
 ## 💽 Usage
 You can download the SWE-bench dataset directly ([dev](https://drive.google.com/uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets) or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 
 To use SWE-Bench, you can:
 * Train your own models on our pre-processed datasets  
-* Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/master/inference/) on existing models (either models you have on-disk like LLaMA, or models you have access to through an API like GPT-4). The inference step is where you get a repo and an issue and have the model try to generate a fix for it.
-* [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/master/harness/) models against SWE-bench. This is where you take a SWE-Bench task and a model-proposed solution and evaluate its correctness. 
-*  Run SWE-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/master/collect/) on your own repositories, to make new SWE-Bench tasks. 
+* Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/main/inference/) on existing models (either models you have on-disk like LLaMA, or models you have access to through an API like GPT-4). The inference step is where you get a repo and an issue and have the model try to generate a fix for it.
+* [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/harness/) models against SWE-bench. This is where you take a SWE-Bench task and a model-proposed solution and evaluate its correctness. 
+*  Run SWE-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/collect/) on your own repositories, to make new SWE-Bench tasks. 
 
 ## ⬇️ Downloads
 | Datasets | Models |
 | - | - |
 | [🤗 SWE-bench](https://huggingface.co/datasets/princeton-nlp/SWE-bench) | [🦙 SWE-Llama 13b](https://huggingface.co/princeton-nlp/SWE-Llama-13b) |
 | [🤗 "Oracle" Retrieval](https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [🦙 SWE-Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) |
 | [🤗 BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-bench_bm25_13K) | [🦙 SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-Llama-7b) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.3 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.4 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -10,44 +10,45 @@
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: chardet Requires-Dist:
 datasets Requires-Dist: ghapi Requires-Dist: GitPython Requires-Dist: python-
 dotenv Requires-Dist: requests Requires-Dist: rich
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
-                                 SWE-bench) |
+     SWE-bench) | [ä¸­æç®ä½](docs/README_CN.md) | [ä¸­æç¹é«](docs/
+                                README_TW.md) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
       _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
-blob/master/CHANGELOG.md) for information on the latest updates to the SWE-
-bench benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
+blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
+benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
 language models on real world software issues collected from GitHub. Given a
 *codebase* and an *issue*, a language model is tasked with generating a *patch*
 that resolves the described problem. [assets/teaser.png]## ð Set Up To build
 SWE-bench from source, follow these steps: 1. Clone this repository locally 2.
 `cd` into the repository. 3. Run `conda env create -f environment.yml` to
 created a conda environment named `swe-bench` 4. Activate the environment with
 `conda activate swe-bench` ## ð½ Usage You can download the SWE-bench dataset
 directly ([dev](https://drive.google.com/
 uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
 drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
 or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 To use SWE-Bench, you can: * Train your own models on our pre-processed
 datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
-master/inference/) on existing models (either models you have on-disk like
-LLaMA, or models you have access to through an API like GPT-4). The inference
-step is where you get a repo and an issue and have the model try to generate a
-fix for it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/
-master/harness/) models against SWE-bench. This is where you take a SWE-Bench
-task and a model-proposed solution and evaluate its correctness. * Run SWE-
-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/
-blob/master/collect/) on your own repositories, to make new SWE-Bench tasks. ##
+main/inference/) on existing models (either models you have on-disk like LLaMA,
+or models you have access to through an API like GPT-4). The inference step is
+where you get a repo and an issue and have the model try to generate a fix for
+it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
+harness/) models against SWE-bench. This is where you take a SWE-Bench task and
+a model-proposed solution and evaluate its correctness. * Run SWE-bench's [data
+collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/
+swebench/collect/) on your own repositories, to make new SWE-Bench tasks. ##
 â¬ï¸ Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
 huggingface.co/datasets/princeton-nlp/SWE-bench) | [ð¦ SWE-Llama 13b](https:/
 /huggingface.co/princeton-nlp/SWE-Llama-13b) | | [ð¤ "Oracle" Retrieval]
 (https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [ð¦ SWE-
 Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) | |
 [ð¤ BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-
 bench_bm25_13K) | [ð¦ SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-
```

### Comparing `swebench-1.0.3/README.md` & `swebench-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <a href="https://github.com/princeton-nlp/Llamao">
     <img src="assets/swellama_banner.png" width="50%" alt="Kawi the SWE-Llama" />
   </a>
 </p>
 
 <div align="center">
 
- | [日本語](docs/README_JP.md) | [English](https://github.com/princeton-nlp/SWE-bench) |
+ | [日本語](docs/README_JP.md) | [English](https://github.com/princeton-nlp/SWE-bench) | [中文简体](docs/README_CN.md) | [中文繁體](docs/README_TW.md) |
 
 </div>
 
 
 ---
 <p align="center">
 Code and data for our ICLR 2024 paper <a href="http://swe-bench.github.io/paper.pdf">SWE-bench: Can Language Models Resolve Real-World GitHub Issues?</a>
@@ -23,15 +23,15 @@
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
     <a href="https://badge.fury.io/py/swebench">
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
-Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/master/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
+Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
@@ -43,17 +43,17 @@
 4. Activate the environment with `conda activate swe-bench`
 
 ## 💽 Usage
 You can download the SWE-bench dataset directly ([dev](https://drive.google.com/uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets) or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 
 To use SWE-Bench, you can:
 * Train your own models on our pre-processed datasets  
-* Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/master/inference/) on existing models (either models you have on-disk like LLaMA, or models you have access to through an API like GPT-4). The inference step is where you get a repo and an issue and have the model try to generate a fix for it.
-* [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/master/harness/) models against SWE-bench. This is where you take a SWE-Bench task and a model-proposed solution and evaluate its correctness. 
-*  Run SWE-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/master/collect/) on your own repositories, to make new SWE-Bench tasks. 
+* Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/main/inference/) on existing models (either models you have on-disk like LLaMA, or models you have access to through an API like GPT-4). The inference step is where you get a repo and an issue and have the model try to generate a fix for it.
+* [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/harness/) models against SWE-bench. This is where you take a SWE-Bench task and a model-proposed solution and evaluate its correctness. 
+*  Run SWE-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/collect/) on your own repositories, to make new SWE-Bench tasks. 
 
 ## ⬇️ Downloads
 | Datasets | Models |
 | - | - |
 | [🤗 SWE-bench](https://huggingface.co/datasets/princeton-nlp/SWE-bench) | [🦙 SWE-Llama 13b](https://huggingface.co/princeton-nlp/SWE-Llama-13b) |
 | [🤗 "Oracle" Retrieval](https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [🦙 SWE-Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) |
 | [🤗 BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-bench_bm25_13K) | [🦙 SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-Llama-7b) |
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
-                                 SWE-bench) |
+     SWE-bench) | [ä¸­æç®ä½](docs/README_CN.md) | [ä¸­æç¹é«](docs/
+                                README_TW.md) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
       _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
-blob/master/CHANGELOG.md) for information on the latest updates to the SWE-
-bench benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
+blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
+benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
 language models on real world software issues collected from GitHub. Given a
 *codebase* and an *issue*, a language model is tasked with generating a *patch*
 that resolves the described problem. [assets/teaser.png]## ð Set Up To build
 SWE-bench from source, follow these steps: 1. Clone this repository locally 2.
 `cd` into the repository. 3. Run `conda env create -f environment.yml` to
 created a conda environment named `swe-bench` 4. Activate the environment with
 `conda activate swe-bench` ## ð½ Usage You can download the SWE-bench dataset
 directly ([dev](https://drive.google.com/
 uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
 drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
 or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 To use SWE-Bench, you can: * Train your own models on our pre-processed
 datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
-master/inference/) on existing models (either models you have on-disk like
-LLaMA, or models you have access to through an API like GPT-4). The inference
-step is where you get a repo and an issue and have the model try to generate a
-fix for it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/
-master/harness/) models against SWE-bench. This is where you take a SWE-Bench
-task and a model-proposed solution and evaluate its correctness. * Run SWE-
-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/
-blob/master/collect/) on your own repositories, to make new SWE-Bench tasks. ##
+main/inference/) on existing models (either models you have on-disk like LLaMA,
+or models you have access to through an API like GPT-4). The inference step is
+where you get a repo and an issue and have the model try to generate a fix for
+it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
+harness/) models against SWE-bench. This is where you take a SWE-Bench task and
+a model-proposed solution and evaluate its correctness. * Run SWE-bench's [data
+collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/
+swebench/collect/) on your own repositories, to make new SWE-Bench tasks. ##
 â¬ï¸ Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
 huggingface.co/datasets/princeton-nlp/SWE-bench) | [ð¦ SWE-Llama 13b](https:/
 /huggingface.co/princeton-nlp/SWE-Llama-13b) | | [ð¤ "Oracle" Retrieval]
 (https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [ð¦ SWE-
 Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) | |
 [ð¤ BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-
 bench_bm25_13K) | [ð¦ SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-
```

### Comparing `swebench-1.0.3/inference/llamao/distributed_attention.py` & `swebench-1.0.4/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.4/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.4/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/make_datasets/create_instance.py` & `swebench-1.0.4/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.4/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.4/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.4/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/make_datasets/utils.py` & `swebench-1.0.4/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/run_api.py` & `swebench-1.0.4/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/run_live.py` & `swebench-1.0.4/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/inference/run_llama.py` & `swebench-1.0.4/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/setup.py` & `swebench-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/__init__.py` & `swebench-1.0.4/swebench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.3/swebench/collect/build_dataset.py` & `swebench-1.0.4/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/collect/build_dataset_ft.py` & `swebench-1.0.4/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.4/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/collect/get_top_pypi.py` & `swebench-1.0.4/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/collect/print_pulls.py` & `swebench-1.0.4/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/collect/utils.py` & `swebench-1.0.4/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/harness/constants.py` & `swebench-1.0.4/swebench/harness/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,14 +560,13 @@
     "matplotlib/matplotlib": {
         "3.1": "py311_23.9.0-0",
         "3.2": "py311_23.9.0-0",
         "3.3": "py311_23.9.0-0",
         "3.4": "py311_23.9.0-0",
         "3.0": "py311_23.10.0-1",
     },
-    "mwaskom/seaborn": {"0.11": None, "0.12": None, "0.13": None},
     "sympy/sympy": {
         "1.0": "py39_23.9.0-0",
     },
 }
 
 DEFAULT_CONDA_LINK = "py39_23.10.0-1"
```

### Comparing `swebench-1.0.3/swebench/harness/context_manager.py` & `swebench-1.0.4/swebench/harness/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import logging, os, platform, subprocess
+import logging, os, platform, subprocess, json
 
 from logging import DEBUG, INFO, WARNING, ERROR, CRITICAL
 from swebench.harness.constants import (
     APPLY_PATCH_FAIL,
     APPLY_PATCH_PASS,
     DEFAULT_CONDA_LINK,
     INSTALL_FAIL,
@@ -58,33 +58,41 @@
             self.logger.log(level, message)
 
 
 class ExecWrapper:
     def __init__(
         self,
         subprocess_args: dict = None,
-        logger: logging.Logger = None,
+        logger: LogWrapper = None,
     ):
         self.logger = logger
         if subprocess_args is None:
             self.subprocess_args = {}
         else:
             self.subprocess_args = subprocess_args
 
     def __call__(self, cmd, raise_error=True, **kwargs):
         try:
+            if isinstance(cmd, list):
+                self.logger.write(f"Command: {' '.join(cmd)}", level=DEBUG)
+            else:
+                self.logger.write(f"Command: {cmd}", level=DEBUG)
             combined_args = {**self.subprocess_args, **kwargs}
+            self.logger.write(f"Subprocess args:\n{json.dumps(combined_args, indent=4)}", level=DEBUG)
             output = subprocess.run(cmd, **combined_args)
+            self.logger.write(f"Std. Output:\n{output.stdout}", level=DEBUG)
+            if output.stderr:
+                self.logger.write(f"Std. Error:\n{output.stderr}", level=DEBUG)
             return output
         except subprocess.CalledProcessError as e:
             if raise_error and self.logger is not None:
-                self.logger.error(f"Error: {e}")
-                self.logger.error(f"Error stdout: {e.stdout}")
-                self.logger.error(f"Error stderr: {e.stderr}")
-                self.logger.error(f"Error traceback: {format_exc()}")
+                self.logger.write(f"Error: {e}", level=ERROR)
+                self.logger.write(f"Error stdout: {e.stdout}", level=ERROR)
+                self.logger.write(f"Error stderr: {e.stderr}", level=ERROR)
+                self.logger.write(f"Error traceback: {format_exc()}", level=ERROR)
                 raise e
 
 
 class TestbedContextManager:
     def __init__(
         self,
         task_instances: list,
@@ -120,15 +128,14 @@
         self.exec = ExecWrapper(
             subprocess_args={
                 "check": True,
                 "shell": False,
                 "capture_output": True,
                 "text": True,
             },
-            logger=logger_testbed,
         )
 
         # Create log, temp directories if they don't exist
         if not os.path.exists(self.log_dir):
             logger_testbed.info(f"[Testbed] Creating log directory {self.log_dir}")
             os.makedirs(self.log_dir, exist_ok=True)
         if temp_dir is not None and not os.path.exists(temp_dir):
@@ -173,14 +180,15 @@
         else:
             # TODO: Make log file name more intelligible, random 4 digit number for now
             # This random naming is necessary due to parallelized execution
             log_file_name += f"_{os.urandom(24).hex()}.log"
 
         self.log_file = os.path.join(self.log_dir, log_file_name)
         self.log = LogWrapper(self.log_file, logger=logger_testbed, prefix="[Testbed]")
+        self.exec.logger = self.log
         self.log.write(f"Created log file {self.log_file}", mode="w")
 
         # Get reference set up instances for each repo/version
         self.setup_refs = {}
         for repo, map_version_to_instances in self.task_instances_grouped.items():
             self.log.write(f"Repo {repo}: {len(map_version_to_instances)} versions")
 
@@ -508,15 +516,15 @@
             subprocess_args={
                 "check": True,
                 "shell": False,
                 "capture_output": True,
                 "text": True,
                 "env": {"CONDA_PKGS_DIRS": self.conda_cache_dir},
             },
-            logger=logger_taskenv,
+            logger=self.log,
         )
 
     def __enter__(self):
         """
         Enter task environment, set up log file
         """
         os.chdir(self.testbed)
```

### Comparing `swebench-1.0.3/swebench/harness/engine_evaluation.py` & `swebench-1.0.4/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/harness/engine_validation.py` & `swebench-1.0.4/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/harness/run_evaluation.py` & `swebench-1.0.4/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/harness/utils.py` & `swebench-1.0.4/swebench/harness/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,17 @@
     env_names = []
     for line in lines:
         if line.startswith("#"):
             continue
         if line.strip() == "":
             continue
         parts = line.split()
-        if len(parts) == 3:
-            env_name = parts[0]
-        if len(parts) == 2:
-            env_name = parts[0]
-        elif len(parts) == 1:
-            env_name = parts[0].split('/')[-1]
+        if len(parts) <= 1:
+            continue
+        env_name = parts[1]
         env_names.append(env_name)
     return env_names
 
 
 def get_environment_yml(
         instance: dict,
         env_name: str,
@@ -346,22 +343,22 @@
 PATCH_HUNK_PATTERN = re.compile(
     r"\@\@\s+\-(\d+),(\d+)\s+\+(\d+),(\d+)\s+\@\@(.+?)(?=diff\ |\-\-\-\ a\/|\@\@\ \-|\Z)",
     re.DOTALL,
 )
 
 
 def get_first_idx(charlist):
-    """Get index of first occurence of "-" or "+" in charlist"""
+    """Get index of first occurrence of "-" or "+" in charlist"""
     first_min = charlist.index("-") if "-" in charlist else len(charlist)
     first_plus = charlist.index("+") if "+" in charlist else len(charlist)
     return min(first_min, first_plus)
 
 
 def get_last_idx(charlist):
-    """Get index of last occurence of "-" or "+" in charlist"""
+    """Get index of last occurrence of "-" or "+" in charlist"""
     char_idx = get_first_idx(charlist[::-1])
     last_idx = len(charlist) - char_idx
     return last_idx + 1
 
 
 def strip_content(hunk):
     """Remove trailing non +/- lines and trailing whitespace per line per hunk"""
```

### Comparing `swebench-1.0.3/swebench/metrics/constants.py` & `swebench-1.0.4/swebench/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/metrics/conversion.py` & `swebench-1.0.4/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/metrics/getters.py` & `swebench-1.0.4/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/metrics/log_parsers.py` & `swebench-1.0.4/swebench/metrics/log_parsers.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/metrics/metrics.py` & `swebench-1.0.4/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/metrics/monitor.py` & `swebench-1.0.4/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/metrics/report.py` & `swebench-1.0.4/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/versioning/constants.py` & `swebench-1.0.4/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/versioning/get_versions.py` & `swebench-1.0.4/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench/versioning/utils.py` & `swebench-1.0.4/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.3/swebench.egg-info/PKG-INFO` & `swebench-1.0.4/swebench.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.3
+Version: 1.0.4
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -31,15 +31,15 @@
   <a href="https://github.com/princeton-nlp/Llamao">
     <img src="assets/swellama_banner.png" width="50%" alt="Kawi the SWE-Llama" />
   </a>
 </p>
 
 <div align="center">
 
- | [日本語](docs/README_JP.md) | [English](https://github.com/princeton-nlp/SWE-bench) |
+ | [日本語](docs/README_JP.md) | [English](https://github.com/princeton-nlp/SWE-bench) | [中文简体](docs/README_CN.md) | [中文繁體](docs/README_TW.md) |
 
 </div>
 
 
 ---
 <p align="center">
 Code and data for our ICLR 2024 paper <a href="http://swe-bench.github.io/paper.pdf">SWE-bench: Can Language Models Resolve Real-World GitHub Issues?</a>
@@ -52,15 +52,15 @@
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
     <a href="https://badge.fury.io/py/swebench">
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
-Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/master/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
+Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
@@ -72,17 +72,17 @@
 4. Activate the environment with `conda activate swe-bench`
 
 ## 💽 Usage
 You can download the SWE-bench dataset directly ([dev](https://drive.google.com/uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets) or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 
 To use SWE-Bench, you can:
 * Train your own models on our pre-processed datasets  
-* Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/master/inference/) on existing models (either models you have on-disk like LLaMA, or models you have access to through an API like GPT-4). The inference step is where you get a repo and an issue and have the model try to generate a fix for it.
-* [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/master/harness/) models against SWE-bench. This is where you take a SWE-Bench task and a model-proposed solution and evaluate its correctness. 
-*  Run SWE-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/master/collect/) on your own repositories, to make new SWE-Bench tasks. 
+* Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/main/inference/) on existing models (either models you have on-disk like LLaMA, or models you have access to through an API like GPT-4). The inference step is where you get a repo and an issue and have the model try to generate a fix for it.
+* [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/harness/) models against SWE-bench. This is where you take a SWE-Bench task and a model-proposed solution and evaluate its correctness. 
+*  Run SWE-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/collect/) on your own repositories, to make new SWE-Bench tasks. 
 
 ## ⬇️ Downloads
 | Datasets | Models |
 | - | - |
 | [🤗 SWE-bench](https://huggingface.co/datasets/princeton-nlp/SWE-bench) | [🦙 SWE-Llama 13b](https://huggingface.co/princeton-nlp/SWE-Llama-13b) |
 | [🤗 "Oracle" Retrieval](https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [🦙 SWE-Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) |
 | [🤗 BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-bench_bm25_13K) | [🦙 SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-Llama-7b) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.3 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.4 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -10,44 +10,45 @@
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: chardet Requires-Dist:
 datasets Requires-Dist: ghapi Requires-Dist: GitPython Requires-Dist: python-
 dotenv Requires-Dist: requests Requires-Dist: rich
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
-                                 SWE-bench) |
+     SWE-bench) | [ä¸­æç®ä½](docs/README_CN.md) | [ä¸­æç¹é«](docs/
+                                README_TW.md) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
       _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
-blob/master/CHANGELOG.md) for information on the latest updates to the SWE-
-bench benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
+blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
+benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
 language models on real world software issues collected from GitHub. Given a
 *codebase* and an *issue*, a language model is tasked with generating a *patch*
 that resolves the described problem. [assets/teaser.png]## ð Set Up To build
 SWE-bench from source, follow these steps: 1. Clone this repository locally 2.
 `cd` into the repository. 3. Run `conda env create -f environment.yml` to
 created a conda environment named `swe-bench` 4. Activate the environment with
 `conda activate swe-bench` ## ð½ Usage You can download the SWE-bench dataset
 directly ([dev](https://drive.google.com/
 uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
 drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
 or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 To use SWE-Bench, you can: * Train your own models on our pre-processed
 datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
-master/inference/) on existing models (either models you have on-disk like
-LLaMA, or models you have access to through an API like GPT-4). The inference
-step is where you get a repo and an issue and have the model try to generate a
-fix for it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/
-master/harness/) models against SWE-bench. This is where you take a SWE-Bench
-task and a model-proposed solution and evaluate its correctness. * Run SWE-
-bench's [data collection procedure](https://github.com/princeton-nlp/SWE-bench/
-blob/master/collect/) on your own repositories, to make new SWE-Bench tasks. ##
+main/inference/) on existing models (either models you have on-disk like LLaMA,
+or models you have access to through an API like GPT-4). The inference step is
+where you get a repo and an issue and have the model try to generate a fix for
+it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
+harness/) models against SWE-bench. This is where you take a SWE-Bench task and
+a model-proposed solution and evaluate its correctness. * Run SWE-bench's [data
+collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/
+swebench/collect/) on your own repositories, to make new SWE-Bench tasks. ##
 â¬ï¸ Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
 huggingface.co/datasets/princeton-nlp/SWE-bench) | [ð¦ SWE-Llama 13b](https:/
 /huggingface.co/princeton-nlp/SWE-Llama-13b) | | [ð¤ "Oracle" Retrieval]
 (https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [ð¦ SWE-
 Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) | |
 [ð¤ BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-
 bench_bm25_13K) | [ð¦ SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-
```

### Comparing `swebench-1.0.3/swebench.egg-info/SOURCES.txt` & `swebench-1.0.4/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

