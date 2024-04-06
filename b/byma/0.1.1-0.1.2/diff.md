# Comparing `tmp/byma-0.1.1.tar.gz` & `tmp/byma-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.1.1.tar", last modified: Thu Apr  4 10:06:01 2024, max compression
+gzip compressed data, was "byma-0.1.2.tar", last modified: Sat Apr  6 16:28:33 2024, max compression
```

## Comparing `byma-0.1.1.tar` & `byma-0.1.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.504755 byma-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-04 10:05:48.000000 byma-0.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-04 10:05:48.000000 byma-0.1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-04 10:05:48.000000 byma-0.1.1/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-04 10:05:48.000000 byma-0.1.1/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-04 10:05:48.000000 byma-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-04 10:06:01.504755 byma-0.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-04 10:05:48.000000 byma-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.493755 byma-0.1.1/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-04 10:05:48.000000 byma-0.1.1/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-04 10:06:01.000000 byma-0.1.1/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.494755 byma-0.1.1/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-04 10:05:48.000000 byma-0.1.1/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-04 10:05:48.000000 byma-0.1.1/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-04 10:05:48.000000 byma-0.1.1/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.494755 byma-0.1.1/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.495755 byma-0.1.1/byma/iteral/nonstationary/
--rw-rw-rw-   0 root         (0) root         (0)     5162 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/nonstationary/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/nonstationary/NonStationary.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/nonstationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.496755 byma-0.1.1/byma/iteral/stationary/
--rw-rw-rw-   0 root         (0) root         (0)     4730 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/stationary/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/stationary/Stationary.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-04 10:05:48.000000 byma-0.1.1/byma/iteral/stationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.496755 byma-0.1.1/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-04 10:05:48.000000 byma-0.1.1/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     7611 2024-04-04 10:05:48.000000 byma-0.1.1/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-04 10:05:48.000000 byma-0.1.1/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-04 10:05:48.000000 byma-0.1.1/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.497755 byma-0.1.1/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-04 10:05:48.000000 byma-0.1.1/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-04 10:05:48.000000 byma-0.1.1/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.503755 byma-0.1.1/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3433 2024-04-04 10:06:01.000000 byma-0.1.1/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1973 2024-04-04 10:06:01.000000 byma-0.1.1/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 10:06:01.000000 byma-0.1.1/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-04 10:06:01.000000 byma-0.1.1/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.497755 byma-0.1.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-04 10:05:48.000000 byma-0.1.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-04 10:05:48.000000 byma-0.1.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-04 10:05:48.000000 byma-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.498755 byma-0.1.1/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.498755 byma-0.1.1/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.498755 byma-0.1.1/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.498755 byma-0.1.1/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.499755 byma-0.1.1/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.499755 byma-0.1.1/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.499755 byma-0.1.1/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3372 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.499755 byma-0.1.1/docs/source/autoapi/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.499755 byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.500755 byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.500755 byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.500755 byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.500755 byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.500755 byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/Stationary/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.501755 byma-0.1.1/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.501755 byma-0.1.1/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.501755 byma-0.1.1/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     4393 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.501755 byma-0.1.1/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4626 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4898 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.502755 byma-0.1.1/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     2752 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.502755 byma-0.1.1/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     2697 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.503755 byma-0.1.1/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-04 10:05:48.000000 byma-0.1.1/docs/source/user/whatisbyma.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.503755 byma-0.1.1/examples/
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-04 10:05:48.000000 byma-0.1.1/examples/example.py
--rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-04 10:05:48.000000 byma-0.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-04 10:05:48.000000 byma-0.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 10:06:01.504755 byma-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-04 10:05:48.000000 byma-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 10:06:01.503755 byma-0.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 10:05:48.000000 byma-0.1.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.872532 byma-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-06 16:28:21.000000 byma-0.1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-06 16:28:21.000000 byma-0.1.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-04-06 16:28:21.000000 byma-0.1.2/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-06 16:28:21.000000 byma-0.1.2/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-06 16:28:21.000000 byma-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-06 16:28:33.872532 byma-0.1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-06 16:28:21.000000 byma-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.861532 byma-0.1.2/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-06 16:28:21.000000 byma-0.1.2/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-06 16:28:33.000000 byma-0.1.2/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.862532 byma-0.1.2/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-06 16:28:21.000000 byma-0.1.2/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-06 16:28:21.000000 byma-0.1.2/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-06 16:28:21.000000 byma-0.1.2/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.862532 byma-0.1.2/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.863532 byma-0.1.2/byma/iteral/nonstationary/
+-rw-rw-rw-   0 root         (0) root         (0)     5168 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/nonstationary/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/nonstationary/NonStationary.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/nonstationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.864532 byma-0.1.2/byma/iteral/stationary/
+-rw-rw-rw-   0 root         (0) root         (0)     4730 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/stationary/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/stationary/Stationary.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-06 16:28:21.000000 byma-0.1.2/byma/iteral/stationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.864532 byma-0.1.2/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7972 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-06 16:28:21.000000 byma-0.1.2/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.865532 byma-0.1.2/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-06 16:28:21.000000 byma-0.1.2/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-06 16:28:21.000000 byma-0.1.2/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3433 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1973 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 16:28:33.000000 byma-0.1.2/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.865532 byma-0.1.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-06 16:28:21.000000 byma-0.1.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-06 16:28:21.000000 byma-0.1.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-06 16:28:21.000000 byma-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.866532 byma-0.1.2/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.866532 byma-0.1.2/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.866532 byma-0.1.2/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3372 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.867532 byma-0.1.2/docs/source/autoapi/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.868532 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/Stationary/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     4393 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.869532 byma-0.1.2/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4626 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4898 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.870532 byma-0.1.2/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     2752 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.870532 byma-0.1.2/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-06 16:28:21.000000 byma-0.1.2/docs/source/user/whatisbyma.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-06 16:28:21.000000 byma-0.1.2/examples/example.py
+-rwxrwxrwx   0 root         (0) root         (0)     1005 2024-04-06 16:28:21.000000 byma-0.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-06 16:28:21.000000 byma-0.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 16:28:33.872532 byma-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-06 16:28:21.000000 byma-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 16:28:33.871532 byma-0.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-06 16:28:21.000000 byma-0.1.2/tests/__init__.py
```

### Comparing `byma-0.1.1/.gitlab-ci.yml` & `byma-0.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/LICENSE.md` & `byma-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/PKG-INFO` & `byma-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.1/README.md` & `byma-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/byma/__init__.py` & `byma-0.1.2/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/byma/interface/BaseInterface.py` & `byma-0.1.2/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/byma/interface/NonlinearHeat.py` & `byma-0.1.2/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/byma/iteral/nonstationary/Newton.py` & `byma-0.1.2/byma/iteral/nonstationary/Newton.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,33 +121,32 @@
     normdx = []
     normf = []
     for iter in range(maxit):
         f_value = f(x)
         df_value = df(x)
         
         if sp.issparse(df_value) and sp.issparse(df_value):
