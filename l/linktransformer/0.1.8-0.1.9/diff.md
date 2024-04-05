# Comparing `tmp/linktransformer-0.1.8.tar.gz` & `tmp/linktransformer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktransformer-0.1.8.tar", last modified: Fri Sep 22 21:54:21 2023, max compression
+gzip compressed data, was "linktransformer-0.1.9.tar", last modified: Mon Sep 25 03:36:28 2023, max compression
```

## Comparing `linktransformer-0.1.8.tar` & `linktransformer-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.008213 linktransformer-0.1.8/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    35149 2023-08-09 22:35:32.000000 linktransformer-0.1.8/LICENSE
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.8/MANIFEST.in
--rw-r--r--   0 abhishekarora  (1008) abhishekarora  (1009)    57268 2023-09-22 21:54:21.008213 linktransformer-0.1.8/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    15775 2023-09-22 21:17:54.000000 linktransformer-0.1.8/README.md
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1259 2023-09-20 22:07:12.000000 linktransformer-0.1.8/pyproject.toml
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-09-22 21:54:21.008213 linktransformer-0.1.8/setup.cfg
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:20.996213 linktransformer-0.1.8/src/
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.000213 linktransformer-0.1.8/src/linktransformer/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      449 2023-09-22 21:20:33.000000 linktransformer-0.1.8/src/linktransformer/__init__.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.000213 linktransformer-0.1.8/src/linktransformer/configs/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      236 2023-09-19 19:58:58.000000 linktransformer-0.1.8/src/linktransformer/configs/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      384 2023-09-20 19:38:31.000000 linktransformer-0.1.8/src/linktransformer/configs/classification.json
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      552 2023-09-20 20:39:59.000000 linktransformer-0.1.8/src/linktransformer/configs/linkage.json
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.004213 linktransformer-0.1.8/src/linktransformer/data/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.8/src/linktransformer/data/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.8/src/linktransformer/data/coarse.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6519 2023-08-23 00:35:56.000000 linktransformer-0.1.8/src/linktransformer/data/company_clusters.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.8/src/linktransformer/data/es_mexican_products.xlsx
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    67473 2023-09-19 23:04:33.000000 linktransformer-0.1.8/src/linktransformer/data/eval_weather.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.8/src/linktransformer/data/fine.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)  3368771 2023-08-07 10:29:39.000000 linktransformer-0.1.8/src/linktransformer/data/jp_pr_tk431.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   109993 2023-09-20 18:26:57.000000 linktransformer-0.1.8/src/linktransformer/data/protest_test.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   518139 2023-09-20 18:26:56.000000 linktransformer-0.1.8/src/linktransformer/data/protest_train.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    96924 2023-09-20 18:26:55.000000 linktransformer-0.1.8/src/linktransformer/data/protest_val.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3313 2023-09-20 21:19:14.000000 linktransformer-0.1.8/src/linktransformer/data/protests_toy_sample_binary.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3313 2023-09-20 21:19:14.000000 linktransformer-0.1.8/src/linktransformer/data/protests_toy_sample_ternary.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    79754 2023-09-19 23:04:33.000000 linktransformer-0.1.8/src/linktransformer/data/test_weather.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.8/src/linktransformer/data/toy_comp_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.8/src/linktransformer/data/toy_comp_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.8/src/linktransformer/data/toy_multi_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.8/src/linktransformer/data/toy_multi_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.8/src/linktransformer/data/toy_pairs.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   362300 2023-09-19 23:04:34.000000 linktransformer-0.1.8/src/linktransformer/data/train_weather.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.8/src/linktransformer/data/translation_1.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.8/src/linktransformer/data/translation_2.csv
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    31540 2023-09-22 21:53:12.000000 linktransformer-0.1.8/src/linktransformer/infer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9118 2023-09-22 19:51:16.000000 linktransformer-0.1.8/src/linktransformer/model_card_templates.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.004213 linktransformer-0.1.8/src/linktransformer/modelling/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    13863 2023-09-22 20:35:55.000000 linktransformer-0.1.8/src/linktransformer/modelling/LinkTransformer.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    10950 2023-09-22 20:40:17.000000 linktransformer-0.1.8/src/linktransformer/modelling/LinkTransformerClassifier.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-21 22:39:25.000000 linktransformer-0.1.8/src/linktransformer/modelling/__init__.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.004213 linktransformer-0.1.8/src/linktransformer/modified_sbert/
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-21 22:39:21.000000 linktransformer-0.1.8/src/linktransformer/modified_sbert/__init__.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3380 2023-08-04 23:50:58.000000 linktransformer-0.1.8/src/linktransformer/modified_sbert/cluster_fns.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.8/src/linktransformer/modified_sbert/data_loaders.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-30 00:13:14.000000 linktransformer-0.1.8/src/linktransformer/modified_sbert/evaluation.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.8/src/linktransformer/modified_sbert/losses.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6831 2023-09-20 23:20:09.000000 linktransformer-0.1.8/src/linktransformer/modified_sbert/train.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    40673 2023-09-01 02:45:42.000000 linktransformer-0.1.8/src/linktransformer/preprocess.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    19294 2023-09-22 00:14:56.000000 linktransformer-0.1.8/src/linktransformer/train_clf_model.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9976 2023-09-01 02:55:42.000000 linktransformer-0.1.8/src/linktransformer/train_model.py
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    11476 2023-09-20 23:20:10.000000 linktransformer-0.1.8/src/linktransformer/utils.py
-drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-22 21:54:21.000213 linktransformer-0.1.8/src/linktransformer.egg-info/
--rw-r--r--   0 abhishekarora  (1008) abhishekarora  (1009)    57268 2023-09-22 21:54:20.000000 linktransformer-0.1.8/src/linktransformer.egg-info/PKG-INFO
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1962 2023-09-22 21:54:20.000000 linktransformer-0.1.8/src/linktransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-09-22 21:54:20.000000 linktransformer-0.1.8/src/linktransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      145 2023-09-22 21:54:20.000000 linktransformer-0.1.8/src/linktransformer.egg-info/requires.txt
--rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-09-22 21:54:20.000000 linktransformer-0.1.8/src/linktransformer.egg-info/top_level.txt
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.065787 linktransformer-0.1.9/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    35149 2023-08-09 22:35:32.000000 linktransformer-0.1.9/LICENSE
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      122 2023-08-01 02:28:30.000000 linktransformer-0.1.9/MANIFEST.in
+-rw-r--r--   0 abhishekarora  (1008) abhishekarora  (1009)    57268 2023-09-25 03:36:28.065787 linktransformer-0.1.9/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    15775 2023-09-22 21:17:54.000000 linktransformer-0.1.9/README.md
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1259 2023-09-25 03:31:58.000000 linktransformer-0.1.9/pyproject.toml
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       38 2023-09-25 03:36:28.065787 linktransformer-0.1.9/setup.cfg
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.033786 linktransformer-0.1.9/src/
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.033786 linktransformer-0.1.9/src/linktransformer/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      449 2023-09-25 03:32:46.000000 linktransformer-0.1.9/src/linktransformer/__init__.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.033786 linktransformer-0.1.9/src/linktransformer/configs/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      236 2023-09-19 19:58:58.000000 linktransformer-0.1.9/src/linktransformer/configs/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      384 2023-09-20 19:38:31.000000 linktransformer-0.1.9/src/linktransformer/configs/classification.json
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      552 2023-09-20 20:39:59.000000 linktransformer-0.1.9/src/linktransformer/configs/linkage.json
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.061787 linktransformer-0.1.9/src/linktransformer/data/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      100 2023-07-30 23:26:04.000000 linktransformer-0.1.9/src/linktransformer/data/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      124 2023-07-29 23:45:13.000000 linktransformer-0.1.9/src/linktransformer/data/coarse.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6519 2023-08-23 00:35:56.000000 linktransformer-0.1.9/src/linktransformer/data/company_clusters.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   436216 2023-07-29 23:45:13.000000 linktransformer-0.1.9/src/linktransformer/data/es_mexican_products.xlsx
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    67473 2023-09-19 23:04:33.000000 linktransformer-0.1.9/src/linktransformer/data/eval_weather.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      355 2023-07-29 23:45:13.000000 linktransformer-0.1.9/src/linktransformer/data/fine.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)  3368771 2023-08-07 10:29:39.000000 linktransformer-0.1.9/src/linktransformer/data/jp_pr_tk431.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   109993 2023-09-20 18:26:57.000000 linktransformer-0.1.9/src/linktransformer/data/protest_test.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   518139 2023-09-20 18:26:56.000000 linktransformer-0.1.9/src/linktransformer/data/protest_train.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    96924 2023-09-20 18:26:55.000000 linktransformer-0.1.9/src/linktransformer/data/protest_val.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3313 2023-09-20 21:19:14.000000 linktransformer-0.1.9/src/linktransformer/data/protests_toy_sample_binary.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3313 2023-09-20 21:19:14.000000 linktransformer-0.1.9/src/linktransformer/data/protests_toy_sample_ternary.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    79754 2023-09-19 23:04:33.000000 linktransformer-0.1.9/src/linktransformer/data/test_weather.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      300 2023-07-29 23:45:13.000000 linktransformer-0.1.9/src/linktransformer/data/toy_comp_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      310 2023-07-29 23:45:13.000000 linktransformer-0.1.9/src/linktransformer/data/toy_comp_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      415 2023-07-30 17:00:18.000000 linktransformer-0.1.9/src/linktransformer/data/toy_multi_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1064 2023-07-30 17:05:16.000000 linktransformer-0.1.9/src/linktransformer/data/toy_multi_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      388 2023-08-04 05:38:49.000000 linktransformer-0.1.9/src/linktransformer/data/toy_pairs.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)   362300 2023-09-19 23:04:34.000000 linktransformer-0.1.9/src/linktransformer/data/train_weather.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      631 2023-07-30 17:19:37.000000 linktransformer-0.1.9/src/linktransformer/data/translation_1.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      529 2023-07-30 17:20:21.000000 linktransformer-0.1.9/src/linktransformer/data/translation_2.csv
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    31540 2023-09-22 22:26:51.000000 linktransformer-0.1.9/src/linktransformer/infer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9118 2023-09-22 19:51:16.000000 linktransformer-0.1.9/src/linktransformer/model_card_templates.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.061787 linktransformer-0.1.9/src/linktransformer/modelling/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    13863 2023-09-22 20:35:55.000000 linktransformer-0.1.9/src/linktransformer/modelling/LinkTransformer.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    10950 2023-09-22 20:40:17.000000 linktransformer-0.1.9/src/linktransformer/modelling/LinkTransformerClassifier.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-21 22:39:25.000000 linktransformer-0.1.9/src/linktransformer/modelling/__init__.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.061787 linktransformer-0.1.9/src/linktransformer/modified_sbert/
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-21 22:39:21.000000 linktransformer-0.1.9/src/linktransformer/modified_sbert/__init__.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     3380 2023-08-04 23:50:58.000000 linktransformer-0.1.9/src/linktransformer/modified_sbert/cluster_fns.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      735 2023-07-30 00:14:40.000000 linktransformer-0.1.9/src/linktransformer/modified_sbert/data_loaders.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    21144 2023-08-30 00:13:14.000000 linktransformer-0.1.9/src/linktransformer/modified_sbert/evaluation.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     4668 2023-07-30 18:14:18.000000 linktransformer-0.1.9/src/linktransformer/modified_sbert/losses.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     6831 2023-09-20 23:20:09.000000 linktransformer-0.1.9/src/linktransformer/modified_sbert/train.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    40673 2023-09-01 02:45:42.000000 linktransformer-0.1.9/src/linktransformer/preprocess.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    19546 2023-09-25 03:29:10.000000 linktransformer-0.1.9/src/linktransformer/train_clf_model.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     9976 2023-09-01 02:55:42.000000 linktransformer-0.1.9/src/linktransformer/train_model.py
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)    11476 2023-09-20 23:20:10.000000 linktransformer-0.1.9/src/linktransformer/utils.py
+drwxrwxr-x   0 abhishekarora  (1008) abhishekarora  (1009)        0 2023-09-25 03:36:28.033786 linktransformer-0.1.9/src/linktransformer.egg-info/
+-rw-r--r--   0 abhishekarora  (1008) abhishekarora  (1009)    57268 2023-09-25 03:36:28.000000 linktransformer-0.1.9/src/linktransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)     1962 2023-09-25 03:36:28.000000 linktransformer-0.1.9/src/linktransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)        1 2023-09-25 03:36:28.000000 linktransformer-0.1.9/src/linktransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)      145 2023-09-25 03:36:28.000000 linktransformer-0.1.9/src/linktransformer.egg-info/requires.txt
+-rw-rw-r--   0 abhishekarora  (1008) abhishekarora  (1009)       16 2023-09-25 03:36:28.000000 linktransformer-0.1.9/src/linktransformer.egg-info/top_level.txt
```

### Comparing `linktransformer-0.1.8/LICENSE` & `linktransformer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/PKG-INFO` & `linktransformer-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A friendly way to do link, aggregate, cluster and de-duplicate dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <linktransformer23@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `linktransformer-0.1.8/README.md` & `linktransformer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/pyproject.toml` & `linktransformer-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linktransformer"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
        "scikit-learn",
         "faiss-cpu",
         "hdbscan",
         "networkx",
         "torch",
         "sentence_transformers",
```

