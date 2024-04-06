# Comparing `tmp/python-microgrid-1.4.0.tar.gz` & `tmp/python-microgrid-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-microgrid-1.4.0.tar", last modified: Tue May 30 20:36:29 2023, max compression
+gzip compressed data, was "python-microgrid-1.4.1.tar", last modified: Sat Apr  6 01:43:15 2024, max compression
```

## Comparing `python-microgrid-1.4.0.tar` & `python-microgrid-1.4.1.tar`

### file list

```diff
@@ -1,373 +1,395 @@
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.972581 python-microgrid-1.4.0/
--rw-r--r--   0 ahalev     (502) staff       (20)     7652 2020-08-13 19:47:38.000000 python-microgrid-1.4.0/LICENSE
--rw-r--r--   0 ahalev     (502) staff       (20)       31 2023-04-05 06:27:25.000000 python-microgrid-1.4.0/MANIFEST.in
--rw-r--r--   0 ahalev     (502) staff       (20)     7383 2023-05-30 20:36:29.972766 python-microgrid-1.4.0/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)     6767 2023-04-19 19:28:19.000000 python-microgrid-1.4.0/README.md
--rw-r--r--   0 ahalev     (502) staff       (20)      191 2023-03-29 00:42:14.000000 python-microgrid-1.4.0/pyproject.toml
--rw-r--r--   0 ahalev     (502) staff       (20)      124 2023-05-30 20:36:29.973139 python-microgrid-1.4.0/setup.cfg
--rw-r--r--   0 ahalev     (502) staff       (20)     1652 2023-04-08 01:25:01.000000 python-microgrid-1.4.0/setup.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.745041 python-microgrid-1.4.0/src/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.748528 python-microgrid-1.4.0/src/pymgrid/
--rw-r--r--   0 ahalev     (502) staff       (20)    26580 2023-02-11 01:32:23.000000 python-microgrid-1.4.0/src/pymgrid/MicrogridGenerator.py
--rw-r--r--   0 ahalev     (502) staff       (20)      513 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.748794 python-microgrid-1.4.0/src/pymgrid/_deprecated/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.753828 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/
--rw-r--r--   0 ahalev     (502) staff       (20)    21520 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Environment.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1991 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Preprocessing.py
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    27816 2022-12-17 17:21:34.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1616 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1614 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csda.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1979 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    55258 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/non_modular_microgrid.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.755318 python-microgrid-1.4.0/src/pymgrid/algos/
--rw-r--r--   0 ahalev     (502) staff       (20)    17127 2022-12-17 17:21:34.000000 python-microgrid-1.4.0/src/pymgrid/algos/Control.py
--rw-r--r--   0 ahalev     (502) staff       (20)       82 2022-12-10 02:06:45.000000 python-microgrid-1.4.0/src/pymgrid/algos/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.755831 python-microgrid-1.4.0/src/pymgrid/algos/mpc/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-10-25 19:17:19.000000 python-microgrid-1.4.0/src/pymgrid/algos/mpc/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    44174 2023-04-27 05:44:00.000000 python-microgrid-1.4.0/src/pymgrid/algos/mpc/mpc.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.757722 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/
--rw-r--r--   0 ahalev     (502) staff       (20)       99 2022-12-17 03:06:50.000000 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     7099 2023-04-25 23:15:20.000000 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2783 2023-02-04 17:02:47.000000 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list_element.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.759141 python-microgrid-1.4.0/src/pymgrid/algos/rbc/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:00:07.000000 python-microgrid-1.4.0/src/pymgrid/algos/rbc/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    13272 2022-12-17 03:06:50.000000 python-microgrid-1.4.0/src/pymgrid/algos/rbc/_nonmodular_rbc.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4139 2023-04-27 05:44:00.000000 python-microgrid-1.4.0/src/pymgrid/algos/rbc/rbc.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.759965 python-microgrid-1.4.0/src/pymgrid/algos/saa/
--rw-r--r--   0 ahalev     (502) staff       (20)       43 2022-10-25 19:17:19.000000 python-microgrid-1.4.0/src/pymgrid/algos/saa/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     7336 2022-12-17 06:16:17.000000 python-microgrid-1.4.0/src/pymgrid/algos/saa/saa.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.780995 python-microgrid-1.4.0/src/pymgrid/convert/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/convert/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      367 2022-11-30 07:09:17.000000 python-microgrid-1.4.0/src/pymgrid/convert/conversion_test_sandbox.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2635 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/convert/convert.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4368 2022-12-10 02:06:16.000000 python-microgrid-1.4.0/src/pymgrid/convert/get_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)    10537 2023-05-19 17:52:32.000000 python-microgrid-1.4.0/src/pymgrid/convert/to_nonmodular_ops.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.781754 python-microgrid-1.4.0/src/pymgrid/data/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.781890 python-microgrid-1.4.0/src/pymgrid/data/co2/
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/co2/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.782391 python-microgrid-1.4.0/src/pymgrid/data/load/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/load/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.782582 python-microgrid-1.4.0/src/pymgrid/data/pv/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/pv/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.783545 python-microgrid-1.4.0/src/pymgrid/data/scenario/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-11-09 16:21:41.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/.DS_Store
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743411 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.802322 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:41:28.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.804022 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:51.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.804454 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:57.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.804751 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71000 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.805408 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    95750 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.806001 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41119 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2348 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.806324 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.729928 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730138 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.806698 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70450 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.807195 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98740 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.807838 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43703 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2955 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.808253 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730346 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730572 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.808588 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.809061 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99947 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.809631 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    40530 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2974 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.810178 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730815 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731031 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.810597 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.811040 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98933 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.811572 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    44288 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2340 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.811908 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731268 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731493 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.812275 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.812931 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   101899 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.813497 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    40454 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2334 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.813764 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731728 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731941 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.814063 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.814569 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   101801 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.814985 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2947 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.815366 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.732157 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.732379 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.815685 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.816031 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    92053 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.817898 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43518 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2336 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.818215 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.735725 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.735987 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.818506 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98126 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.819141 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43802 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2425 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.819589 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736240 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736474 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.819848 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.820154 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    92018 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.820572 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43220 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2382 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.820826 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736711 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736858 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.821487 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    91889 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.843741 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41880 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2439 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.844390 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737077 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737305 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.844914 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.845615 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   101812 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.846351 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42455 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2945 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.846840 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737535 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737670 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.847238 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98334 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.847950 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41498 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2448 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.849729 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737889 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738021 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.850292 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98535 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.864132 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42761 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2433 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.865233 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738251 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738392 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.866229 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100312 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.868494 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43495 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2423 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.868859 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738643 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738795 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.869179 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100892 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.871209 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43999 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2433 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.872151 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739044 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739282 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.872619 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.873871 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99857 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.878056 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42241 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2951 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.878454 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739510 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739661 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.878763 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    97388 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.879368 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42142 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2415 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.879740 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739982 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740260 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.880157 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70790 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.880888 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    91809 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.881443 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42978 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2962 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.904170 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740522 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740673 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.905032 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100230 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.905686 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42513 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2422 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.906065 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740922 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741276 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.906379 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.907322 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99793 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.942276 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42889 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2333 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.943284 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741503 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741641 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.943802 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98745 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.944345 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    38378 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2428 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.944616 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741861 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.742076 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.944923 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.947170 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100276 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.947630 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43091 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2372 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.948041 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.742404 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.742596 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.948333 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99461 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.948793 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42132 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2414 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.949048 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743022 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743322 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.949364 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    72045 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.949828 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    92074 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.950236 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41768 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2974 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.950731 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743554 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743770 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.951036 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71462 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.951443 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98674 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.951973 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    44237 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2991 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml
--rw-r--r--   0 ahalev     (502) staff       (20)  7790780 2022-11-09 16:19:50.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25.pkl
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.952256 python-microgrid-1.4.0/src/pymgrid/envs/
--rw-r--r--   0 ahalev     (502) staff       (20)      141 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/envs/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.952989 python-microgrid-1.4.0/src/pymgrid/envs/base/
--rw-r--r--   0 ahalev     (502) staff       (20)       35 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/base/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    14870 2023-05-30 20:36:18.000000 python-microgrid-1.4.0/src/pymgrid/envs/base/base.py
--rw-r--r--   0 ahalev     (502) staff       (20)      400 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/base/skip_init.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.953374 python-microgrid-1.4.0/src/pymgrid/envs/continuous/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/continuous/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     8940 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/envs/continuous/continuous.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.953689 python-microgrid-1.4.0/src/pymgrid/envs/discrete/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/discrete/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     5524 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/envs/discrete/discrete.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.954324 python-microgrid-1.4.0/src/pymgrid/forecast/
--rw-r--r--   0 ahalev     (502) staff       (20)      119 2022-12-10 02:06:16.000000 python-microgrid-1.4.0/src/pymgrid/forecast/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    14675 2023-05-12 00:09:47.000000 python-microgrid-1.4.0/src/pymgrid/forecast/forecaster.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.955863 python-microgrid-1.4.0/src/pymgrid/microgrid/
--rw-r--r--   0 ahalev     (502) staff       (20)       55 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      784 2022-11-23 02:52:46.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/convert_scenario_sandbox.py
--rw-r--r--   0 ahalev     (502) staff       (20)    40304 2023-05-30 20:36:18.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/microgrid.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4283 2022-11-23 02:52:46.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/modular_microgrid_sandbox.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.957862 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/
--rw-r--r--   0 ahalev     (502) staff       (20)      158 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2484 2023-05-30 20:35:30.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/analyze_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)      565 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/base.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1595 2023-05-30 20:35:30.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/baseline_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1207 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)      471 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/pv_curtailment_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)      504 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/rescale_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)      211 2023-03-17 04:48:01.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/serialization_sandbox.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.958936 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/
--rw-r--r--   0 ahalev     (502) staff       (20)      129 2023-03-04 01:40:10.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      627 2023-03-04 01:40:10.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/base.py
--rw-r--r--   0 ahalev     (502) staff       (20)      383 2023-03-18 01:38:19.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/deterministic.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1025 2023-03-09 22:23:21.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/stochastic.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.959455 python-microgrid-1.4.0/src/pymgrid/microgrid/utils/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-11-23 03:05:26.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/utils/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2018 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/utils/step.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.961657 python-microgrid-1.4.0/src/pymgrid/modules/
--rw-r--r--   0 ahalev     (502) staff       (20)      316 2023-05-19 17:52:32.000000 python-microgrid-1.4.0/src/pymgrid/modules/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.964310 python-microgrid-1.4.0/src/pymgrid/modules/base/
--rw-r--r--   0 ahalev     (502) staff       (20)      122 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    32031 2023-05-23 21:18:26.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/base_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.965106 python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    12400 2023-04-28 04:26:05.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/base_timeseries_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.965696 python-microgrid-1.4.0/src/pymgrid/modules/battery/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    13095 2023-05-19 18:57:42.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/battery_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.967354 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/
--rw-r--r--   0 ahalev     (502) staff       (20)      169 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1077 2023-04-06 17:45:24.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/biased_transition_model.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1196 2023-04-05 06:27:25.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/decay_transition_model.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3566 2023-04-05 06:27:25.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/transition_model.py
--rw-r--r--   0 ahalev     (502) staff       (20)    18628 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/modules/genset_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)    11686 2023-05-30 20:36:18.000000 python-microgrid-1.4.0/src/pymgrid/modules/grid_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4020 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/modules/load_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)    16512 2023-05-25 23:30:21.000000 python-microgrid-1.4.0/src/pymgrid/modules/module_container.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3999 2023-05-19 18:57:42.000000 python-microgrid-1.4.0/src/pymgrid/modules/renewable_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3102 2023-05-19 18:57:42.000000 python-microgrid-1.4.0/src/pymgrid/modules/unbalanced_energy_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.969764 python-microgrid-1.4.0/src/pymgrid/utils/
--rw-r--r--   0 ahalev     (502) staff       (20)    46856 2022-02-25 19:51:24.000000 python-microgrid-1.4.0/src/pymgrid/utils/DataGenerator.py
--rw-r--r--   0 ahalev     (502) staff       (20)       82 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/utils/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      259 2023-04-28 04:22:30.000000 python-microgrid-1.4.0/src/pymgrid/utils/dry_run.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1781 2023-05-12 23:54:14.000000 python-microgrid-1.4.0/src/pymgrid/utils/eq.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1550 2023-05-12 00:09:47.000000 python-microgrid-1.4.0/src/pymgrid/utils/logger.py
--rw-r--r--   0 ahalev     (502) staff       (20)      632 2023-02-01 02:22:51.000000 python-microgrid-1.4.0/src/pymgrid/utils/ray.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4056 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/utils/serialize.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.970833 python-microgrid-1.4.0/src/pymgrid/utils/space/
--rw-r--r--   0 ahalev     (502) staff       (20)      103 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/utils/space/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    15426 2023-05-25 23:30:21.000000 python-microgrid-1.4.0/src/pymgrid/utils/space/space.py
--rw-r--r--   0 ahalev     (502) staff       (20)      484 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/utils/space/utils.py
--rw-r--r--   0 ahalev     (502) staff       (20)       22 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/version.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.971866 python-microgrid-1.4.0/src/python_microgrid.egg-info/
--rw-r--r--   0 ahalev     (502) staff       (20)     7383 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)    12208 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 ahalev     (502) staff       (20)      343 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/requires.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        8 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/top_level.txt
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.972287 python-microgrid-1.4.0/tests/
--rw-r--r--   0 ahalev     (502) staff       (20)     2474 2022-12-10 02:06:16.000000 python-microgrid-1.4.0/tests/test_microgridgenerator.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2071 2022-12-02 00:00:07.000000 python-microgrid-1.4.0/tests/test_nonmodular_microgrid.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.265614 python-microgrid-1.4.1/
+-rw-r--r--   0 ahalev     (502) staff       (20)     7652 2020-08-13 19:47:38.000000 python-microgrid-1.4.1/LICENSE
+-rw-r--r--   0 ahalev     (502) staff       (20)       22 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/MANIFEST.in
+-rw-r--r--   0 ahalev     (502) staff       (20)     7384 2024-04-06 01:43:15.265716 python-microgrid-1.4.1/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)     6768 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/README.md
+-rw-r--r--   0 ahalev     (502) staff       (20)      191 2023-03-29 00:42:14.000000 python-microgrid-1.4.1/pyproject.toml
+-rw-r--r--   0 ahalev     (502) staff       (20)      124 2024-04-06 01:43:15.266006 python-microgrid-1.4.1/setup.cfg
+-rw-r--r--   0 ahalev     (502) staff       (20)     1652 2023-04-08 01:25:01.000000 python-microgrid-1.4.1/setup.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.146418 python-microgrid-1.4.1/src/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.147989 python-microgrid-1.4.1/src/pymgrid/
+-rw-r--r--   0 ahalev     (502) staff       (20)    26896 2024-04-06 01:42:10.000000 python-microgrid-1.4.1/src/pymgrid/MicrogridGenerator.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      513 2023-04-01 21:07:37.000000 python-microgrid-1.4.1/src/pymgrid/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.148181 python-microgrid-1.4.1/src/pymgrid/_deprecated/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.149812 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/
+-rw-r--r--   0 ahalev     (502) staff       (20)    21520 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/Environment.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1991 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/Preprocessing.py
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    27816 2022-12-17 17:21:34.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_csca.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1616 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1614 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_csda.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1979 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    55258 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/_deprecated/non_modular_microgrid.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.150263 python-microgrid-1.4.1/src/pymgrid/algos/
+-rw-r--r--   0 ahalev     (502) staff       (20)    17127 2022-12-17 17:21:34.000000 python-microgrid-1.4.1/src/pymgrid/algos/Control.py
+-rw-r--r--   0 ahalev     (502) staff       (20)       82 2022-12-10 02:06:45.000000 python-microgrid-1.4.1/src/pymgrid/algos/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.150546 python-microgrid-1.4.1/src/pymgrid/algos/mpc/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-10-25 19:17:19.000000 python-microgrid-1.4.1/src/pymgrid/algos/mpc/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    44199 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/algos/mpc/mpc.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.151589 python-microgrid-1.4.1/src/pymgrid/algos/priority_list/
+-rw-r--r--   0 ahalev     (502) staff       (20)       99 2022-12-17 03:06:50.000000 python-microgrid-1.4.1/src/pymgrid/algos/priority_list/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     7099 2023-04-25 23:15:20.000000 python-microgrid-1.4.1/src/pymgrid/algos/priority_list/priority_list.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2783 2023-02-04 17:02:47.000000 python-microgrid-1.4.1/src/pymgrid/algos/priority_list/priority_list_element.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.152220 python-microgrid-1.4.1/src/pymgrid/algos/rbc/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:00:07.000000 python-microgrid-1.4.1/src/pymgrid/algos/rbc/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    13272 2022-12-17 03:06:50.000000 python-microgrid-1.4.1/src/pymgrid/algos/rbc/_nonmodular_rbc.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4140 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/algos/rbc/rbc.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.152606 python-microgrid-1.4.1/src/pymgrid/algos/saa/
+-rw-r--r--   0 ahalev     (502) staff       (20)       43 2022-10-25 19:17:19.000000 python-microgrid-1.4.1/src/pymgrid/algos/saa/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     7336 2022-12-17 06:16:17.000000 python-microgrid-1.4.1/src/pymgrid/algos/saa/saa.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.153562 python-microgrid-1.4.1/src/pymgrid/convert/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/convert/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      367 2022-11-30 07:09:17.000000 python-microgrid-1.4.1/src/pymgrid/convert/conversion_test_sandbox.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2673 2024-04-06 01:42:10.000000 python-microgrid-1.4.1/src/pymgrid/convert/convert.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4368 2024-04-06 01:42:10.000000 python-microgrid-1.4.1/src/pymgrid/convert/get_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    10537 2023-05-19 17:52:32.000000 python-microgrid-1.4.1/src/pymgrid/convert/to_nonmodular_ops.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.154026 python-microgrid-1.4.1/src/pymgrid/data/
+-rw-r--r--   0 ahalev     (502) staff       (20)     8196 2022-11-11 21:35:03.000000 python-microgrid-1.4.1/src/pymgrid/data/.DS_Store
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.154762 python-microgrid-1.4.1/src/pymgrid/data/co2/
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/co2/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)   104138 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/co2/co2_caiso.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)   104185 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/co2/co2_duke.csv
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.157229 python-microgrid-1.4.1/src/pymgrid/data/load/
+-rw-r--r--   0 ahalev     (502) staff       (20)   104229 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/load/RefBldgFullServiceRestaurantNew2004_v1.3_7.1_6A_USA_MN_MINNEAPOLIS.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)   104172 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/load/RefBldgHospitalNew2004_7.1_5.0_3C_USA_CA_SAN_FRANCISCO.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)   104195 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/load/RefBldgLargeHotelNew2004_v1.3_7.1_4A_USA_MD_BALTIMORE.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)   104177 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/load/RefBldgLargeOfficeNew2004_v1.3_7.1_5A_USA_IL_CHICAGO-OHARE.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)   104200 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/load/RefBldgPrimarySchoolNew2004_v1.3_7.1_2A_USA_TX_HOUSTON.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/load/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.158589 python-microgrid-1.4.1/src/pymgrid/data/pv/
+-rw-r--r--   0 ahalev     (502) staff       (20)    25648 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/pv/Houston_722430TYA.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)    25324 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/pv/Minneapolis_726580TYA.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)    25244 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/pv/NewYork_744860TYA.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)    25499 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/pv/Raleigh_723060TYA.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)    25574 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/pv/SanFrancisco_724940TYA.csv
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/pv/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.159057 python-microgrid-1.4.1/src/pymgrid/data/scenario/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-11-09 16:21:41.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/.DS_Store
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.145161 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.168743 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:41:28.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.170622 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:51.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.170992 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:57.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.171164 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71000 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.171897 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    95750 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.172477 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41119 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2348 2023-09-07 23:44:18.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.172916 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.137686 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.137836 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.173223 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70450 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.173545 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98740 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.173967 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43703 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2949 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.174225 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.137989 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.138145 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.174495 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.174972 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99947 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.175439 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    40530 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2968 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.175737 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.138314 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.138466 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.175977 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.176288 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98933 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.176956 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    44288 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2340 2023-09-07 23:44:35.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.177387 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.138622 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.138821 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.177570 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.177832 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   101899 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.178250 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    40454 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2334 2023-09-07 23:44:36.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.178475 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139017 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139188 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.178704 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.179147 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   101801 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.179603 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41997 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2941 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.179800 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139361 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139517 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.180025 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.180382 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    92053 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.180920 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43518 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2336 2023-09-07 23:44:36.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.181147 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139675 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139771 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.181482 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98126 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.181921 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43802 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2419 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.182131 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.139932 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.140088 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.182309 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.182690 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    92018 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.186198 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43220 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2382 2023-09-07 23:44:36.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.186421 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.140250 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.140357 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.186676 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    91889 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.187060 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41880 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2433 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.187254 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.140515 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.140668 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.187494 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.187841 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   101812 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.188299 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42455 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2939 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.188753 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.140827 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.141175 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.189001 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98334 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.189366 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41498 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2442 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.189589 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.141447 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.141580 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.189951 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98535 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.190380 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42761 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2427 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.190592 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.141758 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.141885 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.192182 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100312 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.192697 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43495 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2417 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.193055 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.142049 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.142253 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.193432 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100892 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.193947 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43999 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2427 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.194230 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.142458 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.142627 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.194498 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.195022 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99857 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.195485 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42241 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2945 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.195683 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.142817 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.142927 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.195914 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    97388 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.196278 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42142 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2409 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.196476 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.143097 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.143263 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.196816 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70790 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.197336 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    91809 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.197707 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42978 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2956 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.198050 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.143424 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.143527 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.198295 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100230 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.198762 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42513 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2416 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.199069 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.143718 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.143891 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.199734 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.220447 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99793 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.221786 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42889 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2333 2023-09-07 23:44:34.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.222056 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144075 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144171 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.222366 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98745 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.222951 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    38378 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2422 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.223244 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144350 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144516 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.223500 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.224103 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100276 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.224625 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43091 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2372 2023-09-07 23:44:34.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.225019 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144680 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144782 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.225384 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99461 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.225855 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42132 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2408 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.226089 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.144947 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.145101 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.226353 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    72045 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.226703 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    92074 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.227053 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41768 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2968 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.227749 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.145261 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.145413 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.227982 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71462 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.247929 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98674 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.248742 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    44237 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2985 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml
+-rw-r--r--   0 ahalev     (502) staff       (20)  7790780 2022-11-09 16:19:50.000000 python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25.pkl
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.249114 python-microgrid-1.4.1/src/pymgrid/envs/
+-rw-r--r--   0 ahalev     (502) staff       (20)      141 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/envs/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.249972 python-microgrid-1.4.1/src/pymgrid/envs/base/
+-rw-r--r--   0 ahalev     (502) staff       (20)       35 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/envs/base/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    14874 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/envs/base/base.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      400 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/envs/base/skip_init.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.250306 python-microgrid-1.4.1/src/pymgrid/envs/continuous/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/envs/continuous/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     9320 2023-12-14 23:55:20.000000 python-microgrid-1.4.1/src/pymgrid/envs/continuous/continuous.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.250746 python-microgrid-1.4.1/src/pymgrid/envs/discrete/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/envs/discrete/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     5524 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/envs/discrete/discrete.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.251664 python-microgrid-1.4.1/src/pymgrid/errors/
+-rw-r--r--   0 ahalev     (502) staff       (20)      113 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/errors/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      579 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/errors/env_signature.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      158 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/errors/error.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      192 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/errors/warnings.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.252077 python-microgrid-1.4.1/src/pymgrid/forecast/
+-rw-r--r--   0 ahalev     (502) staff       (20)      119 2022-12-10 02:06:16.000000 python-microgrid-1.4.1/src/pymgrid/forecast/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    15241 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/forecast/forecaster.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.253528 python-microgrid-1.4.1/src/pymgrid/microgrid/
+-rw-r--r--   0 ahalev     (502) staff       (20)       55 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      784 2022-11-23 02:52:46.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/convert_scenario_sandbox.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    40621 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/microgrid.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      285 2024-01-26 19:42:41.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/modular_microgrid_sandbox.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.255596 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/
+-rw-r--r--   0 ahalev     (502) staff       (20)      270 2023-08-30 19:22:58.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3554 2023-08-30 19:22:58.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/base.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2254 2023-09-28 21:19:13.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/baseline_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1111 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      471 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/pv_curtailment_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1952 2023-09-15 21:51:49.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/rescale_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      757 2023-08-30 19:22:58.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/sequential.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      524 2024-04-06 01:42:10.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/standardization_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      211 2023-03-17 04:48:01.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/serialization_sandbox.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.256587 python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/
+-rw-r--r--   0 ahalev     (502) staff       (20)      129 2023-03-04 01:40:10.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      627 2023-03-04 01:40:10.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/base.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      383 2023-03-18 01:38:19.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/deterministic.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1025 2023-03-09 22:23:21.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/stochastic.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.256994 python-microgrid-1.4.1/src/pymgrid/microgrid/utils/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-11-23 03:05:26.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/utils/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2137 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/microgrid/utils/step.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.259017 python-microgrid-1.4.1/src/pymgrid/modules/
+-rw-r--r--   0 ahalev     (502) staff       (20)      316 2023-05-19 17:52:32.000000 python-microgrid-1.4.1/src/pymgrid/modules/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.259497 python-microgrid-1.4.1/src/pymgrid/modules/base/
+-rw-r--r--   0 ahalev     (502) staff       (20)      122 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/modules/base/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    32965 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/base/base_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.259891 python-microgrid-1.4.1/src/pymgrid/modules/base/timeseries/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.1/src/pymgrid/modules/base/timeseries/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    12364 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/base/timeseries/base_timeseries_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.260166 python-microgrid-1.4.1/src/pymgrid/modules/battery/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2023-04-01 21:07:37.000000 python-microgrid-1.4.1/src/pymgrid/modules/battery/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    13283 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/battery/battery_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.260963 python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/
+-rw-r--r--   0 ahalev     (502) staff       (20)      196 2023-12-14 23:55:20.000000 python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1077 2023-04-06 17:45:24.000000 python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/biased_transition_model.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2746 2023-12-14 23:55:20.000000 python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/decay_transition_model.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3566 2023-04-05 06:27:25.000000 python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/transition_model.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    18936 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/genset_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    11933 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/grid_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4207 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/load_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    16487 2023-09-28 21:40:56.000000 python-microgrid-1.4.1/src/pymgrid/modules/module_container.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4187 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/modules/renewable_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3102 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/modules/unbalanced_energy_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.263495 python-microgrid-1.4.1/src/pymgrid/utils/
+-rw-r--r--   0 ahalev     (502) staff       (20)    46856 2022-02-25 19:51:24.000000 python-microgrid-1.4.1/src/pymgrid/utils/DataGenerator.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      118 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/utils/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      944 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/utils/code_link.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1598 2023-12-20 18:16:54.000000 python-microgrid-1.4.1/src/pymgrid/utils/deprecation.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      259 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/utils/dry_run.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1781 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/utils/eq.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1550 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/utils/logger.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      632 2023-02-01 02:22:51.000000 python-microgrid-1.4.1/src/pymgrid/utils/ray.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1089 2024-04-06 01:42:10.000000 python-microgrid-1.4.1/src/pymgrid/utils/running_mean_std.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4141 2023-08-30 19:22:58.000000 python-microgrid-1.4.1/src/pymgrid/utils/serialize.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.264188 python-microgrid-1.4.1/src/pymgrid/utils/space/
+-rw-r--r--   0 ahalev     (502) staff       (20)      103 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/utils/space/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    15450 2023-12-14 23:55:20.000000 python-microgrid-1.4.1/src/pymgrid/utils/space/space.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      484 2023-08-30 19:22:04.000000 python-microgrid-1.4.1/src/pymgrid/utils/space/utils.py
+-rw-r--r--   0 ahalev     (502) staff       (20)       22 2024-04-06 01:42:38.000000 python-microgrid-1.4.1/src/pymgrid/version.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.264944 python-microgrid-1.4.1/src/python_microgrid.egg-info/
+-rw-r--r--   0 ahalev     (502) staff       (20)     7384 2024-04-06 01:43:15.000000 python-microgrid-1.4.1/src/python_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)    13230 2024-04-06 01:43:15.000000 python-microgrid-1.4.1/src/python_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2024-04-06 01:43:15.000000 python-microgrid-1.4.1/src/python_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)      343 2024-04-06 01:43:15.000000 python-microgrid-1.4.1/src/python_microgrid.egg-info/requires.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        8 2024-04-06 01:43:15.000000 python-microgrid-1.4.1/src/python_microgrid.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2024-04-06 01:43:15.265347 python-microgrid-1.4.1/tests/
+-rw-r--r--   0 ahalev     (502) staff       (20)     2474 2022-12-10 02:06:16.000000 python-microgrid-1.4.1/tests/test_microgridgenerator.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2071 2022-12-02 00:00:07.000000 python-microgrid-1.4.1/tests/test_nonmodular_microgrid.py
```

### Comparing `python-microgrid-1.4.0/LICENSE` & `python-microgrid-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/PKG-INFO` & `python-microgrid-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-microgrid
-Version: 1.4.0
+Version: 1.4.1
 Summary: A simulator for tertiary control of electrical microgrids