-            dx = sp.linalg.spsolve(df_value, -f_value)
+            dx = -sp.linalg.spsolve(df_value, f_value)
             dxnorm = sp.linalg.norm(dx)
         else:
-            dx = np.linalg.solve(df_value, -f_value)
+            dx = -np.linalg.solve(df_value, f_value)
             dxnorm = np.linalg.norm(dx)
         
-        x += dx
+        x += dx.reshape((len(dx),))
         
         if sp.issparse(df_value) and sp.issparse(df_value):
             fnorm = sp.linalg.norm(f(x))
         else:
             fnorm = np.linalg.norm(f(x))
             
         normdx.append(dxnorm)
         normf.append(fnorm)
         
-        if  verbose != 0 and verbose != False:
-            if (iter % verbose == 0):
-                print(f"Newton status at iteration {iter + 1}: ||dx|| = {dxnorm} and ||F|| = {fnorm}")
+        if  (verbose != 0 and verbose != False) and (iter % verbose == 0):
+            print(f"Newton status at iteration {iter + 1}: ||dx|| = {dxnorm} and ||F|| = {fnorm}")
         
         if (fnorm < tol and stop == 'residual-check'):
             if verbose:
                 print(f'Newton converged in {iter + 1} iterations with ||F|| = {fnorm}')
             return _returns(x, fnorm=fnorm, dxnorm=normdx, mode=mode, method=stop)
         
         if (dxnorm < tol and stop == 'normal'):
```

### Comparing `byma-0.1.1/byma/iteral/stationary/OrthogonalSubspace.py` & `byma-0.1.2/byma/iteral/stationary/OrthogonalSubspace.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/byma/nuby/Continuation.py` & `byma-0.1.2/byma/nuby/Continuation.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,20 +47,22 @@
             return branch, dxnorms
         elif mode == 'partial':
             return branch
         else:
             return x
 
 
