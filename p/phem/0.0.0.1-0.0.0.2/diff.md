# Comparing `tmp/phem-0.0.0.1.tar.gz` & `tmp/phem-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phem-0.0.0.1.tar", last modified: Sat Apr  6 16:44:18 2024, max compression
+gzip compressed data, was "phem-0.0.0.2.tar", last modified: Sat Apr  6 17:16:19 2024, max compression
```

## Comparing `phem-0.0.0.1.tar` & `phem-0.0.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.819729 phem-0.0.0.1/
--rw-rw-rw-   0        0        0     1073 2024-04-06 14:22:03.000000 phem-0.0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4233 2024-04-06 16:44:18.819729 phem-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1944 2024-04-06 16:31:16.000000 phem-0.0.0.1/README.md
--rw-rw-rw-   0        0        0     3113 2024-04-06 16:44:13.000000 phem-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 16:44:18.820729 phem-0.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.791718 phem-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.794109 phem-0.0.0.1/src/phem/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.802626 phem-0.0.0.1/src/phem/application_utils/
--rw-rw-rw-   0        0        0     1319 2024-04-06 15:09:31.000000 phem-0.0.0.1/src/phem/application_utils/default_configurations.py
--rw-rw-rw-   0        0        0     4443 2024-04-06 16:13:14.000000 phem-0.0.0.1/src/phem/application_utils/methods_factories.py
--rw-rw-rw-   0        0        0     1795 2024-04-06 15:09:31.000000 phem-0.0.0.1/src/phem/application_utils/supported_metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.804625 phem-0.0.0.1/src/phem/base_utils/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.805626 phem-0.0.0.1/src/phem/base_utils/custom_metrics/
--rw-rw-rw-   0        0        0    27336 2024-04-06 14:22:18.000000 phem-0.0.0.1/src/phem/base_utils/custom_metrics/roc_auc.py
--rw-rw-rw-   0        0        0    10942 2024-04-06 14:54:04.000000 phem-0.0.0.1/src/phem/base_utils/diversity_metrics.py
--rw-rw-rw-   0        0        0     5263 2024-04-06 14:54:04.000000 phem-0.0.0.1/src/phem/base_utils/metrics.py
--rw-rw-rw-   0        0        0     1037 2024-04-06 16:31:16.000000 phem-0.0.0.1/src/phem/base_utils/preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.806626 phem-0.0.0.1/src/phem/framework/
--rw-rw-rw-   0        0        0    14216 2024-04-06 16:03:46.000000 phem-0.0.0.1/src/phem/framework/abstract_ensemble.py
--rw-rw-rw-   0        0        0     5434 2024-04-06 15:00:06.000000 phem-0.0.0.1/src/phem/framework/abstract_weighted_ensemble.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.794109 phem-0.0.0.1/src/phem/methods/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.807625 phem-0.0.0.1/src/phem/methods/baselines/
--rw-rw-rw-   0        0        0      134 2024-04-06 16:13:14.000000 phem-0.0.0.1/src/phem/methods/baselines/__init__.py
--rw-rw-rw-   0        0        0     3384 2024-04-06 15:00:06.000000 phem-0.0.0.1/src/phem/methods/baselines/single_best.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.809626 phem-0.0.0.1/src/phem/methods/ensemble_selection/
--rw-rw-rw-   0        0        0      171 2024-04-06 16:31:16.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/__init__.py
--rw-rw-rw-   0        0        0     9406 2024-04-06 15:00:06.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/greedy_ensemble_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.812729 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/
--rw-rw-rw-   0        0        0      436 2024-04-06 16:31:16.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.814729 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_functions/
--rw-rw-rw-   0        0        0      658 2024-04-06 15:40:00.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_functions/basic.py
--rw-rw-rw-   0        0        0     2428 2024-04-06 15:33:37.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_functions/implicit_diversity_metrics.py
--rw-rw-rw-   0        0        0     5937 2024-04-06 15:33:37.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_space.py
--rw-rw-rw-   0        0        0      994 2024-04-06 15:58:20.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_spaces.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.816728 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/
--rw-rw-rw-   0        0        0    14266 2024-04-06 15:33:37.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/custom_sliding_boundaries_archive.py
--rw-rw-rw-   0        0        0     2323 2024-04-06 15:33:37.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/quality_archive.py
--rw-rw-rw-   0        0        0     1713 2024-04-06 15:33:37.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/utils.py
--rw-rw-rw-   0        0        0    49733 2024-04-06 16:21:55.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/emitters.py
--rw-rw-rw-   0        0        0    31462 2024-04-06 16:21:55.000000 phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/qdo_es.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:44:18.816728 phem-0.0.0.1/src/phem.egg-info/
--rw-rw-rw-   0        0        0     4233 2024-04-06 16:44:18.000000 phem-0.0.0.1/src/phem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-04-06 16:44:18.000000 phem-0.0.0.1/src/phem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:44:18.000000 phem-0.0.0.1/src/phem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      543 2024-04-06 16:44:18.000000 phem-0.0.0.1/src/phem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-06 16:44:18.000000 phem-0.0.0.1/src/phem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.172092 phem-0.0.0.2/
+-rw-rw-rw-   0        0        0     1073 2024-04-06 14:22:03.000000 phem-0.0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     6163 2024-04-06 17:16:19.171086 phem-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2024-04-06 17:16:01.000000 phem-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0     3109 2024-04-06 17:16:15.000000 phem-0.0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 17:16:19.172092 phem-0.0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.143791 phem-0.0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.146793 phem-0.0.0.2/src/phem/
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.155473 phem-0.0.0.2/src/phem/application_utils/
+-rw-rw-rw-   0        0        0     1319 2024-04-06 15:09:31.000000 phem-0.0.0.2/src/phem/application_utils/default_configurations.py
+-rw-rw-rw-   0        0        0     4443 2024-04-06 16:13:14.000000 phem-0.0.0.2/src/phem/application_utils/methods_factories.py
+-rw-rw-rw-   0        0        0     1795 2024-04-06 15:09:31.000000 phem-0.0.0.2/src/phem/application_utils/supported_metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.157473 phem-0.0.0.2/src/phem/base_utils/
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.157473 phem-0.0.0.2/src/phem/base_utils/custom_metrics/
+-rw-rw-rw-   0        0        0    27336 2024-04-06 14:22:18.000000 phem-0.0.0.2/src/phem/base_utils/custom_metrics/roc_auc.py
+-rw-rw-rw-   0        0        0    10942 2024-04-06 14:54:04.000000 phem-0.0.0.2/src/phem/base_utils/diversity_metrics.py
+-rw-rw-rw-   0        0        0     5263 2024-04-06 14:54:04.000000 phem-0.0.0.2/src/phem/base_utils/metrics.py
+-rw-rw-rw-   0        0        0     1037 2024-04-06 16:31:16.000000 phem-0.0.0.2/src/phem/base_utils/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.159474 phem-0.0.0.2/src/phem/framework/
+-rw-rw-rw-   0        0        0    14216 2024-04-06 16:03:46.000000 phem-0.0.0.2/src/phem/framework/abstract_ensemble.py
+-rw-rw-rw-   0        0        0     5434 2024-04-06 15:00:06.000000 phem-0.0.0.2/src/phem/framework/abstract_weighted_ensemble.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.146793 phem-0.0.0.2/src/phem/methods/
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.160473 phem-0.0.0.2/src/phem/methods/baselines/
+-rw-rw-rw-   0        0        0      134 2024-04-06 16:13:14.000000 phem-0.0.0.2/src/phem/methods/baselines/__init__.py
+-rw-rw-rw-   0        0        0     3384 2024-04-06 15:00:06.000000 phem-0.0.0.2/src/phem/methods/baselines/single_best.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.161579 phem-0.0.0.2/src/phem/methods/ensemble_selection/
+-rw-rw-rw-   0        0        0      171 2024-04-06 16:31:16.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/__init__.py
+-rw-rw-rw-   0        0        0     9405 2024-04-06 16:56:27.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/greedy_ensemble_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.164583 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/
+-rw-rw-rw-   0        0        0      436 2024-04-06 16:31:16.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.166579 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_functions/
+-rw-rw-rw-   0        0        0      658 2024-04-06 15:40:00.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_functions/basic.py
+-rw-rw-rw-   0        0        0     2428 2024-04-06 15:33:37.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_functions/implicit_diversity_metrics.py
+-rw-rw-rw-   0        0        0     5937 2024-04-06 15:33:37.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_space.py
+-rw-rw-rw-   0        0        0      994 2024-04-06 15:58:20.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_spaces.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.168580 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/
+-rw-rw-rw-   0        0        0    14266 2024-04-06 15:33:37.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/custom_sliding_boundaries_archive.py
+-rw-rw-rw-   0        0        0     2323 2024-04-06 15:33:37.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/quality_archive.py
+-rw-rw-rw-   0        0        0     1713 2024-04-06 15:33:37.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/utils.py
+-rw-rw-rw-   0        0        0    49733 2024-04-06 16:21:55.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/emitters.py
+-rw-rw-rw-   0        0        0    31462 2024-04-06 16:21:55.000000 phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/qdo_es.py
+drwxrwxrwx   0        0        0        0 2024-04-06 17:16:19.168580 phem-0.0.0.2/src/phem.egg-info/
+-rw-rw-rw-   0        0        0     6163 2024-04-06 17:16:19.000000 phem-0.0.0.2/src/phem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-04-06 17:16:19.000000 phem-0.0.0.2/src/phem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 17:16:19.000000 phem-0.0.0.2/src/phem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      539 2024-04-06 17:16:19.000000 phem-0.0.0.2/src/phem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-06 17:16:19.000000 phem-0.0.0.2/src/phem.egg-info/top_level.txt
```

### Comparing `phem-0.0.0.1/LICENSE.txt` & `phem-0.0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/pyproject.toml` & `phem-0.0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phem"
-version = "0.0.0.1"
+version = "0.0.0.2"
 authors = [
     { name = "Lennart Purucker", email = "contact@lennart-purucker.com" },
 ]
 description = "PHEM: A collection of Post Hoc Ensemble Methods for (Auto)ML"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -14,15 +14,15 @@
 ]
 dependencies = [
     "typing_extensions",
     "more_itertools",
     "assembled[openml]==0.0.4",
     "ConfigSpace==0.6.1",
     "scikit-learn",
-    "phem[all_methods]",
+    "phem[all-methods]",
 ]
 license = { file = "LICENSE" }
 
 [project.urls]
 source =  "https://github.com/LennartPurucker/phem"
 documentation = "https://github.com/LennartPurucker/phem/issues"
 