-Download-URL: https://github.com/ahalev/python-microgrid/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/ahalev/python-microgrid/archive/refs/tags/v1.4.1.tar.gz
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: GNU LGPL 3.0
 Project-URL: Source Code, https://github.com/ahalev/python-microgrid
 Project-URL: Documentation, https://python-microgrid.readthedocs.io/
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -117,15 +117,15 @@
 Running the microgrid is straightforward. Simply pass an action for each fixed module to `microgrid.run`. The microgrid
 can also provide you a random action by calling `microgrid.sample_action.` Once the microgrid has been run for a
 certain number of steps, results can be viewed by calling microgrid.get_log.
 
 ```python
 >> for j in range(10):
 >>    action = microgrid.sample_action(strict_bound=True)
->>    microgrid.run(action)
+>>    microgrid.step(action)
 
 >> microgrid.get_log(drop_singleton_key=True)
 
       genset  ...                     balance
       reward  ... fixed_absorbed_by_microgrid
 0  -5.000000  ...                   10.672095
 1 -14.344353  ...                   50.626726
```

### Comparing `python-microgrid-1.4.0/README.md` & `python-microgrid-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 Running the microgrid is straightforward. Simply pass an action for each fixed module to `microgrid.run`. The microgrid
 can also provide you a random action by calling `microgrid.sample_action.` Once the microgrid has been run for a
 certain number of steps, results can be viewed by calling microgrid.get_log.
 
 ```python
 >> for j in range(10):
 >>    action = microgrid.sample_action(strict_bound=True)
->>    microgrid.run(action)
+>>    microgrid.step(action)
 
 >> microgrid.get_log(drop_singleton_key=True)
 
       genset  ...                     balance
       reward  ... fixed_absorbed_by_microgrid
 0  -5.000000  ...                   10.672095
 1 -14.344353  ...                   50.626726
```

