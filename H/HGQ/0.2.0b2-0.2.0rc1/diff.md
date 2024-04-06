# Comparing `tmp/HGQ-0.2.0b2.tar.gz` & `tmp/HGQ-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HGQ-0.2.0b2.tar", last modified: Mon Nov 27 22:22:54 2023, max compression
+gzip compressed data, was "HGQ-0.2.0rc1.tar", last modified: Sat Dec  2 02:51:55 2023, max compression
```

## Comparing `HGQ-0.2.0b2.tar` & `HGQ-0.2.0rc1.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.963009 HGQ-0.2.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.951009 HGQ-0.2.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.955009 HGQ-0.2.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/.github/workflows/sphinx-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15562 2023-11-27 22:22:54.963009 HGQ-0.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.955009 HGQ-0.2.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.955009 HGQ-0.2.0b2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8903 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14525 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/_static/logo-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20384 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/qkeras.md
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/status.md
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/docs/tips.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.955009 HGQ-0.2.0b2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    44996 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/examples/mnist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/examples/qkeras.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 22:22:54.963009 HGQ-0.2.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.951009 HGQ-0.2.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.955009 HGQ-0.2.0b2/src/HGQ/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-11-27 22:22:54.000000 HGQ-0.2.0b2/src/HGQ/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.959009 HGQ-0.2.0b2/src/HGQ/bops/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/bops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/bops/bops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.959009 HGQ-0.2.0b2/src/HGQ/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/batchnorm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18273 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/layers/passive_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.959009 HGQ-0.2.0b2/src/HGQ/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-27 22:22:40.000000 HGQ-0.2.0b2/src/HGQ/proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/proxy/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/proxy/fixed_point_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.959009 HGQ-0.2.0b2/src/HGQ/proxy/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/proxy/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/proxy/plugins/qkeras.py
--rw-r--r--   0 runner    (1001) docker     (127)    16786 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/proxy/precision_derivation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.959009 HGQ-0.2.0b2/src/HGQ/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/quantizer/quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.959009 HGQ-0.2.0b2/src/HGQ/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/src/HGQ/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.963009 HGQ-0.2.0b2/src/HGQ.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15562 2023-11-27 22:22:54.000000 HGQ-0.2.0b2/src/HGQ.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-11-27 22:22:54.000000 HGQ-0.2.0b2/src/HGQ.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 22:22:54.000000 HGQ-0.2.0b2/src/HGQ.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-27 22:22:54.000000 HGQ-0.2.0b2/src/HGQ.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-27 22:22:54.000000 HGQ-0.2.0b2/src/HGQ.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 22:22:54.963009 HGQ-0.2.0b2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/test_syn_hlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/test_syn_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/test_syn_players.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/test_syn_qkeras.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-11-27 22:22:41.000000 HGQ-0.2.0b2/test/test_syn_small.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.214615 HGQ-0.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.198615 HGQ-0.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.202615 HGQ-0.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.github/workflows/sphinx-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15602 2023-12-02 02:51:55.214615 HGQ-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.202615 HGQ-0.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.202615 HGQ-0.2.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8903 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14525 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/_static/logo-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/qkeras.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/status.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/docs/tips.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    44996 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/examples/mnist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/examples/qkeras.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 02:51:55.214615 HGQ-0.2.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.198615 HGQ-0.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/src/HGQ/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/src/HGQ/bops/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/bops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/bops/bops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.206615 HGQ-0.2.0rc1/src/HGQ/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10374 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/batchnorm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18273 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/layers/passive_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/fixed_point_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/proxy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/plugins/qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16786 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/proxy/precision_derivation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11916 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/quantizer/quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/src/HGQ/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/src/HGQ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15602 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-02 02:51:55.000000 HGQ-0.2.0rc1/src/HGQ.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 02:51:55.210615 HGQ-0.2.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_convert_manual_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_end2end_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_hlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_qkeras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2023-12-02 02:51:45.000000 HGQ-0.2.0rc1/test/test_syn_small.py
```

### Comparing `HGQ-0.2.0b2/.github/workflows/python-publish.yml` & `HGQ-0.2.0rc1/.github/workflows/python-publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
+      with:
+        fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `HGQ-0.2.0b2/.github/workflows/sphinx-build.yml` & `HGQ-0.2.0rc1/.github/workflows/sphinx-build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 
 jobs:
   # Build job
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Pages
         uses: actions/configure-pages@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.11'
       - name: Install dependencies
         run: |
```

### Comparing `HGQ-0.2.0b2/.gitignore` & `HGQ-0.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/.pre-commit-config.yaml` & `HGQ-0.2.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/LICENSE` & `HGQ-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/PKG-INFO` & `HGQ-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HGQ
-Version: 0.2.0b2
+Version: 0.2.0rc1
 Summary: High Granularity Quantizarion
 Author-email: Chang Sun <chsun@cern.ch>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,31 +206,32 @@
            limitations under the License.
         
 Project-URL: repository, https://github.com/calad0i/HGQ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
-Requires-Python: <3.12,>=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tensorflow==2.13
+Requires-Dist: tensorflow~=2.13
 Requires-Dist: numpy>=1.23
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: qkeras; extra == "docs"
 Requires-Dist: pyparsing; extra == "docs"
 Provides-Extra: test
 Requires-Dist: qkeras; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-env; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pyparsing; extra == "test"
 
 <img src="docs/_static/logo.svg" alt="HGQ-logo" width="230"/>
 
 
 # High Granularity Quantization
