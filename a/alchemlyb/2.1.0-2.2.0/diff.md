# Comparing `tmp/alchemlyb-2.1.0.tar.gz` & `tmp/alchemlyb-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemlyb-2.1.0.tar", last modified: Thu Jun 22 16:34:11 2023, max compression
+gzip compressed data, was "alchemlyb-2.2.0.tar", last modified: Sat Apr  6 19:25:26 2024, max compression
```

## Comparing `alchemlyb-2.1.0.tar` & `alchemlyb-2.2.0.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.828814 alchemlyb-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/src/alchemlyb/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/src/alchemlyb/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/convergence/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/convergence/pade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/bar_.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/mbar_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/ti_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/amber.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/gmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/gomc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/namd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/postprocessors/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19870 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/preprocessing/subsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_amber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gomc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_namd.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_fep_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_ti_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow_ABFE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/dF_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/mbar_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/ti_dhdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/src/alchemlyb/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33217 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/workflows/abfe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68573 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.685085 alchemlyb-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.685085 alchemlyb-2.2.0/src/alchemlyb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/convergence/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/convergence/pade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/bar_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/mbar_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/ti_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/estimators/ti_gaussian_quadrature_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15731 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/amber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/gmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/gomc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/namd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/parsing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.689085 alchemlyb-2.2.0/src/alchemlyb/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/postprocessors/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.693085 alchemlyb-2.2.0/src/alchemlyb/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20197 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/preprocessing/subsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.693085 alchemlyb-2.2.0/src/alchemlyb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.693085 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_amber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gomc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_namd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_fep_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19462 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_gaussian_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17565 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow_ABFE.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/dF_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/mbar_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/visualisation/ti_dhdl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33431 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/workflows/abfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/src/alchemlyb/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:25:26.697085 alchemlyb-2.2.0/src/alchemlyb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 19:25:26.000000 alchemlyb-2.2.0/src/alchemlyb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-06 19:25:09.000000 alchemlyb-2.2.0/versioneer.py
```

### Comparing `alchemlyb-2.1.0/AUTHORS` & `alchemlyb-2.2.0/AUTHORS`

 * *Files 8% similar despite different names*

```diff
@@ -43,7 +43,9 @@
   - Jérôme Hénin (@jhenin)
   - Thomas T. Joseph (@ttjoseph)
 
 2022
   - Irfan Alibay (@IAlibay)
   - Pascal Merz (@ptmerz)
   - Domenico Marson (@DrDomenicoMarson)
+2023
+  - Haoxi Li (@hl2500)
```

### Comparing `alchemlyb-2.1.0/LICENSE` & `alchemlyb-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/PKG-INFO` & `alchemlyb-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: alchemlyb
-Version: 2.1.0
+Version: 2.2.0
 Summary: the simple alchemistry library
 Author: David Dotson
 Author-email: dotsdl@gmail.com
 Maintainer: Oliver Beckstein
 Maintainer-email: orbeckst@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: numpy
+Requires-Dist: pandas>=2.1
+Requires-Dist: pymbar>=4
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: loguru
+Requires-Dist: pyarrow
 
 alchemlyb: the simple alchemistry library
 =========================================
 
 |doi| |docs| |build| |cov| |anaconda|
 
 **alchemlyb** makes alchemical free energy calculations easier to do