### Comparing `python-microgrid-1.4.0/setup.py` & `python-microgrid-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/MicrogridGenerator.py` & `python-microgrid-1.4.1/src/pymgrid/MicrogridGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,35 +108,41 @@
         >>> m_gen.print_mg_parameters()
         """
 
 
     def __init__(self, nb_microgrid=10,
                  random_seed=42,
                  timestep=1,
-                 path=str(Path(__file__).parent)):
+                 path=str(Path(__file__).parent),
+                 verbose=True):
         
         np.random.seed(random_seed)
         self.microgrids= [] # generate a list of microgrid object
         #self.annual_load
         self.nb_microgrids=nb_microgrid
         self.timestep=1
         self.path=path
+        self.verbose = verbose
 
 
     ###########################################
     #utility functions
     ###########################################
     def _get_random_file(self, path):
         """ Based on a path, and a folder containing data files, return a file chosen randomly."""
         from pathlib import Path
         _path = Path(path)
         data_files = list(_path.glob("*.csv"))
         if not len(data_files):
             raise NameError(f"Unable to find csv data files in {path}")
-        return pd.read_csv(np.random.choice(data_files))
+
+        data_file = np.random.choice(data_files)
+        if self.verbose:
+            print(f'{data_file=}')
+        return pd.read_csv(data_file)
 
     def _scale_ts(self, df_ts, size, scaling_method='sum'):
         """ Scales a time series based on either the sum or the maximum of the time series."""
 
         actual_ratio=1
         if scaling_method =='sum':
             actual_ratio = size/df_ts.sum()#.values[0]
@@ -370,36 +376,38 @@
         return size
 
     def _size_genset(self, load, max_operating_loading = 0.9):
         """ Function that returns the maximum power a genset. """
         #random number > 3 < 20
         # polynomial for fuel consumption
 
-        _size_genset = int(np.ceil(np.max(load)/max_operating_loading))
+        _size_genset = int(np.ceil(np.max(load, axis=0)/max_operating_loading))
 
         return _size_genset
 
 
     def _size_battery(self, load):
         """ Function that returns the capacity of the battery, equivalent to 3 to 5 hours of mean load. """
         #energy duration
-        battery = int(np.ceil(np.random.randint(low=3,high=6)*np.mean(load).item()))
+        battery = int(np.ceil(np.random.randint(low=3,high=6)*np.mean(load, axis=0).item()))
         return battery
 
 
     ###########################################
     #generate the microgrid
     ###########################################
 
     def generate_microgrid(self, modular=True, verbose=False):
         """ Function used to generate the nb_microgrids to append them to the microgrids list. """
 
         convert = lambda x: x.to_modular() if modular else x
 
         for i in range(self.nb_microgrids):
+            if self.verbose:
+                print(f'Generating microgrid ({i})')
             #size=self._size_mg()
             self.microgrids.append(convert(self._create_microgrid()))
         
         if verbose and not modular:
             self.print_mg_parameters()
 
         return self
@@ -450,14 +458,18 @@
         # get the sizing data
         # create microgrid object and append
         # return the list
 
         bin_genset, bin_grid = self._bin_genset_grid()
 
         architecture = {'PV':1, 'battery':1, 'genset':bin_genset, 'grid':bin_grid}
+
+        if self.verbose:
+            print(f'{architecture=}')
+
         size_load = self._size_load()
         load = self._scale_ts(self._get_load_ts(), size_load, scaling_method='max') #obtain dataframe of loads
         size = self._size_mg(load, size_load) #obtain a dictionary of mg sizing components
         column_actions=[]
         column_actual_production=[]
         column_cost = []
         grid_ts=[]
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/__init__.py` & `python-microgrid-1.4.1/src/pymgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Environment.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/Environment.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Preprocessing.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_csca.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csda.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_csda.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/_deprecated/non_modular_microgrid.py` & `python-microgrid-1.4.1/src/pymgrid/_deprecated/non_modular_microgrid.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/Control.py` & `python-microgrid-1.4.1/src/pymgrid/algos/Control.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/mpc/mpc.py` & `python-microgrid-1.4.1/src/pymgrid/algos/mpc/mpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
     def _run_mpc_on_modular(self, forecast_steps=None, verbose=False):
 
         num_iter = self._get_num_iter(forecast_steps)
 
         for _ in tqdm(range(num_iter), desc="MPC Progress", disable=(not verbose)):
             control = self.get_action()
 
-            _, _, done, _ = self.microgrid.run(control, normalized=False)
+            _, _, done, _ = self.microgrid.step(control, normalized=False)
 
             if done:
                 break
 
         return self.microgrid.get_log()
 
     def get_action(self, verbose=0):
@@ -902,17 +902,17 @@
 
         if grid_import > 0 and grid_export > 0:
             if verbose and not np.isclose([grid_import, grid_export], 0, atol=1e-4).any():
                 warn(f"grid_import={grid_import} and grid_export={grid_export} are both nonzero. "
                     f"Flattening to the difference, leading to a {'import' if grid_diff > 0 else 'export'} of {grid_diff}.")
 
         if "grid" in self.microgrid_module_names.keys():
-            control[self.microgrid_module_names["grid"]] = [grid_diff]
+            control[self.microgrid_module_names["grid"]] = [np.array([grid_diff])]
 
-        control[self.microgrid_module_names["battery"]] = [battery_diff]
+        control[self.microgrid_module_names["battery"]] = [np.array([battery_diff])]
 
         return control
 
     def _get_modular_state_values(self):
 
         load_state = -1.0 * self.microgrid.modules[self.microgrid_module_names["load"]].item().state # state is negative, want positive values.
         pv_state = self.microgrid.modules[self.microgrid_module_names["renewable"]].item().state
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list.py` & `python-microgrid-1.4.1/src/pymgrid/algos/priority_list/priority_list.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list_element.py` & `python-microgrid-1.4.1/src/pymgrid/algos/priority_list/priority_list_element.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/rbc/_nonmodular_rbc.py` & `python-microgrid-1.4.1/src/pymgrid/algos/rbc/_nonmodular_rbc.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/rbc/rbc.py` & `python-microgrid-1.4.1/src/pymgrid/algos/rbc/rbc.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             Results of running the rule-based control algorithm.
 
         """
         self.reset()
 
         for _ in tqdm(range(self._get_num_iter(max_steps)), desc="RBC Progress", disable=(not verbose)):
             action = self.get_action()
