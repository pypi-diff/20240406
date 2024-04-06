# Comparing `tmp/autogluon.core-1.0.1b20240404.tar.gz` & `tmp/autogluon.core-1.0.1b20240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-1.0.1b20240404.tar", last modified: Thu Apr  4 09:04:18 2024, max compression
+gzip compressed data, was "autogluon.core-1.0.1b20240405.tar", last modified: Fri Apr  5 09:04:03 2024, max compression
```

## Comparing `autogluon.core-1.0.1b20240404.tar` & `autogluon.core-1.0.1b20240405.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.546267 autogluon.core-1.0.1b20240404/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.546267 autogluon.core-1.0.1b20240404/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.550267 autogluon.core-1.0.1b20240404/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.550267 autogluon.core-1.0.1b20240404/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.554267 autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.554267 autogluon.core-1.0.1b20240404/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.554267 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21151 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.554267 autogluon.core-1.0.1b20240404/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.554267 autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.554267 autogluon.core-1.0.1b20240404/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    99982 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66393 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.558267 autogluon.core-1.0.1b20240404/src/autogluon/core/stacked_overfitting/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/stacked_overfitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   192108 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.562267 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    50729 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-04 09:03:55.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:04:18.550267 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:04:18.000000 autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.028976 autogluon.core-1.0.1b20240405/
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-05 09:04:03.028976 autogluon.core-1.0.1b20240405/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:04:03.028976 autogluon.core-1.0.1b20240405/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.012976 autogluon.core-1.0.1b20240405/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.012976 autogluon.core-1.0.1b20240405/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.016976 autogluon.core-1.0.1b20240405/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.016976 autogluon.core-1.0.1b20240405/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.016976 autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.016976 autogluon.core-1.0.1b20240405/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.016976 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99982 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66393 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.020976 autogluon.core-1.0.1b20240405/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.024976 autogluon.core-1.0.1b20240405/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.024976 autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.024976 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.024976 autogluon.core-1.0.1b20240405/src/autogluon/core/stacked_overfitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/stacked_overfitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.024976 autogluon.core-1.0.1b20240405/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193281 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.028976 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.028976 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.028976 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50695 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-05 09:03:41.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:04:03.016976 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:04:02.000000 autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-1.0.1b20240404/PKG-INFO` & `autogluon.core-1.0.1b20240405/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.0.1b20240404
+Version: 1.0.1b20240405
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-1.0.1b20240404/setup.py` & `autogluon.core-1.0.1b20240405/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,20 +44,18 @@
         f"{ag.PACKAGE_NAME}.common=={version}",
     ]
 )
 
 
 extras_require = {
     "ray": [
-        # TODO: remove this once ray release the support on windows and Python 3.11
-        "ray[default]>=2.6.3,<2.7; sys_platform != 'win32' or python_version < '3.11'",
+        "ray[default]>=2.10.0,<2.11",  # sync with common/src/autogluon/common/utils/try_import.py
     ],
     "raytune": [
-        # TODO: remove this once ray release the support on windows and Python 3.11
-        "ray[default,tune]>=2.6.3,<2.7; sys_platform != 'win32' or python_version < '3.11'",
+        "ray[default,tune]>=2.10.0,<2.11",  # sync with common/src/autogluon/common/utils/try_import.py
         # TODO: consider alternatives as hyperopt is not actively maintained.
         "hyperopt>=0.2.7,<0.2.8",  # This is needed for the bayes search to work.
         # 'GPy>=1.10.0,<1.11.0'  # TODO: Enable this once PBT/PB2 are supported by ray lightning
     ],
 }
 
 tests_require = [
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/_setup_utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/constants.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/data/cleaner.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/dataset.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/executors.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         run_config_kwargs = dict()
     tuner = tune.Tuner(
         tune.with_resources(tune.with_parameters(trainable, **trainable_args), resources_per_trial),
         param_space=search_space,
         tune_config=tune.TuneConfig(
             num_samples=num_samples, search_alg=searcher, scheduler=scheduler, metric=metric, mode=mode, time_budget_s=time_budget_s, **tune_config_kwargs
         ),
-        run_config=air.RunConfig(name=os.path.basename(save_dir), local_dir=os.path.dirname(save_dir), verbose=verbose, **run_config_kwargs),
+        run_config=air.RunConfig(name=os.path.basename(save_dir), storage_path=os.path.dirname(save_dir), verbose=verbose, **run_config_kwargs),
         _tuner_kwargs={"trial_name_creator": _trial_name_creator, "trial_dirname_creator": _trial_dirname_creator},
     )
     results = tuner.fit()
 
     os.chdir(original_path)  # go back to the original directory to avoid relative path being broken
     return results._experiment_analysis
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/__init__.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/_utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/abstract/model_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 def init_model(args, model_cls, init_params, backend, is_bagged_model=False):
     args = args.copy()
 
     if backend == CUSTOM_BACKEND:
         task_id = args.pop("task_id")
         file_prefix = f"T{task_id+1}"  # append to all file names created during this trial. Do NOT change!
     elif backend == RAY_BACKEND:
-        from ray import tune
+        from ray import train
 
-        task_id = tune.get_trial_id()
+        task_id = train.get_context().get_trial_id()
         file_prefix = task_id
     else:
         raise ValueError(f"Invalid backend: {backend}. Valid options are [{CUSTOM_BACKEND}, {RAY_BACKEND}]")
 
     if is_bagged_model:
         if "model_base_kwargs" not in init_params:
             init_params["model_base_kwargs"] = {}
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
+
 import logging
 import time
 from collections import Counter
+from typing import List
 
 import numpy as np
+import pandas as pd
 
 from ...constants import PROBLEM_TYPES
 from ...metrics import log_loss
 from ...utils import compute_weighted_metric, get_pred_from_proba
 
 logger = logging.getLogger(__name__)
 
@@ -31,33 +35,35 @@
         self,
         ensemble_size: int,
         problem_type: str,
         metric,
         sorted_initialization: bool = False,
         bagging: bool = False,
         tie_breaker: str = "random",
+        subsample_size: int | None = None,
         random_state: np.random.RandomState = None,
         **kwargs,
     ):
         self.ensemble_size = ensemble_size
         self.problem_type = problem_type
         self.metric = metric
         self.sorted_initialization = sorted_initialization
         self.bagging = bagging
         self.use_best = True
         if tie_breaker not in ["random", "second_metric"]:
             raise ValueError(f"Unknown tie_breaker value: {tie_breaker}. Must be one of: ['random', 'second_metric']")
         self.tie_breaker = tie_breaker