```

### Comparing `HGQ-0.2.0b2/README.md` & `HGQ-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/Makefile` & `HGQ-0.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/_static/icon.svg` & `HGQ-0.2.0rc1/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/_static/logo-icon.svg` & `HGQ-0.2.0rc1/docs/_static/logo-icon.svg`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/_static/logo.svg` & `HGQ-0.2.0rc1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/conf.py` & `HGQ-0.2.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/faq.md` & `HGQ-0.2.0rc1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/getting_started.md` & `HGQ-0.2.0rc1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/index.rst` & `HGQ-0.2.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/install.md` & `HGQ-0.2.0rc1/docs/install.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # Installation
 
-Use `pip install --pre HGQ` to install the latest version from PyPI. You will need a environment with `python==3.11` installed.
+Use `pip install --pre HGQ` to install the latest version from PyPI. You will need a environment with `python>=3.10` installed. Currently, only `python3.10 and 3.11` are tested.
 
 ```{warning}
 This framework requires an **unmerged** [PR](https://github.com/fastmachinelearning/hls4ml/pull/914) of hls4ml. Please install it by running `pip install "git+https://github.com/calad0i/hls4ml@HGQ-integration"`. Or, conversion will fail with unsupported layer error.
 ```
 
 ```{note}
 The current varsion requires an **unmerged** version of hls4ml. Please install it by running `pip install git+https://github.com/calad0i/hls4ml`.
 ```
 
 ```{warning}
-HGQ v0.2 requires `python3.10/3.11` and `tensorflow==2.13`. Please make sure that you have the correct version of python and tensorflow installed.
+HGQ v0.2 requires `tensorflow==2.13` and `python>=3.10`. Please make sure that you have the correct version of python and tensorflow installed.
 ```
 
-If you want to use the legency v0.1 version, please run `pip install HGQ "tensorflow==2.11" "numpy>=1.23"` to install it from PyPI. You will need a environment with `python==3.10` installed.
-
 ```{warning}
 Due to broken dependency declaration, you will need to specify the version of tensorflow manually. Otherwise, there will likely to be version conflicts.
 ```
```

### Comparing `HGQ-0.2.0b2/docs/qkeras.md` & `HGQ-0.2.0rc1/docs/qkeras.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/reference.md` & `HGQ-0.2.0rc1/docs/reference.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,9 +90,9 @@
 Though the proxy model is bit-accurate with hls4ml in general, exceptions exist:
 
 1. Some intermediate values cannot be represented by the floating point format used by tensorflow, which is usually `float32` (23 bits mantissa) or `TF32` (10 bits mantissa).
 2. For activations, bit-accuracy cannot be guaranteed. A great example of this is `softmax`. Also, unary nonlinear activations may or may not be bit-accurate with the current hls4ml implementation. Currently, if the bitwidth is very high and the input value's range is greater than a certain value, bit-accuracy will be lost due to some hardcoded LUT size in hls4ml.
 ```
 
 ```{tip}
-The proxy model can also be used to convert a `QKeras` model to a bit-accurate hls4ml-ready proxy model. See more details in the [QKeras User?](qkeras.md) section.
+The proxy model can also be used to convert a `QKeras` model to a bit-accurate hls4ml-ready proxy model. See more details in the [Regarding QKeras](qkeras.md) section.
 ```
```

### Comparing `HGQ-0.2.0b2/docs/status.md` & `HGQ-0.2.0rc1/docs/status.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/docs/tips.md` & `HGQ-0.2.0rc1/docs/tips.md`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/examples/mnist.ipynb` & `HGQ-0.2.0rc1/examples/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/examples/qkeras.ipynb` & `HGQ-0.2.0rc1/examples/qkeras.ipynb`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/pyproject.toml` & `HGQ-0.2.0rc1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm>=8"]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HGQ"
-version = "0.2.0b2"
+version = "0.2.0rc1"
 authors = [{ name = "Chang Sun", email = "chsun@cern.ch" }]
 description = "High Granularity Quantizarion"
 readme = "README.md"
-requires-python = ">=3.11,<3.12"
+requires-python = ">=3.10"
 license = { file = "LICENSE" }
 
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
   "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
 ]
 
-dependencies = ['tensorflow==2.13', 'numpy>=1.23']
+dependencies = ['tensorflow~=2.13', 'numpy>=1.23']
 
 [project.urls]
 repository = "https://github.com/calad0i/HGQ"
 
 [tool.setuptools_scm]
 write_to = "src/HGQ/_version.py"
 
@@ -33,9 +33,10 @@
 test = [
   # "git+https://github.com/calad0i/hls4ml@HGQ-integration",
   "qkeras",
   "pytest",
   "pytest-xdist",
   "pytest-env",
   "pytest-cov",
+  "pytest-sugar",
   "pyparsing",
 ]
```

### Comparing `HGQ-0.2.0b2/src/HGQ/__init__.py` & `HGQ-0.2.0rc1/src/HGQ/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 try:
     from ._version import version as __version__
     from ._version import version_tuple
 except ImportError:
     __version__ = "unknown version"
     version_tuple = (0, 0, "unknown version")
 
+from . import _patch
+
 
 class Shutup:
     def write(self, s):
         pass
 
     def flush(self):
         pass
@@ -34,8 +36,8 @@
 
 with shutup:
 
     from .bops import CalibratedBOPs, FreeBOPs, ResetMinMax, trace_minmax
     from .layers import HConv1D, HConv1DBatchNorm, HConv2D, HConv2DBatchNorm, HDense, HDenseBatchNorm, HQuantize, PAvgPool1D, PAvgPool2D, PConcatenate, PFlatten, PMaxPool1D, PMaxPool2D, PReshape, Signature
     from .proxy import to_proxy_model
     from .quantizer import HGQ
-    from .utils import get_default_kq_conf, get_default_paq_config, set_default_kq_conf, set_default_paq_conf
+    from .utils import get_default_kq_conf, get_default_paq_conf, set_default_kq_conf, set_default_paq_conf
```

### Comparing `HGQ-0.2.0b2/src/HGQ/bops/bops.py` & `HGQ-0.2.0rc1/src/HGQ/bops/bops.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,21 +61,30 @@
     if cover_factor != 1.0:
         assert cover_factor > 0.
         if cover_factor < 1:
             warn(f'cover_factor<1.0 will likely to result in overflows.')
         for layer in model.layers:
             if not isinstance(layer, HLayerBase):
                 continue