-            _, _, done, _ = self.microgrid.run(action, normalized=False)
+            _, _, done, _ = self.microgrid.step(action, normalized=False)
             if done:
                 break
 
         return self.microgrid.get_log(as_frame=True)
 
     def _get_num_iter(self, max_steps):
         if max_steps is not None:
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/algos/saa/saa.py` & `python-microgrid-1.4.1/src/pymgrid/algos/saa/saa.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/convert/convert.py` & `python-microgrid-1.4.1/src/pymgrid/convert/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pymgrid.convert.to_nonmodular_ops import check_viability, add_params_from_module, get_empty_params, finalize_params
 
 
 def to_modular(nonmodular, raise_errors=False):
     modules = [('load', get_module('load', nonmodular, raise_errors)),
                ('unbalanced_energy', get_module('unbalanced_energy', nonmodular, raise_errors))]
     for component, exists in nonmodular.architecture.items():
+        component = component.lower()
         if exists:
             module = get_module(component, nonmodular, raise_errors)
             modules.append((component, module))
     return Microgrid(modules, add_unbalanced_module=False)
 
 
 def to_nonmodular(modular):
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/convert/get_module.py` & `python-microgrid-1.4.1/src/pymgrid/convert/get_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from pymgrid.modules import LoadModule, RenewableModule, BatteryModule, GridModule, GensetModule, UnbalancedEnergyModule
 
 
 def get_module(component, nonmodular, raise_errors):
     if component == 'load':
         return get_load_module(nonmodular, raise_errors)
-    elif component == 'PV':
+    elif component == 'pv':
         return get_pv_module(nonmodular, raise_errors)
     elif component == 'battery':
         return get_battery_module(nonmodular, raise_errors)
     elif component == 'genset':
         return get_genset_module(nonmodular, raise_errors)
     elif component == 'grid':
         return get_grid_module(nonmodular, raise_errors)
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/convert/to_nonmodular_ops.py` & `python-microgrid-1.4.1/src/pymgrid/convert/to_nonmodular_ops.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/.DS_Store` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:18 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:18 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:18 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:32 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:32 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:32 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 3353.5
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 3341.3500000000004
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -66,63 +66,63 @@
       init_start_up: true
       initial_step: 0
       normalized_action_bounds:
       - 0
       - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 19941.3
-      running_min_production: 1107.8500000000001
+      running_max_production: 64065.6
+      running_min_production: 3559.2000000000003
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 47556
-      max_charge: 11889
-      max_discharge: 11889
-      min_capacity: 9511.2
+      max_capacity: 105583
+      max_charge: 26396
+      max_discharge: 26396
+      min_capacity: 21116.600000000002
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 9511.2
+      current_charge: 21116.600000000002
       soc: 0.2
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 39882
-      max_import: 39882
+      max_export: 128130
+      max_import: 128130
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 960.9000000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:36 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 1736.5
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 1912.15
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 84.95
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -66,45 +66,45 @@
       init_start_up: true
       initial_step: 0
       normalized_action_bounds:
       - 0
       - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 43725.6
-      running_min_production: 2429.2000000000003
+      running_max_production: 95435.1
+      running_min_production: 5301.950000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 66116
-      max_charge: 16529
-      max_discharge: 16529
-      min_capacity: 13223.2
+      max_capacity: 170694
+      max_charge: 42674
+      max_discharge: 42674
+      min_capacity: 34138.8
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 13223.2
+      current_charge: 34138.8
       soc: 0.2
 trajectory_func: null
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 4399.25
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -66,45 +66,45 @@
       init_start_up: true
       initial_step: 0
       normalized_action_bounds:
       - 0
       - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 95435.1
-      running_min_production: 5301.950000000001
+      running_max_production: 11798.1
+      running_min_production: 655.45
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 1
       initial_step: 0
-      max_capacity: 170694
-      max_charge: 42674
-      max_discharge: 42674
-      min_capacity: 34138.8
+      max_capacity: 19334
+      max_charge: 4834
+      max_discharge: 4834
+      min_capacity: 3866.8
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 34138.8
-      soc: 0.2
+      current_charge: 19334
+      soc: 1.0
 trajectory_func: null
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 4465.150000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:37 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 525.2
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:38 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:38 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:38 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 2786.5
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 4341.5
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
       running_min_production: 1586.7
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:34 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -66,45 +66,67 @@
       init_start_up: true
       initial_step: 0
       normalized_action_bounds:
       - 0
       - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 11798.1
-      running_min_production: 655.45
+      running_max_production: 19941.3
+      running_min_production: 1107.8500000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 1
+      init_soc: 0.2
       initial_step: 0
-      max_capacity: 19334
-      max_charge: 4834
-      max_discharge: 4834
-      min_capacity: 3866.8
+      max_capacity: 47556
+      max_charge: 11889
+      max_discharge: 11889
+      min_capacity: 9511.2
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 19334
-      soc: 1.0
+      current_charge: 9511.2
+      soc: 0.2
+- - grid
+  - !GridModule
+    cls_params:
+      cost_per_unit_co2: 0.1
+      final_step: 8759
+      forecast_horizon: 23
+      forecaster: oracle
+      forecaster_increase_uncertainty: false
+      forecaster_relative_noise: false
+      initial_step: 0
+      max_export: 39882
+      max_import: 39882
+      normalized_action_bounds:
+      - 0
+      - 1
+      raise_errors: false
+      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
+    name:
+    - grid
+    - 0
+    state:
+      _current_step: 0
 trajectory_func: null
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -66,63 +66,63 @@
       init_start_up: true
       initial_step: 0
       normalized_action_bounds:
       - 0
       - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 64065.6
-      running_min_production: 3559.2000000000003
+      running_max_production: 98996.40000000001
+      running_min_production: 5499.8
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 0.5374787046064285
       initial_step: 0
-      max_capacity: 105583
-      max_charge: 26396
-      max_discharge: 26396
-      min_capacity: 21116.600000000002
+      max_capacity: 199587
+      max_charge: 49897
+      max_discharge: 49897
+      min_capacity: 39917.4
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 21116.600000000002
-      soc: 0.2
+      current_charge: 107273.76221628326
+      soc: 0.5374787046064285
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 128130
-      max_import: 128130
+      max_export: 197992
+      max_import: 197992
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Thu Sep  7 23:44:35 2023, max compression
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -66,67 +66,45 @@
       init_start_up: true
       initial_step: 0
       normalized_action_bounds:
       - 0
       - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 98996.40000000001
-      running_min_production: 5499.8
+      running_max_production: 43725.6
+      running_min_production: 2429.2000000000003
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
-      _current_status: true
+      _current_status: 1
       _current_step: 0
-      _goal_status: true
+      _goal_status: 1
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
       battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.5374787046064285
+      init_soc: 0.2
       initial_step: 0
-      max_capacity: 199587
-      max_charge: 49897
-      max_discharge: 49897
-      min_capacity: 39917.4
+      max_capacity: 66116
+      max_charge: 16529
+      max_discharge: 16529
+      min_capacity: 13223.2
       normalized_action_bounds:
       - 0
       - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 107273.76221628326
-      soc: 0.5374787046064285
-- - grid
-  - !GridModule
-    cls_params:
-      cost_per_unit_co2: 0.1
-      final_step: 8759
-      forecast_horizon: 23
-      forecaster: oracle
-      forecaster_increase_uncertainty: false
-      forecaster_relative_noise: false
-      initial_step: 0
-      max_export: 197992
-      max_import: 197992
-      normalized_action_bounds:
-      - 0
-      - 1
-      raise_errors: false
-      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
-    name:
-    - grid
-    - 0
-    state:
-      _current_step: 0
+      current_charge: 13223.2
+      soc: 0.2
 trajectory_func: null
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25.pkl` & `python-microgrid-1.4.1/src/pymgrid/data/scenario/pymgrid25.pkl`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/envs/base/base.py` & `python-microgrid-1.4.1/src/pymgrid/envs/base/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import pandas as pd
 