### Comparing `linktransformer-0.1.8/src/linktransformer/configs/linkage.json` & `linktransformer-0.1.9/src/linktransformer/configs/linkage.json`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/company_clusters.csv` & `linktransformer-0.1.9/src/linktransformer/data/company_clusters.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/es_mexican_products.xlsx` & `linktransformer-0.1.9/src/linktransformer/data/es_mexican_products.xlsx`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/eval_weather.csv` & `linktransformer-0.1.9/src/linktransformer/data/eval_weather.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/jp_pr_tk431.csv` & `linktransformer-0.1.9/src/linktransformer/data/jp_pr_tk431.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/protest_test.csv` & `linktransformer-0.1.9/src/linktransformer/data/protest_test.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/protest_train.csv` & `linktransformer-0.1.9/src/linktransformer/data/protest_train.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/protest_val.csv` & `linktransformer-0.1.9/src/linktransformer/data/protest_val.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/protests_toy_sample_binary.csv` & `linktransformer-0.1.9/src/linktransformer/data/protests_toy_sample_binary.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/protests_toy_sample_ternary.csv` & `linktransformer-0.1.9/src/linktransformer/data/protests_toy_sample_ternary.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/test_weather.csv` & `linktransformer-0.1.9/src/linktransformer/data/test_weather.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/toy_multi_2.csv` & `linktransformer-0.1.9/src/linktransformer/data/toy_multi_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/train_weather.csv` & `linktransformer-0.1.9/src/linktransformer/data/train_weather.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/translation_1.csv` & `linktransformer-0.1.9/src/linktransformer/data/translation_1.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/data/translation_2.csv` & `linktransformer-0.1.9/src/linktransformer/data/translation_2.csv`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/infer.py` & `linktransformer-0.1.9/src/linktransformer/infer.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/model_card_templates.py` & `linktransformer-0.1.9/src/linktransformer/model_card_templates.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modelling/LinkTransformer.py` & `linktransformer-0.1.9/src/linktransformer/modelling/LinkTransformer.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modelling/LinkTransformerClassifier.py` & `linktransformer-0.1.9/src/linktransformer/modelling/LinkTransformerClassifier.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modified_sbert/cluster_fns.py` & `linktransformer-0.1.9/src/linktransformer/modified_sbert/cluster_fns.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modified_sbert/data_loaders.py` & `linktransformer-0.1.9/src/linktransformer/modified_sbert/data_loaders.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modified_sbert/evaluation.py` & `linktransformer-0.1.9/src/linktransformer/modified_sbert/evaluation.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modified_sbert/losses.py` & `linktransformer-0.1.9/src/linktransformer/modified_sbert/losses.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/modified_sbert/train.py` & `linktransformer-0.1.9/src/linktransformer/modified_sbert/train.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/preprocess.py` & `linktransformer-0.1.9/src/linktransformer/preprocess.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/train_clf_model.py` & `linktransformer-0.1.9/src/linktransformer/train_clf_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -406,30 +406,39 @@
     datasets = {}
     for dataset in ["train", "eval", "test"]:
         datasets[dataset] = tokenize_data_for_finetuning(
             directory=os.path.join(data_dir,f'{dataset}.csv'),
             hf_model=model
         )
 