+
             aq = layer.paq
-            aq._min.assign(aq(aq._min * cover_factor))  # type: ignore
-            aq._max.assign(aq(aq._max * cover_factor))  # type: ignore
+            _min, _max = aq._min.numpy(), aq._max.numpy()  # type: ignore
+            cover_factor_min = np.full_like(_min, cover_factor)
+            cover_factor_min[_min > 0] = 1. / cover_factor
+            cover_factor_max = np.full_like(_max, cover_factor)
+            cover_factor_max[_max < 0] = 1. / cover_factor
+
+            aq._min.assign(aq(aq._min * cover_factor_min))  # type: ignore
+            aq._max.assign(aq(aq._max * cover_factor_max))  # type: ignore
 
     for layer in model.layers:
         if not hasattr(layer, 'activation'):
             continue
+        if not isinstance(layer, HLayerBase):
+            continue
         aq = layer.paq
         if layer.activation is tf.keras.activations.softmax:
             # softmax_lut behaves slightly differently from softmax, which is more likely to generate exact 1s. Overflows may occur with traced min-max.
             aq._min.assign(tf.zeros_like(aq._min))  # type: ignore
             aq._max.assign(tf.ones_like(aq._max))  # type: ignore
 
         if layer.activation is tf.keras.activations.sigmoid:
```

### Comparing `HGQ-0.2.0b2/src/HGQ/layers/base.py` & `HGQ-0.2.0rc1/src/HGQ/layers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Callable
 
 import numpy as np
 import tensorflow as tf
 from keras.activations import linear, relu
 
 from ..quantizer import HGQ
-from ..utils import apf_to_tuple, get_default_kq_conf, get_default_paq_config, tuple_to_apf, warn
+from ..utils import apf_to_tuple, get_default_kq_conf, get_default_paq_conf, tuple_to_apf, warn
 
 
 @staticmethod  # type: ignore
 @tf.function(jit_compile=True)
 def scale_grad(x, scale):
     sx = x * scale
     return sx + tf.stop_gradient(x - sx)
@@ -21,14 +21,15 @@
     def last_layer(self):
         assert len(self._inbound_nodes) == 1, f'input_container is only available for layers used only once. {self.name} is used {len(self._inbound_nodes)} times.'
         assert not isinstance(self._inbound_nodes[0].inbound_layers, list), f'input_container is only available for layers with a single input. {self.name} has {len(self._inbound_nodes[0].inbound_layers)} inputs.'
         return self._inbound_nodes[0].inbound_layers
 
     @property
     def input_bw(self):
+        assert len(self._inbound_nodes) <= 1, f"Layer {self.name} is reused {len(self._inbound_nodes)} times. This is not allowed."
         try:
             return self.last_layer.act_bw
         except AssertionError:
             return None
 
 
 class HLayerBase(ABSBaseLayer):