+from collections import OrderedDict
 from gym import Env
 from gym.spaces import Box, Dict, Tuple, flatten_space, flatten
 from abc import abstractmethod
 
 from pymgrid import NonModularMicrogrid, Microgrid
-from pymgrid.envs.base.skip_init import skip_init
+from pymgrid.errors.env_signature import environment_signature_error
 
 
 class BaseMicrogridEnv(Microgrid, Env):
     """
     Base class for all microgrid environments.
 
     Implements the `OpenAI Gym API <https://www.gymlibrary.dev//>`_ for a microgrid;
@@ -65,47 +66,30 @@
 
     action_space = None
     'Space object corresponding to valid actions.'
 
     observation_space = None
     'Space object corresponding to valid observations.'
 
-    def __new__(cls, modules, *args, **kwargs):
-        if isinstance(modules, (NonModularMicrogrid, Microgrid)):
-            import warnings
-            warnings.warn('Initializing an environment with a microgrid will be deprecated in a future version.'
-                          'Use from_microgrid() instead.', category=FutureWarning)
-
-            instance = cls.from_microgrid(modules, **kwargs)
-
-        elif isinstance(modules, int):
-            import warnings
-            warnings.warn('Initializing an environment with a scenario integer will be deprecated in a future version.'
-                          'Use from_scenario() instead.', category=FutureWarning)
-            instance = cls.from_scenario(modules, **kwargs)
-
-        else:
-            return super().__new__(cls)
-
-        cls.__init__ = skip_init(cls, cls.__init__)
-        return instance
-
     def __init__(self,
                  modules,
                  add_unbalanced_module=True,
                  loss_load_cost=10,
                  overgeneration_cost=2,
                  reward_shaping_func=None,
                  trajectory_func=None,
                  flat_spaces=True,
                  observation_keys=(),
                  step_callback=None,
                  reset_callback=None
                  ):
 
+        if isinstance(modules, (NonModularMicrogrid, Microgrid, int)):
+            environment_signature_error(self.__class__.__name__, modules)
+
         super().__init__(modules,
                          add_unbalanced_module=add_unbalanced_module,
                          loss_load_cost=loss_load_cost,
                          overgeneration_cost=overgeneration_cost,
                          reward_shaping_func=reward_shaping_func,
                          trajectory_func=trajectory_func)
 
@@ -120,75 +104,81 @@
     def _validate_observation_keys(self, keys):
         if not keys:
             return keys
 
         if isinstance(keys, str):
             keys = [keys]
 
+        keys = np.array(keys)
+
         possible_keys = self.potential_observation_keys()
         bad_keys = [key for key in keys if key not in possible_keys]
 
         if bad_keys:
             raise NameError(f'Keys {bad_keys} not found in state.')
 
-        return keys
+        # Put net load at the beginning, to match where it will be in the action space
+        net_load_pos = np.where(np.array(keys) == 'net_load')[0]
+
+        if net_load_pos.size:
+            keys[[0, net_load_pos.item()]] = keys[[net_load_pos.item(), 0]]
+
+        return keys.tolist()
 
     @abstractmethod
     def _get_action_space(self, remove_redundant_actions=False):
         pass
 
     def _get_observation_space(self):
         obs_space = {}
 
         state_series = self.state_series()
 
+        observation_keys = self.observation_keys or state_series.index.get_level_values(-1)
+
+        if 'net_load' in observation_keys:
+            obs_space['general'] = Tuple([Box(low=-np.inf, high=1, shape=(1, ), dtype=np.float64)])
+
         for name, module_list in self.modules.iterdict():
             tup = []
             for module_num, module in enumerate(module_list):
                 normalized_space = module.observation_space['normalized']
 
-                if not self.observation_keys:
-                    tup.append(normalized_space)
-                else:
-                    try:
-                        relevant_state_idx = state_series.loc[pd.IndexSlice[name, module_num]].index
-                    except KeyError:
-                        continue
-
-                    locs = [
-                        relevant_state_idx.get_loc(key) for key in self.observation_keys if key in relevant_state_idx
-                    ]
-                    if locs:
-                        box_slice = Box(
-                            normalized_space.low[locs],
-                            normalized_space.high[locs],
-                            shape=(len(locs), ),
-                            dtype=normalized_space.dtype
-                        )
+                try:
+                    relevant_state_idx = state_series.loc[pd.IndexSlice[name, module_num]].index
+                except KeyError:
+                    continue
+
+                locs = [
+                    relevant_state_idx.get_loc(key) for key in observation_keys if key in relevant_state_idx
+                ]
+                if locs:
+                    box_slice = Box(
+                        normalized_space.low[locs],
+                        normalized_space.high[locs],
+                        shape=(len(locs), ),
+                        dtype=normalized_space.dtype
+                    )
 
-                        tup.append(box_slice)
+                    tup.append(box_slice)
             if tup:
                 obs_space[name] = Tuple(tup)
 
-        if self.observation_keys and 'net_load' in self.observation_keys:
-            obs_space['net_load'] = Tuple([Box(low=-np.inf, high=1, shape=(1, ), dtype=np.float64)])
-
-        obs_space = Dict(obs_space)
+        # Prevent sorting of keys; first cast to OrderedDict
+        obs_space = Dict(OrderedDict(obs_space))
 
         return (flatten_space(obs_space) if self._flat_spaces else obs_space), obs_space
 
     def potential_observation_keys(self):
         return self.state_series().index.get_level_values(-1).unique()
 
     def reset(self):
-        obs = super().reset()
-        obs.pop('balance')
-        obs.pop('other')
+        super().reset()
         self.reset_callback()
-        return self._get_obs(obs)
+        return self._get_obs()
 
     def step(self, action, normalized=True):
         """
         Run one timestep of the environment's dynamics.
 
         When the end of the episode is reached, you are responsible for calling `reset()`
         to reset the environment's state.
@@ -217,19 +207,22 @@
         done : bool
             Whether the microgrid terminates.
 
         info : dict
             Additional information from this step.
 
         """
+        self._microgrid_logger.log(net_load=self.compute_net_load())
+
         action = self.convert_action(action)
         self._log_action(action, normalized)
 
-        obs, reward, done, info = self.run(action, normalized=normalized)
-        obs = self._get_obs(obs)
+        obs, reward, done, info = super().step(action, normalized=normalized)
+        obs = self._get_obs()
+
         self.step_callback(**self._get_step_callback_info(action, obs, reward, done, info))
 
         return obs, reward, done, info
 
     @abstractmethod
     def convert_action(self, action):
         """
@@ -263,25 +256,27 @@
                 for j, act in enumerate(action_list):
                     if not pd.api.types.is_list_like(act):
                         act = [act]
                     d.update({(key, j, f'{module}_{el_num}'): act_n for el_num, act_n in enumerate(act)})
 
         self._microgrid_logger.log(d)
 
-    def _get_obs(self, obs):
+    def _get_obs(self):
         if self.observation_keys:
             obs = self.state_series(normalized=True).loc[pd.IndexSlice[:, :, self.observation_keys]]
 
             if self._flat_spaces:
                 obs = obs.values
             else:
                 obs = obs.to_frame().unstack(level=1).T.droplevel(level=1, axis=1).to_dict(orient='list')
 
         elif self._flat_spaces:
-            obs = self.flatten_obs(self._nested_observation_space, obs)
+            obs = self.state_series(normalized=True).values
+        else:
+            obs = self.state_dict(normalized=True, as_run_output=True)
 
         return obs
 
     def _get_step_callback_info(self, action, obs, reward, done, info):
         return {
             'action': action,
             'obs': obs,
@@ -307,52 +302,56 @@
         Returns
         -------
         net_load : float
             Net load.
 
         """
 
-        if self.current_step == self.final_step:
-            return 0.0
-
         try:
             fixed_consumption = self.modules.fixed.get_attrs('max_consumption', as_pandas=False, drop_attr_names=True)
             fixed_consumption = np.sum(list(fixed_consumption.values()))
         except AttributeError:
             fixed_consumption = 0.0
+        except IndexError:
+            # Exhausted available data. Episode should be over
+            assert self.current_step == self.final_step
+            return 0.0
+
+        try:
+            flex_max_prod = [m.max_production for m in self.modules.flex.iterlist() if m.marginal_cost == 0]
+        except IndexError:
+            # Exhausted available data. Episode should be over
+            assert self.current_step == self.final_step
+            return 0.0
 
-        flex_max_prod = [m.max_production for m in self.modules.flex.iterlist() if m.marginal_cost == 0]
         flex_production = sum(flex_max_prod)
 
         net_load = fixed_consumption - flex_production
 
         if normalized:
             if fixed_consumption:
                 return net_load / fixed_consumption
             return -1.0
 
         return net_load
 
-    def state_dict(self, normalized=False, as_run_output=False):
-        sd = super().state_dict(normalized=normalized, as_run_output=as_run_output)
-
+    def state_dict(self, normalized=False, as_run_output=False, _initial=None):
         net_load = self.compute_net_load(normalized=normalized)
 
         if as_run_output:
             net_load_entry = np.array([net_load])
         else:
             net_load_entry = {'net_load': net_load}
 
-        sd['general'] = [net_load_entry]
-
-        return sd
+        state_dict = {'general': [net_load_entry]}
+        return super().state_dict(normalized=normalized, as_run_output=as_run_output, _initial=state_dict)
 
     @staticmethod
     def flatten_obs(observation_space, obs):
-        return np.concatenate([flatten(observation_space[k], v) for k, v in obs.items()])
+        return np.concatenate([flatten(space, obs[k]) for k, space in observation_space.items()])
 
     @property
     def unwrapped(self):
         """:meta private:"""
         return super().unwrapped
 
     @property
@@ -420,8 +419,8 @@
         if kwargs:
             return cls.from_microgrid(env, **kwargs)
 
         return env
 
     @classmethod
     def load(cls, stream):
-        return cls(super().load(stream))
+        return cls.from_microgrid(super().load(stream))
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/envs/continuous/continuous.py` & `python-microgrid-1.4.1/src/pymgrid/envs/continuous/continuous.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,27 +120,27 @@
             self._slack_module_ref = controllable_modules_dict[self._slack_module]
         except KeyError:
             controllable_modules_dict_lists = self.modules.controllable.to_dict()
             try:
                 self._slack_module_ref = controllable_modules_dict_lists[self._slack_module].item()
                 self._slack_module = self._slack_module_ref.name
             except ValueError:
-                msg = f"Module name {self._slack_module} does not point to one controllable candidate."
+                msg = f"Module name {self._slack_module} does not point to unique controllable candidate."
             except KeyError:
-                msg = f"No module '{self._slack_module}' amongst controllable candidates {controllable_modules_dict}"
+                msg = f"No module '{self._slack_module}' amongst controllable candidates " \
+                      f"{list(controllable_modules_dict.keys())}"
 
             if msg:
                 raise NameError(msg)
 
     def step(self, action):
         return super().step(action, normalized=False)
 
-    def convert_action(self, action, to_microgrid=True):
+    def convert_action(self, action, to_microgrid=True, normalize=False):
         net_load = self.compute_net_load()
-        self._microgrid_logger.log(net_load=net_load)
 
         if to_microgrid:
             relative_action = unflatten(self._nested_action_space, action)
 
             self._log_action(relative_action, normalized=False, log_column='net_load_action')
 
             absolute_action = self.make_absolute(relative_action, net_load)
@@ -188,19 +188,27 @@
 
         return action
 
     def add_slack(self, action, net_load):
         if self._slack_module is None:
             return action
 
-        slack_action = np.ones(self._slack_module_ref.action_space.shape)
         current_prod = sum([act[-1] for act_list in action.values() for act in act_list])
         remaining_net_load = net_load - current_prod
+
+        if remaining_net_load > 0:
+            slack_action = np.ones(self._slack_module_ref.action_space.shape)
+        else:
+            # Genset off. Ignored in all other slack modules; overwritten below.
+            slack_action = np.zeros(self._slack_module_ref.action_space.shape)
+
         slack_action[-1] = remaining_net_load
 
+
+
         module_name, module_num = self._slack_module
 
         try:
             action[module_name].insert(module_num, slack_action)
         except KeyError:
             assert module_num == 0
             action[module_name] = [slack_action]
@@ -234,8 +242,12 @@
         return self._slack_module_ref
 
 
 def clip_module_action(action, module):
     low = -1 * module.max_consumption
     high = module.max_production
 
+    if len(action) > 1:
+        low = [*module.action_space.unnormalized.low[:-1], low]
+        high = [*module.action_space.unnormalized.high[:-1], high]
+
     return module.action_space.clip(action, low=low, high=high)
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/envs/discrete/discrete.py` & `python-microgrid-1.4.1/src/pymgrid/envs/discrete/discrete.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/forecast/forecaster.py` & `python-microgrid-1.4.1/src/pymgrid/forecast/forecaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,30 @@
 
 class OracleForecaster(Forecaster):
     def _forecast(self, val_c, val_c_n, n):
         return val_c_n
 
 
 class GaussianNoiseForecaster(Forecaster):
+    """
+    Forecaster that adds Gaussian noise to true future values.
+    """
+    increase_uncertainty: bool
+    """
+    Whether uncertainty should increase for points farther in the future.
+    
+    If True, uncertainty increases logarithmically in the number of steps ahead.
+    """
+    relative_noise: bool
+    """
+    Whether the Gaussian noise should be relative to the scale of the time series.
+    
+    If True, the noise_std will be computed as `input_noise_std * time_series.mean()`.
+    If False, the noise_std will be equal to `input_noise_std`.
+    """
     def __init__(self,
                  noise_std,
                  observation_space,
                  forecast_shape,
                  time_series=None,
                  increase_uncertainty=False,
                  relative_noise=False):
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/convert_scenario_sandbox.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/convert_scenario_sandbox.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/microgrid.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/microgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pymgrid.microgrid import DEFAULT_HORIZON
 from pymgrid.modules import ModuleContainer, UnbalancedEnergyModule
 from pymgrid.microgrid.utils.step import MicrogridStep
 from pymgrid.utils.eq import verbose_eq
 from pymgrid.utils.logger import ModularLogger
 from pymgrid.utils.serialize import add_numpy_pandas_representers, add_numpy_pandas_constructors, dump_data
 from pymgrid.utils.space import MicrogridSpace
+from pymgrid.utils.deprecation import deprecation_err
 
 
 class Microgrid(yaml.YAMLObject):
     """
     Microgrid class, used to define and simulate an environment with a variety of modules.
 
     Parameters
@@ -221,15 +222,19 @@
 
     def _set_trajectory(self):
         if self.trajectory_func is not None:
             initial_step, final_step = self.trajectory_func(self._initial_step, self._final_step)
             self._set_initial_step(initial_step, modules_only=True)
             self._set_final_step(final_step, modules_only=True)
 
+    @deprecation_err('Microgrid.step')
     def run(self, control, normalized=True):
+        pass
+
+    def step(self, control, normalized=True):
         """
 
         Run the microgrid for a single step.
 
         Parameters
         ----------
         control : dict[str, list[float]]
@@ -317,15 +322,15 @@
                     else:
                         source_amt = energy_needed
 
                     module_step = module.step(source_amt, normalized=False)
                     microgrid_step.append(name, *module_step)
                     energy_needed -= source_amt
 
-        provided, consumed, reward, shaped_reward = microgrid_step.balance()
+        provided, consumed, reward, shaped_reward = microgrid_step.balance(shape_reward=True)
 
         log_dict = self._get_log_dict(
             provided-controllable_fixed_provided,
             consumed-controllable_fixed_consumed,
             log_dict=log_dict,
             prefix='flex'
         )
@@ -490,15 +495,15 @@
 
         try:
             df = pd.DataFrame(_log_dict, index=pd.RangeIndex(start=initial_step, stop=self.current_step))
         except ValueError as e:
             if 'Length of values' in e.args[0]:
                 module_log_lengths = pd.Series([len(log_dict) for log_dict in _log_dict.values()])
 
-                msg = f"Length of module log dicts ({module_log_lengths.unique().item()}) " \
+                msg = f"Length of module log dicts ({module_log_lengths.unique()}) " \
                       f"do not match self.current_step-initial_step ({self.current_step-initial_step}). " \
                       f"Did you set a trajectory attribute " \
                       f"('initial_step', 'final_step', 'trajectory_func') without calling Microgrid.reset()?"
 
                 raise ValueError(msg)
 
             else:
@@ -727,44 +732,49 @@
         -------
         modules : :class:`pymgrid.modules.module_container.ModuleContainer`
             View of the container.
 
         """
         return self._modules
 
-    def state_dict(self, normalized=False, as_run_output=False):
+    def state_dict(self, normalized=False, as_run_output=False, _initial=None):
         """
         State of the microgrid as a dict.
 
         Keys are module names and values are lists of state dicts for all modules with said name.
 
         Parameters
         ----------
         normalized : bool, default False
             Whether to return a dict of normalized values.
 
         as_run_output : bool, default False
             Whether to return output in the same format as the output of :meth:`Microgrid.run`.
             Inner values are numpy arrays and not dict in this case.
 
+        _initial : dict or None
+            Internal parameter, do not use.
 
         Returns
         -------
         state_dict : dict[str, list[dict]] or dict[str[list[np.ndarray]]]
             State of the microgrid as a nested dict.
 
         """
         def as_run_output_f(state_dict):
             if as_run_output:
                 return np.array(list(state_dict.values()))
             return state_dict
 
-        return {name: [
-            as_run_output_f(module.state_dict(normalized=normalized)) for module in modules
-        ] for name, modules in self._modules.iterdict()}
+        state_dict = _initial or dict()
+
+        for name, modules in self._modules.iterdict():
+            state_dict[name] = [as_run_output_f(module.state_dict(normalized=normalized)) for module in modules]
+
+        return state_dict
 
     @property
     def log(self):
         """
         Microgrid's log as a DataFrame.
 
         This is equivalent to `:meth:`get_log`.
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/baseline_shaper.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/rescale_shaper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 import numpy as np
 
 from pymgrid.microgrid.reward_shaping.base import BaseRewardShaper
 
 
-class BaselineShaper(BaseRewardShaper):
+class RescaleShaper(BaseRewardShaper):
     """
     Reward is the original reward scaled by some scale factor.
 
     ``scaled_reward = self.scale_factor * original_reward ``.
 
     """
 
-    yaml_tag = u"!BaselineShaper"
+    yaml_tag = u"!RescaleShaper"
 
-    def __init__(self, module=('grid', 0)):
+    def __init__(self, scale_factor=1.0):
+        self.scale_factor = scale_factor
+
+    def serializable_state_attributes(self):
+        return 'scale_factor',
+
+    def __call__(self, original_reward, step_info, cost_info):
+        return self.scale_factor * original_reward
+
+
+class LearnedScaleRescaleShaper(RescaleShaper):
+    yaml_tag = u"!LearnedScaleRescaleShaper"
+
+    def __init__(self, module=('unbalanced_energy', 0)):
+        super().__init__(scale_factor=1.0)
         self.module = module
 
-    @staticmethod
-    def compute_net_load(step_info):
-        try:
-            load_info = step_info['load']
-        except KeyError:
-            raise NameError("Microgrid has no module with name 'load'")
+        self.max_load = 0.0
+        self.max_renewable = 0.0
 
-        try:
-            renewable_info = step_info.get('renewable', step_info['pv'])
-        except KeyError:
-            raise NameError("Microgrid has no module with name 'renewable' or 'pv'.")
-
-        total_load = sum(d['absorbed_energy'] for d in load_info)
-        total_renewable = sum(d['provided_energy'] for d in renewable_info)
-        return total_load - total_renewable
+    def _update_scale(self, step_info, cost_info):
+        total_load = self.compute_total_load(step_info)
+        total_renewable = self.compute_total_renewable(step_info)
+
+        if total_load > self.max_load:
+            self._max_load = total_load
 
-    def compute_baseline_cost(self, step_info, cost_info):
-        net_load = self.compute_net_load(step_info)
+        if total_renewable > self.max_renewable:
+            self._max_renewable = total_renewable
 
         try:
             baseline_cost_info = cost_info[self.module[0]][self.module[1]]
         except (KeyError, IndexError):
             raise NameError(f"Microgrid has no module in position '{self.module}'")
 
-        baseline_cost = net_load * baseline_cost_info['production_marginal_cost']
-        return baseline_cost
+        baseline = (self.max_load - self.max_renewable) * baseline_cost_info['production_marginal_cost']
+        self.scale_factor = 1 / baseline if baseline else self.scale_factor
 
-    def __call__(self, original_reward, step_info, cost_info):
-        baseline_cost = self.compute_baseline_cost(step_info, cost_info)
-        return original_reward + baseline_cost
+    def serializable_state_attributes(self):
+        return 'module', 'max_load', 'max_renewable', 'scale_factor'
 
+    def __call__(self, original_reward, step_info, cost_info):
+        self._update_scale(step_info, cost_info)
+        assert self.scale_factor > 0
+        return super().__call__(original_reward, step_info, cost_info)
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     yaml_tag = u"!BatteryDischargeShaper"
 
     def __call__(self, original_reward, step_info, cost_info):
         battery_discharge = self.sum_module_val(step_info, 'battery', 'provided_energy')
         load = self.sum_module_val(step_info, 'load', 'absorbed_energy')
         loss_load = self.sum_module_val(step_info, 'unbalanced_energy', 'provided_energy')
 
-        # battery_discharge is in [0, load-loss_load]; loss_load is in [0, load].
+        # battery_discharge should be in [0, load-loss_load]; loss_load should be in [0, load].
         try:
             percent_battery = (battery_discharge - loss_load) / load
         except ZeroDivisionError:
             return 0.0
 
-        assert -1 <= percent_battery <= 1 or np.isclose(percent_battery, 1) or np.isclose(percent_battery, 0)
         return percent_battery
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/base.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/base.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/stochastic.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/trajectory/stochastic.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/microgrid/utils/step.py` & `python-microgrid-1.4.1/src/pymgrid/microgrid/utils/step.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,22 @@
 
         for key, value in info.items():
             try:
                 self._info[key].append(value)
             except KeyError:
                 pass
 
-    def balance(self):
+    def balance(self, shape_reward=False):
         provided_energy = np.sum(self._info['provided_energy'])
         absorbed_energy = np.sum(self._info['absorbed_energy'])
-        return provided_energy, absorbed_energy, self._reward, self.shaped_reward()
+
+        if shape_reward:
+            return provided_energy, absorbed_energy, self._reward, self.shaped_reward()
+
+        return provided_energy, absorbed_energy, self._reward, None
 
     def output(self):
         return self._obs, self.shaped_reward(), self._done, self._output_info()
 
     def shaped_reward(self):
         if self._reward_shaping_func is None:
             return self._reward
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/base/base_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/base/base_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,16 +133,20 @@
             Whether the module terminates.
         info : dict
             Additional information from this step.
             Will include either``provided_energy`` or ``absorbed_energy`` as a key, denoting the amount of energy
             this module provided to or absorbed from the microgrid.
 
         """
-
-        denormalized_action = self._action_space.denormalize(action) if normalized else action
+        if normalized:
+            denormalized_action = self._action_space.denormalize(action)
+        elif self._action_space.clip_vals:
+            denormalized_action = self._action_space.clip(action, normalized=False)
+        else:
+            denormalized_action = action
 
         try:
             denormalized_action = denormalized_action[self._energy_pos]
         except (IndexError, TypeError):
             if not isinstance(denormalized_action, (float, int)):
                 try:
                     flat_dim = np.product(denormalized_action.shape)
@@ -270,28 +274,27 @@
             absorbed_energy = energy_excess
 
         assert absorbed_energy >= 0
 
         return self.update(absorbed_energy, as_sink=True)
 
     def _log(self, state_dict_pre_step, provided_energy=None, absorbed_energy=None, **info):
-        _info = info.copy()
+        energy_info = dict()
 
         if self.provided_energy_name is not None:
-            _info[self.provided_energy_name] = provided_energy if provided_energy is not None else 0.0
+            energy_info[self.provided_energy_name] = provided_energy if provided_energy is not None else 0.0
         else:
             assert provided_energy is None, 'Cannot log provided_energy with NoneType provided_energy_name.'
 
         if self.absorbed_energy_name is not None:
-            _info[self.absorbed_energy_name] = absorbed_energy if absorbed_energy is not None else 0.0
+            energy_info[self.absorbed_energy_name] = absorbed_energy if absorbed_energy is not None else 0.0
         else:
             assert absorbed_energy is None, 'Cannot log absorbed_energy with NoneType absorbed_energy_name.'
 
-        _info.update(state_dict_pre_step)
-        self._logger.log(**_info)
+        self._logger.log(**info, **energy_info, **state_dict_pre_step)
 
     def _update_step(self, reset=False):
         if reset:
             self._current_step = self.initial_step
         else:
             self._current_step += 1
 
@@ -676,18 +679,46 @@
             Average marginal cost.
 
         """
         return self.production_marginal_cost
 
     @property
     def production_marginal_cost(self):
+        """
+        Expected marginal cost of energy production.
+
+        Cost of producing one unit of energy.
+
+        .. warning::
+            This is a scalar value, and thus will be inaccurate for modules that do not have scalar costs.
+            It is thus only an expectation.
+
+        Returns
+        -------
+        production_marginal_cost : float
+
+        """
         return 0.0
 
     @property
     def absorption_marginal_cost(self):
+        """
+        Expected marginal cost of energy absorption.
+
+        Cost of absorbing one unit of energy.
+
+        .. warning::
+            This is a scalar value, and thus will be inaccurate for modules that do not have scalar costs.
+            It is thus only an expectation.
+
+        Returns
+        -------
+        absorption_marginal_cost : float
+
+        """
         return 0.0
 
     @property
     def action_space(self):
         """
         Action spaces of the module.
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/base_timeseries_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/base/timeseries/base_timeseries_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,37 +273,37 @@
                                                 )
 
         self._forecaster.observation_space = self._observation_space
 
     @property
     def forecaster_increase_uncertainty(self):
         """
-        View of :class:`pymgrid.forecast.GaussianNoiseForecaster``.increase_uncertainty`.
+        View of :attr:`.GaussianNoiseForecaster.increase_uncertainty`.
 
         Required for serialization as a mirror to the class parameter.
-        Will only ever be True if ``self.forecaster`` is a ``GaussianNoiseForecaster``.
+        Will only ever be True if :attr:`.forecaster` is a :class:`.GaussianNoiseForecaster`.
 
         Returns
         -------
         forecaster_increase_uncertainty : bool
-            Associated attribute of ``self.forecaster``.
+            Associated attribute of `:attr:`.forecaster`.
 
         """
         try:
             return self._forecaster.increase_uncertainty
         except AttributeError:
             return False
 
     @property
     def forecaster_relative_noise(self):
         """
-        View of :class:`pymgrid.forecast.GaussianNoiseForecaster``.forecaster_relative_noise`.
+        View of :attr:`.GaussianNoiseForecaster.relative_noise`.
 
         Required for serialization as a mirror to the class parameter.
-        Will only ever be True if ``self.forecaster`` is a ``GaussianNoiseForecaster``.
+        Will only ever be True if ``self.forecaster`` is a :class:`.GaussianNoiseForecaster`.
 
         Returns
         -------
         forecaster_relative_noise : bool
             Associated attribute of ``self.forecaster``.
 
         """
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/battery/battery_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/battery/battery_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         If both are passed, ``init_soc`` is ignored and ``init_charge`` is used.
 
     init_soc : float or None, default None
         Initial state of charge of the battery.
         One of ``init_charge`` or ``init_soc`` must be passed, else an exception is raised.
         If both are passed, ``init_soc`` is ignored and ``init_charge`` is used.
 