+        self.subsample_size = subsample_size
         if random_state is not None:
             self.random_state = random_state
         else:
             self.random_state = np.random.RandomState(seed=0)
         self.quantile_levels = kwargs.get("quantile_levels", None)
 
-    def fit(self, predictions, labels, time_limit=None, identifiers=None, sample_weight=None):
+    def fit(self, predictions: List[np.ndarray], labels: np.ndarray, time_limit=None, identifiers=None, sample_weight=None):
         self.ensemble_size = int(self.ensemble_size)
         if self.ensemble_size < 1:
             raise ValueError("Ensemble size cannot be less than one!")
         if not self.problem_type in PROBLEM_TYPES:
             raise ValueError("Unknown problem type %s." % self.problem_type)
         # if not isinstance(self.metric, Scorer):
         #     raise ValueError('Metric must be of type scorer')
@@ -65,21 +71,31 @@
         self._fit(predictions=predictions, labels=labels, time_limit=time_limit, sample_weight=sample_weight)
         self._calculate_weights()
         logger.log(15, "Ensemble weights: ")
         logger.log(15, self.weights_)
         return self
 
     # TODO: Consider having a removal stage, remove each model and see if score is affected, if improves or not effected, remove it.
-    def _fit(self, predictions, labels, time_limit=None, sample_weight=None):
+    def _fit(self, predictions: List[np.ndarray], labels: np.ndarray, time_limit=None, sample_weight=None):
         ensemble_size = self.ensemble_size