-def step(x, df, dfmu, dx, dmu, **kwargs):
+def step(x, f, df, dfmu, dx, dmu, **kwargs):
         """
     Perform one step of the continuation.
 
     :param x: array_like
         Current state.
+    :param f: callable
+        Function to evaluate the Jacobian matrix with respect to state variable x.
     :param df: callable
         Function to evaluate the Jacobian matrix with respect to state variable x.
     :param dfmu: callable
         Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
     :param dx: array_like
         Current tangent with respect to state variable.
     :param dmu: float or array_like
@@ -77,40 +79,42 @@
         
         # Predictor
         x += dmu * dx
         kwargs['mode'] = 'partial'
         kwargs['stop'] = 'normal'
   
         # Corrector 
-        x, dxnorm = newton(x = x, f = dfmu, df = df, **kwargs)
+        x, dxnorm = newton(x = x, f = f, df = df, **kwargs)
 
         # Compute the tangent
-        dfx1 = df(x)
-        dfmu1 = dfmu(x)
+        dfx1 = df(x = x)
+        dfmu1 = dfmu(x = x)
         if sp.issparse(dfx1) and sp.issparse(dfmu1):
             dx = sp.linalg.spsolve(dfx1, -dfmu1)
             
         else:
             dx = np.linalg.solve(dfx1, -dfmu1)
-            
+        
         return x, dxnorm, dx
 
 @bs.set_defaults(default_cls = Bf, default_opts=_DEFAULT_OPTS)
-def cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs):
+def cont(x0, dx0, start, f, df, dfmu, dmu=None, target=None, **kwargs):
     """
     Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
     This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
     :param x0: array_like
         Initial state.
     :param dx0: array_like
         Initial tangent with respect to state variable.
     :param start: float
         Starting parameter value.
+    :param f: callable
+        Function to evaluate the Jacobian matrix with respect to state variable x.
     :param df: callable
         Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
     :param dfmu: callable
         Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
     :param dmu: float or array_like, optional
         Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
     :param target: float or None, optional
@@ -156,54 +160,58 @@
     """
     _opts = bs.opts(**kwargs)
     mode_con = _opts['mode']
     method = _opts['method']
     maxit_con = _opts['maxit_cont']
     verbose = _opts['verbose']
     
-    x = x0
-    dx = dx0
-    mu = start
+    dx = dx0.copy()
+    mu = start.copy()
 
     # Set some parameters
     if (target is None) and (dmu is None):
         raise ValueError("Either 'dmu' or 'target' should be not 'None'")
     
     else:
         mus = np.linspace(mu, target, maxit_con)
+        dmu = mus[1] - mu
+        
         
     # Perform the continuation
     branch = []
     dxnorms = []
     
     if verbose:
         print('------ Continuation Method summary ------')
         print(f'starting solution: {x0}')
         print(f'starting parameter: {start}')
         print(f'maximum iter: {maxit_con}')
         print(f'method: {method}')
+        if isinstance(dmu, float):
+            print(f'Constand dmu: {dmu}')
     
         print('------ Start iteration ------')
 
     for j in range(maxit_con):
         
         if target is None:
             mu0 = mu0 + dmu if isinstance(dmu, float) else mu0 + dmu[j]
         else:
-            mu0 = mus[j]
-            dmu = mu - mu0 if mu != start else mu0 - mus[j]
+            mu0 = mus[j].copy()
 
+        f1 = lambda x: f(x = x, mu = mu0)
         df1 = lambda x: df(x = x, mu = mu0)
         dfmu1 = lambda x: dfmu(x = x, mu = mu0)
         
         if method == 'normal':
-            x, dxnorm, dx = step(x, df=df1, dfmu=dfmu1, dx=dx, dmu=dmu, **kwargs)
+            x0, dxnorm, dx = step(x = x0, f=f1, df=df1, dfmu=dfmu1, dx=dx, dmu=dmu, **kwargs)
         elif method == 'pseudo-arclength':
             raise ValueError("Pseudo-arclength'conitnuation is not yet avialible")
         else:
             raise ValueError("Invalid continuation method. Choose either 'normal' or 'pseudo-arclength'.")
 
-        branch.append(x)
+        branch.append(x0.copy())
         dxnorms.append(dxnorm)
 
     mode = mode_con
+    x = x0.copy()
     return _returns(x, branch, target, mode, dxnorms, mu0)
```

### Comparing `byma-0.1.1/byma/pyplot/plots.py` & `byma-0.1.2/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/byma.egg-info/PKG-INFO` & `byma-0.1.2/byma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Project-URL: documentation, https://bytemath.gitlab.io/python/ByMa/index.html
 Project-URL: source, https://gitlab.com/ByteMath/python/ByMa
 Project-URL: download, https://pypi.org/project/byma/#files
```

### Comparing `byma-0.1.1/byma.egg-info/SOURCES.txt` & `byma-0.1.2/byma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/Makefile` & `byma-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/make.bat` & `byma-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/interface/BaseInterface/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/interface/BaseInterface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/interface/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/interface/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/nuby/Continuation/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/nuby/_nuby/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/nuby/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.2/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/conf.py` & `byma-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/docs/source/index.rst` & `byma-0.1.2/docs/source/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    contain the root `toctree` directive.
 
 ByMa's documentation
 ================================
 
 
 .. toctree::
-   :maxdepth: 4
+   :maxdepth: 5
    :hidden:
 
    User Guide <user/index>
    API reference <reference/index>
    Building from source <building/index>
    release
```

### Comparing `byma-0.1.1/examples/example.py` & `byma-0.1.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/pyproject.toml` & `byma-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.1.1/setup.py` & `byma-0.1.2/setup.py`

 * *Files identical despite different names*

