# Comparing `tmp/MEArec-1.9.0.tar.gz` & `tmp/MEArec-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEArec-1.9.0.tar", last modified: Tue May 23 13:26:17 2023, max compression
+gzip compressed data, was "MEArec-1.9.1.tar", last modified: Sat Apr  6 15:02:09 2024, max compression
```

## Comparing `MEArec-1.9.0.tar` & `MEArec-1.9.1.tar`

### file list

```diff
@@ -1,595 +1,595 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.382394 MEArec-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-23 13:11:28.000000 MEArec-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-23 13:26:17.382394 MEArec-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 13:11:28.000000 MEArec-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-23 13:11:28.000000 MEArec-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:26:17.382394 MEArec-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-23 13:11:28.000000 MEArec-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.294393 MEArec-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.298393 MEArec-1.9.0/src/MEArec/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.294393 MEArec-1.9.0/src/MEArec/cell_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.298393 MEArec-1.9.0/src/MEArec/cell_models/bbp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.302393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.306393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.306393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)    89239 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology/C240300C1_-_Scale_x1.000_y1.050_z1.000_-_Clone_17.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5331 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.306393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)    49137 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.306393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.310393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.310393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)    72103 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology/C160998B-I_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5333 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.310393 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   151542 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.314394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.314394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.314394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   409097 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology/C091000D-I3_-_Scale_x1.000_y1.025_z1.000_-_Clone_6.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5339 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6809 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.318394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   244967 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.318394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.322394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.322394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   732565 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology/rp100428-12_idC_-_Scale_x1.000_y1.025_z1.000_-_Clone_1.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5333 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.322394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)    69674 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.326394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.326394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.326394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   780506 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology/og061123b1-3_idB_-_Scale_x1.000_y0.975_z1.000_-_Clone_4.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5333 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.330394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   358510 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.330394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.334394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.334394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   604368 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology/C040601.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5331 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.334394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   231703 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18146 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.338394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.338394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.338394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   323350 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology/C080301B1_-_Scale_x1.000_y1.050_z1.000_-_Clone_2.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5333 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.342394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   376717 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    30392 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.342394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.346394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.346394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   334377 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology/rp110125_L5-2_idA_-_Scale_x1.000_y0.950_z1.000_-_Clone_42.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5335 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6805 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.346394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)    40598 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.350394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.350394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca.mod
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.350394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   266052 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology/og061106a1_idA_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5335 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6805 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.350394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   121199 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.354394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.354394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.354394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   200764 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology/dend-C231296A-P3_axon-C231296A-P3_-_Clone_9.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5341 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6811 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.358394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   628013 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    50783 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.362394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.362394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.362394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   954647 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology/dend-C060114A2_axon-C060114A5.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5343 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.366394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   931577 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    84112 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.370394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.370394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.370394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   728920 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology/dend-C060114A7_axon-C060116A3_-_Clone_2.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5343 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.374394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   835414 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    79007 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/template.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.378394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/README
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/biophysics.hoc
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/cellinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/constants.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/creategui.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/createsimulation.hoc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/current_amps.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/init.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.378394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_HVA.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_LVAst.mod
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ih.mod
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Im.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Pst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Tst.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTa_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTs2_t.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Nap_Et2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SK_E2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SKv3_1.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.378394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)   575337 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology/dend-Fluo15_left_axon-Fluo15_left_-_Scale_x1.000_y0.950_z1.000_-_Clone_30.asc
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mosinit.hoc
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/ringplot.hoc
--rwxr-xr-x   0 runner    (1001) docker     (123)     5341 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6811 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_RmpRiTau.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_RmpRiTau_py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_hoc.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      114 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_py.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.382394 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/mtype_map.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.hoc
--rw-r--r--   0 runner    (1001) docker     (123)   248218 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18612 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synconf.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/template.hoc
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.382394 MEArec-1.9.0/src/MEArec/default_params/
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/default_params/recordings_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/default_params/templates_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/drift_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/generation_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.382394 MEArec-1.9.0/src/MEArec/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/generators/recgensteps.py
--rw-r--r--   0 runner    (1001) docker     (123)    69651 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/generators/recordinggenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/generators/spiketraingenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/generators/templategenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    48421 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/simulate_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.382394 MEArec-1.9.0/src/MEArec/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48070 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/tests/test_generators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   145191 2023-05-23 13:11:28.000000 MEArec-1.9.0/src/MEArec/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:26:17.302393 MEArec-1.9.0/src/MEArec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-23 13:26:17.000000 MEArec-1.9.0/src/MEArec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32828 2023-05-23 13:26:17.000000 MEArec-1.9.0/src/MEArec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:26:17.000000 MEArec-1.9.0/src/MEArec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 13:26:17.000000 MEArec-1.9.0/src/MEArec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-23 13:26:17.000000 MEArec-1.9.0/src/MEArec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 13:26:17.000000 MEArec-1.9.0/src/MEArec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.128447 MEArec-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-06 15:01:35.000000 MEArec-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-06 15:02:09.128447 MEArec-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-06 15:01:35.000000 MEArec-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-06 15:01:35.000000 MEArec-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:02:09.128447 MEArec-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-06 15:01:35.000000 MEArec-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.012447 MEArec-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.020447 MEArec-1.9.1/src/MEArec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.012447 MEArec-1.9.1/src/MEArec/cell_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.016447 MEArec-1.9.1/src/MEArec/cell_models/bbp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.024447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.028447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.028447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)    89239 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology/C240300C1_-_Scale_x1.000_y1.050_z1.000_-_Clone_17.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5331 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6801 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.028447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)    49137 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.032447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.032447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.032447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)    72103 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology/C160998B-I_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6803 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.036447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   151542 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.036447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.040447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.040447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   409097 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology/C091000D-I3_-_Scale_x1.000_y1.025_z1.000_-_Clone_6.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5339 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6809 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.040447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   244967 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    18852 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.044447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.048447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.048447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   732565 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology/rp100428-12_idC_-_Scale_x1.000_y1.025_z1.000_-_Clone_1.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6803 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.048447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)    69674 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.052447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.056447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.056447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   780506 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology/og061123b1-3_idB_-_Scale_x1.000_y0.975_z1.000_-_Clone_4.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6803 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.060447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   358510 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    28325 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.060447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.064447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.064447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   604368 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology/C040601.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5331 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6801 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.068447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   231703 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.068447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.072447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.072447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   323350 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology/C080301B1_-_Scale_x1.000_y1.050_z1.000_-_Clone_2.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5333 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6803 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.076447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   376717 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    30392 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.076447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.080447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.080447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   334377 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology/rp110125_L5-2_idA_-_Scale_x1.000_y0.950_z1.000_-_Clone_42.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5335 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6805 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.080447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)    40598 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.084447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.088447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.088447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   266052 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology/og061106a1_idA_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-06 15:01:35.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5335 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6805 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.088447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   121199 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.092447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.096447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.096447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   200764 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology/dend-C231296A-P3_axon-C231296A-P3_-_Clone_9.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5341 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6811 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.096447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   628013 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    50783 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.100447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.104447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.104447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   954647 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology/dend-C060114A2_axon-C060114A5.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5343 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6813 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.108447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   931577 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    84112 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.108447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.112447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.112447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   728920 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology/dend-C060114A7_axon-C060116A3_-_Clone_2.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5343 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6813 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.116447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   835414 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    79007 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/template.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.120447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/README
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/biophysics.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/cellinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/constants.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/creategui.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/createsimulation.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/current_amps.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/init.hoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.120447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_HVA.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_LVAst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ih.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Im.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Pst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Tst.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTa_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTs2_t.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Nap_Et2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SK_E2.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SKv3_1.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.120447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)   575337 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology/dend-Fluo15_left_axon-Fluo15_left_-_Scale_x1.000_y0.950_z1.000_-_Clone_30.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mosinit.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/ringplot.hoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5341 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6811 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_RmpRiTau.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_RmpRiTau_py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_hoc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_py.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.124447 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/mtype_map.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)   248218 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synconf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/template.hoc
+-rw-r--r--   0 runner    (1001) docker     (127)    25845 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.124447 MEArec-1.9.1/src/MEArec/default_params/
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/default_params/recordings_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/default_params/templates_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/drift_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/generation_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.124447 MEArec-1.9.1/src/MEArec/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/generators/recgensteps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69984 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/generators/recordinggenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/generators/spiketraingenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/generators/templategenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48465 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/simulate_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.124447 MEArec-1.9.1/src/MEArec/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48070 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/tests/test_generators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   145947 2024-04-06 15:01:36.000000 MEArec-1.9.1/src/MEArec/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:02:09.124447 MEArec-1.9.1/src/MEArec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-06 15:02:08.000000 MEArec-1.9.1/src/MEArec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32828 2024-04-06 15:02:09.000000 MEArec-1.9.1/src/MEArec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:02:08.000000 MEArec-1.9.1/src/MEArec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-06 15:02:08.000000 MEArec-1.9.1/src/MEArec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-06 15:02:08.000000 MEArec-1.9.1/src/MEArec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:02:08.000000 MEArec-1.9.1/src/MEArec.egg-info/top_level.txt
```

### Comparing `MEArec-1.9.0/LICENSE` & `MEArec-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/README.md` & `MEArec-1.9.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-[![Build Status](https://github.com/alejoe91/MEArec/actions/workflows/python-package.yml/badge.svg)](https://github.com/alejoe91/MEArec/actions/workflows/python-package.yml/badge.svg) [![PyPI version](https://badge.fury.io/py/MEArec.svg)](https://badge.fury.io/py/MEArec)
+[![Build Status](https://github.com/SpikeInterface/MEArec/actions/workflows/python-package.yml/badge.svg)](https://github.com/SpikeInterface/MEArec/actions/workflows/python-package.yml/badge.svg) [![PyPI version](https://badge.fury.io/py/MEArec.svg)](https://badge.fury.io/py/MEArec)
 
 # MEArec: Fast and customizable simulation of extracellular recordings on Multi-Electrode-Arrays
 
 MEArec is a package for generating biophysical extracellular neural recording on Multi-Electrode Arrays (MEA). The recording generations combines a Extracellular Action Potentials (EAP) templates generation and spike trains generation. The recordings are built by convoluting and modulating EAP templates with spike trains and adding noise.
 
 To clone this repo open your terminal and run:
 
-`git clone https://github.com/alejoe91/MEArec.git`
+`git clone https://github.com/SpikeInterface/MEArec.git`
 
 ## Installation
 
 The MEArec package can be installed with:
 
 ```
 pip install MEArec
```

### Comparing `MEArec-1.9.0/pyproject.toml` & `MEArec-1.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MEArec"
-version = "1.9.0"
+version = "1.9.1"
 authors = [
   { name="Alessio Buccino", email="alessiop.buccino@gmail.com" },
 ]
 description = "Python toolkit for biophysical simulation of extracellular electrophysiology recordings"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
@@ -53,16 +53,16 @@
 namespaces = false
 exclude = ["MEArec.*.tests"]
 
 [tool.black]
 line-length = 120
 
 [project.urls]
-homepage = "https://github.com/alejoe91/MEArec"
-repository = "https://github.com/alejoe91/MEArec"
+homepage = "https://github.com/SpikeInterface/MEArec"
+repository = "https://github.com/SpikeInterface/MEArec"
 documentation = "https://mearec.readthedocs.io/"
 
 
 [project.optional-dependencies]
 
 templates = [
     "neuron",
```

### Comparing `MEArec-1.9.0/src/MEArec/__init__.py` & `MEArec-1.9.1/src/MEArec/__init__.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology/C240300C1_-_Scale_x1.000_y1.050_z1.000_-_Clone_17.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology/C240300C1_-_Scale_x1.000_y1.050_z1.000_-_Clone_17.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BP_bAC217_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology/C160998B-I_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology/C160998B-I_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_BTC_bAC217_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology/C091000D-I3_-_Scale_x1.000_y1.025_z1.000_-_Clone_6.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology/C091000D-I3_-_Scale_x1.000_y1.025_z1.000_-_Clone_6.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_ChC_cACint209_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology/rp100428-12_idC_-_Scale_x1.000_y1.025_z1.000_-_Clone_1.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology/rp100428-12_idC_-_Scale_x1.000_y1.025_z1.000_-_Clone_1.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_DBC_bAC217_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology/og061123b1-3_idB_-_Scale_x1.000_y0.975_z1.000_-_Clone_4.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology/og061123b1-3_idB_-_Scale_x1.000_y0.975_z1.000_-_Clone_4.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_LBC_bAC217_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology/C040601.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology/C040601.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_MC_bAC217_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology/C080301B1_-_Scale_x1.000_y1.050_z1.000_-_Clone_2.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology/C080301B1_-_Scale_x1.000_y1.050_z1.000_-_Clone_2.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NBC_bAC217_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology/rp110125_L5-2_idA_-_Scale_x1.000_y0.950_z1.000_-_Clone_42.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology/rp110125_L5-2_idA_-_Scale_x1.000_y0.950_z1.000_-_Clone_42.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_NGC_bNAC219_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology/og061106a1_idA_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology/og061106a1_idA_-_Scale_x1.000_y1.050_z1.000_-_Clone_5.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_SBC_bNAC219_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_HVA.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology/dend-C231296A-P3_axon-C231296A-P3_-_Clone_9.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology/dend-C231296A-P3_axon-C231296A-P3_-_Clone_9.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_STPC_cADpyr232_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_HVA.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology/dend-C060114A2_axon-C060114A5.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology/dend-C060114A2_axon-C060114A5.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC1_cADpyr232_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_HVA.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology/dend-C060114A7_axon-C060116A3_-_Clone_2.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology/dend-C060114A7_axon-C060116A3_-_Clone_2.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_TTPC2_cADpyr232_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/LICENSE` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/README` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/README`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/biophysics.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/biophysics.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/constants.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/constants.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/creategui.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/creategui.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/createsimulation.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/createsimulation.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/init.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/init.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/CaDynamics_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_HVA.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_LVAst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ca_LVAst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ih.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Ih.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Im.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Im.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Pst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Pst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Tst.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/K_Tst.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTa_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTa_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTs2_t.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/NaTs2_t.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Nap_Et2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/Nap_Et2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbAMPANMDA_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/ProbGABAAB_EMS.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SK_E2.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SK_E2.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SKv3_1.mod` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mechanisms/SKv3_1.mod`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology/dend-Fluo15_left_axon-Fluo15_left_-_Scale_x1.000_y0.950_z1.000_-_Clone_30.asc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology/dend-Fluo15_left_axon-Fluo15_left_-_Scale_x1.000_y0.950_z1.000_-_Clone_30.asc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/morphology.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mosinit.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/mosinit.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/ringplot.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/ringplot.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_RmpRiTau.py` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/run_RmpRiTau.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/mtype_map.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/mtype_map.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.tsv` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synapses.tsv`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synconf.txt` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/synapses/synconf.txt`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/template.hoc` & `MEArec-1.9.1/src/MEArec/cell_models/bbp/L5_UTPC_cADpyr232_1/template.hoc`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/cli.py` & `MEArec-1.9.1/src/MEArec/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,14 +401,17 @@
     if kwargs["filter"]:
         params_dict["recordings"]["filter"] = True
     else:
         params_dict["recordings"]["filter"] = False
     if kwargs["filt_cutoff"] is not None:
         if isinstance(kwargs["filt_cutoff"], tuple):
             kwargs["filt_cutoff"] = list(kwargs["filt_cutoff"])
+        # for high-pass filter, make a scalar
+        if len(kwargs["filt_cutoff"]) == 1:
+            kwargs["filt_cutoff"] = kwargs["filt_cutoff"][0]
         params_dict["recordings"]["filter_cutoff"] = kwargs["filt_cutoff"]
     if kwargs["filt_order"] is not None:
         params_dict["recordings"]["filt_order"] = kwargs["filt_order"]
     if kwargs["fs"] is not None:
         params_dict["recordings"]["fs"] = kwargs["fs"]
     else:
         params_dict["recordings"]["fs"] = None
```

### Comparing `MEArec-1.9.0/src/MEArec/default_params/recordings_params.yaml` & `MEArec-1.9.1/src/MEArec/default_params/recordings_params.yaml`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/default_params/templates_params.yaml` & `MEArec-1.9.1/src/MEArec/default_params/templates_params.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 probe: Neuronexus-32 # extracellular probe (if None probes are listed)
 ncontacts: 10 # number of contacts per recording site
 overhang: 30 # extension in um beyond MEA boundaries for neuron locations (if lim is null)
 offset: 0 # plane offset (um) for MEA
 xlim: [10,80] # limits ( low high ) for neuron locations in the x-axis (depth)
 ylim: null # limits ( low high ) for neuron locations in the y-axis
 zlim: null # limits ( low high ) for neuron locations in the z-axis
-x_distr: 'uniform' # distribution of x locsations ('uniform' | 'beta')
+x_distr: 'uniform' # distribution of x locations ('uniform' | 'beta')
 beta_distr_params: [1.5, 5] # parameters for beta distribution of x locations (depth)
 min_amp: 30 # minimum amplitude for detection
 check_eap_shape: True # if True, EAPs with negative peaks smaller than positive peaks are discarded
 n: 50 # number of EAPs per cell model
 seed: null # random seed for positions and rotations
 
 drifting: False # if True, drifting templates are simulated
```

### Comparing `MEArec-1.9.0/src/MEArec/drift_tools.py` & `MEArec-1.9.1/src/MEArec/drift_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,25 +133,25 @@
 
             # compute half period for a regular drift speed
             half_period = slow_drift_amplitude / (slow_drift_velocity / 60)
 
             # triangle / sine frequency depends on the velocity
             freq = 1.0 / (2 * half_period)
 
-            times = np.arange(end_drift_index - start_drift_index) / drift_fs
+            drift_times = np.arange(end_drift_index - start_drift_index) / drift_fs
 
             if slow_drift_waveform == "triangluar":
-                triangle = np.abs(scipy.signal.sawtooth(2 * np.pi * freq * times + np.pi / 2))
+                triangle = np.abs(scipy.signal.sawtooth(2 * np.pi * freq * drift_times + np.pi / 2))
                 triangle *= slow_drift_amplitude
                 triangle -= slow_drift_amplitude / 2.0
 
                 drift_vector_um[start_drift_index:end_drift_index] = triangle
                 drift_vector_um[end_drift_index:] = triangle[-1]
             elif slow_drift_waveform == "sine":
-                sine = np.cos(2 * np.pi * freq * times + np.pi / 2)
+                sine = np.cos(2 * np.pi * freq * drift_times + np.pi / 2)
                 sine *= slow_drift_amplitude / 2.0
 
                 drift_vector_um[start_drift_index:end_drift_index] = sine
                 drift_vector_um[end_drift_index:] = sine[-1]
             else:
                 raise NotImplementedError("slow_drift_waveform")
```

### Comparing `MEArec-1.9.0/src/MEArec/generation_tools.py` & `MEArec-1.9.1/src/MEArec/generation_tools.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/generators/recgensteps.py` & `MEArec-1.9.1/src/MEArec/generators/recgensteps.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 ):
     np.random.seed(seed_list[ch])
     length = i_stop - i_start
     additive_noise = noise_level * np.random.randn(length, num_chan)
 
     if noise_color:
         # iir peak filter
-        b_iir, a_iir = scipy.signal.iirpeak(color_peak, Q=color_q, fs=fs)
+        b_iir, a_iir = scipy.signal.iirpeak(color_peak, Q=color_q, fs=float(fs))
         additive_noise = scipy.signal.filtfilt(b_iir, a_iir, additive_noise, axis=0, padlen=1000)
         additive_noise += (
             color_noise_floor
             * np.std(additive_noise)
             * np.random.randn(additive_noise.shape[0], additive_noise.shape[1])
         )
         additive_noise = additive_noise * (noise_level / np.std(additive_noise))
@@ -350,15 +350,15 @@
 ):
     np.random.seed(seed_list[ch])
     length = i_stop - i_start
 
     additive_noise = noise_level * np.random.multivariate_normal(np.zeros(n_elec), cov_dist, size=length)
     if noise_color:
         # iir peak filter
-        b_iir, a_iir = scipy.signal.iirpeak(color_peak, Q=color_q, fs=fs)
+        b_iir, a_iir = scipy.signal.iirpeak(color_peak, Q=color_q, fs=float(fs))
         additive_noise = scipy.signal.filtfilt(b_iir, a_iir, additive_noise, axis=0, padlen=1000)
         additive_noise = additive_noise + color_noise_floor * np.std(additive_noise) * np.random.multivariate_normal(
             np.zeros(n_elec), cov_dist, size=length
         )
     additive_noise = additive_noise * (noise_level / np.std(additive_noise))
 
     return_dict = {}
```

### Comparing `MEArec-1.9.0/src/MEArec/generators/recordinggenerator.py` & `MEArec-1.9.1/src/MEArec/generators/recordinggenerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,15 @@
             tmp_prefix = "".join([random.choice(string.ascii_letters) for i in range(5)]) + "_"
         if self.tmp_mode is not None:
             if self.tmp_folder is None:
                 self.tmp_folder = Path(tempfile.mkdtemp())
                 self._is_tmp_folder_local = False
             else:
                 self.tmp_folder = Path(self.tmp_folder)
+                self.tmp_folder.mkdir(exist_ok=True, parents=True)
                 self._is_tmp_folder_local = True
         else:
             self._is_tmp_folder_local = False
 
         self._verbose = verbose
         if self._verbose is not None and isinstance(self._verbose, bool) or isinstance(self._verbose, int):
             verbose_1 = self._verbose >= 1
@@ -444,15 +445,15 @@
                     assert len(rec_params["exp_decay"]) == n_bursting, (
                         "'exp_decay' should have the same length as " "the number of bursting units"
                     )
                     params["recordings"]["exp_decay"] = rec_params["exp_decay"]
             exp_decay = params["recordings"]["exp_decay"]
 
             if "n_burst_spikes" not in rec_params.keys():
-                params["recordings"]["exp_decay"] = [10] * n_bursting
+                params["recordings"]["n_burst_spikes"] = [10] * n_bursting
             else:
                 if not isinstance(rec_params["n_burst_spikes"], list):
                     assert isinstance(rec_params["n_burst_spikes"], int), "'n_burst_spikes' can be list or int"
                     params["recordings"]["n_burst_spikes"] = [rec_params["n_burst_spikes"]] * n_bursting
                 else:
                     assert len(rec_params["n_burst_spikes"]) == n_bursting, (
                         "'n_burst_spikes' should have the same " "length as the number of bursting units"
@@ -682,15 +683,15 @@
                 spike_traces[:] = 0
                 # spike_traces = spike_traces.transpose()
             # file names for templates
             tmp_templates_pad = self.tmp_folder / (tmp_prefix + "templates_pad.raw")
             tmp_templates_rs = self.tmp_folder / (tmp_prefix + "templates_resample.raw")
             tmp_templates_jit = self.tmp_folder / (tmp_prefix + "templates_jitter.raw")
             self._to_remove_on_delete.extend(
-                [tmp_path_0, tmp_path_1, tmp_templates_pad, tmp_templates_rs, tmp_templates_jit]
+                [tmp_path_0, tmp_path_1, tmp_templates_pad, tmp_templates_jit]
             )
         else:
             recordings = np.zeros((n_samples, n_elec), dtype=dtype)
             spike_traces = np.zeros((n_samples, n_neurons), dtype=dtype)
             tmp_templates_pad = None
             tmp_templates_rs = None
             tmp_templates_jit = None
@@ -820,15 +821,17 @@
                     else:
                         reordered_idx_cells = idxs_cells
 
                     template_celltypes = celltypes[reordered_idx_cells]
                     template_locs = np.array(locs)[reordered_idx_cells]
                     template_rots = np.array(rots)[reordered_idx_cells]
                     template_bin = np.array(bin_cat)[reordered_idx_cells]
-                    templates = np.array(eaps)[reordered_idx_cells]
+                    templates = np.empty((len(reordered_idx_cells), *eaps.shape[1:]), dtype=eaps.dtype)
+                    for i, reordered_idx in enumerate(reordered_idx_cells):
+                        templates[i] = eaps[reordered_idx]
                     self.template_ids = reordered_idx_cells
                 else:
                     print(f"Using provided template ids: {self.template_ids}")
                     ordered_ids = np.all(np.diff(self.template_ids) > 0)
                     if ordered_ids:
                         template_celltypes = celltypes[self.template_ids]
                         template_locs = np.array(locs[self.template_ids])
@@ -943,14 +946,17 @@
                         tmp_file=tmp_templates_rs,
                         parallel=parallel_templates,
                     )
                     # adjust pad_samples to account for resampling
                     pad_samples = [int((pp * fs.rescale("kHz")).magnitude) for pp in pad_len]
                     if verbose_1:
                         print("Elapsed resample time:", time.time() - t_rs)
+                    self._to_remove_on_delete.extend(
+                        [tmp_templates_rs]
+                    )
                 else:
                     templates_rs = templates_pad
 
                 if verbose_1:
                     print("Creating time jittering")
                 jitter = 1.0 / fs
                 t_j = time.time()
@@ -983,15 +989,15 @@
                     sig = sigmoid(sigmoid_x, b) + 0.5
                     window = np.ones(templates.shape[-1])
                     window[:sigmoid_samples] = sig
                     window[-sigmoid_samples:] = sig[::-1]
 
                     if verbose_1:
                         print("Smoothing templates")
-                    templates = templates * window
+                    templates *= window
 
                 # delete temporary preprocessed templates
                 del templates_rs, templates_pad
             else:
                 gain_to_int = None
                 templates = self.templates
                 pre_peak_fraction = (pad_len[0] + cut_outs[0]) / (np.sum(pad_len) + np.sum(cut_outs))
```

### Comparing `MEArec-1.9.0/src/MEArec/generators/spiketraingenerator.py` & `MEArec-1.9.1/src/MEArec/generators/spiketraingenerator.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/generators/templategenerator.py` & `MEArec-1.9.1/src/MEArec/generators/templategenerator.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/simulate_cells.py` & `MEArec-1.9.1/src/MEArec/simulate_cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,15 +871,15 @@
             saved += 1
         else:
             pass
 
     if verbose >= 1:
         print(f"Done generating EAPs for {cell_name}")
 
-    saved_eaps = np.array(saved_eaps)
+    saved_eaps = np.array(saved_eaps, dtype=np.float32)
     saved_positions = np.array(saved_positions)
     saved_rotations = np.array(saved_rotations)
 
     if save:
         np.save(str(save_folder / f"eap-{cell_save_name}"), saved_eaps)
         np.save(str(save_folder / f"pos-{cell_save_name}"), saved_positions)
         np.save(str(save_folder / f"rot-{cell_save_name}"), saved_rotations)
@@ -1103,15 +1103,15 @@
 
         Returns
         --------
         R : 3x3 matrix
             random rotation matrix
         """
         gamma = np.random.uniform(0, 2.0 * np.pi)
-        rotation_z = np.matrix([[np.cos(gamma), -np.sin(gamma), 0], [np.sin(gamma), np.cos(gamma), 0], [0, 0, 1]])
+        rotation_z = np.array([[np.cos(gamma), -np.sin(gamma), 0], [np.sin(gamma), np.cos(gamma), 0], [0, 0, 1]])
         x = np.random.uniform(size=2)
         v = np.array(
             [np.cos(2.0 * np.pi * x[0]) * np.sqrt(x[1]), np.sin(2.0 * np.pi * x[0]) * np.sqrt(x[1]), np.sqrt(1 - x[1])]
         )
         H = np.identity(3) - 2.0 * np.outer(v, v)
         M = -np.dot(H, rotation_z)
         return M
@@ -1264,22 +1264,22 @@
     else:
         cell.set_pos(pos[0], pos[1], pos[2])
         found_position = True
 
     cell.set_rotation(x=x_rot, y=y_rot, z=z_rot)
     rot = [x_rot, y_rot, z_rot]
 
-    lfp = electrodes.get_transformation_matrix() @ cell.imem
+    lfp = np.array(electrodes.get_transformation_matrix() @ cell.imem, dtype=np.float32)
 
     # Reverse rotation to bring cell back into initial rotation state
     if rotation is not None:
         rev_rot = [-r for r in rot]
         cell.set_rotation(rev_rot[0], rev_rot[1], rev_rot[2], rotation_order="zyx")
 
-    return 1000 * lfp, pos, rot, found_position
+    return 1e3 * lfp, pos, rot, found_position
 
 
 def str2bool(v):
     """Transform string to bool
 
     Parameters
     -----------
```

### Comparing `MEArec-1.9.0/src/MEArec/tests/test_generators.py` & `MEArec-1.9.1/src/MEArec/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `MEArec-1.9.0/src/MEArec/tools.py` & `MEArec-1.9.1/src/MEArec/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
     for idx, f in enumerate(eaplist):
         celltype = f.parts[-1].split("-")[1][:-4]
         if verbose:
             print("loading cell type: ", f)
         if celltypes is not None:
             if celltype in celltypes:
-                eaps = np.load(str(eaplist[idx]))
+                eaps = np.load(str(eaplist[idx]), mmap_mode="r")
                 locs = np.load(str(loclist[idx]))
                 rots = np.load(str(rotlist[idx]))
 
                 if samples_per_cat is None or samples_per_cat > len(eaps):
                     samples_to_read = len(eaps)
                 else:
                     samples_to_read = samples_per_cat
@@ -226,33 +226,40 @@
                 rot_list.extend(rots[:samples_to_read])
                 loc_list.extend(locs[:samples_to_read])
                 cat_list.extend([celltype] * samples_to_read)
                 loaded_categories.add(celltype)
             else:
                 ignored_categories.add(celltype)
         else:
-            eaps = np.load(str(eaplist[idx]))
+            eaps = np.load(str(eaplist[idx]), mmap_mode="r")
             locs = np.load(str(loclist[idx]))
             rots = np.load(str(rotlist[idx]))
 
             if samples_per_cat is None or samples_per_cat > len(eaps):
                 samples_to_read = len(eaps)
             else:
                 samples_to_read = samples_per_cat
 
             eap_list.extend(eaps[:samples_to_read])
             rot_list.extend(rots[:samples_to_read])
             loc_list.extend(locs[:samples_to_read])
             cat_list.extend([celltype] * samples_to_read)
             loaded_categories.add(celltype)
 
+    if len(eap_list) > 0:
+        all_eaps = np.lib.format.open_memmap(templates_folder / "all_eaps.npy", mode="w+", dtype=eaps[0].dtype, shape=(len(eap_list), *eap_list[0].shape))
+        for i in range(len(eap_list)):
+            all_eaps[i, ...] = eap_list[i]
+    else:
+        all_eaps = np.array([])
+
     if verbose:
         print("Done loading spike data ...")
 
-    return np.array(eap_list), np.array(loc_list), np.array(rot_list), np.array(cat_list, dtype=str)
+    return all_eaps, np.array(loc_list), np.array(rot_list), np.array(cat_list, dtype=str)
 
 
 def load_templates(templates, return_h5_objects=True, verbose=False, check_suffix=True):
     """
     Load generated eap templates.
 
     Parameters
@@ -549,60 +556,64 @@
             f.create_dataset("rotations", data=tempgen.rotations)
         if len(tempgen.templates) > 0:
             f.create_dataset("templates", data=tempgen.templates)
     if verbose:
         print("\nSaved  templates in", filename, "\n")
 
 
-def save_recording_generator(recgen, filename=None, verbose=False):
+def save_recording_generator(recgen, filename=None, verbose=False, include_spike_traces: bool = True):
     """
     Save recordings to disk.
 
     Parameters
     ----------
     recgen : RecordingGenerator
         RecordingGenerator object to be saved
     filename : str
         Path to .h5 file
     verbose : bool
         If True output is verbose
+    include_spike_traces: bool, default=True
+        If True, will include the spike traces (which can be large for many units)
     """
     filename = Path(filename)
     if not filename.parent.is_dir():
         os.makedirs(str(filename.parent))
     assert filename.suffix in [".h5", ".hdf5"], "Provide an .h5 or .hdf5 file name"
     with h5py.File(filename, "w") as f:
         f.attrs["mearec_version"] = mearec_version
         f.attrs["date"] = datetime.now().strftime("%y-%m-%d %H:%M:%S")
-        save_recording_to_file(recgen, f)
+        save_recording_to_file(recgen, f, include_spike_traces=include_spike_traces)
     if verbose:
         print("\nSaved recordings in", filename, "\n")
 
 
-def save_recording_to_file(recgen, f, path=""):
+def save_recording_to_file(recgen, f, path="", include_spike_traces: bool = True):
     """
     Save recordings to file handler.
 
     Parameters
     ----------
     recgen : RecordingGenerator
         RecordingGenerator object to be saved
     filename : _io.TextIOWrapper
         File handler
+    include_spike_traces: bool, default=True
+        If True, will include the spike traces (can be heavy)
     """
     save_dict_to_hdf5(recgen.info, f, path + "info/")
     if len(recgen.voltage_peaks) > 0:
         f.create_dataset(path + "voltage_peaks", data=recgen.voltage_peaks)
     if len(recgen.channel_positions) > 0:
         f.create_dataset(path + "channel_positions", data=recgen.channel_positions)
     if len(recgen.recordings) > 0:
         f.create_dataset(path + "recordings", data=recgen.recordings)
         if recgen.gain_to_uV is not None:
             f["recordings"].attrs["gain_to_uV"] = recgen.gain_to_uV
-    if len(recgen.spike_traces) > 0:
+    if len(recgen.spike_traces) > 0 and include_spike_traces:
         f.create_dataset(path + "spike_traces", data=recgen.spike_traces)
     if len(recgen.spiketrains) > 0:
         for ii in range(len(recgen.spiketrains)):
             st = recgen.spiketrains[ii]
             f.create_dataset(path + "spiketrains/{}/times".format(ii), data=st.times.rescale("s").magnitude)
             f.create_dataset(path + "spiketrains/{}/t_stop".format(ii), data=st.t_stop)
             if st.waveforms is not None:
@@ -1799,26 +1810,26 @@
     -------
     padded_template : np.array
         Padded template
 
     """
     import scipy.interpolate as interp
 
-    n_pre = pad_samples[0]
-    n_post = pad_samples[1]
+    assert len(pad_samples) == 2, "'pad_samples' should be a list/tuple/array of length 2!"
+    n_pre, n_post = pad_samples
 
     padded_template = np.zeros((template.shape[0], int(n_pre) + template.shape[1] + n_post))
     splines = np.zeros((template.shape[0], int(n_pre) + template.shape[1] + n_post))
 
     for i, sp in enumerate(template):
         # Remove inital offset
         sp_copy = deepcopy(sp)
         padded_sp = np.zeros(n_pre + len(sp) + n_post)
         padded_t = np.arange(len(padded_sp))
-        initial_offset = np.mean(sp[0])
+        initial_offset = sp[0]
         sp_copy -= initial_offset
 
         x_pre = float(n_pre)
         x_pre_pad = np.arange(n_pre)
         x_post = float(n_post)
         x_post_pad = np.arange(n_post)[::-1]
 
@@ -3753,15 +3764,15 @@
 
     if not drifting:
         template_jitter = np.zeros((n_jitters, template.shape[0], template.shape[1]))
         temp_up = ss.resample_poly(template, upsample, 1, axis=1)
         nsamples_up = temp_up.shape[1]
         for n in np.arange(n_jitters):
             # align waveform
-            shift = int((jitter * (rng.random() - 0.5) * upsample * fs).magnitude)
+            shift = int((jitter * (rng.rand() - 0.5) * upsample * fs).magnitude)
             if shift > 0:
                 t_jitt = np.pad(temp_up, [(0, 0), (np.abs(shift), 0)], "constant")[:, :nsamples_up]
             elif shift < 0:
                 t_jitt = np.pad(temp_up, [(0, 0), (0, np.abs(shift))], "constant")[:, -nsamples_up:]
             else:
                 t_jitt = temp_up
             temp_down = t_jitt[:, ::upsample]
@@ -3771,15 +3782,15 @@
             print("Jittering: neuron ", i)
         template_jitter = np.zeros((template.shape[0], n_jitters, template.shape[1], template.shape[2]))
         for tp, tem_p in enumerate(template):
             temp_up = ss.resample_poly(tem_p, upsample, 1, axis=1)
             nsamples_up = temp_up.shape[1]
             for n in np.arange(n_jitters):
                 # align waveform
-                shift = int((jitter * rng.randn() * upsample * fs).magnitude)
+                shift = int((jitter * rng.rand() * upsample * fs).magnitude)
                 if shift > 0:
                     t_jitt = np.pad(temp_up, [(0, 0), (np.abs(shift), 0)], "constant")[:, :nsamples_up]
                 elif shift < 0:
                     t_jitt = np.pad(temp_up, [(0, 0), (0, np.abs(shift))], "constant")[:, -nsamples_up:]
                 else:
                     t_jitt = temp_up
                 temp_down = t_jitt[:, ::upsample]
```

### Comparing `MEArec-1.9.0/src/MEArec.egg-info/SOURCES.txt` & `MEArec-1.9.1/src/MEArec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

