# Comparing `tmp/mloptimizer-0.8.4.tar.gz` & `tmp/mloptimizer-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mloptimizer-0.8.4.tar", last modified: Mon Apr  1 22:30:06 2024, max compression
+gzip compressed data, was "mloptimizer-0.8.5.tar", last modified: Sat Apr  6 16:14:07 2024, max compression
```

## Comparing `mloptimizer-0.8.4.tar` & `mloptimizer-0.8.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.734282 mloptimizer-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-01 22:30:06.734282 mloptimizer-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.718282 mloptimizer-0.8.4/mloptimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.722282 mloptimizer-0.8.4/mloptimizer/aux/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.722282 mloptimizer-0.8.4/mloptimizer/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/SVC_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/default_hyperparameter_spaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.722282 mloptimizer-0.8.4/mloptimizer/core/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/core/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/evaluation/model_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/genetic/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/deapoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/garunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/individual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/hyperparams/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/hyperparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/hyperparams/hyperparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/hyperparams/hyperspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_aux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_CustomXGBClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_evaluation/test_model_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:30:06.734282 mloptimizer-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.848642 mloptimizer-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-06 16:14:07.848642 mloptimizer-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.836642 mloptimizer-0.8.5/mloptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.836642 mloptimizer-0.8.5/mloptimizer/aux/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/aux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/aux/alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/aux/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/aux/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/aux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/SVC_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/conf/default_hyperparameter_spaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/core/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/evaluation/model_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/genetic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/genetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/genetic/deapoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/genetic/garunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/genetic/individual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/hyperparams/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/hyperparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/hyperparams/hyperparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/hyperparams/hyperspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/test/test_aux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_aux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_aux/test_CustomXGBClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_aux/test_alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_aux/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_aux/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.840642 mloptimizer-0.8.5/mloptimizer/test/test_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_evaluation/test_model_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.844642 mloptimizer-0.8.5/mloptimizer/test/test_genoptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_genoptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_genoptimizer/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.844642 mloptimizer-0.8.5/mloptimizer/test/test_hyperparams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_hyperparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_hyperparams/test_hyperparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/mloptimizer/test/test_hyperparams/test_hyperspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:14:07.844642 mloptimizer-0.8.5/mloptimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-06 16:14:07.000000 mloptimizer-0.8.5/mloptimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-06 16:14:07.000000 mloptimizer-0.8.5/mloptimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:14:07.000000 mloptimizer-0.8.5/mloptimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-06 16:14:07.000000 mloptimizer-0.8.5/mloptimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:14:07.000000 mloptimizer-0.8.5/mloptimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:14:07.848642 mloptimizer-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-04-06 16:14:04.000000 mloptimizer-0.8.5/setup.py
```

### Comparing `mloptimizer-0.8.4/LICENSE` & `mloptimizer-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/PKG-INFO` & `mloptimizer-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.8.4
+Version: 0.8.5
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini López, Javier Arroyo Gallardo
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10, <4
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: catboost>=1.1.1
 Requires-Dist: deap>=1.3.3
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: python-dateutil>=2.8.1
@@ -24,14 +28,15 @@
 Requires-Dist: scikit-learn>=1.2.1
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: six>=1.15.0
 Requires-Dist: xgboost>=1.7.3
 Requires-Dist: plotly>=5.15.0
 Requires-Dist: kaleido
+Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: catboost>=1.1.1; extra == "dev"
 Requires-Dist: deap>=1.3.3; extra == "dev"
 Requires-Dist: joblib>=1.2.0; extra == "dev"
 Requires-Dist: keras==2.12.0; extra == "dev"
 Requires-Dist: pandas>=1.5.3; extra == "dev"
 Requires-Dist: python-dateutil>=2.8.1; extra == "dev"
@@ -48,14 +53,15 @@
 Requires-Dist: sphinx-gallery==0.14.0; extra == "dev"
 Requires-Dist: sphinx_book_theme; extra == "dev"
 Requires-Dist: sphinx_mdinclude; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: sphinx-favicon; extra == "dev"
 Requires-Dist: mlflow; extra == "dev"
 Requires-Dist: sphinxcontrib-mermaid; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: catboost>=1.1.1; extra == "docs"
 Requires-Dist: deap>=1.3.3; extra == "docs"
 Requires-Dist: joblib>=1.2.0; extra == "docs"
 Requires-Dist: keras==2.12.0; extra == "docs"
 Requires-Dist: pandas>=1.5.3; extra == "docs"
 Requires-Dist: python-dateutil>=2.8.1; extra == "docs"