+    specified_training_args = training_args
+
     ##Load config as training args
     training_args = load_default_training_args(config)
     
+    ##Override if training_args is not empty
+    if len(training_args)>0:
+        training_args.update(specified_training_args)
+    print("Updating training args with: ", specified_training_args)
+    
     ##Override some args
     if lr is not None:
         training_args["learning_rate"] = lr
     if batch_size is not None:
         training_args["per_device_train_batch_size"] = batch_size
         training_args["per_device_eval_batch_size"] = batch_size
     if epochs is not None:
         training_args["num_train_epochs"] = epochs
     if eval_steps is not None:
         training_args["evaluation_strategy"] = "steps"
         training_args["eval_steps"] = eval_steps
     if save_steps is not None:
         training_args["save_steps"] = save_steps
+
+    
     
 
     ##Get weight list from data if needed
     weight_list=weight_list if weight_list is not None else [1-prop for prop in prop_labels] if weighted_loss else None
 
     ##Train model
     best_model_path, best_metric = train_model(
```

### Comparing `linktransformer-0.1.8/src/linktransformer/train_model.py` & `linktransformer-0.1.9/src/linktransformer/train_model.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer/utils.py` & `linktransformer-0.1.9/src/linktransformer/utils.py`

 * *Files identical despite different names*

### Comparing `linktransformer-0.1.8/src/linktransformer.egg-info/PKG-INFO` & `linktransformer-0.1.9/src/linktransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktransformer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A friendly way to do link, aggregate, cluster and de-duplicate dataframes using large language models.
 Author-email: "Abhishek Arora, Sam Jones and Melissa Dell" <linktransformer23@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `linktransformer-0.1.8/src/linktransformer.egg-info/SOURCES.txt` & `linktransformer-0.1.9/src/linktransformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