+        if isinstance(labels, pd.Series):
+            labels = labels.values
         self.num_input_models_ = len(predictions)
         ensemble = []
         trajectory = []
         order = []
         used_models = set()
+        num_samples_total = len(labels)
+
+        if self.subsample_size is not None and self.subsample_size < num_samples_total:
+            logger.log(15, f"Subsampling to {self.subsample_size} samples to speedup ensemble selection...")
+            subsample_indices = self.random_state.choice(num_samples_total, self.subsample_size, replace=False)
+            labels = labels[subsample_indices]
+            for i in range(self.num_input_models_):
+                predictions[i] = predictions[i][subsample_indices]
 
         # if self.sorted_initialization:
         #     n_best = 20
         #     indices = self._sorted_initialization(predictions, labels, n_best)
         #     for idx in indices:
         #         ensemble.append(predictions[idx])
         #         order.append(idx)
@@ -186,15 +202,15 @@
         else:
             self.indices_ = order
             self.trajectory_ = trajectory
             self.train_score_ = trajectory[-1]
 
         logger.debug("Ensemble indices: " + str(self.indices_))
 
-    def _calculate_regret(self, y_true, y_pred_proba, metric, sample_weight=None):
+    def _calculate_regret(self, y_true: np.ndarray, y_pred_proba: np.ndarray, metric, sample_weight=None):
         if metric.needs_pred or metric.needs_quantile:
             preds = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=self.problem_type)
         else:
             preds = y_pred_proba
         score = compute_weighted_metric(y_true, preds, metric, sample_weight, quantile_levels=self.quantile_levels)
         return metric._optimum - score
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
         super().__init__(**kwargs)
         self.model_base = model_base
         self.num_pred_cols_per_model = None
         self.base_model_names = base_model_names
         self.weights_ = None
 
     def _set_default_params(self):
-        default_params = {"ensemble_size": 100}
+        default_params = {
+            "ensemble_size": 25,  # TabRepo reports that values above 25 lead to no measurable improvement.
+            "subsample_size": 1000000,  # subsample to this many rows if training row count exceeds this value to speed up training
+        }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             drop_unique=False,
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/problem_type.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/stacked_overfitting/utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/stacked_overfitting/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1286,23 +1286,15 @@
                         reuse_first_fold = not model._bagged_mode
                 if not reuse_first_fold:
                     if isinstance(model, BaggedEnsembleModel):
                         can_refit_full = model._get_tags_child().get("can_refit_full", False)
                     else:
                         can_refit_full = model._get_tags().get("can_refit_full", False)
                     reuse_first_fold = not can_refit_full
-                if reuse_first_fold:
-                    # Perform fallback black-box refit logic that doesn't retrain.
-                    model_full = model.convert_to_refit_full_via_copy()
-                    # FIXME: validation time not correct for infer 1 batch time, needed to hack _is_refit=True to fix
-                    logger.log(20, f"Fitting model: {model_full.name} | Skipping fit via cloning parent ...")
-                    self._add_model(model_full, stack_name=REFIT_FULL_NAME, level=level, _is_refit=True)
-                    self.save_model(model_full)
-                    models_trained = [model_full.name]
-                else:
+                if not reuse_first_fold:
                     model_full = model.convert_to_refit_full_template()
                     # Mitigates situation where bagged models barely had enough memory and refit requires more. Worst case results in OOM, but this lowers chance of failure.
                     model_full._user_params_aux["max_memory_usage_ratio"] = model.params_aux["max_memory_usage_ratio"] * 1.15
                     # TODO: Do it for all models in the level at once to avoid repeated processing of data?
                     base_model_names = self.get_base_model_names(model_name)
                     # FIXME: Logs for inference speed (1 row) are incorrect because
                     #  parents are non-refit models in this sequence and later correct after logging.
@@ -1322,14 +1314,38 @@
                         feature_prune=False,
                         k_fold=0,
                         n_repeats=1,
                         ensemble_type=type(model),
                         refit_full=True,
                         **kwargs,
                     )