```

### Comparing `alchemlyb-2.1.0/README.rst` & `alchemlyb-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/setup.py` & `alchemlyb-2.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,33 +25,33 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows ",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages("src"),
     package_dir={"": "src"},
     license="BSD",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     tests_require=["pytest", "alchemtest"],
     install_requires=[
         "numpy",
-        "pandas>=1.4",
+        "pandas>=2.1",
         "pymbar>=4",
         "scipy",
         "scikit-learn",
         "matplotlib",
         "loguru",
         "pyarrow",
     ],
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/__init__.py` & `alchemlyb-2.2.0/src/alchemlyb/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/convergence/convergence.py` & `alchemlyb-2.2.0/src/alchemlyb/convergence/convergence.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/estimators/bar_.py` & `alchemlyb-2.2.0/src/alchemlyb/estimators/bar_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/estimators/mbar_.py` & `alchemlyb-2.2.0/src/alchemlyb/estimators/mbar_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/estimators/ti_.py` & `alchemlyb-2.2.0/src/alchemlyb/estimators/ti_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/__init__.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/amber.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/amber.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/gmx.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/gmx.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/gomc.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/gomc.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/namd.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/namd.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/parquet.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/parquet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,46 @@
 import pandas as pd
+from loguru import logger
 
 from . import _init_attrs
 
 
-@_init_attrs
+def _read_parquet_with_metadata(path: str, T: float) -> pd.DataFrame:
+    """
+    Check if the metadata is included in the Dataframe and has the correct
+    temperature.
+
+    Parameters
+    ----------
+    path : str
+        Path to parquet file to extract dataframe from.
+    T : float
+        Temperature in Kelvin of the simulations.
+
+    Returns
+    -------
+    DataFrame
+    """
+    df = pd.read_parquet(path)
+    if "temperature" not in df.attrs:
+        logger.warning(
+            f"No temperature metadata found in {path}. "
+            f"Serialise the Dataframe with pandas>=2.1 to preserve the metadata."
+        )
+        df.attrs["temperature"] = T
+        df.attrs["energy_unit"] = "kT"
+    else:
+        if df.attrs["temperature"] != T:
+            raise ValueError(
+                f"Temperature in the input ({T}) doesn't match the temperature "
+                f"in the dataframe ({df.attrs['temperature']})."
+            )
+    return df
+
+
 def extract_u_nk(path, T):
     r"""Return reduced potentials `u_nk` (unit: kT) from a pandas parquet file.
 
     The parquet file should be serialised from the dataframe output
     from any parser with command
     (``u_nk_df.to_parquet(path=path, index=True)``).
 
@@ -32,15 +65,15 @@
     Also parquet serialisation doesn't preserve the :attr:`pandas.DataFrame.attrs`.
     So the temperature is assigned in this function.
 
 
     .. versionadded:: 2.1.0
 
     """