@@ -36,15 +37,15 @@
     """
 
     def __init__(self, kq_conf=None, paq_conf=None, beta=0., **kwargs):
         self._has_kernel = None
         self._has_bias = None
         self.kq_config = kq_conf or get_default_kq_conf()
         "kernel quantizer config"
-        self.paq_config = paq_conf or get_default_paq_config()
+        self.paq_config = paq_conf or get_default_paq_conf()
         "pre-activation quantizer config"
         self.beta = tf.constant(beta, dtype=tf.float32, name='beta')
         "BOPs-regularization strength"
         self.record_minmax = False
         self._has_last_layer = False
         self._do_adapt_kernel_bits = kwargs.pop('do_adapt_kernel_bits', True)
         self._delayed_kernel_bits_adaption = False
@@ -214,15 +215,15 @@
             raise ValueError('channel_loc must be -1 or 1')
 
         fbw = tf.reduce_max(self.paq.fbw, axis=dims, keepdims=False)
         fbw = tf.broadcast_to(fbw, bias.shape)
         mask = tf.reduce_max(self.act_bw, axis=dims, keepdims=False) > 0
 
         if self.paq.rnd_strategy != 3 and self.can_bias_cover_rnd:
-            bias = tf.pow(2., -tf.floor(fbw + 0.5) - 1) + bias  # type: ignore
+            bias = tf.pow(2., -tf.round(fbw) - 1) + bias  # type: ignore
 
         return tf.where(mask, bias, 0.)
 
     def reset_minmax(self):
         """Resets the recorded minmax values for the pre-activation quantizer."""
         self.paq.minmax_reg_reset()  # type: ignore
```

### Comparing `HGQ-0.2.0b2/src/HGQ/layers/conv.py` & `HGQ-0.2.0rc1/src/HGQ/layers/conv.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/src/HGQ/layers/dense.py` & `HGQ-0.2.0rc1/src/HGQ/layers/dense.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/src/HGQ/layers/misc.py` & `HGQ-0.2.0rc1/src/HGQ/layers/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,37 +46,28 @@
             self.forward: Callable = tf.function(jit_compile=True)(self.__forward)  # type: ignore
 
         else:
             self.forward: Callable = self.__forward
 
         super().post_build(input_shape)
 
-    # @tf.function(jit_compile=True)
     def __forward(self, x, training=None, record_minmax=None):
         x = self.activation(x)  # type: ignore
         return self.paq(x, training=training, record_minmax=record_minmax)  # type: ignore
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
-    @property
-    def table_container(self) -> str:
-        if self.activation is not tf.keras.activations.softmax:
-            return self.result_container
-        return 'ap_fixed<18,8,AP_RND>'  # No bit-match for softmax anyway, just maxout it for now.
-
 
 @register_keras_serializable(package="HGQ")
 class HAdd(HLayerBase, _Merge):
 
     @tf.function(jit_compile=True)
     def forward(self, inputs, training=None, record_minmax=None):
-        output = inputs[0]
-        for i in range(1, len(inputs)):
-            output += inputs[i]
+        output = tf.reduce_sum(inputs, axis=0)
         return self.paq(output, training=training, record_minmax=record_minmax)  # type: ignore
 
     def compute_output_shape(self, input_shape):
         return input_shape[0]
 
 
 # class HMultply(HLayerBase, _Merge):
```

### Comparing `HGQ-0.2.0b2/src/HGQ/layers/passive_layers.py` & `HGQ-0.2.0rc1/src/HGQ/layers/passive_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,27 @@
     @property
     def act_bw(self):
         """Returns the bitwidth of the pre-activation values. Differentiable."""
         shape = (1,) + self.output_shape[1:]
         input_bw = tf.reshape(self.input_bw, shape)
         return tf.ensure_shape(input_bw, shape)
 
-    @property
-    def act_container(self) -> str:
-        return self.last_layer.act_container
-
-    @property
-    def result_container(self) -> str:
-        return self.act_container
-
 
 @register_keras_serializable(package="HGQ")
 class Signature(PLayerBase):
 
     def __init__(self, keep_negative, bits, int_bits, **kwargs):
         super().__init__(**kwargs)
+        if not hasattr(keep_negative, 'shape'):
+            keep_negative = tf.constant(keep_negative, dtype=tf.int8)
+        if not hasattr(bits, 'shape'):
+            bits = tf.constant(bits, dtype=tf.int8)
+        if not hasattr(int_bits, 'shape'):
+            int_bits = tf.constant(int_bits, dtype=tf.int8)
+
         self.bits = bits
         self.int_bits = int_bits
         self.keep_negative = keep_negative
 
     def build(self, input_shape):
         self.built = True
         self.bits = tf.broadcast_to(self.bits, (1,) + input_shape[1:])
@@ -53,29 +52,21 @@
 
     @property
     @tf.function(jit_compile=True)
     def act_bw(self):
         return tf.keras.backend.cast_to_floatx(self.bits)
 
     @property
-    def act_container(self) -> str:
-        k = self.keep_negative.numpy().max().astype(bool).item()  # type: ignore
-        i = self.int_bits.numpy().max().astype(int).item()  # type: ignore
-        b = self.bits.numpy().max().astype(int).item()  # type: ignore
-        f = b - i - k
-        return tuple_to_apf((k, i, f))
-
-    @property
     def input_bw(self):
         raise ValueError('Signature layer does not have input_bw')
 
     def get_config(self):
         return {
             'name': self.name,
-            'cat': self.keep_negative.numpy().tolist(),  # type: ignore
+            'keep_negative': self.keep_negative.numpy().tolist(),  # type: ignore
             'bits': self.bits.numpy().tolist(),  # type: ignore
             'int_bits': self.int_bits.numpy().tolist(),  # type: ignore
         }
 
 
 @register_keras_serializable(package="HGQ")
 class PReshape(tf.keras.layers.Reshape, PLayerBase):
@@ -95,29 +86,19 @@
     def act_bw(self):
         """Returns the bitwidth of the pre-activation values. Differentiable."""
         shape = (1,) + self.output_shape[1:]
         return tf.concat(self.input_bw, axis=self.axis)
 
     @property
     def input_bw(self):
-        if len(self._inbound_nodes) <= 1:
-            raise ValueError("Concatenate layer should have at least two inputs")
+        assert len(self._inbound_nodes) <= 1, f"Layer {self.name} is reused {len(self._inbound_nodes)} times. This is not allowed."
+        assert len(self._inbound_nodes[0].inbound_layers) > 1, "Concatenate layer should have at least two inputs"
         input_bws = [l.act_bw for l in self._inbound_nodes[0].inbound_layers]
         return tf.concat(input_bws, axis=self.axis)
 
-    @property
-    def act_container(self) -> str:
-        if not self._inbound_nodes:
-            raise ValueError(f"Layer {self.name} does not have inbound nodes")
-
-        input_containers = np.array([apf_to_tuple(l.act_container) for l in self._inbound_nodes[0].inbound_layers])
-
-        container = tuple_to_apf(tuple(np.max(input_containers, axis=0)))
-        return container
-
 
 @register_keras_serializable(package="HGQ")
 class PPool2D(PLayerBase, Pooling2D):
 
     def build(self, input_shape):
         super().build(input_shape)
         self._tf_data_format = conv_utils.convert_data_format(self.data_format, 4)
```

### Comparing `HGQ-0.2.0b2/src/HGQ/proxy/convert.py` & `HGQ-0.2.0rc1/src/HGQ/proxy/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     dependencies_list: list[tuple[keras.layers.Layer, list[Node], Node]] = []
     "List of (layer, requires, provides) tuples; requires is a list of nodes, provides is a single node."
 
     for node in nodes:
         if node.is_input:
             continue
         layer = node.layer
+        if layer not in model.layers:
+            continue
         requires = list(node.parent_nodes)
         provides = node
         dependencies_list.append((layer, requires, provides))
     return input_nodes, output_nodes, dependencies_list
 
 
 def get_weight(layer: keras.layers.Layer, name: str):
@@ -57,26 +59,24 @@
         if name in w.name:
             return w
     return None
 
 
 def copy_fused_weights(src: keras.layers.Layer, dst: keras.layers.Layer):
     """For HGQ layers, some layers may have different fused weights for kernel and bias (Processed weights are deployment). This function copies the fused kernel and bias to the keras proxy."""
-    if hasattr(dst, 'kernel'):
+    if hasattr(dst, 'kernel') and dst.kernel is not None:
         if (k := getattr(src, 'fused_qkernel', None)) is not None:
             dst.kernel.assign(k)
         else:
             dst.kernel.assign(src.kernel)
-    if hasattr(dst, 'bias'):
+    if hasattr(dst, 'bias') and dst.bias is not None:
         if (b := getattr(src, 'fused_qbias', None)) is not None:
             dst.bias.assign(b)
-        elif (b := getattr(src, 'bias', None)) is not None:
-            dst.bias.assign(b)
         else:
-            warn(f'No bias found for layer {src.name}.')
+            dst.bias.assign(src.bias)
     for dst_w in dst.weights:
         if 'kernel:0' in dst_w.name or 'bias:0' in dst_w.name:
             continue
         src_w = get_weight(src, dst_w.name)
         if src_w is not None:
             dst_w.assign(src_w)
         else:
@@ -208,15 +208,15 @@
 
 @to_proxy_layers.register
 def _(layer: ABSBaseLayer, name: str, SAT: str):
     proxy_quantizer_layers = ()
     layers = []
     proxy_layers = list(extract_keras_layers(layer, name))
 
-    if hasattr(layer, 'paq'):
+    if hasattr(layer, 'paq') or isinstance(layer, Signature):
         proxy_quantizer_layers = list(extract_quantizers(layer, name, SAT))
     if len(proxy_layers) > len(proxy_quantizer_layers) and isinstance(layer, HLayerBase):
         warn(f'Layer {layer.name} does not have a quantizer attached!')
 
     while proxy_layers or proxy_quantizer_layers:
         if proxy_layers:
             layers.append(proxy_layers.pop(0))
```

### Comparing `HGQ-0.2.0b2/src/HGQ/proxy/fixed_point_quantizer.py` & `HGQ-0.2.0rc1/src/HGQ/proxy/fixed_point_quantizer.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/src/HGQ/proxy/plugins/qkeras.py` & `HGQ-0.2.0rc1/src/HGQ/proxy/plugins/qkeras.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/src/HGQ/proxy/precision_derivation.py` & `HGQ-0.2.0rc1/src/HGQ/proxy/precision_derivation.py`

 * *Files identical despite different names*

### Comparing `HGQ-0.2.0b2/src/HGQ/quantizer/quantizer.py` & `HGQ-0.2.0rc1/src/HGQ/quantizer/quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from collections.abc import Callable
 from functools import singledispatchmethod
 
 import numpy as np
 import tensorflow as tf
 
-from ..utils import L1, L1L2, L2, strategy_dict
+from ..utils import strategy_dict
 
 two = tf.constant(2, dtype=tf.float32)
 log2 = tf.constant(np.log(2), dtype=tf.float32)
 
 
 @tf.function(jit_compile=True)
 def q_round(x: tf.Tensor, strategy: int = 0):
@@ -50,15 +51,15 @@
     int_bits = high_pos - low_pos - fb
     return kn.astype(np.int8), int_bits.astype(np.int8), fb.astype(np.int8)
 
 
 class HGQ:
     """Heterogenous quantizer."""
 
-    def __init__(self, init_bw: float, skip_dims, rnd_strategy: str | int = 'floor', exact_q_value=True, dtype=None, bw_clip=(-23, 23), trainable=True, regularizer=None, minmax_record=False):
+    def __init__(self, init_bw: float, skip_dims, rnd_strategy: str | int = 'floor', exact_q_value=True, dtype=None, bw_clip=(-23, 23), trainable=True, regularizer: Callable | None = None, minmax_record=False):
         self.init_bw = init_bw
         self.skip_dims = skip_dims
         """tuple: Dimensions to use uniform quantizer. If None, use full heterogenous quantizer."""
         self.rnd_strategy = strategy_dict.get(rnd_strategy, -1) if isinstance(rnd_strategy, str) else rnd_strategy
         """How to round the quantized value. 0: standard round (default, round to nearest, round-up 0.5), 1: stochastic round, 2: fast uniform noise injection (uniform noise in [-0.5, 0.5]), 3: floor"""
         self.exact_q_value = exact_q_value
         """bool: Whether to use exact quantized value during training."""
@@ -146,15 +147,19 @@
             record_minmax: if set to True, min and max of quantized values will be recorded for deriving the necessary integer bits. Only necessary for activation/pre-activation values.
         """
         if self.exact_q_value or not training:
             scale = tf.pow(two, tf.round(self.fbw))
         else:
             scale = tf.pow(two, self.fbw)
 