+    normalized_action_bounds : tuple of int or float, default (0, 1).
+        Bounds of normalized actions.
+        Change to (-1, 1) for e.g. an RL policy with a Tanh output activation.
+
     raise_errors : bool, default False
         Whether to raise errors if bounds are exceeded in an action.
         If False, actions are clipped to the limit possible.
 
     """
     module_type = ('battery', 'controllable')
     yaml_tag = f"!BatteryModule"
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/biased_transition_model.py` & `python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/biased_transition_model.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/transition_model.py` & `python-microgrid-1.4.1/src/pymgrid/modules/battery/transition_models/transition_model.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/genset_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/genset_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 
     allow_abortion : bool, default True
         Whether the genset is able to remain shut down while in the process of starting up and vice versa.
 
     init_start_up : bool, default True
         Whether the genset is running upon reset.
 
+    normalized_action_bounds : tuple of int or float, default (0, 1).
+        Bounds of normalized actions.
+        Change to (-1, 1) for e.g. an RL policy with a Tanh output activation.
+
     raise_errors : bool, default False
         Whether to raise errors if bounds are exceeded in an action.
         If False, actions are clipped to the limit possible.
 
     provided_energy_name : str, default "genset_production"
         Name of the energy provided by this module, to be used in logging.
 
@@ -142,14 +146,16 @@
             Additional information from this step.
             Will include either `provided_energy` or `absorbed_energy` as a key, denoting the amount of energy
             this module provided to or absorbed from the microgrid.
 
         """
         if normalized:
             denormalized = self._action_space.denormalize(action)
+        elif self._action_space.clip_vals:
+            denormalized = self._action_space.clip(action, normalized=False)
         else:
             denormalized = action
 
         goal_status = denormalized[0]
 
         assert 0 <= goal_status <= 1
         self.update_status(goal_status)
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/grid_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/grid_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 
     forecaster_increase_uncertainty : bool, default False
         Whether to increase uncertainty for farther-out dates if using a GaussianNoiseForecaster. Ignored otherwise.
 
     cost_per_unit_co2 : float, default 0.0
         Marginal cost of grid co2 production.
 
+    normalized_action_bounds : tuple of int or float, default (0, 1).
+        Bounds of normalized actions.
+        Change to (-1, 1) for e.g. an RL policy with a Tanh output activation.
+
     raise_errors : bool, default False
         Whether to raise errors if bounds are exceeded in an action.
         If False, actions are clipped to the limit possible.
 
     """
 
     module_type = ('grid', 'controllable')
@@ -319,19 +323,19 @@
 
     @property
     def max_consumption(self):
         return self.max_export * self.current_status
 
     @property
     def production_marginal_cost(self):
-        return self.import_price[0]
+        return -1 * self.get_cost(1, as_source=True, as_sink=False)
 
     @property
     def absorption_marginal_cost(self):
-        return self.export_price[0]
+        return self.get_cost(1, as_source=False, as_sink=True)
 
     @property
     def is_source(self):
         return True
 
     @property
     def is_sink(self):
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/load_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/load_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,19 @@
 
         * If ``None``, no forecast.
 
     forecast_horizon : int.
         Number of steps in the future to forecast. If forecaster is None, ignored and 0 is returned.
 
     forecaster_increase_uncertainty : bool, default False
-        Whether to increase uncertainty for farther-out dates if using a GaussianNoiseForecaster. Ignored otherwise..
+        Whether to increase uncertainty for farther-out dates if using a GaussianNoiseForecaster. Ignored otherwise.
+
+    normalized_action_bounds : tuple of int or float, default (0, 1).
+        Bounds of normalized actions.
+        Change to (-1, 1) for e.g. an RL policy with a Tanh output activation.
 
     raise_errors : bool, default False
         Whether to raise errors if bounds are exceeded in an action.
         If False, actions are clipped to the limit possible.
 
     """
     module_type = ('load', 'fixed')
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/module_container.py` & `python-microgrid-1.4.1/src/pymgrid/modules/module_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
                     return self.to_dict(orient='records')[item]
                 else:
                     return self.to_dict()[item]
             except KeyError:
                 raise KeyError(item)
 
     def __getattr__(self, item):
