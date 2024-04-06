# Comparing `tmp/PhysioKit2-1.8.7.tar.gz` & `tmp/PhysioKit2-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhysioKit2-1.8.7.tar", last modified: Tue Feb 20 13:11:32 2024, max compression
+gzip compressed data, was "PhysioKit2-1.8.8.tar", last modified: Sat Apr  6 21:27:47 2024, max compression
```

## Comparing `PhysioKit2-1.8.7.tar` & `PhysioKit2-1.8.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.877380 PhysioKit2-1.8.7/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1084 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/LICENSE
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13452 2024-02-20 13:11:32.877031 PhysioKit2-1.8.7/PKG-INFO
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    12723 2023-11-28 04:17:58.000000 PhysioKit2-1.8.7/README.md
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)       38 2024-02-20 13:11:32.877416 PhysioKit2-1.8.7/setup.cfg
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1878 2024-02-20 10:46:06.000000 PhysioKit2-1.8.7/setup.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.862753 PhysioKit2-1.8.7/src/
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.865354 PhysioKit2-1.8.7/src/PhysioKit2/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.866311 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    33220 2023-11-30 23:47:14.000000 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/process_signals.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.866820 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/sample_data/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/sample_data/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/sample_data/download data from PhysioKit GitHub repo page.txt
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.866992 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/utils/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/utils/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3203 2023-10-21 20:33:26.000000 PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/utils/load_data.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.867354 PhysioKit2-1.8.7/src/PhysioKit2/configs/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.868215 PhysioKit2-1.8.7/src/PhysioKit2/configs/arm_due/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/arm_due/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      365 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/arm_due/sw_config.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      374 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/arm_due/sw_config_client.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      375 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/arm_due/sw_config_server.json
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.868883 PhysioKit2-1.8.7/src/PhysioKit2/configs/avr_default/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/avr_default/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      364 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/avr_default/sw_config.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/avr_default/sw_config_client.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/avr_default/sw_config_server.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1109 2023-10-24 18:51:21.000000 PhysioKit2-1.8.7/src/PhysioKit2/configs/exp_config_phys.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    22491 2023-10-21 22:16:23.000000 PhysioKit2-1.8.7/src/PhysioKit2/form.ui
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    19094 2023-10-21 22:16:23.000000 PhysioKit2-1.8.7/src/PhysioKit2/form_ui.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.869700 PhysioKit2-1.8.7/src/PhysioKit2/images/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/images/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    42512 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/images/banner.png
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3095 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/images/color_bar.png
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    91499 2023-10-23 00:50:14.000000 PhysioKit2-1.8.7/src/PhysioKit2/images/sq_indication.png
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    35146 2024-02-20 13:07:55.000000 PhysioKit2-1.8.7/src/PhysioKit2/main.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/register_dummy.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.870608 PhysioKit2-1.8.7/src/PhysioKit2/sqa/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/__init__.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.870817 PhysioKit2-1.8.7/src/PhysioKit2/sqa/ckpt/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/ckpt/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)   213429 2024-02-20 11:50:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/ckpt/sqa_bvp.pth
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.871553 PhysioKit2-1.8.7/src/PhysioKit2/sqa/config/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/config/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      613 2024-02-20 11:50:21.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/config/sqa_bvp.json
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3858 2023-11-30 23:37:38.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/inference.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5732 2024-02-20 13:11:17.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/inference_thread.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.874453 PhysioKit2-1.8.7/src/PhysioKit2/sqa/model/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/model/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13245 2024-02-20 11:50:14.000000 PhysioKit2-1.8.7/src/PhysioKit2/sqa/model/sqa_bvp.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.876657 PhysioKit2-1.8.7/src/PhysioKit2/utils/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/__init__.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     8235 2023-12-01 00:16:35.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/acquisition.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    10939 2023-12-01 13:56:18.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/biofeedback.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      384 2023-11-01 02:26:11.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/config.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1877 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/data_processing_lib.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3999 2023-12-01 00:17:10.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/external_sync.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5682 2023-12-01 13:54:03.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/file_ops.py
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     2186 2023-10-21 17:57:29.000000 PhysioKit2-1.8.7/src/PhysioKit2/utils/load_data.py
-drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-02-20 13:11:32.876833 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13452 2024-02-20 13:11:32.000000 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/PKG-INFO
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1965 2024-02-20 13:11:32.000000 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/SOURCES.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)        1 2024-02-20 13:11:32.000000 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/dependency_links.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      119 2024-02-20 13:11:32.000000 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/entry_points.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)      139 2024-02-20 13:11:32.000000 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/requires.txt
--rw-r--r--   0 jiteshjoshi   (501) staff       (20)       11 2024-02-20 13:11:32.000000 PhysioKit2-1.8.7/src/PhysioKit2.egg-info/top_level.txt
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.693620 PhysioKit2-1.8.8/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1084 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/LICENSE
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13452 2024-04-06 21:27:47.693277 PhysioKit2-1.8.8/PKG-INFO
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    12723 2023-11-28 04:17:58.000000 PhysioKit2-1.8.8/README.md
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)       38 2024-04-06 21:27:47.693673 PhysioKit2-1.8.8/setup.cfg
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1878 2024-04-06 17:07:46.000000 PhysioKit2-1.8.8/setup.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.677377 PhysioKit2-1.8.8/src/
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.681639 PhysioKit2-1.8.8/src/PhysioKit2/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.682790 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    33222 2024-04-06 16:59:36.000000 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/process_signals.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.683157 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/sample_data/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/sample_data/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/sample_data/download data from PhysioKit GitHub repo page.txt
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.683400 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/utils/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/utils/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3203 2023-10-21 20:33:26.000000 PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/utils/load_data.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.683822 PhysioKit2-1.8.8/src/PhysioKit2/configs/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.684877 PhysioKit2-1.8.8/src/PhysioKit2/configs/arm_due/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/arm_due/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      365 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/arm_due/sw_config.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      374 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/arm_due/sw_config_client.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      375 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/arm_due/sw_config_server.json
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.685657 PhysioKit2-1.8.8/src/PhysioKit2/configs/avr_default/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/avr_default/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      364 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/avr_default/sw_config.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/avr_default/sw_config_client.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      369 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/avr_default/sw_config_server.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1109 2023-10-24 18:51:21.000000 PhysioKit2-1.8.8/src/PhysioKit2/configs/exp_config_phys.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    22491 2023-10-21 22:16:23.000000 PhysioKit2-1.8.8/src/PhysioKit2/form.ui
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    19094 2023-10-21 22:16:23.000000 PhysioKit2-1.8.8/src/PhysioKit2/form_ui.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.686759 PhysioKit2-1.8.8/src/PhysioKit2/images/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/images/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    42512 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/images/banner.png
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3095 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/images/color_bar.png
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    91499 2023-10-23 00:50:14.000000 PhysioKit2-1.8.8/src/PhysioKit2/images/sq_indication.png
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    35148 2024-04-06 16:59:36.000000 PhysioKit2-1.8.8/src/PhysioKit2/main.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/register_dummy.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.687948 PhysioKit2-1.8.8/src/PhysioKit2/sqa/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.689466 PhysioKit2-1.8.8/src/PhysioKit2/sqa/ckpt/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)   484328 2024-04-05 12:35:26.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/ckpt/SQAPhysMD.pth
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/ckpt/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.689778 PhysioKit2-1.8.8/src/PhysioKit2/sqa/config/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      616 2024-04-06 17:04:06.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/config/SQAPhysMD.json
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/config/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3860 2024-04-06 16:59:36.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/inference.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5734 2024-04-06 16:59:36.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/inference_thread.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.690338 PhysioKit2-1.8.8/src/PhysioKit2/sqa/model/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13247 2024-04-06 16:59:36.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/model/SQAPhysMD.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/sqa/model/__init__.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.692712 PhysioKit2-1.8.8/src/PhysioKit2/utils/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        0 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/__init__.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     8235 2024-04-06 16:54:52.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/acquisition.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    10939 2023-12-01 13:56:18.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/biofeedback.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      384 2023-11-01 02:26:11.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/config.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1877 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/data_processing_lib.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     3999 2023-12-01 00:17:10.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/external_sync.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     5682 2023-12-01 13:54:03.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/file_ops.py
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     2186 2023-10-21 17:57:29.000000 PhysioKit2-1.8.8/src/PhysioKit2/utils/load_data.py
+drwxr-xr-x   0 jiteshjoshi   (501) staff       (20)        0 2024-04-06 21:27:47.692974 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)    13452 2024-04-06 21:27:47.000000 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/PKG-INFO
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)     1971 2024-04-06 21:27:47.000000 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/SOURCES.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)        1 2024-04-06 21:27:47.000000 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/dependency_links.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      119 2024-04-06 21:27:47.000000 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/entry_points.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)      139 2024-04-06 21:27:47.000000 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/requires.txt
+-rw-r--r--   0 jiteshjoshi   (501) staff       (20)       11 2024-04-06 21:27:47.000000 PhysioKit2-1.8.8/src/PhysioKit2.egg-info/top_level.txt
```

### Comparing `PhysioKit2-1.8.7/LICENSE` & `PhysioKit2-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/PKG-INFO` & `PhysioKit2-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhysioKit2
-Version: 1.8.7
+Version: 1.8.8
 Summary: PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single- and Multi-User Studies
 Home-page: https://github.com/PhysiologicAILab/PhysioKit
 Author: ['Jitesh Joshi', 'Katherine wang', 'Youngjun Cho']
 Author-email: youngjun.cho@ucl.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PhysioKit2-1.8.7/README.md` & `PhysioKit2-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/setup.py` & `PhysioKit2-1.8.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='PhysioKit2',