-        xq = q_round(x * scale, self.rnd_strategy) / scale  # type: ignore
+        rnd_strategy = self.rnd_strategy
+        if not training and rnd_strategy != 3:  # not std round or floor
+            rnd_strategy = 0
+        xq = q_round(x * scale, rnd_strategy) / scale  # type: ignore
+
         delta = tf.stop_gradient(xq - x)
         if training:
             prod = delta * self.fbw * log2  # type: ignore
             delta = tf.stop_gradient(delta + prod) - prod
 
         if not record_minmax:
             return x + delta
@@ -183,15 +188,19 @@
         fbw = tf.reduce_max(self.fbw, axis=dims, keepdims=False)
 
         if self.exact_q_value or not training:
             scale = tf.pow(two, tf.round(fbw))
         else:
             scale = tf.pow(two, fbw)
 
-        xq = q_round(x * scale, self.rnd_strategy) / scale  # type: ignore
+        rnd_strategy = self.rnd_strategy
+        if not training and rnd_strategy != 3:  # not std round or floor
+            rnd_strategy = 0
+        xq = q_round(x * scale, rnd_strategy) / scale  # type: ignore
+
         delta = tf.stop_gradient(xq - x)
 
         if training:
             prod = delta * fbw * log2  # type: ignore
             delta = tf.stop_gradient(delta + prod) - prod
 
         return x + delta
```

### Comparing `HGQ-0.2.0b2/src/HGQ.egg-info/PKG-INFO` & `HGQ-0.2.0rc1/src/HGQ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HGQ
-Version: 0.2.0b2
+Version: 0.2.0rc1
 Summary: High Granularity Quantizarion
 Author-email: Chang Sun <chsun@cern.ch>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,31 +206,32 @@
            limitations under the License.
         
 Project-URL: repository, https://github.com/calad0i/HGQ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
