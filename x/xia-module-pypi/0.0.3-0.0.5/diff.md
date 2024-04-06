# Comparing `tmp/xia-module-pypi-0.0.3.tar.gz` & `tmp/xia-module-pypi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-pypi-0.0.3.tar", last modified: Mon Apr  1 14:21:32 2024, max compression
+gzip compressed data, was "xia-module-pypi-0.0.5.tar", last modified: Sat Apr  6 15:47:58 2024, max compression
```

## Comparing `xia-module-pypi-0.0.3.tar` & `xia-module-pypi-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/base/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.400582 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/template/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 14:21:23.000000 xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/template/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:32.396582 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 14:21:32.000000 xia-module-pypi-0.0.3/xia_module_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.166815 xia-module-pypi-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-06 15:47:57.000000 xia-module-pypi-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 15:47:58.166815 xia-module-pypi-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:47:58.166815 xia-module-pypi-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/template/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.158815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/init/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/init/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/init/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/init/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/init/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 15:47:48.000000 xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/template/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:47:58.162815 xia-module-pypi-0.0.5/xia_module_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-06 15:47:58.000000 xia-module-pypi-0.0.5/xia_module_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-06 15:47:58.000000 xia-module-pypi-0.0.5/xia_module_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:47:58.000000 xia-module-pypi-0.0.5/xia_module_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:47:58.000000 xia-module-pypi-0.0.5/xia_module_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 15:47:58.000000 xia-module-pypi-0.0.5/xia_module_pypi.egg-info/top_level.txt
```

### Comparing `xia-module-pypi-0.0.3/LICENSE` & `xia-module-pypi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/setup.py` & `xia-module-pypi-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/pypi.py` & `xia-module-pypi-0.0.5/xia_module_pypi/pypi.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/activate/main.tf`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-name: 'GCP Authentication'
-description: 'Deploy to Google Cloud Platform'
+name: 'Publish to Google Artifact Registry'
+description: 'Deploy Pypi package to Google Artifact Registry'
 inputs:
   project_id:
     description: 'GCP Project ID'
     required: true
 
 runs:
   using: 'composite'
   steps:
       - name: Install Python
         uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
       - name: Install dependencies
+        shell: bash
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel twine
 
       - name: Build Python package
+        shell: bash
         run: |
           python setup.py sdist bdist_wheel
           CHECK_VERSION=$(ls dist/*-${GITHUB_REF#refs/tags/}*.tar.gz)
 
       - name: Connecting Artifact Registry for twine
+        shell: bash
         run: |
           pip install keyring
           pip install keyrings.google-artifactregistry-auth
 
       - name: Upload package to Google Artifact Registry
+        shell: bash
         env:
-          TWINE_REPOSITORY_URL: https://europe-west1-python.pkg.dev/${{ vars.project_id }}/pypi-custom
+          TWINE_REPOSITORY_URL: https://europe-west1-python.pkg.dev/${{ inputs.project_id }}/pypi-custom
         run: twine upload --non-interactive dist/*
```

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/.gitignore` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/.gitignore`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/LICENSE` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi/templates/module-pypi/init/setup.py` & `xia-module-pypi-0.0.5/xia_module_pypi/templates/gcp-module-pypi/init/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-pypi-0.0.3/xia_module_pypi.egg-info/SOURCES.txt` & `xia-module-pypi-0.0.5/xia_module_pypi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,22 @@
 xia_module_pypi.egg-info/top_level.txt
 xia_module_pypi/templates/gcp-module-pypi/activate/main.tf
 xia_module_pypi/templates/gcp-module-pypi/activate/variables.tf
 xia_module_pypi/templates/gcp-module-pypi/base/activate.tf
 xia_module_pypi/templates/gcp-module-pypi/base/main.tf
 xia_module_pypi/templates/gcp-module-pypi/cicd/github/workflow.yml
 xia_module_pypi/templates/gcp-module-pypi/cicd/github/actions/publish-pypi-gcp/action.yml
+xia_module_pypi/templates/gcp-module-pypi/init/.gitignore
+xia_module_pypi/templates/gcp-module-pypi/init/LICENSE
+xia_module_pypi/templates/gcp-module-pypi/init/README.rst
+xia_module_pypi/templates/gcp-module-pypi/init/requirements.txt
+xia_module_pypi/templates/gcp-module-pypi/init/setup.py
 xia_module_pypi/templates/gcp-module-pypi/module/main.tf
 xia_module_pypi/templates/gcp-module-pypi/module/variables.tf
+xia_module_pypi/templates/gcp-module-pypi/template/__init__.py.jinja
 xia_module_pypi/templates/module-pypi/cicd/github/workflow.yml
 xia_module_pypi/templates/module-pypi/cicd/github/actions/publish-pypi/action.yml
 xia_module_pypi/templates/module-pypi/init/.gitignore
 xia_module_pypi/templates/module-pypi/init/LICENSE
 xia_module_pypi/templates/module-pypi/init/README.rst
 xia_module_pypi/templates/module-pypi/init/requirements.txt
 xia_module_pypi/templates/module-pypi/init/setup.py
```