-      version='1.8.7',
+      version='1.8.8',
       description="PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single- and Multi-User Studies",
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/PhysiologicAILab/PhysioKit',
       author=['Jitesh Joshi', 'Katherine wang', 'Youngjun Cho'],
       author_email='youngjun.cho@ucl.ac.uk',
       license='MIT',
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/process_signals.py` & `PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/process_signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 self.sqi_high_freq = 2.0
                 self.noise_low_freq = 0
                 self.noise_high_freq = self.max_freq_ppg
                 self.SQI_threshold = float(self.exp_dict["SQI_threshold"])
 
                 self.sqi_window_len_sec = float(self.exp_dict["sqi_window_len_sec"])
                 self.sqi_step_sec = float(self.exp_dict["sqi_step_sec"])
-                self.sqa_config = files('PhysioKit2.sqa.config').joinpath('sqa_bvp.json')
+                self.sqa_config = files('PhysioKit2.sqa.config').joinpath('SQAPhysMD.json')
                 self.sqa_inference_obj = sqaPPGInference(self.sqa_config, debug=False)
 
                 self.min_epoch_count = np.round(0.70 * (300 - self.exp_dict["winlen"]) /(self.exp_dict["step_len"]))
 
                 if datadict != "":
                     self.datadict = datadict
                     if os.path.exists(self.datadict):
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/analysis_helper/utils/load_data.py` & `PhysioKit2-1.8.8/src/PhysioKit2/analysis_helper/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/configs/exp_config_phys.json` & `PhysioKit2-1.8.8/src/PhysioKit2/configs/exp_config_phys.json`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/form.ui` & `PhysioKit2-1.8.8/src/PhysioKit2/form.ui`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/form_ui.py` & `PhysioKit2-1.8.8/src/PhysioKit2/form_ui.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/images/banner.png` & `PhysioKit2-1.8.8/src/PhysioKit2/images/banner.png`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/images/color_bar.png` & `PhysioKit2-1.8.8/src/PhysioKit2/images/color_bar.png`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/images/sq_indication.png` & `PhysioKit2-1.8.8/src/PhysioKit2/images/sq_indication.png`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/main.py` & `PhysioKit2-1.8.8/src/PhysioKit2/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
                 self.ui.graphicsView.setScene(self.graphic_scene)
                 self.ui.graphicsView.show()
 
                 if "ppg" in config.CHANNEL_TYPES and self.ui.params_dict["exp"]["assess_signal_quality"]:
                     sq_legend_image = files('PhysioKit2.images').joinpath('sq_indication.png')
                     pixmap = QPixmap(sq_legend_image)
                     self.ui.label_sq_legend.setPixmap(pixmap)                
-                    self.sqa_config = files('PhysioKit2.sqa.config').joinpath('sqa_bvp.json')
+                    self.sqa_config = files('PhysioKit2.sqa.config').joinpath('SQAPhysMD.json')
                     self.ui.ppg_sq_indices = list(np.where(np.array(config.CHANNEL_TYPES) == "ppg")[0])
                     num_sq_ch = len(self.ui.ppg_sq_indices)
                     self.ui.sq_inference_thread = sqaPPGInference(
                         self.sqa_config, config.SAMPLING_RATE, num_sq_ch, axis=1, parent=self)
                     self.ui.sq_inference_thread.update_sq_vec.connect(self.myAnim.addSQData)
                     self.ui.sq_thread_created = True
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/sqa/config/sqa_bvp.json` & `PhysioKit2-1.8.8/src/PhysioKit2/sqa/config/SQAPhysMD.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8452380952380952%*

 * *Differences: {"'ckpt_name'": "'SQAPhysMD.pth'",*

 * * "'data'": "{'window_len_sec': 10}",*

 * * "'model_params'": "{'MD_D': 64, 'MD_R': 8}"}*

```diff
@@ -1,24 +1,24 @@
 {
-    "ckpt_name": "sqa_bvp.pth",
+    "ckpt_name": "SQAPhysMD.pth",
     "data": {
         "sq_resolution_sec": 0,
         "target_fs": 30,
-        "window_len_sec": 5
+        "window_len_sec": 10
     },
     "model_params": {
         "CHEESE_FACTOR": 1,
         "DUAL": false,
         "ETA": 0.9,
         "EVAL_STEPS": 6,
         "HAM_TYPE": "NMF",
         "INPUT_CHANNELS": 1,
         "INV_T": 1,
-        "MD_D": 24,
-        "MD_R": 16,
+        "MD_D": 64,
+        "MD_R": 8,
         "MD_S": 1,
         "RAND_INIT": true,
         "TRAIN_STEPS": 6,
         "VERSION": "V2",
         "ZERO_HAM": true
     },
     "train_params": {
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/sqa/inference.py` & `PhysioKit2-1.8.8/src/PhysioKit2/sqa/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 
 import torch
 import torch.nn as nn
 import matplotlib.pyplot as plt
 from scipy import signal
 
-from PhysioKit2.sqa.model.sqa_bvp import Model as sqPPG
+from PhysioKit2.sqa.model.SQAPhysMD import Model as sqPPG
 from importlib.resources import files
 
 class sqaPPGInference(object):
     """
         The class to infer signal quality for BVP signal
     """
     def __init__(self, model_config, debug=False) -> None:
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/sqa/inference_thread.py` & `PhysioKit2-1.8.8/src/PhysioKit2/sqa/inference_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 
 import torch
 from scipy import signal
 from PySide6.QtCore import Signal, QThread, Signal
 from importlib.resources import files
 
-from PhysioKit2.sqa.model.sqa_bvp import Model as sqPPG
+from PhysioKit2.sqa.model.SQAPhysMD import Model as sqPPG
 
 class sqaPPGInference(QThread):
     """
         The class to infer signal quality for BVP signal
     """
     update_sq_vec = Signal(list)
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/sqa/model/sqa_bvp.py` & `PhysioKit2-1.8.8/src/PhysioKit2/sqa/model/SQAPhysMD.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
 def test_model():
     import os
     import json
     from torch.utils.tensorboard import SummaryWriter
     writer = SummaryWriter('test_run/Model')
 
-    config_path = os.path.join("utils", "sqa", "config", "sqa_bvp.json")
+    config_path = os.path.join("utils", "sqa", "config", "SQAPhysMD.json")
     if os.path.exists(config_path):
         with open(config_path) as json_file:
             model_config = json.load(json_file)
         json_file.close()
     else:
         print("Model config file not found")
         exit()
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/utils/acquisition.py` & `PhysioKit2-1.8.8/src/PhysioKit2/utils/acquisition.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.stop_flag = False
         self.filt_objs = {}
         self.eda_moving_average_window_size = int(self.config.SAMPLING_RATE/4.0)
 
         self.resp_lowcut = 0.1
         self.resp_highcut = 0.5
         self.ppg_lowcut = 0.5
-        self.ppg_highcut = 3.5
+        self.ppg_highcut = 2.5
         self.filt_order = 2
 
         self.bf_out_flag = False
 
         self.ser = serial.Serial()
         self.timeout = None  # specify timeout when using readline()
         self.ports = lp.comports()
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/utils/biofeedback.py` & `PhysioKit2-1.8.8/src/PhysioKit2/utils/biofeedback.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/utils/data_processing_lib.py` & `PhysioKit2-1.8.8/src/PhysioKit2/utils/data_processing_lib.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/utils/external_sync.py` & `PhysioKit2-1.8.8/src/PhysioKit2/utils/external_sync.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/utils/file_ops.py` & `PhysioKit2-1.8.8/src/PhysioKit2/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2/utils/load_data.py` & `PhysioKit2-1.8.8/src/PhysioKit2/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2.egg-info/PKG-INFO` & `PhysioKit2-1.8.8/src/PhysioKit2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhysioKit2
-Version: 1.8.7
+Version: 1.8.8
 Summary: PhysioKit: An Open-Source, Low-Cost Physiological Computing Toolkit for Single- and Multi-User Studies
 Home-page: https://github.com/PhysiologicAILab/PhysioKit
 Author: ['Jitesh Joshi', 'Katherine wang', 'Youngjun Cho']
 Author-email: youngjun.cho@ucl.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PhysioKit2-1.8.7/src/PhysioKit2.egg-info/SOURCES.txt` & `PhysioKit2-1.8.8/src/PhysioKit2.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 src/PhysioKit2/images/__init__.py
 src/PhysioKit2/images/banner.png
 src/PhysioKit2/images/color_bar.png
 src/PhysioKit2/images/sq_indication.png
 src/PhysioKit2/sqa/__init__.py
 src/PhysioKit2/sqa/inference.py
 src/PhysioKit2/sqa/inference_thread.py
+src/PhysioKit2/sqa/ckpt/SQAPhysMD.pth
 src/PhysioKit2/sqa/ckpt/__init__.py
-src/PhysioKit2/sqa/ckpt/sqa_bvp.pth
+src/PhysioKit2/sqa/config/SQAPhysMD.json
 src/PhysioKit2/sqa/config/__init__.py
-src/PhysioKit2/sqa/config/sqa_bvp.json
+src/PhysioKit2/sqa/model/SQAPhysMD.py
 src/PhysioKit2/sqa/model/__init__.py
-src/PhysioKit2/sqa/model/sqa_bvp.py
 src/PhysioKit2/utils/__init__.py
 src/PhysioKit2/utils/acquisition.py
 src/PhysioKit2/utils/biofeedback.py
 src/PhysioKit2/utils/config.py
 src/PhysioKit2/utils/data_processing_lib.py
 src/PhysioKit2/utils/external_sync.py
 src/PhysioKit2/utils/file_ops.py
```