-    u_nk = pd.read_parquet(path)
+    u_nk = _read_parquet_with_metadata(path, T)
     columns = list(u_nk.columns)
     if isinstance(columns[0], str) and columns[0][0] == "(":
         new_columns = []
         for column in columns:
             new_columns.append(
                 tuple(
                     map(
@@ -77,8 +110,8 @@
     Parquet serialisation doesn't preserve the :attr:`pandas.DataFrame.attrs`.
     So the temperature is assigned in this function.
 
 
     .. versionadded:: 2.1.0
 
     """
-    return pd.read_parquet(path)
+    return _read_parquet_with_metadata(path, T)
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/parsing/util.py` & `alchemlyb-2.2.0/src/alchemlyb/parsing/util.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/postprocessors/units.py` & `alchemlyb-2.2.0/src/alchemlyb/postprocessors/units.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/preprocessing/__init__.py` & `alchemlyb-2.2.0/src/alchemlyb/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/preprocessing/subsampling.py` & `alchemlyb-2.2.0/src/alchemlyb/preprocessing/subsampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,14 +359,23 @@
     Returns
     -------
     df : DataFrame or Series
         Formatted DataFrame or Series.
     series : Series
         Formatted Series.
     """
+    if series is None:
+        warnings.warn(
+            "The series input is `None`, would not subsample according to statistical inefficiency."
+        )
+
+    elif len(df) != len(series):
+        raise ValueError(
+            f"The length of df ({len(df)}) should be same as the length of series ({len(series)})."
+        )
     if _check_multiple_times(df):
         if drop_duplicates:
             df, series = _drop_duplicates(df, series)
         else:
             raise KeyError(
                 "Duplicate time values found; statistical inefficiency "
                 "only works on a single, contiguous, "
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/conftest.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Storing the fixture to be used for the tests. Note that this file will only contain
 fixture that are made directly from parsing the files. Any additional operations like
 concat should be done at local level."""
 
 import pytest
 from _pytest.logging import LogCaptureFixture
-from alchemtest.amber import load_bace_example, load_simplesolvated
+from alchemtest.amber import load_bace_example, load_simplesolvated, load_tyk2_example
 from alchemtest.gmx import (
     load_benzene,
+    load_ethanol,
     load_expanded_ensemble_case_1,
     load_expanded_ensemble_case_2,
     load_expanded_ensemble_case_3,
     load_water_particle_with_total_energy,
     load_water_particle_with_potential_energy,
     load_water_particle_without_energy,
     load_ABFE,
@@ -40,14 +41,30 @@
 
 @pytest.fixture
 def gmx_benzene_VDW_dHdl(gmx_benzene):
     return [gmx.extract_dHdl(file, T=300) for file in gmx_benzene["VDW"]]
 
 
 @pytest.fixture
+def gmx_ethanol():
+    dataset = load_ethanol()
+    return dataset["data"]
+
+
+@pytest.fixture
+def gmx_ethanol_Coulomb_dHdl(gmx_ethanol):
+    return [gmx.extract_dHdl(file, T=300) for file in gmx_ethanol["Coulomb"]]
+
+
+@pytest.fixture
+def gmx_ethanol_VDW_dHdl(gmx_ethanol):
+    return [gmx.extract_dHdl(file, T=300) for file in gmx_ethanol["VDW"]]
+
+
+@pytest.fixture
 def gmx_benzene_Coulomb_u_nk(gmx_benzene):
     return [gmx.extract_u_nk(file, T=300) for file in gmx_benzene["Coulomb"]]
 
 
 @pytest.fixture
 def gmx_benzene_VDW_u_nk(gmx_benzene):
     return [gmx.extract_u_nk(file, T=300) for file in gmx_benzene["VDW"]]
@@ -61,15 +78,15 @@
 @pytest.fixture
 def gmx_ABFE():
     dataset = load_ABFE()
     return dataset["data"]
 
 
 @pytest.fixture
-def gmx_ABFE_complex_n_uk(gmx_ABFE):
+def gmx_ABFE_complex_u_nk(gmx_ABFE):
     return [gmx.extract_u_nk(file, T=300) for file in gmx_ABFE["complex"]]
 
 
 @pytest.fixture
 def gmx_ABFE_complex_dHdl(gmx_ABFE):
     return [gmx.extract_dHdl(file, T=300) for file in gmx_ABFE["complex"]]
 
@@ -217,14 +234,23 @@
     return [
         amber.extract_u_nk(filename, T=298.0)
         for filename in dataset["data"]["complex"]["vdw"]
     ]
 
 
 @pytest.fixture
+def amber_tyk2_example_complex():
+    dataset = load_tyk2_example()
+
+    return [
+        amber.extract_dHdl(filename, T=300.0) for filename in dataset["data"]["complex"]
+    ]
+
+
+@pytest.fixture
 def gomc_benzene():
     dataset = gomc_load_benzene()
     return dataset["data"]
 
 
 @pytest.fixture
 def gomc_benzene_u_nk(gomc_benzene):
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_amber.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_amber.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Amber parser tests.
 
 """
+
 import bz2
 import logging
 
 import pandas as pd
 import pytest
 from alchemtest.amber import load_bace_example
 from alchemtest.amber import load_bace_improper
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gmx.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gmx.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gomc.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_gomc.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_namd.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_namd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """NAMD parser tests.
 
 """
+
 import bz2
 from os.path import basename
 from re import search
 
 import pytest
 from alchemtest.namd import load_idws
 from alchemtest.namd import load_restarted
 from alchemtest.namd import load_restarted_reversed
 from alchemtest.namd import load_tyr2ala
 
 from alchemlyb.parsing.namd import extract_u_nk, extract
 
+
 # Indices of lambda values in the following line in NAMD fepout files:
 # #NEW FEP WINDOW: LAMBDA SET TO 0.6 LAMBDA2 0.7 LAMBDA_IDWS 0.5
 LAMBDA1_IDX_NEW = 6
 LAMBDA2_IDX_NEW = 8
 LAMBDA_IDWS_IDX_NEW = 10
 # Indices of lambda values in the following type of line in NAMD fepout files:
 # #Free energy change for lambda window [ 0.6 0.7 ] is 0.12345 ; net change until now is 0.12345
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_util.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/parsing/test_util.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_convergence.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_convergence.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_fep_estimators.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_fep_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for all FEP-based estimators in ``alchemlyb``.
 
 """
+
 import pytest
 
 import alchemlyb
 from alchemlyb.estimators import MBAR, BAR
 
 
 class FEPestimatorMixin:
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_preprocessing.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for preprocessing functions.
 
 """
+
 import logging
 
 import numpy as np
 import pytest
 from numpy.testing import assert_allclose
 
 import alchemlyb
@@ -37,16 +38,16 @@
 
 @pytest.fixture()
 def u_nk(gmx_benzene_Coulomb_u_nk):
     return gmx_benzene_Coulomb_u_nk[0]
 
 
 @pytest.fixture()
-def multi_index_u_nk(gmx_ABFE_complex_n_uk):
-    return gmx_ABFE_complex_n_uk[0]
+def multi_index_u_nk(gmx_ABFE_complex_u_nk):
+    return gmx_ABFE_complex_u_nk[0]
 
 
 @pytest.fixture()
 def multi_index_dHdl(gmx_ABFE_complex_dHdl):
     return gmx_ABFE_complex_dHdl[0]
 
 
@@ -466,15 +467,15 @@
                 multi_index_dHdl,
             )
         )
         == 501
     )
 
 
-def test_raise_non_uk(multi_index_dHdl):
+def test_raise_nou_nk(multi_index_dHdl):
     with pytest.raises(ValueError):
         decorrelate_u_nk(
             multi_index_dHdl,
         )
 
 
 class TestDhdl2series:
@@ -540,7 +541,20 @@
     def test_statistical_inefficiency(self, caplog, u_nk):
         with caplog.at_level(logging.DEBUG):
             decorrelate_u_nk(u_nk)
 
             assert "Running statistical inefficiency analysis." in caplog.text
             assert "Statistical inefficiency:" in caplog.text
             assert "Number of uncorrelated samples:" in caplog.text
+
+
+def test_unequil_input(dHdl):
+    with pytest.raises(ValueError, match="should be same as the length of series"):
+        statistical_inefficiency(dHdl, series=dHdl[:10])
+
+
+def test_series_none(dHdl):
+    with pytest.warns(
+        UserWarning,
+        match="The series input is `None`, would not subsample according to statistical inefficiency.",
+    ):
+        statistical_inefficiency(dHdl, series=None)
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_ti_estimators.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_ti_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for all TI-based estimators in ``alchemlyb``.
 
 """
+
 import pandas as pd
 import pytest
 
 import alchemlyb
 from alchemlyb.estimators import TI
 from alchemlyb.parsing import amber
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_units.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_visualisation.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_visualisation.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow_ABFE.py` & `alchemlyb-2.2.0/src/alchemlyb/tests/test_workflow_ABFE.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         breakdown=True,
         forwrev=10,
     )
     return workflow
 
 
 class TestInit:
-    def test_nofilematch(self):
+    def test_nofilematch(self, tmp_path):
         with pytest.raises(ValueError, match="No file has been matched to"):
             ABFE(
-                dir="./",
+                dir=str(tmp_path),
                 prefix="dhdl",
                 suffix="xvg",
                 T=310,
             )
 
     def test_notdir(self):
         with pytest.raises(ValueError, match="The input directory `dir`="):
@@ -254,15 +254,15 @@
     def test_single_estimator_ti(self, workflow, monkeypatch):
         monkeypatch.setattr(workflow, "estimator", dict())
         monkeypatch.setattr(workflow, "summary", None)
         workflow.estimate(estimators="TI")
         summary = workflow.generate_result()
         assert np.isclose(summary["TI"]["Stages"]["TOTAL"], 21.51472826028906, 0.1)
 
-    def test_unprocessed_n_uk(self, workflow, monkeypatch):
+    def test_unprocessed_u_nk(self, workflow, monkeypatch):
         monkeypatch.setattr(workflow, "u_nk_sample_list", None)
         monkeypatch.setattr(workflow, "estimator", dict())
         workflow.estimate()
         assert len(workflow.estimator) == 3
         assert "MBAR" in workflow.estimator
 
     def test_unpertubed_lambda(self, workflow, monkeypatch, gmx_benzene_Coulomb_dHdl):
@@ -364,14 +364,20 @@
             workflow.check_convergence(10, estimator="aaa")
 
     def test_ti_convergence(self, workflow, monkeypatch):
         monkeypatch.setattr(workflow, "convergence", None)
         workflow.check_convergence(10, estimator="TI")
         assert len(workflow.convergence) == 10
 
+    def test_preserve_unit(self, workflow, monkeypatch):
+        monkeypatch.setattr(workflow, "convergence", None)
+        monkeypatch.setattr(workflow, "units", "kcal/mol")
+        workflow.check_convergence(2, estimator="TI")
+        assert np.allclose(workflow.convergence["data_fraction"], [0.5, 1.0])
+
     def test_unprocessed_dhdl(self, workflow, monkeypatch):
         monkeypatch.setattr(workflow, "dHdl_sample_list", None)
         monkeypatch.setattr(workflow, "convergence", None)
         workflow.check_convergence(10, estimator="TI")
         assert len(workflow.convergence) == 10
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/visualisation/convergence.py` & `alchemlyb-2.2.0/src/alchemlyb/visualisation/convergence.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/visualisation/dF_state.py` & `alchemlyb-2.2.0/src/alchemlyb/visualisation/dF_state.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/visualisation/mbar_matrix.py` & `alchemlyb-2.2.0/src/alchemlyb/visualisation/mbar_matrix.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/visualisation/ti_dhdl.py` & `alchemlyb-2.2.0/src/alchemlyb/visualisation/ti_dhdl.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb/workflows/abfe.py` & `alchemlyb-2.2.0/src/alchemlyb/workflows/abfe.py`

 * *Files 2% similar despite different names*

```diff
@@ -797,14 +797,17 @@
             msg = (
                 f"Estimator {estimator} is not supported. Choose one from "
                 f"{FEP_ESTIMATORS + TI_ESTIMATORS}."
             )
             logger.error(msg)
             raise ValueError(msg)
 
-        self.convergence = get_unit_converter(self.units)(convergence)
+        unit_converted_convergence = get_unit_converter(self.units)(convergence)
+        # Otherwise the data_fraction column is converted as well.
+        unit_converted_convergence["data_fraction"] = convergence["data_fraction"]
+        self.convergence = unit_converted_convergence
 
         logger.info(f"Plot convergence analysis to {dF_t} under {self.out}.")
 
         ax = plot_convergence(self.convergence, units=self.units, ax=ax)
         ax.figure.savefig(join(self.out, dF_t))
         return ax
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb/workflows/base.py` & `alchemlyb-2.2.0/src/alchemlyb/workflows/base.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.1.0/src/alchemlyb.egg-info/PKG-INFO` & `alchemlyb-2.2.0/src/alchemlyb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: alchemlyb
-Version: 2.1.0
+Version: 2.2.0
 Summary: the simple alchemistry library
 Author: David Dotson
 Author-email: dotsdl@gmail.com
 Maintainer: Oliver Beckstein
 Maintainer-email: orbeckst@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: numpy
+Requires-Dist: pandas>=2.1
+Requires-Dist: pymbar>=4
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: loguru
+Requires-Dist: pyarrow
 
 alchemlyb: the simple alchemistry library
 =========================================
 
 |doi| |docs| |build| |cov| |anaconda|
 
 **alchemlyb** makes alchemical free energy calculations easier to do
```

### Comparing `alchemlyb-2.1.0/src/alchemlyb.egg-info/SOURCES.txt` & `alchemlyb-2.2.0/src/alchemlyb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/alchemlyb/convergence/convergence.py
 src/alchemlyb/convergence/pade.py
 src/alchemlyb/estimators/__init__.py
 src/alchemlyb/estimators/bar_.py
 src/alchemlyb/estimators/base.py
 src/alchemlyb/estimators/mbar_.py
 src/alchemlyb/estimators/ti_.py
+src/alchemlyb/estimators/ti_gaussian_quadrature_.py
 src/alchemlyb/parsing/__init__.py
 src/alchemlyb/parsing/amber.py
 src/alchemlyb/parsing/gmx.py
 src/alchemlyb/parsing/gomc.py
 src/alchemlyb/parsing/namd.py
 src/alchemlyb/parsing/parquet.py
 src/alchemlyb/parsing/util.py
@@ -34,14 +35,15 @@
 src/alchemlyb/tests/__init__.py
 src/alchemlyb/tests/conftest.py
 src/alchemlyb/tests/test_convergence.py
 src/alchemlyb/tests/test_fep_estimators.py
 src/alchemlyb/tests/test_import.py
 src/alchemlyb/tests/test_preprocessing.py
 src/alchemlyb/tests/test_ti_estimators.py
+src/alchemlyb/tests/test_ti_gaussian_quadrature.py
 src/alchemlyb/tests/test_units.py
 src/alchemlyb/tests/test_version.py
 src/alchemlyb/tests/test_visualisation.py
 src/alchemlyb/tests/test_workflow.py
 src/alchemlyb/tests/test_workflow_ABFE.py
 src/alchemlyb/tests/parsing/__init__.py
 src/alchemlyb/tests/parsing/test_amber.py
```

### Comparing `alchemlyb-2.1.0/versioneer.py` & `alchemlyb-2.2.0/versioneer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 
-# Version: 0.18
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +82,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -162,45 +187,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -220,39 +245,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -261,186 +275,263 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
 
-def get_root():
+
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = ("Versioneer was unable to run the project root directory. "
                "Versioneer requires setup.py to be executed from "
                "its immediate directory (like 'python setup.py COMMAND'), "
                "or in a way that lets it use sys.argv[0] to find the root "
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -448,16 +539,23 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -467,161 +565,187 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-    def decorate(f):
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -629,52 +753,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -683,15 +852,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -708,34 +877,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -752,31 +922,79 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -795,20 +1013,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -817,15 +1064,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -837,15 +1084,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -857,47 +1104,51 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -910,15 +1161,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -937,83 +1188,95 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1021,52 +1284,97 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1075,15 +1383,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1100,91 +1408,95 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1193,50 +1505,49 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
                           indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1253,31 +1564,79 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1296,20 +1655,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1318,15 +1706,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1338,15 +1726,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1358,32 +1746,36 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1394,30 +1786,30 @@
             "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert cfg.versionfile_source is not None, \
         "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
@@ -1470,109 +1862,152 @@
         print("unable to compute version")
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py: Any = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext: Any = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self) -> None:
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1588,20 +2023,20 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1614,30 +2049,67 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info: Any = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist: Any = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -1682,29 +2154,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
 
-def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+
+def do_setup() -> int:
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1716,70 +2193,45 @@
                         "TAG_PREFIX": cfg.tag_prefix,
                         "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                         "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -1808,14 +2260,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

