# Comparing `tmp/autogluon.timeseries-1.0.1b20240405.tar.gz` & `tmp/autogluon.timeseries-1.0.1b20240406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.0.1b20240405.tar", last modified: Fri Apr  5 09:05:04 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.0.1b20240406.tar", last modified: Sat Apr  6 09:05:30 2024, max compression
```

## Comparing `autogluon.timeseries-1.0.1b20240405.tar` & `autogluon.timeseries-1.0.1b20240406.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.577087 autogluon.timeseries-1.0.1b20240405/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-05 09:05:04.577087 autogluon.timeseries-1.0.1b20240405/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:05:04.577087 autogluon.timeseries-1.0.1b20240405/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.565087 autogluon.timeseries-1.0.1b20240405/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.565087 autogluon.timeseries-1.0.1b20240405/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.569088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.569088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.569088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.569088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.569088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23009 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30834 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/chronos/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25546 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19217 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.573088 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    71538 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.577087 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52432 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.577087 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.577087 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-05 09:03:41.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:04.569088 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:05:04.000000 autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.616128 autogluon.timeseries-1.0.1b20240406/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.616128 autogluon.timeseries-1.0.1b20240406/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23391 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81011 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.624128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.628128 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-06 09:04:13.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:30.620128 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:05:30.000000 autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.0.1b20240405/PKG-INFO` & `autogluon.timeseries-1.0.1b20240406/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.0.1b20240405
+Version: 1.0.1b20240406
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.0.1b20240405/setup.py` & `autogluon.timeseries-1.0.1b20240406/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/learner.py`

 * *Files 23% similar despite different names*

```diff
@@ -194,22 +194,91 @@
         use_cache: bool = True,
     ) -> float:
         data = self.feature_generator.transform(data)
         return self.load_trainer().score(data=data, model=model, metric=metric, use_cache=use_cache)
 
     def evaluate(
         self,
-        data: Union[TimeSeriesDataFrame, pd.DataFrame, str],
+        data: TimeSeriesDataFrame,
         model: Optional[str] = None,
         metrics: Optional[Union[str, TimeSeriesScorer, List[Union[str, TimeSeriesScorer]]]] = None,
         use_cache: bool = True,
     ) -> Dict[str, float]:
         data = self.feature_generator.transform(data)
         return self.load_trainer().evaluate(data=data, model=model, metrics=metrics, use_cache=use_cache)
 
+    def get_feature_importance(
+        self,
+        data: Optional[TimeSeriesDataFrame] = None,
+        model: Optional[str] = None,
+        metric: Optional[Union[str, TimeSeriesScorer]] = None,
+        features: Optional[List[str]] = None,
+        time_limit: Optional[float] = None,
+        method: Literal["naive", "permutation"] = "permutation",
+        subsample_size: int = 50,
+        num_iterations: int = 1,
+        random_seed: Optional[int] = None,
+        relative_scores: bool = False,
+        include_confidence_band: bool = True,
+        confidence_level: float = 0.99,
+    ) -> pd.DataFrame:
+        trainer = self.load_trainer()
+        if data is None:
+            data = trainer.load_val_data() or trainer.load_train_data()
+
+        # if features are provided in the dataframe, check that they are valid features in the covariate metadata
+        provided_static_columns = [] if data.static_features is None else data.static_features.columns
+        unused_features = [
+            f
+            for f in set(provided_static_columns).union(set(data.columns) - {self.target})
+            if f not in self.feature_generator.covariate_metadata.all_features
+        ]
+
+        if features is None:
+            features = self.feature_generator.covariate_metadata.all_features
+        else:
+            if len(features) == 0:
+                raise ValueError(
+                    "No features provided to compute feature importance. At least some valid features should be provided."
+                )
+            for fn in features:
+                if fn not in self.feature_generator.covariate_metadata.all_features and fn not in unused_features:
+                    raise ValueError(f"Feature {fn} not found in covariate metadata or the dataset.")
+
+        if len(set(features)) < len(features):
+            logger.warning(
+                "Duplicate feature names provided to compute feature importance. This will lead to unexpected behavior. "
+                "Please provide unique feature names across both static features and covariates."
+            )
+
+        data = self.feature_generator.transform(data)
+
+        importance_df = trainer.get_feature_importance(
+            data=data,
+            features=features,
+            model=model,
+            metric=metric,
+            time_limit=time_limit,
+            method=method,
+            subsample_size=subsample_size,
+            num_iterations=num_iterations,
+            random_seed=random_seed,
+            relative_scores=relative_scores,
+            include_confidence_band=include_confidence_band,
+            confidence_level=confidence_level,
+        )
+
+        for feature in set(features).union(unused_features):
+            if feature not in importance_df.index:
+                importance_df.loc[feature] = (
+                    [0, 0, 0] if not include_confidence_band else [0, 0, 0, float("nan"), float("nan")]
+                )
+
+        return importance_df
+
     def leaderboard(self, data: Optional[TimeSeriesDataFrame] = None, use_cache: bool = True) -> pd.DataFrame:
         if data is not None:
             data = self.feature_generator.transform(data)
         return self.load_trainer().leaderboard(data, use_cache=use_cache)
 
     def get_info(self, include_model_info: bool = False, **kwargs) -> Dict[str, Any]:
         learner_info = super().get_info(include_model_info=include_model_info)
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import re
 import time
 from contextlib import nullcontext
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from autogluon.common import space
 from autogluon.common.loaders import load_pkl
 from autogluon.common.savers import save_pkl
 from autogluon.core.hpo.exceptions import EmptySearchSpace
 from autogluon.core.hpo.executors import HpoExecutor, RayHpoExecutor
 from autogluon.core.models import AbstractModel