-Requires-Python: <3.12,>=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tensorflow==2.13
+Requires-Dist: tensorflow~=2.13
 Requires-Dist: numpy>=1.23
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: qkeras; extra == "docs"
 Requires-Dist: pyparsing; extra == "docs"
 Provides-Extra: test
 Requires-Dist: qkeras; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-env; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pyparsing; extra == "test"
 
 <img src="docs/_static/logo.svg" alt="HGQ-logo" width="230"/>
 
 
 # High Granularity Quantization
```

### Comparing `HGQ-0.2.0b2/src/HGQ.egg-info/SOURCES.txt` & `HGQ-0.2.0rc1/src/HGQ.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 docs/tips.md
 docs/_static/icon.svg
 docs/_static/logo-icon.svg
 docs/_static/logo.svg
 examples/mnist.ipynb
 examples/qkeras.ipynb
 src/HGQ/__init__.py
+src/HGQ/_patch.py
 src/HGQ/_version.py
 src/HGQ.egg-info/PKG-INFO
 src/HGQ.egg-info/SOURCES.txt
 src/HGQ.egg-info/dependency_links.txt
 src/HGQ.egg-info/requires.txt
 src/HGQ.egg-info/top_level.txt
 src/HGQ/bops/__init__.py
@@ -44,12 +45,14 @@
 src/HGQ/proxy/plugins/qkeras.py
 src/HGQ/quantizer/__init__.py
 src/HGQ/quantizer/quantizer.py
 src/HGQ/utils/__init__.py
 src/HGQ/utils/utils.py
 test/helpers.py
 test/pytest.ini
+test/test_convert_manual_proxy.py
+test/test_end2end_tiny.py
 test/test_syn_hlayers.py
 test/test_syn_large.py
 test/test_syn_players.py
 test/test_syn_qkeras.py
 test/test_syn_small.py
```

### Comparing `HGQ-0.2.0b2/test/helpers.py` & `HGQ-0.2.0rc1/test/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import shutil
 from warnings import warn
 
 import numpy as np
 import pytest
 import tensorflow as tf
 
+tf.config.experimental_run_functions_eagerly(True)  # noqa
 tf.config.threading.set_inter_op_parallelism_threads(1)  # noqa
 tf.config.threading.set_intra_op_parallelism_threads(1)  # noqa
 
 from hls4ml.converters import convert_from_keras_model
 from tensorflow import keras
 
 from HGQ import trace_minmax
@@ -29,15 +30,15 @@
     if not test_root:
         test_root = '/tmp/unit_test'
     test_dir = os.path.join(test_root, cur_test)
     os.makedirs(test_dir, exist_ok=True)
     return test_dir
 
 