+                    if len(models_trained) == 0:
+                        reuse_first_fold = True
+                        logger.log(
+                            30,
+                            f"WARNING: Refit training failure detected for '{model_name}'... "
+                            f"Falling back to using first fold to avoid downstream exception."
+                            f"\n\tThis is likely due to an out-of-memory error or other memory related issue. "
+                            f"\n\tPlease create a GitHub issue if this was triggered from a non-memory related problem.",
+                        )
+                        if not model.params.get("save_bag_folds", True):
+                            raise AssertionError(
+                                f"Cannot avoid training failure during refit for '{model_name}' by falling back to "
+                                f"copying the first fold because it does not exist! (save_bag_folds=False)"
+                                f"\n\tPlease specify `save_bag_folds=True` in the `.fit` call to avoid this exception."
+                            )
+
+                if reuse_first_fold:
+                    # Perform fallback black-box refit logic that doesn't retrain.
+                    model_full = model.convert_to_refit_full_via_copy()
+                    # FIXME: validation time not correct for infer 1 batch time, needed to hack _is_refit=True to fix
+                    logger.log(20, f"Fitting model: {model_full.name} | Skipping fit via cloning parent ...")
+                    self._add_model(model_full, stack_name=REFIT_FULL_NAME, level=level, _is_refit=True)
+                    self.save_model(model_full)
+                    models_trained = [model_full.name]
                 if len(models_trained) == 1:
                     model_refit_map[model_name] = models_trained[0]
                 for model_trained in models_trained:
                     self._update_model_attr(
                         model_trained,
                         refit_full=True,
                         refit_full_parent=model_name,
@@ -3755,14 +3771,15 @@
         X: pd.DataFrame | None = None,
         y: np.array | None = None,
         metric: str | Scorer | None = None,
         model: str = "best",
         weights=None,
         decision_thresholds: int | List[float] = 50,
         verbose: bool = True,
+        **kwargs,
     ) -> float:
         # TODO: Docstring
         assert self.problem_type == BINARY, f'calibrate_decision_threshold is only available for `problem_type="{BINARY}"`'
 
         if metric is None:
             metric = self.eval_metric
         elif isinstance(metric, str):
@@ -3813,8 +3830,9 @@
         return calibrate_decision_threshold(
             y=y,
             y_pred_proba=y_pred_proba,
             metric=lambda y, y_pred: self._score_with_y_pred(y=y, y_pred=y_pred, weights=weights, metric=metric),
             decision_thresholds=decision_thresholds,
             metric_name=metric.name,
             verbose=verbose,
+            **kwargs,
         )
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/trainer/utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/decorators.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/files.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/plots.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/time.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,17 +286,17 @@
             decision_threshold = 0.5
         # Using > instead of >= to align with Pandas `.idxmax` logic which picks the left-most column during ties.
         # If this is not done, then predictions can be inconsistent when converting in binary classification from multiclass-form pred_proba and
         # binary-form pred_proba when the pred_proba is 0.5 for positive and negative classes.
         if len(y_pred_proba.shape) == 2:
             assert y_pred_proba.shape[1] == 2
             # Assume positive class is in 2nd position
-            y_pred = [1 if pred > decision_threshold else 0 for pred in y_pred_proba[:, 1]]
+            y_pred = (y_pred_proba[:, 1] > decision_threshold).astype(int)
         else:
-            y_pred = [1 if pred > decision_threshold else 0 for pred in y_pred_proba]
+            y_pred = (y_pred_proba > decision_threshold).astype(int)
     elif problem_type == REGRESSION:
         y_pred = y_pred_proba
     elif problem_type == QUANTILE:
         y_pred = y_pred_proba
     else:
         y_pred = []
         if not len(y_pred_proba) == 0:
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon/core/utils/version_utils.py` & `autogluon.core-1.0.1b20240405/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.0.1b20240404
+Version: 1.0.1b20240405
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-1.0.1b20240404/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-1.0.1b20240405/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