@@ -70,14 +70,18 @@
     _convert_proba_to_unified_form = None
     _compute_permutation_importance = None
     _estimate_memory_usage = None
     _preprocess = None
     _preprocess_nonadaptive = None
     _preprocess_set_features = None
 
+    supports_known_covariates: bool = False
+    supports_past_covariates: bool = False
+    supports_static_features: bool = False
+
     def __init__(
         self,
         freq: Optional[str] = None,
         prediction_length: int = 1,
         path: Optional[str] = None,
         name: Optional[str] = None,
         metadata: Optional[CovariateMetadata] = None,
@@ -292,14 +296,15 @@
         -------
         predictions: TimeSeriesDataFrame
             pandas data frames with a timestamp index, where each input item from the input
             data is given as a separate forecast item in the dictionary, keyed by the `item_id`s
             of input items.
         """
         data = self.preprocess(data, is_train=False)
+        known_covariates = self.preprocess_known_covariates(known_covariates)
         predictions = self._predict(data=data, known_covariates=known_covariates, **kwargs)
         logger.debug(f"Predicting with model {self.name}")
         # "0.5" might be missing from the quantiles if self is a wrapper (MultiWindowBacktestingModel or ensemble)
         if "0.5" in predictions.columns:
             if self.eval_metric.optimized_by_median:
                 predictions["mean"] = predictions["0.5"]
             if self.must_drop_median:
@@ -354,28 +359,28 @@
         Returns
         -------
         score: float
             The computed forecast evaluation score on the last `self.prediction_length`
             time steps of each time series.
         """
         past_data, known_covariates = data.get_model_inputs_for_scoring(
-            prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates_real
+            prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates
         )
         predictions = self.predict(past_data, known_covariates=known_covariates)
         return self._score_with_predictions(data=data, predictions=predictions, metric=metric)
 
     def score_and_cache_oof(
         self,
         val_data: TimeSeriesDataFrame,
         store_val_score: bool = False,
         store_predict_time: bool = False,
     ) -> None:
         """Compute val_score, predict_time and cache out-of-fold (OOF) predictions."""
         past_data, known_covariates = val_data.get_model_inputs_for_scoring(
-            prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates_real
+            prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates
         )
         predict_start_time = time.time()
         oof_predictions = self.predict(past_data, known_covariates=known_covariates)
         self._oof_predictions = [oof_predictions]
         if store_predict_time:
             self.predict_time = time.time() - predict_start_time
         if store_val_score:
@@ -490,17 +495,22 @@
                 model_name=self.name,
                 model_path_root=self.path_root,
                 time_start=time_start,
             )
 
         return hpo_models, analysis
 
-    def preprocess(self, data: TimeSeriesDataFrame, is_train: bool = False, **kwargs) -> Any:
+    def preprocess(self, data: TimeSeriesDataFrame, is_train: bool = False, **kwargs) -> TimeSeriesDataFrame:
         return data
 
+    def preprocess_known_covariates(
+        self, known_covariates: Optional[TimeSeriesDataFrame]
+    ) -> Optional[TimeSeriesDataFrame]:
+        return known_covariates
+
     def get_memory_size(self, **kwargs) -> Optional[int]:
         return None
 
     def convert_to_refit_full_via_copy(self) -> "AbstractTimeSeriesModel":
         refit_model = super().convert_to_refit_full_via_copy()
         refit_model.val_score = None
         refit_model.predict_time = None
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         include_target: bool = True,
     ) -> pd.DataFrame:
         """Convert TimeSeriesDataFrame to a format expected by MLForecast methods `predict` and `preprocess`.
 
         Each row contains unique_id, ds, y, and (optionally) known covariates & static features.
         """
         # TODO: Add support for past_covariates
-        selected_columns = self.metadata.known_covariates_real.copy()
+        selected_columns = self.metadata.known_covariates.copy()
         column_name_mapping = {ITEMID: MLF_ITEMID, TIMESTAMP: MLF_TIMESTAMP}
         if include_target:
             selected_columns += [self.target]
             column_name_mapping[self.target] = MLF_TARGET
 
         df = pd.DataFrame(data)[selected_columns].reset_index()
         if static_features is not None:
@@ -421,14 +421,17 @@
     max_num_items : int or None, default = 20_000
         If not None, the model will randomly select this many time series for training and validation.
     max_num_samples : int or None, default = 1_000_000
         If not None, training dataset passed to TabularPredictor will contain at most this many rows (starting from the
         end of each time series).
     """
 
+    supports_known_covariates = True
+    supports_static_features = True
+
     @property
     def is_quantile_model(self) -> bool:
         return self.eval_metric.needs_quantile
 
     def _get_model_params(self) -> dict:
         model_params = super()._get_model_params()
         model_params.setdefault("scaler", "mean_abs")
@@ -572,14 +575,17 @@
     max_num_items : int or None, default = 20_000
         If not None, the model will randomly select this many time series for training and validation.
     max_num_samples : int or None, default = 1_000_000
         If not None, training dataset passed to TabularPredictor will contain at most this many rows (starting from the
         end of each time series).
     """
 