-        if item == 'data' or item.startswith('__') or item not in dir(self):
+        if item == 'data' or item.startswith('__'):
             raise AttributeError(item)
         try:
             return self[item]
         except KeyError:
             raise AttributeError(item)
 
     def __len__(self):
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/renewable_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/renewable_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
     forecaster_increase_uncertainty : bool, default False
         Whether to increase uncertainty for farther-out dates if using a GaussianNoiseForecaster. Ignored otherwise.
 
     provided_energy_name: str, default "renewable_used"
         Name of the energy provided by this module, to be used in logging.
 
+    normalized_action_bounds : tuple of int or float, default (0, 1).
+        Bounds of normalized actions.
+        Change to (-1, 1) for e.g. an RL policy with a Tanh output activation.
+
     raise_errors : bool, default False
         Whether to raise errors if bounds are exceeded in an action.
         If False, actions are clipped to the limit possible.
 
     """
     module_type = ('renewable', 'flex')
     yaml_tag = u"!RenewableModule"
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/modules/unbalanced_energy_module.py` & `python-microgrid-1.4.1/src/pymgrid/modules/unbalanced_energy_module.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/utils/DataGenerator.py` & `python-microgrid-1.4.1/src/pymgrid/utils/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/utils/eq.py` & `python-microgrid-1.4.1/src/pymgrid/utils/eq.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/utils/logger.py` & `python-microgrid-1.4.1/src/pymgrid/utils/logger.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/utils/ray.py` & `python-microgrid-1.4.1/src/pymgrid/utils/ray.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/src/pymgrid/utils/serialize.py` & `python-microgrid-1.4.1/src/pymgrid/utils/serialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,18 @@
         StochasticTrajectory,
         FixedLengthStochasticTrajectory
     )
 
     from pymgrid.microgrid.reward_shaping import (
         PVCurtailmentShaper,
         BatteryDischargeShaper,
-        RescaleShaper
+        RescaleShaper,
+        LearnedScaleRescaleShaper,
+        BaselineShaper,
+        SequentialShaper
     )
 
     from pymgrid.modules.battery.transition_models import (
         BatteryTransitionModel,
         BiasedTransitionModel,
         DecayTransitionModel
     )
```

### Comparing `python-microgrid-1.4.0/src/pymgrid/utils/space/space.py` & `python-microgrid-1.4.1/src/pymgrid/utils/space/space.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,21 +349,21 @@
 
         try:
             return denormalized.item()
         except (AttributeError, ValueError):
             return denormalized
 
     def _bounds_check(self, val, low, high):
-        clipped = np.clip(val, low, high)
-
-        if self.verbose or not self.clip_vals and (clipped != val).any():
+        if (low <= val).all() & (val <= high).all():
+            return val
+        elif self.verbose or not self.clip_vals:
             warnings.warn(f'Value {val} resides out of expected bounds of value to be normalized: [{low}, {high}].')
 
         if self.clip_vals:
-            return clipped
+            return np.clip(val, low, high)
 
         return val
 
 
 class MicrogridSpace(_PymgridSpace):
     def __init__(self, unnormalized, normalized=None, seed=None):
```

### Comparing `python-microgrid-1.4.0/src/python_microgrid.egg-info/PKG-INFO` & `python-microgrid-1.4.1/src/python_microgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-microgrid
-Version: 1.4.0
+Version: 1.4.1
 Summary: A simulator for tertiary control of electrical microgrids
-Download-URL: https://github.com/ahalev/python-microgrid/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/ahalev/python-microgrid/archive/refs/tags/v1.4.1.tar.gz
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: GNU LGPL 3.0
 Project-URL: Source Code, https://github.com/ahalev/python-microgrid
 Project-URL: Documentation, https://python-microgrid.readthedocs.io/
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -117,15 +117,15 @@
 Running the microgrid is straightforward. Simply pass an action for each fixed module to `microgrid.run`. The microgrid
 can also provide you a random action by calling `microgrid.sample_action.` Once the microgrid has been run for a
 certain number of steps, results can be viewed by calling microgrid.get_log.
 
 ```python
 >> for j in range(10):
 >>    action = microgrid.sample_action(strict_bound=True)
->>    microgrid.run(action)
+>>    microgrid.step(action)
 
 >> microgrid.get_log(drop_singleton_key=True)
 
       genset  ...                     balance
       reward  ... fixed_absorbed_by_microgrid
 0  -5.000000  ...                   10.672095
 1 -14.344353  ...                   50.626726
```

### Comparing `python-microgrid-1.4.0/src/python_microgrid.egg-info/SOURCES.txt` & `python-microgrid-1.4.1/src/python_microgrid.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,17 +29,30 @@
 src/pymgrid/algos/saa/__init__.py
 src/pymgrid/algos/saa/saa.py
 src/pymgrid/convert/__init__.py
 src/pymgrid/convert/conversion_test_sandbox.py
 src/pymgrid/convert/convert.py
 src/pymgrid/convert/get_module.py
 src/pymgrid/convert/to_nonmodular_ops.py
+src/pymgrid/data/.DS_Store
 src/pymgrid/data/__init__.py
 src/pymgrid/data/co2/__init__.py
+src/pymgrid/data/co2/co2_caiso.csv
+src/pymgrid/data/co2/co2_duke.csv
+src/pymgrid/data/load/RefBldgFullServiceRestaurantNew2004_v1.3_7.1_6A_USA_MN_MINNEAPOLIS.csv
+src/pymgrid/data/load/RefBldgHospitalNew2004_7.1_5.0_3C_USA_CA_SAN_FRANCISCO.csv
+src/pymgrid/data/load/RefBldgLargeHotelNew2004_v1.3_7.1_4A_USA_MD_BALTIMORE.csv
+src/pymgrid/data/load/RefBldgLargeOfficeNew2004_v1.3_7.1_5A_USA_IL_CHICAGO-OHARE.csv
+src/pymgrid/data/load/RefBldgPrimarySchoolNew2004_v1.3_7.1_2A_USA_TX_HOUSTON.csv
 src/pymgrid/data/load/__init__.py
+src/pymgrid/data/pv/Houston_722430TYA.csv
+src/pymgrid/data/pv/Minneapolis_726580TYA.csv
+src/pymgrid/data/pv/NewYork_744860TYA.csv
+src/pymgrid/data/pv/Raleigh_723060TYA.csv
+src/pymgrid/data/pv/SanFrancisco_724940TYA.csv
 src/pymgrid/data/pv/__init__.py
 src/pymgrid/data/scenario/.DS_Store
 src/pymgrid/data/scenario/__init__.py
 src/pymgrid/data/scenario/pymgrid25.pkl
 src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store
 src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml
 src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store
@@ -137,28 +150,33 @@
 src/pymgrid/envs/base/__init__.py
 src/pymgrid/envs/base/base.py
 src/pymgrid/envs/base/skip_init.py
 src/pymgrid/envs/continuous/__init__.py
 src/pymgrid/envs/continuous/continuous.py
 src/pymgrid/envs/discrete/__init__.py
 src/pymgrid/envs/discrete/discrete.py
+src/pymgrid/errors/__init__.py
+src/pymgrid/errors/env_signature.py
+src/pymgrid/errors/error.py
+src/pymgrid/errors/warnings.py
 src/pymgrid/forecast/__init__.py
 src/pymgrid/forecast/forecaster.py
 src/pymgrid/microgrid/__init__.py
 src/pymgrid/microgrid/convert_scenario_sandbox.py
 src/pymgrid/microgrid/microgrid.py
 src/pymgrid/microgrid/modular_microgrid_sandbox.py
 src/pymgrid/microgrid/serialization_sandbox.py
 src/pymgrid/microgrid/reward_shaping/__init__.py
-src/pymgrid/microgrid/reward_shaping/analyze_shaper.py
 src/pymgrid/microgrid/reward_shaping/base.py
 src/pymgrid/microgrid/reward_shaping/baseline_shaper.py
 src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py
 src/pymgrid/microgrid/reward_shaping/pv_curtailment_shaper.py
 src/pymgrid/microgrid/reward_shaping/rescale_shaper.py
+src/pymgrid/microgrid/reward_shaping/sequential.py
+src/pymgrid/microgrid/reward_shaping/standardization_shaper.py
 src/pymgrid/microgrid/trajectory/__init__.py
 src/pymgrid/microgrid/trajectory/base.py
 src/pymgrid/microgrid/trajectory/deterministic.py
 src/pymgrid/microgrid/trajectory/stochastic.py
 src/pymgrid/microgrid/utils/__init__.py
 src/pymgrid/microgrid/utils/step.py
 src/pymgrid/modules/__init__.py
@@ -176,18 +194,21 @@
 src/pymgrid/modules/battery/battery_module.py
 src/pymgrid/modules/battery/transition_models/__init__.py
 src/pymgrid/modules/battery/transition_models/biased_transition_model.py
 src/pymgrid/modules/battery/transition_models/decay_transition_model.py
 src/pymgrid/modules/battery/transition_models/transition_model.py
 src/pymgrid/utils/DataGenerator.py
 src/pymgrid/utils/__init__.py
+src/pymgrid/utils/code_link.py
+src/pymgrid/utils/deprecation.py
 src/pymgrid/utils/dry_run.py
 src/pymgrid/utils/eq.py
 src/pymgrid/utils/logger.py
 src/pymgrid/utils/ray.py
+src/pymgrid/utils/running_mean_std.py
 src/pymgrid/utils/serialize.py
 src/pymgrid/utils/space/__init__.py
 src/pymgrid/utils/space/space.py
 src/pymgrid/utils/space/utils.py
 src/python_microgrid.egg-info/PKG-INFO
 src/python_microgrid.egg-info/SOURCES.txt
 src/python_microgrid.egg-info/dependency_links.txt
```

### Comparing `python-microgrid-1.4.0/tests/test_microgridgenerator.py` & `python-microgrid-1.4.1/tests/test_microgridgenerator.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.4.0/tests/test_nonmodular_microgrid.py` & `python-microgrid-1.4.1/tests/test_nonmodular_microgrid.py`

 * *Files identical despite different names*