-def _run_synth_match_test(proxy: keras.Model, data, io_type: str, backend: str, dir: str):
+def _run_synth_match_test(proxy: keras.Model, data, io_type: str, backend: str, dir: str, cond=None):
 
     output_dir = dir + '/hls4ml_prj'
     hls_model = convert_from_keras_model(
         proxy,
         io_type=io_type,
         output_dir=output_dir,
         backend=backend,
@@ -53,17 +54,20 @@
         r_hls = [x.reshape(r_proxy[i].shape) for i, x in enumerate(r_hls)]
     else:
         r_proxy: list[np.ndarray] = [proxy(data).numpy()]  # type: ignore
         r_hls: list[np.ndarray] = [hls_model.predict(data).reshape(r_proxy[0].shape)]  # type: ignore
 
     errors = []
     for i, (p, h) in enumerate(zip(r_proxy, r_hls)):
-        mismatch_ph = p != h
         try:
-            assert np.sum(mismatch_ph) == 0, f"Proxy-HLS4ML mismatch for out {i}: {np.sum(np.any(mismatch_ph,axis=1))} out of {data_len} samples are different. Sample: {p[mismatch_ph].ravel()[:5]} vs {h[mismatch_ph].ravel()[:5]}"
+            if cond is None:
+                mismatch_ph = p != h
+                assert np.sum(mismatch_ph) == 0, f"Proxy-HLS4ML mismatch for out {i}: {np.sum(np.any(mismatch_ph,axis=1))} out of {data_len} samples are different. Sample: {p[mismatch_ph].ravel()[:5]} vs {h[mismatch_ph].ravel()[:5]}"
+            else:
+                cond(p, h)
         except AssertionError as e:
             errors.append(e)
     if len(errors) > 0:
         msgs = [str(e) for e in errors]
         raise AssertionError('\n'.join(msgs))
 
 
@@ -104,24 +108,41 @@
         if not len(errors) == 0:
             raise AssertionError('\n'.join([str(e) for e in errors]))
     else:
         if len(errors) == 0:
             warn(f"Keras-Proxy perfect match when overflow should happen: cover_factor={cover_factor}.")
 
 
-def run_model_test(model: keras.Model, cover_factor: float | None, data, io_type: str, backend: str, dir: str, aggressive: bool, no_exact_match: bool = False, skip_sl_test=False):
+def _run_gradient_test(model, data):
+    with tf.GradientTape() as tape:
+        out = model(data, training=True)
+        if isinstance(out, list):
+            loss = tf.reduce_mean([tf.reduce_sum(tf.abs(x)) for x in out])
+        else:
+            loss = tf.reduce_sum(tf.abs(out))
+
+    trainable_weights = model.trainable_weights
+    grad = tape.gradient(loss, trainable_weights)
+
+    for w, g in zip(trainable_weights, grad):
+        assert tf.reduce_any(g != 0), f"Gradient for {w.name} is zero"
+
+
+def run_model_test(model: keras.Model, cover_factor: float | None, data, io_type: str, backend: str, dir: str, aggressive: bool, cond=None, skip_sl_test=False, test_gard=False):
     data_len = data.shape[0] if isinstance(data, np.ndarray) else data[0].shape[0]
+    if test_gard:
+        _run_gradient_test(model, data)
     if cover_factor is not None:
         trace_minmax(model, data, cover_factor=cover_factor, bsz=data_len)
     proxy = to_proxy_model(model, aggressive=aggressive)
     try:
         if not skip_sl_test:
             _run_model_sl_test(model, proxy, data, dir)
         _run_model_proxy_match_test(model, proxy, data, cover_factor)
-        _run_synth_match_test(proxy, data, io_type, backend, dir)
+        _run_synth_match_test(proxy, data, io_type, backend, dir, cond=cond)
     except AssertionError as e:
         raise e
     except Warning as w:
         warn(w)
     else:
         shutil.rmtree(dir)
```

### Comparing `HGQ-0.2.0b2/test/pytest.ini` & `HGQ-0.2.0rc1/test/pytest.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [pytest]
 filterwarnings =
     ignore:WARNING\W Pytorch converter is not enabled!:UserWarning
     ignore:.\[93mcover_factor<1.0 will likely to result in overflows:UserWarning
     ignore:You are saving your model as an HDF5 file:UserWarning
+    ignore:Even though the `tf.config.experimental_run_functions_eagerly`:UserWarning
     ignore:pkg_resources is deprecated as an API:DeprecationWarning
     ignore:distutils Version classes are deprecated:DeprecationWarning
     ignore:module 'sre_constants' is deprecated:DeprecationWarning
     ignore:Deprecated call to `pkg_resources.declare_namespace\('[a-z]+'\)`:DeprecationWarning
 
 env =
     TF_CPP_MIN_LOG_LEVEL=3
```

### Comparing `HGQ-0.2.0b2/test/test_syn_hlayers.py` & `HGQ-0.2.0rc1/test/test_syn_large.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,81 @@
+import os
+import random
+
 import numpy as np
 import pytest
 import tensorflow as tf
 from helpers import get_test_dir, run_model_test, set_seed
 from tensorflow import keras
 
-import HGQ
-from HGQ import get_default_paq_config, set_default_paq_conf
-from HGQ.layers import HQuantize, PReshape
+from HGQ import get_default_paq_conf, set_default_paq_conf
+from HGQ.layers import HActivation, HAdd, HConv1D, HConv2D, HDense, HQuantize, PConcatenate, PDropout, PFlatten, PMaxPool1D, PMaxPool2D, PReshape
 
 
-def create_model(layer: str, rnd_strategy: str, io_type: str):
-    pa_config = get_default_paq_config()
-    pa_config['rnd_strategy'] = rnd_strategy
+def create_model(rnd_strategy: str, io_type: str):
+
+    pa_config = get_default_paq_conf()
     pa_config['skip_dims'] = 'all' if io_type == 'io_stream' else 'batch'
+    pa_config['rnd_strategy'] = rnd_strategy
     set_default_paq_conf(pa_config)
 
-    inp = keras.Input(shape=(16))
-    if 'Add' in layer:
-        _inp = [HQuantize()(inp)] * 2
-    elif 'Conv2D' in layer:
-        _inp = PReshape((4, 4, 1))(HQuantize()(inp))
-    elif 'Conv1D' in layer:
-        _inp = PReshape((16, 1))(HQuantize()(inp))
-    elif 'Dense' in layer or 'Activation' in layer:
-        _inp = HQuantize()(inp)
-    else:
-        raise Exception(f'Please add test for {layer}')
-    out = eval('HGQ.layers.' + layer)(_inp)
-    model = keras.Model(inp, out)
+    inp = keras.Input(shape=(10, 10))
+    qinp = HQuantize()(inp)
+    x = PReshape((10, 10, 1))(qinp)  # 10x10
+    x = HConv2D(5, (3, 3), activation='relu', padding='valid', parallel_factor=64)(x)  # 5x8x8
+    x = PMaxPool2D((1, 2))(x)  # 5x8x4
+    x = HActivation('relu')(x)
+    mp = PMaxPool2D((4, 4))(x)  # 5x2x1
+    x = PReshape((10,))(mp)  # 5
+    x = HDense(10)(x)
+    y = PReshape((20, 5))(qinp)  # 20x5
+    y = HConv1D(5, 5, strides=5, padding='valid', parallel_factor=4)(y)  # 4x5
+    po = PMaxPool1D(2)(y)  # 2x5
+    ay = HActivation('relu')(po)
+    y = PFlatten()(ay)  # 5
+    y = PDropout(0.5)(y)
+    y = HDense(10)(y)
+    z = PFlatten()(qinp)  # 5
+    x = HAdd()([x, y])  # 5
+    xy = PConcatenate()([x, y])  # 5
+    z = HDense(10, activation='relu')(z)  # 5
+    z = HDense(10, activation=None)(z)  # 5
+    out = PConcatenate()([xy, z])  # 5
+    out = HActivation('relu')(out)
+    horrible_model = keras.Model(inp, out)
 
-    for layer in model.layers:
+    for layer in horrible_model.layers:
         # Randomize weight bitwidths
         if hasattr(layer, 'kq'):
             fbw: tf.Variable = layer.kq.fbw
             fbw.assign(tf.constant(np.random.uniform(2, 8, fbw.shape).astype(np.float32)))
         # And activation bitwidths
         if hasattr(layer, 'paq'):
             fbw: tf.Variable = layer.paq.fbw
-            fbw.assign(tf.constant(np.random.uniform(2, 8, fbw.shape).astype(np.float32)))
-
-    return model
+            fbw.assign(tf.constant(np.random.uniform(2, 6, fbw.shape).astype(np.float32)))
+        if hasattr(layer, 'bias') and layer.bias is not None:
+            bias: tf.Variable = layer.bias
+            bias.assign(tf.constant(np.random.uniform(-4, 4, layer.bias.shape).astype(np.float32)))
+    return horrible_model
 
 
 def get_data(N: int, sigma: float, max_scale: float, seed):
     rng = np.random.default_rng(seed)
-    a1 = rng.normal(0, sigma, (N, 16)).astype(np.float32)
-    a2 = rng.uniform(0, max_scale, (1, 16)).astype(np.float32)
+    a1 = rng.normal(0, sigma, (N, 10, 10, 1)).astype(np.float32)
+    a2 = rng.uniform(0, max_scale, (1, 10, 10, 1)).astype(np.float32)
     return (a1 * a2).astype(np.float32)
 
 
-@pytest.mark.parametrize('layer',
-                         ["HDense(10)",
-                          "HDenseBatchNorm(10)",
-                          "HConv1D(2, 3, padding='same')",
-                          "HConv1D(2, 3, padding='valid')",
-                          "HConv1D(2, 3, padding='valid', strides=2)",
-                          "HConv1D(2, 3, padding='same', strides=2)",
-                          "HConv1DBatchNorm(2, 3, padding='valid')",
-                          "HConv2D(2, (3,3), padding='same')",
-                          "HConv2D(2, (3,3), padding='valid')",
-                          "HConv2D(2, (3,3), padding='valid', strides=2)",
-                          "HConv2D(2, (3,3), padding='same', strides=2)",
-                          "HConv2DBatchNorm(2, (3,3), padding='valid')",
-                          "HAdd()",
-                          "HActivation('relu')",
-                          #   "HActivation('leaky_relu')",
-                          "HActivation('relu6')",
-                          "HActivation('tanh')",
-                          "HActivation('sigmoid')",
-                          #   "HActivation('softmax')",
-                          ]
-                         )
-@pytest.mark.parametrize("N", [1000, 10])
-@pytest.mark.parametrize("rnd_strategy", ['auto', 'standard_round', 'floor'])
+@pytest.mark.parametrize("N", [50000, 10])
+@pytest.mark.parametrize("rnd_strategy", ['auto'])
 @pytest.mark.parametrize("io_type", ['io_parallel', 'io_stream'])
-@pytest.mark.parametrize("cover_factor", [0.5, 1.0])
+@pytest.mark.parametrize("cover_factor", [0.49, 1.0])
 @pytest.mark.parametrize("aggressive", [True, False])
-@pytest.mark.parametrize("backend", ['vivado'])
+@pytest.mark.parametrize("backend", ['vivado'])  # , 'vitis'])
 @pytest.mark.parametrize("seed", [42])
-def test_syn_hlayers(layer, N: int, rnd_strategy: str, io_type: str, cover_factor: float, aggressive: bool, backend: str, seed: int):
+def test_syn_large(N: int, rnd_strategy: str, io_type: str, cover_factor: float, aggressive: bool, backend: str, seed: int):
     dir = get_test_dir()
     set_seed(seed)
-    model = create_model(layer=layer, rnd_strategy=rnd_strategy, io_type=io_type)
-    data = get_data(N, 1, 1, seed)
+    model = create_model(rnd_strategy=rnd_strategy, io_type=io_type)
+    data = get_data(N, 8, 1, seed)
 
     run_model_test(model, cover_factor, data, io_type, backend, dir, aggressive)
-
-
-if __name__ == '__main__':
-    test_syn_hlayers('HActivation("tanh")', 10, 'floor', 'io_parallel', 0.5, True, 'vivado', 42)
```

### Comparing `HGQ-0.2.0b2/test/test_syn_qkeras.py` & `HGQ-0.2.0rc1/test/test_syn_qkeras.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
     L = l(10)
 
     inp = keras.layers.Input((10,))
     q_inp = qkeras.QActivation(qkeras.quantized_bits(8, 4, alpha=1.))(inp)
     out = L(q_inp)
     out1 = L(out)
+    out1 = r(out1)
+    out1 = L(out1)
     out2 = l(20)(out1)
     out2 = r(out2)
     out3 = l(20)(out2)
     out2 = keras.layers.Reshape((2, 5, 2))(out2)
     out2 = c(2)(out2)
     out2 = rr(out2)
     out2 = keras.layers.Flatten()(out2)
```

### Comparing `HGQ-0.2.0b2/test/test_syn_small.py` & `HGQ-0.2.0rc1/test/test_syn_small.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 import numpy as np
 import pytest
 import tensorflow as tf
 from helpers import get_test_dir, run_model_test, set_seed
 from tensorflow import keras
 
-from HGQ import get_default_paq_config, set_default_paq_conf
+from HGQ import get_default_paq_conf, set_default_paq_conf
 from HGQ.layers import HActivation, HAdd, HConv1D, HConv2D, HDense, HQuantize, PConcatenate, PDropout, PFlatten, PMaxPool1D, PMaxPool2D, PReshape
 
 
 def create_model(rnd_strategy: str, io_type: str):
 
-    pa_config = get_default_paq_config()
+    pa_config = get_default_paq_conf()
     pa_config['skip_dims'] = 'all' if io_type == 'io_stream' else 'batch'
     pa_config['rnd_strategy'] = rnd_strategy
     set_default_paq_conf(pa_config)
 
     model = keras.Sequential([
         HQuantize(input_shape=(6, 6, 1), name='inp_q'),
         HConv2D(4, 2, activation='relu'),
@@ -35,14 +35,17 @@
         if hasattr(layer, 'kq'):
             fbw: tf.Variable = layer.kq.fbw
             fbw.assign(tf.constant(np.random.uniform(2, 8, fbw.shape).astype(np.float32)))
         # And activation bitwidths
         if hasattr(layer, 'paq'):
             fbw: tf.Variable = layer.paq.fbw
             fbw.assign(tf.constant(np.random.uniform(2, 6, fbw.shape).astype(np.float32)))
+        if hasattr(layer, 'bias') and layer.bias is not None:
+            bias: tf.Variable = layer.bias
+            bias.assign(tf.constant(np.random.uniform(-4, 4, layer.bias.shape).astype(np.float32)))
     return model
 
 
 def get_data(N: int, sigma: float, max_scale: float, seed):
     rng = np.random.default_rng(seed)
     a1 = rng.normal(0, sigma, (N, 6, 6, 1)).astype(np.float32)
     a2 = rng.uniform(0, max_scale, (1, 6, 6, 1)).astype(np.float32)
```