+    supports_known_covariates = True
+    supports_static_features = True
+
     def _get_model_params(self) -> dict:
         model_params = super()._get_model_params()
         model_params.setdefault("scaler", "standard")
         model_params.setdefault("differences", [get_seasonality(self.freq)])
         return model_params
 
     def _predict(
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     hidden_size : int, default = 40
         Number of RNN cells for each layer
     dropout_rate : float, default = 0.1
         Dropout regularization parameter
     embedding_dimension : int, optional
         Dimension of the embeddings for categorical features
         (if None, defaults to [min(50, (cat+1)//2) for cat in cardinality])
+    max_cat_cardinality : int, default = 100
+        Maximum number of dimensions to use when one-hot-encoding categorical known_covariates.
     distr_output : gluonts.torch.distributions.DistributionOutput, default = StudentTOutput()
         Distribution to use to evaluate observations and sample predictions
     scaling: bool, default = True
         Whether to automatically scale the target values
     max_epochs : int, default = 100
         Number of epochs the model will be trained for
     batch_size : int, default = 64
@@ -80,14 +82,15 @@
     early_stopping_patience : int or None, default = 20
         Early stop training if the validation loss doesn't improve for this many epochs.
     keep_lightning_logs : bool, default = False
         If True, ``lightning_logs`` directory will NOT be removed after the model finished training.
     """
 
     supports_known_covariates = True
+    supports_static_features = True
 
     def _get_estimator_class(self) -> Type[GluonTSEstimator]:
         from gluonts.torch.model.deepar import DeepAREstimator
 
         return DeepAREstimator
 
     def _get_estimator_init_args(self) -> Dict[str, Any]:
@@ -195,14 +198,16 @@
         Early stop training if the validation loss doesn't improve for this many epochs.
     keep_lightning_logs : bool, default = False
         If True, ``lightning_logs`` directory will NOT be removed after the model finished training.
     """
 
     supports_known_covariates = True
     supports_past_covariates = True
+    supports_cat_covariates = True
+    supports_static_features = True
 
     @property
     def default_context_length(self) -> int:
         return min(512, max(64, 2 * self.prediction_length))
 
     def _get_estimator_class(self) -> Type[GluonTSEstimator]:
         from gluonts.torch.model.tft import TemporalFusionTransformerEstimator
@@ -215,14 +220,19 @@
             init_kwargs["dynamic_dims"] = [self.num_feat_dynamic_real]
         if self.num_past_feat_dynamic_real > 0:
             init_kwargs["past_dynamic_dims"] = [self.num_past_feat_dynamic_real]
         if self.num_feat_static_real > 0:
             init_kwargs["static_dims"] = [self.num_feat_static_real]
         if len(self.feat_static_cat_cardinality):
             init_kwargs["static_cardinalities"] = self.feat_static_cat_cardinality
+        if len(self.feat_dynamic_cat_cardinality):
+            init_kwargs["dynamic_cardinalities"] = self.feat_dynamic_cat_cardinality
+        if len(self.past_feat_dynamic_cat_cardinality):
+            init_kwargs["past_dynamic_cardinalities"] = self.past_feat_dynamic_cat_cardinality
+
         init_kwargs.setdefault("time_features", get_time_features_for_frequency(self.freq))
         return init_kwargs
 
 
 class DLinearModel(AbstractGluonTSModel):
     """Simple feedforward neural network that subtracts trend before forecasting [Zeng2023]_.
 
@@ -368,14 +378,16 @@
         The seasonality of the time series. By default is set based on the ``freq`` of the data.
     embedding_dimension : int, default = 5
         The dimension of the embeddings for categorical features.
     use_log_scale_feature : bool, default = True
         If True, logarithm of the scale of the past data will be used as an additional static feature.
     negative_data : bool, default = True
         Flag indicating whether the time series take negative values.
+    max_cat_cardinality : int, default = 100
+        Maximum number of dimensions to use when one-hot-encoding categorical known_covariates.
     max_epochs : int, default = 100
         Number of epochs the model will be trained for
     batch_size : int, default = 64
         Size of batches used during training
     predict_batch_size : int, default = 500
         Size of batches used during prediction.
     num_batches_per_epoch : int, default = 50
@@ -389,14 +401,15 @@
     weight_decay : float, default = 1e-8
         Weight decay regularization parameter.
     keep_lightning_logs : bool, default = False
         If True, ``lightning_logs`` directory will NOT be removed after the model finished training.
     """
 
     supports_known_covariates = True
+    supports_static_features = True
     default_num_samples: int = 100
 
     def _get_estimator_class(self) -> Type[GluonTSEstimator]:
         from gluonts.torch.model.wavenet import WaveNetEstimator
 
         return WaveNetEstimator
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,26 @@
         self.model_base_type = type(self.model_base)
         self.info_per_val_window = []
 
         self.most_recent_model: AbstractTimeSeriesModel = None
         self.most_recent_model_folder: Optional[str] = None
         super().__init__(**kwargs)
 
+    @property
+    def supports_static_features(self) -> bool:
+        return self.model_base_type.supports_static_features
+
+    @property
+    def supports_known_covariates(self) -> bool:
+        return self.model_base_type.supports_known_covariates
+
+    @property
+    def supports_past_covariates(self) -> bool:
+        return self.model_base_type.supports_past_covariates
+
     def _get_model_base(self):
         return self.model_base
 
     def _get_hpo_backend(self) -> str:
         return self._get_model_base()._get_hpo_backend()
 
     def _is_gpu_available(self) -> bool:
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/predictor.py`

 * *Files 10% similar despite different names*

```diff
@@ -566,15 +566,15 @@
             Hyperparameter tuning strategy and kwargs (for example, how many HPO trials to run).
             If None, then hyperparameter tuning will not be performed.
 
             If type is ``str``, then this argument specifies a preset.
             Valid preset values:
 
             * "auto": Performs HPO via bayesian optimization search on GluonTS-backed neural forecasting models and
-                random search on other models using local scheduler.
+              random search on other models using local scheduler.
             * "random": Performs HPO via random search.
 
             You can also provide a dict to specify searchers and schedulers
             Valid keys:
 
             * "num_trials": How many HPO trials to run
             * "scheduler": Which scheduler to use. Valid values:
@@ -889,14 +889,145 @@
         self._check_data_for_evaluation(data)
         scores_dict = self._learner.evaluate(data, model=model, metrics=metrics, use_cache=use_cache)
         if display:
             logger.info("Evaluations on test data:")
             logger.info(json.dumps(scores_dict, indent=4))
         return scores_dict
 
+    def feature_importance(
+        self,
+        data: Optional[Union[TimeSeriesDataFrame, pd.DataFrame, Path, str]] = None,
+        model: Optional[str] = None,
+        metric: Optional[Union[str, TimeSeriesScorer]] = None,
+        features: Optional[List[str]] = None,
+        time_limit: Optional[float] = None,
+        method: Literal["naive", "permutation"] = "permutation",
+        subsample_size: int = 50,
+        num_iterations: Optional[int] = None,
+        random_seed: Optional[int] = 123,
+        relative_scores: bool = False,
+        include_confidence_band: bool = True,
+        confidence_level: float = 0.99,
+    ):
+        """
+        Calculates feature importance scores for the given model via replacing each feature by a shuffled version of the same feature
+        (also known as permutation feature importance) or by assigning a constant value representing the median or mode of the feature,
+        and computing the relative decrease in the model's predictive performance.
+
+        A feature's importance score represents the performance drop that results when the model makes predictions on a perturbed copy
+        of the data where this feature's values have been randomly shuffled across rows. A feature score of 0.01 would indicate that the
+        predictive performance dropped by 0.01 when the feature was randomly shuffled or replaced. The higher the score a feature has,
+        the more important it is to the model's performance.
+
+        If a feature has a negative score, this means that the feature is likely harmful to the final model, and a model trained with
+        the feature removed would be expected to achieve a better predictive performance. Note that calculating feature importance can
+        be a computationally expensive process, particularly if the model uses many features. In many cases, this can take longer than
+        the original model training. Roughly, this will equal to the number of features in the data multiplied by ``num_iterations``
+        (or, 1 when ``method="naive"``) and time taken when ``evaluate()`` is called on a dataset with ``subsample_size``.
+
+        Parameters
+        ----------
+        data : TimeSeriesDataFrame, pd.DataFrame, Path or str, optional
+            The data to evaluate feature importances on. The last ``prediction_length`` time steps of the data set, for each
+            item, will be held out for prediction and forecast accuracy will be calculated on these time steps.
+            More accurate feature importances will be obtained from new data that was held-out during ``fit()``.
+
+            If ``known_covariates_names`` were specified when creating the predictor, ``data`` must include the columns
+            listed in ``known_covariates_names`` with the covariates values aligned with the target time series.
+            This data must contain the label column with the same column name as specified during ``fit()``.
+
+            If ``train_data`` used to train the predictor contained past covariates or static features, then ``data``
+            must also include them (with same column names and dtypes).
+
+            If provided data is an instance of pandas DataFrame, AutoGluon will attempt to automatically convert it
+            to a ``TimeSeriesDataFrame``. If str or Path is passed, ``data`` will be loaded using the str value as the file path.
+
+            If ``data`` is not provided, then validation (tuning) data provided during training (or the held out data used for
+            validation if ``tuning_data`` was not explicitly provided ``fit()``) will be used.
+        model : str, optional
+            Name of the model that you would like to evaluate. By default, the best model during training
+            (with highest validation score) will be used.
+        metric : str or TimeSeriesScorer, optional
+            Metric to be used for computing feature importance. If None, the ``eval_metric`` specified during initialization of
+            the ``TimeSeriesPredictor`` will be used.
+        features : List[str], optional
+            List of feature names that feature importances are calculated for and returned. By default, all feature importances
+            will be returned.
+        method : {"permutation", "naive"}, default = "permutation"
+            Method to be used for computing feature importance.
+
+            * ``naive``: computes feature importance by replacing the values of each feature by a constant value and computing
+              feature importances as the relative improvement in the evaluation metric. The constant value is the median for
+              real-valued features and the mode for categorical features, for both covariates and static features, obtained from the
+              feature values in ``data`` provided.
+            * ``permutation``: computes feature importance by naively shuffling the values of the feature across different items
+              and time steps. Each feature is shuffled for ``num_iterations`` times and feature importances are computed as the
+              relative improvement in the evaluation metric. Refer to https://explained.ai/rf-importance/ for an explanation of
+              permutation importance.
+
+        subsample_size : int, default = 50
+            The number of items to sample from `data` when computing feature importance. Larger values increase the accuracy of
+            the feature importance scores. Runtime linearly scales with `subsample_size`.
+        time_limit : float, optional
+            Time in seconds to limit the calculation of feature importance. If None, feature importance will calculate without early stopping.
+            If ``method="permutation"``, a minimum of 1 full shuffle set will always be evaluated. If a shuffle set evaluation takes longer than
+            ``time_limit``, the method will take the length of a shuffle set evaluation to return regardless of the `time_limit`.
+        num_iterations : int, optional
+            The number of different iterations of the data that are evaluated. If ``method="permutation"``, this will be interpreted
+            as the number of shuffle sets (equivalent to ``num_shuffle_sets`` in :meth:`TabularPredictor.feature_importance`). If ``method="naive"``, the
+            constant replacement approach is repeated for ``num_iterations`` times, and a different subsample of data (of size ``subsample_size``) will
+            be taken in each iteration.
+            Default is 1 for ``method="naive"`` and 5 for ``method="permutation"``. The value will be ignored if ``method="naive"`` and the subsample
+            size is greater than the number of items in ``data`` as additional iterations will be redundant.
+            Larger values will increase the quality of the importance evaluation.
+            It is generally recommended to increase ``subsample_size`` before increasing ``num_iterations``.
+            Runtime scales linearly with ``num_iterations``.
+        random_seed : int or None, default = 123
+            If provided, fixes the seed of the random number generator for all models. This guarantees reproducible
+            results for feature importance.
+        relative_scores : bool, default = False
+            By default, this method will return expected average *absolute* improvement in the eval metric due to the feature. If True, then
+            the statistics will be computed over the *relative* (percentage) improvements.
+        include_confidence_band: bool, default = True
+            If True, returned DataFrame will include two additional columns specifying confidence interval for the true underlying importance value of
+            each feature. Increasing ``subsample_size`` and ``num_iterations`` will tighten the confidence interval.
+        confidence_level: float, default = 0.99
+            This argument is only considered when ``include_confidence_band=True``, and can be used to specify the confidence level used
+            for constructing confidence intervals. For example, if ``confidence_level`` is set to 0.99, then the returned DataFrame will include
+            columns ``p99_high`` and ``p99_low`` which indicates that the true feature importance will be between ``p99_high`` and ``p99_low`` 99% of
+            the time (99% confidence interval). More generally, if ``confidence_level`` = 0.XX, then the columns containing the XX% confidence interval
+            will be named ``pXX_high`` and ``pXX_low``.
+
+        Returns
+        -------
+        :class:`pd.DataFrame` of feature importance scores with 2 columns:
+            index: The feature name.
+            'importance': The estimated feature importance score.
+            'stddev': The standard deviation of the feature importance score. If NaN, then not enough ``num_iterations`` were used.
+        """
+        if data is not None:
+            data = self._check_and_prepare_data_frame(data)
+            self._check_data_for_evaluation(data)
+
+        fi_df = self._learner.get_feature_importance(
+            data=data,
+            model=model,
+            metric=metric,
+            features=features,
+            time_limit=time_limit,
+            method=method,
+            subsample_size=subsample_size,
+            num_iterations=num_iterations,
+            random_seed=random_seed,
+            relative_scores=relative_scores,
+            include_confidence_band=include_confidence_band,
+            confidence_level=confidence_level,
+        )
+        return fi_df
+
     @classmethod
     def _load_version_file(cls, path: str) -> str:
         version_file_path = os.path.join(path, cls._predictor_version_file_name)
         version = load_str.load(path=version_file_path)
         return version
 
     @classmethod
@@ -1223,15 +1354,15 @@
         val_data = trainer.load_val_data()
         base_models = trainer.get_model_names(level=0)
         pred_proba_dict_val: Dict[str, List[TimeSeriesDataFrame]] = {
             model: trainer._get_model_oof_predictions(model) for model in base_models
         }
 
         past_data, known_covariates = test_data.get_model_inputs_for_scoring(
-            prediction_length=self.prediction_length, known_covariates_names=trainer.metadata.known_covariates_real
+            prediction_length=self.prediction_length, known_covariates_names=trainer.metadata.known_covariates
         )
         pred_proba_dict_test: Dict[str, TimeSeriesDataFrame] = trainer.get_model_pred_dict(
             base_models, data=past_data, known_covariates=known_covariates
         )
 
         y_val: List[TimeSeriesDataFrame] = [
             select_target(df) for df in trainer._get_ensemble_oof_data(train_data=train_data, val_data=val_data)
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 from autogluon.core.utils.savers import save_json, save_pkl
 from autogluon.timeseries import TimeSeriesDataFrame
 from autogluon.timeseries.metrics import TimeSeriesScorer, check_get_evaluation_metric
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 from autogluon.timeseries.models.ensemble import AbstractTimeSeriesEnsembleModel, TimeSeriesGreedyEnsemble
 from autogluon.timeseries.models.presets import contains_searchspace
 from autogluon.timeseries.splitter import AbstractWindowSplitter, ExpandingWindowSplitter
-from autogluon.timeseries.utils.features import CovariateMetadata
+from autogluon.timeseries.utils.features import (
+    ConstantReplacementFeatureImportanceTransform,
+    CovariateMetadata,
+    PermutationFeatureImportanceTransform,
+)
 from autogluon.timeseries.utils.warning_filters import disable_tqdm
 
 logger = logging.getLogger("autogluon.timeseries.trainer")
 
 
 # TODO: This class is meant to be moved to `core`, where it will likely
 # TODO: be renamed `AbstractTrainer` and the current `AbstractTrainer`
@@ -238,14 +242,17 @@
     def predict(self, *args, **kwargs):
         raise NotImplementedError
 
 
 class AbstractTimeSeriesTrainer(SimpleAbstractTrainer):
     _cached_predictions_filename = "cached_predictions.pkl"
 
+    max_rel_importance_score: float = 1e5
+    eps_abs_importance_score: float = 1e-5
+
     def __init__(
         self,
         path: str,
         prediction_length: Optional[int] = 1,
         eval_metric: Union[str, TimeSeriesScorer, None] = None,
         eval_metric_seasonal_period: Optional[int] = None,
         save_data: bool = True,
@@ -759,15 +766,15 @@
                 "score_val": self.get_model_attribute(model_name, "val_score"),
                 "fit_time_marginal": self.get_model_attribute(model_name, "fit_time"),
                 "pred_time_val": self.get_model_attribute(model_name, "predict_time"),
             }
 
         if data is not None:
             past_data, known_covariates = data.get_model_inputs_for_scoring(
-                prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates_real
+                prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates
             )
             logger.info(
                 "Additional data provided, testing on additional data. Resulting leaderboard "
                 "will be sorted according to test score (`score_test`)."
             )
             model_predictions, pred_time_dict = self.get_model_pred_dict(
                 model_names=model_names,
@@ -845,27 +852,30 @@
         unpersisted_models = []
         for model in model_names:
             if model in self.models:
                 self.models.pop(model)
                 unpersisted_models.append(model)
         return unpersisted_models
 
-    def _get_model_for_prediction(self, model: Optional[Union[str, AbstractTimeSeriesModel]] = None) -> str:
+    def _get_model_for_prediction(
+        self, model: Optional[Union[str, AbstractTimeSeriesModel]] = None, verbose: bool = True
+    ) -> str:
         """Given an optional identifier or model object, return the name of the model with which to predict.
 
         If the model is not provided, this method will default to the best model according to the validation score.
         """
         if model is None:
             if self.model_best is None:
                 best_model_name: str = self.get_model_best()
                 self.model_best = best_model_name
-            logger.info(
-                f"Model not specified in predict, will default to the model with the "
-                f"best validation score: {self.model_best}",
-            )
+            if verbose:
+                logger.info(
+                    f"Model not specified in predict, will default to the model with the "
+                    f"best validation score: {self.model_best}",
+                )
             return self.model_best
         else:
             if isinstance(model, AbstractTimeSeriesModel):
                 return model.name
             else:
                 return model
 
@@ -919,27 +929,170 @@
         self,
         data: TimeSeriesDataFrame,
         model: Optional[Union[str, AbstractTimeSeriesModel]] = None,
         metrics: Optional[Union[str, TimeSeriesScorer, List[Union[str, TimeSeriesScorer]]]] = None,
         use_cache: bool = True,
     ) -> Dict[str, float]:
         past_data, known_covariates = data.get_model_inputs_for_scoring(
-            prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates_real
+            prediction_length=self.prediction_length, known_covariates_names=self.metadata.known_covariates
         )
         predictions = self.predict(data=past_data, known_covariates=known_covariates, model=model, use_cache=use_cache)
         if not isinstance(metrics, list):  # a single metric is provided
             metrics = [metrics]
         scores_dict = {}
         for metric in metrics:
             eval_metric = self.eval_metric if metric is None else check_get_evaluation_metric(metric)
             scores_dict[eval_metric.name] = self._score_with_predictions(
                 data=data, predictions=predictions, metric=eval_metric
             )
         return scores_dict
 
+    def get_feature_importance(
+        self,
+        data: TimeSeriesDataFrame,
+        features: List[str],
+        model: Optional[Union[str, AbstractTimeSeriesModel]] = None,
+        metric: Optional[Union[str, TimeSeriesScorer]] = None,
+        time_limit: Optional[float] = None,
+        method: Literal["naive", "permutation"] = "permutation",
+        subsample_size: int = 50,
+        num_iterations: int = 1,
+        random_seed: Optional[int] = None,
+        relative_scores: bool = False,
+        include_confidence_band: bool = True,
+        confidence_level: float = 0.99,
+    ) -> pd.DataFrame:
+        assert method in ["naive", "permutation"], f"Invalid feature importance method {method}."
+        metric = check_get_evaluation_metric(metric) if metric is not None else self.eval_metric
+
+        logger.info("Computing feature importance")
+
+        # seed everything if random_seed is provided
+        if random_seed is not None:
+            seed_everything(random_seed)
+
+        # start timer and cap subsample size if it's greater than the number of items in the provided data set
+        time_start = time.time()
+        if subsample_size > data.num_items:
+            logger.info(
+                f"Subsample_size {subsample_size} is larger than the number of items in the data and will be ignored"
+            )
+            subsample_size = data.num_items
+
+        # set default number of iterations and cap iterations if the number of items in the data is smaller
+        # than the subsample size for the naive method
+        num_iterations = num_iterations or (5 if method == "permutation" else 1)
+        if method == "naive" and data.num_items <= subsample_size:
+            num_iterations = 1
+
+        # initialize the importance transform
+        importance_transform_type = {
+            "permutation": PermutationFeatureImportanceTransform,
+            "naive": ConstantReplacementFeatureImportanceTransform,
+        }.get(method)
+        importance_transform = importance_transform_type(
+            covariate_metadata=self.metadata,
+            prediction_length=self.prediction_length,
+            random_seed=random_seed,
+        )
+
+        # if model is not provided, use the best model according to the validation score
+        model = self._get_model_for_prediction(model, verbose=False)
+
+        # persist trainer to speed up repeated inference
+        persisted_models = self.persist(model_names=[model], with_ancestors=True)
+
+        importance_samples = defaultdict(list)
+        for n in range(num_iterations):
+            if subsample_size < data.num_items:
+                item_ids_sampled = data.item_ids.to_series().sample(subsample_size)  # noqa
+                data_sample = data.query("item_id in @item_ids_sampled")
+            else:
+                data_sample = data
+
+            base_score = self.evaluate(data=data_sample, model=model, metrics=metric, use_cache=False)[metric.name]
+
+            for feature in features:
+                # override importance for unused features
+                if not self._model_uses_feature(model, feature):
+                    continue
+                else:
+                    data_sample_replaced = importance_transform.transform(data_sample, feature_name=feature)
+                    score = self.evaluate(data=data_sample_replaced, model=model, metrics=metric, use_cache=False)[
+                        metric.name
+                    ]
+
+                    importance = base_score - score
+                    if relative_scores:
+                        importance /= np.abs(base_score - self.eps_abs_importance_score)
+                        importance = min(self.max_rel_importance_score, importance)
+
+                    importance_samples[feature].append(importance)
+
+            if time_limit is not None and time.time() - time_start > time_limit:
+                logger.info(f"Time limit reached, stopping feature importance computation after {n} iterations")
+                break
+
+        self.unpersist(model_names=persisted_models)
+
+        importance_df = (
+            (
+                pd.DataFrame(importance_samples)
+                .agg(["mean", "std", "count"])
+                .T.rename(columns={"mean": "importance", "std": "stdev", "count": "n"})
+            )
+            if len(importance_samples) > 0
+            else pd.DataFrame(columns=["importance", "stdev", "n"])
+        )
+
+        if include_confidence_band:
+            importance_df = self._add_ci_to_feature_importance(importance_df, confidence_level=confidence_level)
+
+        return importance_df
+
+    def _model_uses_feature(self, model: Optional[Union[str, AbstractTimeSeriesModel]], feature: str) -> bool:
+        """Check if the given model uses the given feature."""
+        models_with_ancestors = set(self.get_minimum_model_set(model))
+
+        if feature in self.metadata.static_features:
+            return any(self.load_model(m).supports_static_features for m in models_with_ancestors)
+        elif feature in self.metadata.known_covariates:
+            return any(self.load_model(m).supports_known_covariates for m in models_with_ancestors)
+        elif feature in self.metadata.past_covariates:
+            return any(self.load_model(m).supports_past_covariates for m in models_with_ancestors)
+
+        return False
+
+    def _add_ci_to_feature_importance(
+        self, importance_df: pd.DataFrame, confidence_level: float = 0.99
+    ) -> pd.DataFrame:
+        """Add confidence intervals to the feature importance."""
+        import scipy.stats
+
+        if confidence_level <= 0.5 or confidence_level >= 1.0:
+            raise ValueError("confidence_level must lie between 0.5 and 1.0")
+        ci_str = "{:.0f}".format(confidence_level * 100)
+
+        alpha = 1 - confidence_level
+        importance_df[f"p{ci_str}_low"] = np.nan
+        importance_df[f"p{ci_str}_high"] = np.nan
+
+        for i in importance_df.index:
+            r = importance_df.loc[i]
+            importance, stdev, n = r["importance"], r["stdev"], r["n"]
+            if np.isnan(importance) or np.isnan(stdev) or np.isnan(n) or n <= 1:
+                continue
+
+            t_crit = scipy.stats.t.ppf(1 - alpha / 2, df=n - 1)
+
+            importance_df.loc[i, f"p{ci_str}_low"] = importance - t_crit * stdev / np.sqrt(n)
+            importance_df.loc[i, f"p{ci_str}_high"] = importance + t_crit * stdev / np.sqrt(n)
+
+        return importance_df
+
     def _predict_model(
         self,
         model: Union[str, AbstractTimeSeriesModel],
         data: TimeSeriesDataFrame,
         model_pred_dict: Dict[str, TimeSeriesDataFrame],
         known_covariates: Optional[TimeSeriesDataFrame] = None,
     ) -> TimeSeriesDataFrame:
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/features.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 import reprlib
 from dataclasses import dataclass, field
-from typing import List, Optional, Tuple
+from typing import Any, List, Literal, Optional, Tuple
 
+import numpy as np
 import pandas as pd
 
 from autogluon.common.features.types import R_FLOAT, R_INT
 from autogluon.features.generators import (
     AsTypeFeatureGenerator,
     CategoryFeatureGenerator,
     IdentityFeatureGenerator,
     PipelineFeatureGenerator,
 )
-from autogluon.timeseries import TimeSeriesDataFrame
+from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TimeSeriesDataFrame
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CovariateMetadata:
     """Provides mapping from different covariate types to columns in the dataset."""
@@ -25,14 +26,18 @@
     static_features_real: List[str] = field(default_factory=list)
     known_covariates_real: List[str] = field(default_factory=list)
     known_covariates_cat: List[str] = field(default_factory=list)
     past_covariates_real: List[str] = field(default_factory=list)
     past_covariates_cat: List[str] = field(default_factory=list)
 
     @property
+    def static_features(self) -> List[str]:
+        return self.static_features_cat + self.static_features_real
+
+    @property
     def known_covariates(self) -> List[str]:
         return self.known_covariates_cat + self.known_covariates_real
 
     @property
     def past_covariates(self) -> List[str]:
         return self.past_covariates_cat + self.past_covariates_real
 
@@ -44,14 +49,26 @@
     def covariates_real(self) -> List[str]:
         return self.known_covariates_real + self.past_covariates_real
 
     @property
     def covariates_cat(self) -> List[str]:
         return self.known_covariates_cat + self.past_covariates_cat
 
+    @property
+    def real_features(self) -> List[str]:
+        return self.static_features_real + self.covariates_real
+
+    @property
+    def cat_features(self) -> List[str]:
+        return self.static_features_cat + self.covariates_cat
+
+    @property
+    def all_features(self) -> List[str]:
+        return self.static_features + self.covariates
+
 
 class ContinuousAndCategoricalFeatureGenerator(PipelineFeatureGenerator):
     """Generates categorical and continuous features for time series models.
 
     Imputes missing categorical features with the most frequent value in the training set.
     """
 
@@ -280,7 +297,106 @@
         data: TimeSeriesDataFrame, required_column_names: List[str], data_frame_name: str
     ) -> None:
         missing_columns = pd.Index(required_column_names).difference(data.columns)
         if len(missing_columns) > 0:
             raise ValueError(
                 f"{len(missing_columns)} columns are missing from {data_frame_name}: {reprlib.repr(missing_columns.to_list())}"
             )
+
+
+class AbstractFeatureImportanceTransform:
+    """Abstract class for transforms that replace a given feature with dummy or shuffled values,
+    for use in feature importance operations.
+    """
+
+    def __init__(
+        self,
+        covariate_metadata: CovariateMetadata,
+        prediction_length: int,
+        **kwargs,
+    ):
+        self.covariate_metadata: CovariateMetadata = covariate_metadata
+        self.prediction_length: int = prediction_length
+
+    def _transform_series(self, data: pd.Series, is_categorical: bool, **kwargs) -> TimeSeriesDataFrame:
+        """Transforms a series with the same index as the pandas DataFrame"""
+        raise NotImplementedError
+
+    def transform(self, data: TimeSeriesDataFrame, feature_name: str, **kwargs) -> TimeSeriesDataFrame:
+        if feature_name not in self.covariate_metadata.all_features:
+            raise ValueError(f"Target feature {feature_name} not found in covariate metadata")
+
+        # feature transform works on a shallow copy of the main time series data frame
+        # but a deep copy of the static features.
+        data = data.copy(deep=False)
+
+        is_categorical = feature_name in self.covariate_metadata.cat_features
+
+        if feature_name in self.covariate_metadata.past_covariates:
+            # we'll have to work on the history of the data alone
+            data[feature_name] = data[feature_name].copy()
+            feature_data = data[feature_name].groupby(level=ITEMID, sort=False).head(-self.prediction_length)
+            data[feature_name].update(self._transform_series(feature_data, is_categorical=is_categorical))
+        elif feature_name in self.covariate_metadata.static_features:
+            feature_data = data.static_features[feature_name].copy()
+            feature_data.reset_index(drop=True, inplace=True)
+            data.static_features[feature_name] = self._transform_static_series(
+                feature_data, is_categorical=is_categorical
+            )
+        else:  # known covariates
+            data[feature_name] = self._transform_series(data[feature_name], is_categorical=is_categorical)
+
+        return data
+
+
+class PermutationFeatureImportanceTransform(AbstractFeatureImportanceTransform):
+    """Naively shuffles a given feature."""
+
+    def __init__(
+        self,
+        covariate_metadata: CovariateMetadata,
+        prediction_length: int,
+        random_seed: Optional[int] = None,
+        shuffle_type: Literal["itemwise", "naive"] = "itemwise",
+        **kwargs,
+    ):
+        super().__init__(covariate_metadata, prediction_length, **kwargs)
+        self.shuffle_type = shuffle_type
+        self.random_seed = random_seed
+
+    def _transform_static_series(self, feature_data: pd.Series, is_categorical: bool) -> Any:
+        return feature_data.sample(frac=1, random_state=self.random_seed).values
+
+    def _transform_series(self, feature_data: pd.Series, is_categorical: bool) -> pd.Series:
+        # set random state once to shuffle 'independently' for different items
+        rng = np.random.RandomState(self.random_seed)
+
+        if self.shuffle_type == "itemwise":
+            return feature_data.groupby(level=ITEMID, sort=False).transform(
+                lambda x: x.sample(frac=1, random_state=rng).values
+            )
+        elif self.shuffle_type == "naive":
+            return pd.Series(feature_data.sample(frac=1, random_state=rng).values, index=feature_data.index)
+
+
+class ConstantReplacementFeatureImportanceTransform(AbstractFeatureImportanceTransform):
+    """Replaces a target feature with the median if it's a real-valued feature, and the mode if it's a
+    categorical feature."""
+
+    def __init__(
+        self,
+        covariate_metadata: CovariateMetadata,
+        prediction_length: int,
+        real_value_aggregation: Literal["mean", "median"] = "mean",
+        **kwargs,
+    ):
+        super().__init__(covariate_metadata, prediction_length, **kwargs)
+        self.real_value_aggregation = real_value_aggregation
+
+    def _transform_static_series(self, feature_data: pd.Series, is_categorical: bool) -> Any:
+        return feature_data.mode()[0] if is_categorical else feature_data.agg(self.real_value_aggregation)
+
+    def _transform_series(self, feature_data: pd.Series, is_categorical: bool) -> pd.Series:
+        if is_categorical:
+            return feature_data.groupby(level=ITEMID, sort=False).transform(lambda x: x.mode()[0])
+        else:
+            return feature_data.groupby(level=ITEMID, sort=False).transform(self.real_value_aggregation)
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.0.1b20240406/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.0.1b20240405
+Version: 1.0.1b20240406
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.0.1b20240405/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.0.1b20240406/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.0.1b20240405
-autogluon.common==1.0.1b20240405
-autogluon.tabular[catboost,lightgbm,xgboost]==1.0.1b20240405
+autogluon.core[raytune]==1.0.1b20240406
+autogluon.common==1.0.1b20240406
+autogluon.tabular[catboost,lightgbm,xgboost]==1.0.1b20240406
 
 [all]
 optimum[nncf,openvino]<1.18,>=1.17
 optimum[onnxruntime]<1.18,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.18,>=1.17
```