@@ -71,14 +77,15 @@
 Requires-Dist: kaleido; extra == "docs"
 Requires-Dist: sphinx-gallery==0.14.0; extra == "docs"
 Requires-Dist: sphinx_book_theme; extra == "docs"
 Requires-Dist: sphinx_mdinclude; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
 Requires-Dist: sphinx-favicon; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid; extra == "docs"
+Requires-Dist: tqdm; extra == "docs"
 
 ![mloptimizer_banner](https://raw.githubusercontent.com/Caparrini/mloptimizer-static/main/logos/mloptimizer_banner_readme.png)
 
 [![Documentation Status](https://readthedocs.org/projects/mloptimizer/badge/?version=master)](https://mloptimizer.readthedocs.io/en/master/?badge=master)
 [![PyPI version](https://badge.fury.io/py/mloptimizer.svg)](https://badge.fury.io/py/mloptimizer)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mloptimizer.svg)](https://pypi.python.org/pypi/mloptimizer/)
 [![Tests](https://github.com/Caparrini/mloptimizer/actions/workflows/CI.yml/badge.svg)](https://github.com/Caparrini/mloptimizer/actions/workflows/CI.yml)
```

### Comparing `mloptimizer-0.8.4/README.md` & `mloptimizer-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/aux/alg_wrapper.py` & `mloptimizer-0.8.5/mloptimizer/aux/alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/aux/plots.py` & `mloptimizer-0.8.5/mloptimizer/aux/plots.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/aux/tracker.py` & `mloptimizer-0.8.5/mloptimizer/aux/tracker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from mloptimizer.aux.utils import create_optimization_folder, init_logger
 import os
 import shutil
 from datetime import datetime
 import importlib
 import joblib
 import pandas as pd
+import tqdm
 
 
 class Tracker:
     """
     Tracker class for logging and tracking the optimization process.
 
     Parameters
@@ -19,15 +20,16 @@
         Folder where the optimization process will be stored.
     log_file : str
         Name of the log file.
     use_mlflow : bool
         If True, the optimization process will be tracked using MLFlow.
     """
 
-    def __init__(self, name, folder=os.curdir, log_file="mloptimizer.log", use_mlflow=False):
+    def __init__(self, name, folder=os.curdir, log_file="mloptimizer.log", use_mlflow=False,
+                 use_parallel=False):
 
         self.name = name
         self.gen = 0
         # Main folder, current by default
         self.folder = create_optimization_folder(folder)
         # Log files
         self.mloptimizer_logger, self.log_file = init_logger(log_file, self.folder)
@@ -37,34 +39,46 @@
         self.opt_run_folder = None
         self.opt_run_checkpoint_path = None
         self.progress_path = None
         self.progress_path = None
         self.results_path = None
         self.graphics_path = None
 
+        # tqdm is not compatible with parallel execution
+        self.use_parallel = use_parallel
+
+        if not self.use_parallel:
+            self.gen_pbar = None
+
         # MLFlow
         self.use_mlflow = use_mlflow
 
         if self.use_mlflow:
             self.mlflow = importlib.import_module("mlflow")
 
-    def start_optimization(self, opt_class):
+    def start_optimization(self, opt_class, generations: int):
         """
         Start the optimization process.
 
         Parameters
         ----------
         opt_class : str
             Name of the optimization class.
+        generations : int
+            Number of generations for the optimization process.
         """
         # Inform the user that the optimization is starting
         self.mloptimizer_logger.info(f"Initiating genetic optimization...")
         # self.mloptimizer_logger.info("Algorithm: {}".format(type(self).__name__))
         self.mloptimizer_logger.info(f"Algorithm: {opt_class}")
 
+        # tqdm is not compatible with parallel execution
+        if not self.use_parallel:
+            self._init_progress_bar(generations)
+
     def start_checkpoint(self, opt_run_folder_name):
         """
         Start a checkpoint for the optimization process.
 
         Parameters
         ----------
         opt_run_folder_name : str
@@ -102,15 +116,15 @@
             self.optimization_logger.info(f"Generation {generation} - Classifier TOP {i}")
             self.optimization_logger.info(f"Classifier: {classifiers_list[i]}")
             self.optimization_logger.info(f"Fitness: {fitness_list[i]}")
             self.optimization_logger.info("Hyperparams: {}".format(str(classifiers_list[i].get_params())))
         self.gen = generation + 1
 
     def log_evaluation(self, classifier, metrics):
-        self.optimization_logger.info(f"Adding to mlflow...\nClassifier: {classifier}\nMetrics: {metrics}")
+        self.optimization_logger.debug(f"Adding to mlflow...\nClassifier: {classifier}\nMetrics: {metrics}")
 
         if self.use_mlflow:
             with self.mlflow.start_run():
                 self.mlflow.log_params(classifier.get_params())
                 # We use the generation as the step
                 # self.mlflow.log_metric(key="fitness", value=metric, step=self.gen)
                 self.mlflow.log_metrics(metrics, step=self.gen)
@@ -118,15 +132,15 @@
     def load_checkpoint(self, checkpoint):
 
         # Extract checkpoint_path from checkpoint file
         self.opt_run_checkpoint_path = os.path.dirname(checkpoint)
         self.opt_run_folder = os.path.dirname(self.opt_run_checkpoint_path)
         self.optimization_logger, _ = init_logger(os.path.join(self.opt_run_folder,
                                                                f"opt_{os.path.basename(checkpoint)}.log"))
-        self.optimization_logger.info("Initiating from checkpoint {}...".format(checkpoint))
+        self.optimization_logger.debug("Initiating from checkpoint {}...".format(checkpoint))
 
         self.results_path = os.path.join(self.opt_run_folder, "results")
         self.graphics_path = os.path.join(self.opt_run_folder, "graphics")
         self.progress_path = os.path.join(self.opt_run_folder, "progress")
         cp = joblib.load(checkpoint)
         return cp
 
@@ -141,42 +155,55 @@
         filename : str, optional (default=None)
             filename to save the logbook
         """
         if filename is None:
             filename = os.path.join(self.results_path, 'logbook.csv')
         pd.DataFrame(logbook).to_csv(filename, index=False)
 
-    def write_population_file(self, populations, filename=None):
+    def write_population_file(self, populations: pd.DataFrame, filename=None):
         """
         Method to write the population to a csv file
 
         Parameters
         ----------
+        populations: pd.DataFrame
+            population of the optimization process
         filename : str, optional (default=None)
             filename to save the population
         """
         if filename is None:
             filename = os.path.join(self.results_path, 'populations.csv')
         populations.sort_values(by=['fitness'], ascending=False
                                 ).to_csv(filename, index=False)
 
     def start_progress_file(self, gen: int):
+        # tqdm is not compatible with parallel execution
+        if not self.use_parallel:
+            self.gen_pbar.update()
         progress_gen_path = os.path.join(self.progress_path, "Generation_{}.csv".format(gen))
         header_progress_gen_file = "i;total;Individual;fitness\n"
         with open(progress_gen_path, "w") as progress_gen_file:
             progress_gen_file.write(header_progress_gen_file)
             progress_gen_file.close()
-        self.optimization_logger.info("Generation: {}".format(gen))
+        self.optimization_logger.debug("Generation: {}".format(gen))
 
-    def append_progress_file(self, gen, c, evaluations_pending, ind_formatted, fit):
-        self.optimization_logger.info(
+        # self.pbar.refresh()
+
+    def append_progress_file(self, gen: int, ngen: int, c: int, evaluations_pending: int, ind_formatted, fit):
+        self.optimization_logger.debug(
             "Fitting individual (informational purpose): gen {} - ind {} of {}".format(
                 gen, c, evaluations_pending
             )
         )
         progress_gen_path = os.path.join(self.progress_path, "Generation_{}.csv".format(gen))
         with open(progress_gen_path, "a") as progress_gen_file:
             progress_gen_file.write(
                 "{};{};{};{}\n".format(c,
                                        evaluations_pending,
                                        ind_formatted, fit)
             )
+        if not self.use_parallel and gen == ngen and c == evaluations_pending:
+            self.gen_pbar.close()
+
+    def _init_progress_bar(self, n_generations, msg="Genetic execution"):
+        self.gen_pbar = tqdm.tqdm(desc=msg, total=n_generations+1)
+        # self.pbar.refresh()
```

### Comparing `mloptimizer-0.8.4/mloptimizer/aux/utils.py` & `mloptimizer-0.8.5/mloptimizer/aux/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,63 @@
 import logging
 import os
-from logging import FileHandler
-from logging import Formatter
 
 
-def init_logger(filename='mloptimizer.log', log_path="."):
+def init_logger(filename='mloptimizer.log', log_path=".", debug=False):
     """
     Initializes a logger and returns it.
 
     Parameters
     ----------
     filename : str, optional
         The name of the log file. The default is 'mloptimizer.log'.
     log_path : str, optional
         The path of the log file. The default is ".".
-
+    debug : bool, optional
+        Activate debug level. The default is False.
     Returns
     -------
     custom_logger : logging.Logger
         The logger.
     """
-    filename = os.path.join(log_path, filename)
-    log_format = (
-        "%(asctime)s [%(levelname)s]: %(message)s in %(pathname)s:%(lineno)d")
+    # Some logger variables
+    logfile_path = os.path.join(log_path, filename)
+
     log_level = logging.INFO
+
+    if debug:
+        log_level = logging.DEBUG
+
+    # Create a custom logger
     custom_logger = logging.getLogger(filename)
     custom_logger.setLevel(log_level)
-    custom_logger_file_handler = FileHandler(filename)
-    custom_logger_file_handler.setLevel(log_level)
-    custom_logger_file_handler.setFormatter(Formatter(log_format))
-    custom_logger.addHandler(custom_logger_file_handler)
+
+    # Create logger formatter
+    log_format = (
+        "%(asctime)s [%(levelname)s]: %(message)s in %(pathname)s:%(lineno)d")
+    logger_formatter = logging.Formatter(log_format)
+
+    # Create handler for the logger
+    file_handler = logging.FileHandler(logfile_path)
+    file_handler.setLevel(logging.DEBUG)
+    file_handler.setFormatter(logger_formatter)
+
+    console_handler = logging.StreamHandler()
+    console_handler.setLevel(logging.CRITICAL)
+    console_handler.setFormatter(logger_formatter)
+
+    # Add the handler to the logger
+    custom_logger.addHandler(file_handler)
+    custom_logger.addHandler(console_handler)
+
+    # custom_logger.propagate = False
+
+    # Logger configured
     custom_logger.debug("Logger configured")
-    return custom_logger, filename
+    return custom_logger, logfile_path
 
 
 def create_optimization_folder(folder):
     """
     Creates a folder to save the results of the optimization.
 
     Parameters
@@ -47,11 +69,11 @@
     -------
     folder : str
         The path of the folder created.
     """
     if os.path.exists(folder):
         logging.warning("The folder {} already exists and it will be used".format(folder))
     elif os.makedirs(folder, exist_ok=True):
-        logging.info("The folder {} has been created.".format(folder))
+        logging.warning("The folder {} has been created.".format(folder))
     else:
         logging.error("The folder {} could not be created.".format(folder))
     return folder
```

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/SVC_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/SVC_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.5/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/conf/default_hyperparameter_spaces.json` & `mloptimizer-0.8.5/mloptimizer/conf/default_hyperparameter_spaces.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/core/base.py` & `mloptimizer-0.8.5/mloptimizer/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         seed for the random functions
     use_parallel : bool
         flag to use parallel processing
     use_mlflow : bool
         flag to use mlflow
     """
 
-    def __init__(self, estimator_class, features: np.array, labels: np.array, folder=os.curdir, log_file="mloptimizer.log",
+    def __init__(self, estimator_class, features: np.array, labels: np.array,
+                 folder=os.curdir, log_file="mloptimizer.log",
                  hyperparam_space: HyperparameterSpace = None,
                  eval_function=train_score,
                  fitness_score="accuracy", metrics=None, seed=random.randint(0, 1000000),
                  use_parallel=False, use_mlflow=False):
         """
         Creates object BaseOptimizer.
 
@@ -97,15 +98,16 @@
         # Parallel
         self.use_parallel = use_parallel
 
         # mlflow
         self.use_mlflow = use_mlflow
 
         # Tracker
-        self.tracker = Tracker(name="mloptimizer", folder=folder, log_file=log_file, use_mlflow=self.use_mlflow)
+        self.tracker = Tracker(name="mloptimizer", folder=folder, log_file=log_file, use_mlflow=self.use_mlflow,
+                               use_parallel=self.use_parallel)
 
         # Evaluator
         self.individual_utils = IndividualUtils(hyperparam_space=self.hyperparam_space,
                                                 estimator_class=self.estimator_class, mlopt_seed=self.mlopt_seed)
         self.evaluator = Evaluator(features=features, labels=labels,
                                    eval_function=eval_function, fitness_score=fitness_score,
                                    metrics=metrics, tracker=self.tracker,
@@ -185,15 +187,15 @@
 
         Returns
         -------
         clf : classifier
             classifier with the best hyperparams
         """
         # Log initialization
-        self.tracker.start_optimization(type(self).__name__)
+        self.tracker.start_optimization(type(self).__name__, generations=generations)
 
         # Creation of folders and checkpoint
         self.tracker.start_checkpoint(opt_run_folder_name)
 
         # Creation of deap optimizer
         self.deap_optimizer = DeapOptimizer(hyperparam_space=self.hyperparam_space, seed=self.mlopt_seed,
                                             use_parallel=self.use_parallel)
```

### Comparing `mloptimizer-0.8.4/mloptimizer/core/keras.py` & `mloptimizer-0.8.5/mloptimizer/core/keras.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/evaluation/evaluator.py` & `mloptimizer-0.8.5/mloptimizer/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/evaluation/model_evaluation.py` & `mloptimizer-0.8.5/mloptimizer/evaluation/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/genetic/deapoptimizer.py` & `mloptimizer-0.8.5/mloptimizer/genetic/deapoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/genetic/garunner.py` & `mloptimizer-0.8.5/mloptimizer/genetic/garunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,25 +268,25 @@
             invalid_ind = [ind for ind in population if not ind.fitness.valid]
             fitnesses = toolbox.map(toolbox.evaluate, invalid_ind)
             c = 1
             evaluations_pending = len(invalid_ind)
             for ind, fit in zip(invalid_ind, fitnesses):
                 ind.fitness.values = fit
                 ind_formatted = self.deap_optimizer.individual2dict(ind)
-                self.tracker.append_progress_file(gen, c, evaluations_pending, ind_formatted, fit)
+                self.tracker.append_progress_file(gen, ngen, c, evaluations_pending, ind_formatted, fit)
 
                 c = c + 1
 
             halloffame.update(population)
 
             record = stats.compile(population) if stats else {}
 
             logbook.record(gen=gen, nevals=len(invalid_ind), **record)
-            if verbose:
-                self.tracker.optimization_logger.info(logbook.stream)
+            # if verbose:
+            #    self.tracker.optimization_logger.info(logbook.stream)
 
             # Select the next generation individuals
             population = toolbox.select(population, len(population))
 
             # halloffame_classifiers = list(map(self.get_clf, halloffame[:2]))
             # halloffame_fitness = [ind.fitness.values[:] for ind in halloffame[:2]]
             # self.tracker.log_clfs(classifiers_list=halloffame_classifiers, generation=gen,
```

### Comparing `mloptimizer-0.8.4/mloptimizer/genetic/individual.py` & `mloptimizer-0.8.5/mloptimizer/genetic/individual.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/hyperparams/hyperparam.py` & `mloptimizer-0.8.5/mloptimizer/hyperparams/hyperparam.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/hyperparams/hyperspace.py` & `mloptimizer-0.8.5/mloptimizer/hyperparams/hyperspace.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_CustomXGBClassifier.py` & `mloptimizer-0.8.5/mloptimizer/test/test_aux/test_CustomXGBClassifier.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_alg_wrapper.py` & `mloptimizer-0.8.5/mloptimizer/test/test_aux/test_alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_plots.py` & `mloptimizer-0.8.5/mloptimizer/test/test_aux/test_plots.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_utils.py` & `mloptimizer-0.8.5/mloptimizer/test/test_aux/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from mloptimizer.aux.utils import init_logger, create_optimization_folder
 
 
 def test_init_logger(tmp_path):
     # Create a temporary path for testing
     log_file = 'test.log'
     log_path = str(tmp_path)
-    logger, filename = init_logger(log_file, log_path)
+    logger, logfile_path = init_logger(log_file, log_path)
 
     # Check if the logger file is created
-    assert os.path.isfile(filename), "Log file should be created"
+    assert os.path.isfile(logfile_path), "Log file should be created"
 
     # Check if the filename is correct
-    assert filename == os.path.join(log_path, log_file), "Logger filename should match"
+    assert logfile_path == os.path.join(log_path, log_file), "Logger filename should match"
 
 
 def test_create_optimization_folder(tmp_path):
     # Create a temporary path for testing
     folder_path = os.path.join(tmp_path, 'opt_folder')
 
     # Test creating a new folder
```

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_evaluation/test_model_evaluation.py` & `mloptimizer-0.8.5/mloptimizer/test/test_evaluation/test_model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/test_base.py` & `mloptimizer-0.8.5/mloptimizer/test/test_genoptimizer/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,30 +27,30 @@
         "accuracy": accuracy_score,
     }
 
 
 @pytest.mark.parametrize('estimator_class',
                          (DecisionTreeClassifier, RandomForestClassifier, ExtraTreesClassifier,
                           GradientBoostingClassifier, XGBClassifier, SVC))
-def test_sklearn_optimizer(estimator_class):
+def test_sklearn_optimizer(estimator_class, tmp_path):
     X, y = load_iris(return_X_y=True)
     evolvable_hyperparams = HyperparameterSpace.get_default_hyperparameter_space(estimator_class)
     mlopt = Optimizer(estimator_class=estimator_class,
                       hyperparam_space=evolvable_hyperparams,
-                      features=X, labels=y)
+                      features=X, labels=y, folder=tmp_path)
     mlopt.optimize_clf(5, 5)
     assert mlopt is not None
 
 
 @pytest.mark.parametrize('use_mlflow', [True, False])
-def test_mloptimizer(use_mlflow):
+def test_mloptimizer(use_mlflow, tmp_path):
     X, y = load_breast_cancer(return_X_y=True)
     mlopt = Optimizer(estimator_class=XGBClassifier,
                       hyperparam_space=HyperparameterSpace.get_default_hyperparameter_space(XGBClassifier),
-                      features=X, labels=y, use_mlflow=use_mlflow)
+                      features=X, labels=y, use_mlflow=use_mlflow, folder=tmp_path)
     mlopt.optimize_clf(5, 5)
     assert mlopt is not None
 
 
 def test_checkpoints():
     X, y = load_breast_cancer(return_X_y=True)
     mlopt = Optimizer(estimator_class=XGBClassifier,
@@ -68,53 +68,56 @@
                               )
     clf2 = mlopt2.optimize_clf(5, 5,
                                checkpoint=checkpoint)
     assert mlopt is not None
     assert str(clf) == str(clf2)
 
 
+
 @pytest.mark.parametrize('estimator_class',
                          (DecisionTreeClassifier, RandomForestClassifier, ExtraTreesClassifier,
                           GradientBoostingClassifier, XGBClassifier, SVC))
 @pytest.mark.parametrize('dataset',
                          (load_breast_cancer, load_iris))
-def test_optimizer(estimator_class, dataset, default_metrics_dict):
+def test_optimizer(estimator_class, dataset, default_metrics_dict, tmp_path):
     X, y = dataset(return_X_y=True)
     evolvable_hyperparams = HyperparameterSpace.get_default_hyperparameter_space(estimator_class)
     opt = Optimizer(features=X, labels=y, fitness_score="accuracy",
                     metrics=default_metrics_dict, estimator_class=estimator_class,
-                    hyperparam_space=evolvable_hyperparams)
+                    hyperparam_space=evolvable_hyperparams, folder=tmp_path)
     clf = opt.optimize_clf(2, 2)
     assert clf is not None
 
 
 @pytest.mark.parametrize('estimator_class',
                          (DecisionTreeClassifier, RandomForestClassifier, ExtraTreesClassifier,
                           GradientBoostingClassifier, SVC))
 @pytest.mark.parametrize('dataset',
                          (load_breast_cancer, load_iris))
-def test_optimizer_use_parallel(estimator_class, dataset, default_metrics_dict):
+def test_optimizer_use_parallel(estimator_class, dataset, default_metrics_dict, tmp_path):
     X, y = dataset(return_X_y=True)
     evolvable_hyperparams = HyperparameterSpace.get_default_hyperparameter_space(estimator_class)
     my_seed = 25
-    population = 50
+    population = 60
     generations = 4
 
     opt_with_parallel = Optimizer(features=X, labels=y, fitness_score="accuracy",
                                   metrics=default_metrics_dict,
                                   seed=my_seed, use_parallel=True,
-                                  hyperparam_space=evolvable_hyperparams, estimator_class=estimator_class)
+                                  hyperparam_space=evolvable_hyperparams, estimator_class=estimator_class,
+                                  folder=tmp_path)
 
     start_time_parallel = time.time()
     clf_with_parallel = opt_with_parallel.optimize_clf(population, generations)
     end_time_parallel = time.time()
 
     opt = Optimizer(features=X, labels=y, fitness_score="accuracy", metrics=default_metrics_dict,
                     seed=my_seed, use_parallel=False,
-                    hyperparam_space=evolvable_hyperparams, estimator_class=estimator_class)
+                    hyperparam_space=evolvable_hyperparams, estimator_class=estimator_class,
+                    folder=tmp_path)
 
     start_time = time.time()
     clf = opt.optimize_clf(population, generations)
     end_time = time.time()
 
     elapsed_time_parallel = end_time_parallel - start_time_parallel
     elapsed_time = end_time - start_time
@@ -127,28 +130,28 @@
     assert elapsed_time_parallel < elapsed_time
 
 
 @pytest.mark.parametrize('estimator_class',
                          (DecisionTreeClassifier, RandomForestClassifier, ExtraTreesClassifier,
                           GradientBoostingClassifier, XGBClassifier, SVC))
 @pytest.mark.parametrize('target_score', (kfold_score, train_score, train_test_score))
-def test_reproducibility(estimator_class, target_score, default_metrics_dict):
+def test_reproducibility(estimator_class, target_score, default_metrics_dict, tmp_path):
     X, y = load_iris(return_X_y=True)
     evolvable_hyperparams = HyperparameterSpace.get_default_hyperparameter_space(estimator_class)
     population = 2
     generations = 2
     seed = 25
     distinct_seed = 2
     optimizer1 = Optimizer(features=X, labels=y, fitness_score="accuracy", metrics=default_metrics_dict,
                            eval_function=target_score, seed=seed, estimator_class=estimator_class,
-                           hyperparam_space=evolvable_hyperparams)
+                           hyperparam_space=evolvable_hyperparams, folder=tmp_path)
     result1 = optimizer1.optimize_clf(population_size=population, generations=generations)
     optimizer2 = Optimizer(features=X, labels=y, fitness_score="accuracy", metrics=default_metrics_dict,
                            eval_function=target_score, seed=seed, estimator_class=estimator_class,
-                           hyperparam_space=evolvable_hyperparams)
+                           hyperparam_space=evolvable_hyperparams, folder=tmp_path)
     result2 = optimizer2.optimize_clf(population_size=population, generations=generations)
     optimizer3 = Optimizer(features=X, labels=y, fitness_score="accuracy", metrics=default_metrics_dict,
                            eval_function=target_score, seed=distinct_seed, estimator_class=estimator_class,
-                           hyperparam_space=evolvable_hyperparams)
+                           hyperparam_space=evolvable_hyperparams, folder=tmp_path)
     result3 = optimizer3.optimize_clf(population_size=population, generations=generations)
     assert str(result1) == str(result2)
     assert str(result1) != str(result3)
```

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperparam.py` & `mloptimizer-0.8.5/mloptimizer/test/test_hyperparams/test_hyperparam.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperspace.py` & `mloptimizer-0.8.5/mloptimizer/test/test_hyperparams/test_hyperspace.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer.egg-info/PKG-INFO` & `mloptimizer-0.8.5/mloptimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.8.4
+Version: 0.8.5
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini López, Javier Arroyo Gallardo
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10, <4
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: catboost>=1.1.1
 Requires-Dist: deap>=1.3.3
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: python-dateutil>=2.8.1
@@ -24,14 +28,15 @@
 Requires-Dist: scikit-learn>=1.2.1
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: seaborn==0.12.2
 Requires-Dist: six>=1.15.0
 Requires-Dist: xgboost>=1.7.3
 Requires-Dist: plotly>=5.15.0
 Requires-Dist: kaleido
+Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: catboost>=1.1.1; extra == "dev"
 Requires-Dist: deap>=1.3.3; extra == "dev"
 Requires-Dist: joblib>=1.2.0; extra == "dev"
 Requires-Dist: keras==2.12.0; extra == "dev"
 Requires-Dist: pandas>=1.5.3; extra == "dev"
 Requires-Dist: python-dateutil>=2.8.1; extra == "dev"
@@ -48,14 +53,15 @@
 Requires-Dist: sphinx-gallery==0.14.0; extra == "dev"
 Requires-Dist: sphinx_book_theme; extra == "dev"
 Requires-Dist: sphinx_mdinclude; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: sphinx-favicon; extra == "dev"
 Requires-Dist: mlflow; extra == "dev"
 Requires-Dist: sphinxcontrib-mermaid; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: catboost>=1.1.1; extra == "docs"
 Requires-Dist: deap>=1.3.3; extra == "docs"
 Requires-Dist: joblib>=1.2.0; extra == "docs"
 Requires-Dist: keras==2.12.0; extra == "docs"
 Requires-Dist: pandas>=1.5.3; extra == "docs"
 Requires-Dist: python-dateutil>=2.8.1; extra == "docs"
@@ -71,14 +77,15 @@
 Requires-Dist: kaleido; extra == "docs"
 Requires-Dist: sphinx-gallery==0.14.0; extra == "docs"
 Requires-Dist: sphinx_book_theme; extra == "docs"
 Requires-Dist: sphinx_mdinclude; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
 Requires-Dist: sphinx-favicon; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid; extra == "docs"
+Requires-Dist: tqdm; extra == "docs"
 
 ![mloptimizer_banner](https://raw.githubusercontent.com/Caparrini/mloptimizer-static/main/logos/mloptimizer_banner_readme.png)
 
 [![Documentation Status](https://readthedocs.org/projects/mloptimizer/badge/?version=master)](https://mloptimizer.readthedocs.io/en/master/?badge=master)
 [![PyPI version](https://badge.fury.io/py/mloptimizer.svg)](https://badge.fury.io/py/mloptimizer)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mloptimizer.svg)](https://pypi.python.org/pypi/mloptimizer/)
 [![Tests](https://github.com/Caparrini/mloptimizer/actions/workflows/CI.yml/badge.svg)](https://github.com/Caparrini/mloptimizer/actions/workflows/CI.yml)
```

### Comparing `mloptimizer-0.8.4/mloptimizer.egg-info/SOURCES.txt` & `mloptimizer-0.8.5/mloptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.4/mloptimizer.egg-info/requires.txt` & `mloptimizer-0.8.5/mloptimizer.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 scikit-learn>=1.2.1
 scipy>=1.10.0
 seaborn==0.12.2
 six>=1.15.0
 xgboost>=1.7.3
 plotly>=5.15.0
 kaleido
+tqdm
 
 [dev]
 catboost>=1.1.1
 deap>=1.3.3
 joblib>=1.2.0
 keras==2.12.0
 pandas>=1.5.3
@@ -32,14 +33,15 @@
 sphinx-gallery==0.14.0
 sphinx_book_theme
 sphinx_mdinclude
 sphinx-autoapi
 sphinx-favicon
 mlflow
 sphinxcontrib-mermaid
+tqdm
 
 [docs]
 catboost>=1.1.1
 deap>=1.3.3
 joblib>=1.2.0
 keras==2.12.0
 pandas>=1.5.3
@@ -56,7 +58,8 @@
 kaleido
 sphinx-gallery==0.14.0
 sphinx_book_theme
 sphinx_mdinclude
 sphinx-autoapi
 sphinx-favicon
 sphinxcontrib-mermaid
+tqdm
```

### Comparing `mloptimizer-0.8.4/setup.py` & `mloptimizer-0.8.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     name="mloptimizer",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.8.4",  # Required
+    version="0.8.5",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="mloptimizer is a Python library "
                 "for optimizing hyperparameters of machine learning algorithms using genetic algorithms.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
@@ -79,15 +79,19 @@
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
         # Pick your license as you wish
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
@@ -106,15 +110,15 @@
     #   py_modules=["my_module"],
     #
     packages=find_packages(),  # Required
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.10, <4",
+    python_requires=">=3.9, <3.12",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=read_requirements("requirements.txt"),
```