@@ -46,17 +46,17 @@
   "mike",
   "pillow",
   "cairosvg",
   "black",
 ]
 
 # Different methodss
-all_methods = ["phem[qdo_es, cma_es]"]
-qdo_es = ["ribs==0.4.0"]
-cma_es = ["cma==3.2.2"]
+all-methods = ["phem[qdoes, cmaes]"]
+qdoes = ["ribs==0.4.0"]
+cmaes = ["cma==3.2.2"]
 
 [tool.ruff]
 target-version = "py310"
 line-length = 100
 output-format = "full"
 src = ["src", "tests", "examples"]
```

### Comparing `phem-0.0.0.1/src/phem/application_utils/default_configurations.py` & `phem-0.0.0.2/src/phem/application_utils/default_configurations.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/application_utils/methods_factories.py` & `phem-0.0.0.2/src/phem/application_utils/methods_factories.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/application_utils/supported_metrics.py` & `phem-0.0.0.2/src/phem/application_utils/supported_metrics.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/base_utils/custom_metrics/roc_auc.py` & `phem-0.0.0.2/src/phem/base_utils/custom_metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/base_utils/diversity_metrics.py` & `phem-0.0.0.2/src/phem/base_utils/diversity_metrics.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/base_utils/metrics.py` & `phem-0.0.0.2/src/phem/base_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/base_utils/preprocessing.py` & `phem-0.0.0.2/src/phem/base_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/framework/abstract_ensemble.py` & `phem-0.0.0.2/src/phem/framework/abstract_ensemble.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/framework/abstract_weighted_ensemble.py` & `phem-0.0.0.2/src/phem/framework/abstract_weighted_ensemble.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/baselines/single_best.py` & `phem-0.0.0.2/src/phem/methods/baselines/single_best.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/greedy_ensemble_selection.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/greedy_ensemble_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                           different results, even with the same object.
     use_best: bool = True
         After finishing all iterations, use the best found ensemble instead of the last found ensemble.
     """
 
     def __init__(self, base_models: list[Callable], n_iterations: int, metric: AbstractMetric, n_jobs: int = -1,
                  random_state: int | np.random.RandomState | None = None,
-                 use_best: bool = False) -> None:
+                 use_best: bool = True) -> None:
         #base_models = base_models[:20]
 
         super().__init__(base_models, "predict_proba")
         self.ensemble_size = n_iterations
         self.metric = metric
         self.use_best = use_best
```

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_functions/basic.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_functions/basic.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_functions/implicit_diversity_metrics.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_functions/implicit_diversity_metrics.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_space.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_space.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/behavior_spaces.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/behavior_spaces.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/custom_sliding_boundaries_archive.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/custom_sliding_boundaries_archive.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/quality_archive.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/quality_archive.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/custom_archives/utils.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/custom_archives/utils.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/emitters.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/emitters.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem/methods/ensemble_selection/qdo/qdo_es.py` & `phem-0.0.0.2/src/phem/methods/ensemble_selection/qdo/qdo_es.py`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem.egg-info/SOURCES.txt` & `phem-0.0.0.2/src/phem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phem-0.0.0.1/src/phem.egg-info/requires.txt` & `phem-0.0.0.2/src/phem.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 typing_extensions
 more_itertools
 assembled[openml]==0.0.4
 ConfigSpace==0.6.1
 scikit-learn
-phem[all_methods]
+phem[all-methods]
 
-[all_methods]
-phem[cma_es,qdo_es]
+[all-methods]
+phem[cmaes,qdoes]
 
-[cma_es]
+[cmaes]
 cma==3.2.2
 
 [dev]
 phem[doc,examples,test,tooling]
 
 [doc]
 mkdocs
@@ -29,15 +29,15 @@
 pillow
 cairosvg
 black
 
 [examples]
 openml
 
-[qdo_es]
+[qdoes]
 ribs==0.4.0
 
 [test]
 pytest<8
 pytest-coverage
 pytest-cases
```

