# Comparing `tmp/lephare-0.1.1.tar.gz` & `tmp/lephare-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.1.tar", last modified: Wed Apr  3 20:42:19 2024, max compression
+gzip compressed data, was "lephare-0.1.2.tar", last modified: Sat Apr  6 06:55:39 2024, max compression
```

## Comparing `lephare-0.1.1.tar` & `lephare-0.1.2.tar`

### file list

```diff
@@ -1,135 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.576478 lephare-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 20:42:09.000000 lephare-0.1.1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-03 20:42:09.000000 lephare-0.1.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 20:42:09.000000 lephare-0.1.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-03 20:42:09.000000 lephare-0.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.560478 lephare-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.560478 lephare-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.560478 lephare-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/workflows/compile-cpp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 20:42:09.000000 lephare-0.1.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-03 20:42:09.000000 lephare-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 20:42:09.000000 lephare-0.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-03 20:42:09.000000 lephare-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-03 20:42:09.000000 lephare-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-03 20:42:09.000000 lephare-0.1.1/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-03 20:42:09.000000 lephare-0.1.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 20:42:09.000000 lephare-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-03 20:42:19.576478 lephare-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-03 20:42:09.000000 lephare-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.560478 lephare-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.560478 lephare-0.1.1/docs/doxygen/
--rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/doxygen/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.564478 lephare-0.1.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/Building_list_of_onesources.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/Data_retrieval.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/Example_of_usage_of_magSvc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   173732 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/example_full_run.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 20:42:09.000000 lephare-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.564478 lephare-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-03 20:42:09.000000 lephare-0.1.1/examples/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-03 20:42:09.000000 lephare-0.1.1/examples/figuresLPP.py
--rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-04-03 20:42:09.000000 lephare-0.1.1/examples/figuresLPZ.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-03 20:42:09.000000 lephare-0.1.1/examples/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-03 20:42:09.000000 lephare-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:42:19.576478 lephare-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-03 20:42:09.000000 lephare-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.556478 lephare-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.564478 lephare-0.1.1/src/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/_flt.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/_photoz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/filterSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/magSvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/mag_gal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/sedtolib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lephare/zphota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.576478 lephare-0.1.1/src/lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 20:42:19.000000 lephare-0.1.1/src/lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.572478 lephare-0.1.1/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/PDF.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/PDF.h
--rw-r--r--   0 runner    (1001) docker     (127)    72114 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/SED.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/SED.h
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/SEDLib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/SEDLib.h
--rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/_bindings.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/cosmology.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/cosmology.h
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/ext.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/ext_curv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/filter_extinc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/flt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/flt.h
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/globals.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/globals.h
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/keyword.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/keyword.h
--rw-r--r--   0 runner    (1001) docker     (127)    31597 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/mag.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/mag.h
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/mag_gal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/oneElLambda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/oneElLambda.h
--rw-r--r--   0 runner    (1001) docker     (127)    80040 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/onesource.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/onesource.h
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/opa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/opa.h
--rw-r--r--   0 runner    (1001) docker     (127)    61007 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/photoz_lib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/photoz_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/sedtolib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-03 20:42:09.000000 lephare-0.1.1/src/lib/zphota.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.572478 lephare-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.572478 lephare-0.1.1/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/calzetti.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.572478 lephare-0.1.1/tests/data/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/examples/COSMOS.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.556478 lephare-0.1.1/tests/data/filt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.572478 lephare-0.1.1/tests/data/filt/subaru/
--rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/filt/subaru/IB527.pb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.576478 lephare-0.1.1/tests/data/sed/
--rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/sed/WDgd71.sed.ext
--rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/sed/o5v.sed.ext
--rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/tau10.out
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/test_data_registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/data/test_file_names.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:42:19.576478 lephare-0.1.1/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_cosmology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_dataRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_oneElLambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_onesource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-03 20:42:09.000000 lephare-0.1.1/tests/lephare/test_sed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.749007 lephare-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-06 06:55:31.000000 lephare-0.1.2/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-06 06:55:31.000000 lephare-0.1.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-06 06:55:31.000000 lephare-0.1.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-06 06:55:31.000000 lephare-0.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/compile-cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-06 06:55:31.000000 lephare-0.1.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-06 06:55:31.000000 lephare-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-06 06:55:31.000000 lephare-0.1.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-06 06:55:31.000000 lephare-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-06 06:55:31.000000 lephare-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-06 06:55:31.000000 lephare-0.1.2/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 06:55:31.000000 lephare-0.1.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-06 06:55:31.000000 lephare-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-06 06:55:39.749007 lephare-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-06 06:55:31.000000 lephare-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/docs/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)   112662 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/doxygen/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/keywords.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/legacy_install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.733007 lephare-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Building_list_of_onesources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Data_retrieval.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_SED_manipulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_cosmo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16531 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_full_run.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Example_of_usage_of_magSvc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.737007 lephare-0.1.2/docs/notebooks/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/data/COSMOS.para
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks/data/output.para
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-06 06:55:31.000000 lephare-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.737007 lephare-0.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11097 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39348 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/figuresLPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31984 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/figuresLPZ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-06 06:55:31.000000 lephare-0.1.2/examples/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-06 06:55:31.000000 lephare-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:55:39.749007 lephare-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-06 06:55:31.000000 lephare-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.737007 lephare-0.1.2/src/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_flt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_photoz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/filterSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/magSvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/mag_gal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/sedtolib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lephare/zphota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/src/lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 06:55:39.000000 lephare-0.1.2/src/lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3003 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/PDF.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/PDF.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72114 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SED.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SED.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SEDLib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/SEDLib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/_bindings.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/cosmology.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/cosmology.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/ext.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/ext_curv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/filter_extinc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/flt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/flt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/globals.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/globals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/keyword.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/keyword.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31597 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/mag.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/mag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/mag_gal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/oneElLambda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/oneElLambda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80040 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/onesource.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/onesource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/opa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/opa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61007 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/photoz_lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/photoz_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/sedtolib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-06 06:55:31.000000 lephare-0.1.2/src/lib/zphota.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41606 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/calzetti.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/examples/COSMOS.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.729007 lephare-0.1.2/tests/data/filt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/filt/subaru/
+-rw-r--r--   0 runner    (1001) docker     (127)    25919 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/filt/subaru/IB527.pb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/data/sed/
+-rw-r--r--   0 runner    (1001) docker     (127)    54522 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/sed/WDgd71.sed.ext
+-rw-r--r--   0 runner    (1001) docker     (127)    81892 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/sed/o5v.sed.ext
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22781 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/tau10.out
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/test_data_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/data/test_file_names.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:55:39.745007 lephare-0.1.2/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_dataRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_oneElLambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_onesource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-06 06:55:31.000000 lephare-0.1.2/tests/lephare/test_sed.py
```

### Comparing `lephare-0.1.1/.copier-answers.yml` & `lephare-0.1.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.gitattributes` & `lephare-0.1.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `lephare-0.1.2/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `lephare-0.1.2/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/pull_request_template.md` & `lephare-0.1.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/workflows/compile-cpp.yml` & `lephare-0.1.2/.github/workflows/compile-cpp.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/workflows/pre-commit-ci.yml` & `lephare-0.1.2/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/workflows/publish-to-pypi.yml` & `lephare-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/workflows/smoke-test.yml` & `lephare-0.1.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.github/workflows/testing-and-coverage.yml` & `lephare-0.1.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.gitignore` & `lephare-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/.pre-commit-config.yaml` & `lephare-0.1.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
   - repo: https://github.com/pre-commit/mirrors-clang-format
     rev: v18.1.1
     hooks:
     - id: clang-format
       name: clang-format
       types_or: [c++, c]
     # Clear output from jupyter notebooks so that only the input cells are committed.
-  # - repo: local
-  #   hooks:
-  #     - id: jupyter-nb-clear-output
-  #       name: Clear output from Jupyter notebooks
-  #       description: Clear output from Jupyter notebooks.
-  #       files: \.ipynb$
-  #       stages: [commit]
-  #       language: system
-  #       entry: jupyter nbconvert --clear-output
+  - repo: local
+    hooks:
+      - id: jupyter-nb-clear-output
+        name: Clear output from Jupyter notebooks
+        description: Clear output from Jupyter notebooks.
+        files: \.ipynb$
+        stages: [commit]
+        language: system
+        entry: jupyter nbconvert --clear-output
     # Prevents committing directly branches named 'main' and 'master'.
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: no-commit-to-branch
         name: Prevent main branch commits
         description: Prevent the user from committing directly to the primary branch.
```

### Comparing `lephare-0.1.1/.setup_dev.sh` & `lephare-0.1.2/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/CMakeLists.txt` & `lephare-0.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/LICENSE` & `lephare-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/PKG-INFO` & `lephare-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.1
+Version: 0.1.2
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Johann Cohen-Tanugi <johann.cohentanugi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
@@ -58,24 +58,33 @@
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/lephare/)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/lephare/smoke-test.yml)](https://github.com/lephare-photoz/lephare/actions/workflows/smoke-test.yml)
 [![Codecov](https://codecov.io/gh/lephare-photoz/lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/lephare-photoz/lephare)
 [![Read The Docs](https://img.shields.io/readthedocs/lephare)](https://lephare.readthedocs.io/)
 
-This project is in an early development stage. If you wish to use and run LePHARE please download it from the [official repository](https://gitlab.lam.fr/Galaxies/LEPHARE/).
+IMPORTANT! This project is in an early development stage. If you wish to use and run LePHARE please download it from the [official repository](https://gitlab.lam.fr/Galaxies/LEPHARE/).
 
-This project was automatically generated using the LINCC-Frameworks 
-[python-project-template](https://github.com/lincc-frameworks/python-project-template).
+LePHARE (PHotometric Analysis for Redshift Estimation) is a Python package built on a complete rewrite in C++ of the [Fortran code](https://www.cfht.hawaii.edu/~arnouts/LEPHARE/acknowledgement.html) LePhare.
+LePHARE computes photometric redshifts and physical parameters by fitting spectral energy distributions (SED) to a dataset of photometric fluxes or apparent magnitudes.
 
-A repository badge was added to show that this project uses the python-project-template, however it's up to
-you whether or not you'd like to display it!
+## Installation
 
-For more information about the project template see the 
-[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
+The simplest way to install lephare is using pip:
+
+```
+pip install lephare
+```
+
+
+If you prefer to use binary executables from the command line you may wish to conduct a [legacy installation](https://gitlab.lam.fr/Galaxies/LEPHARE/).  
+
+## Example usage
+
+We provide a number of [Jupyter notebooks](docs/notebooks/) demonstrating various aspects of the Python code.
 
 ## Dev Guide - Getting Started
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
@@ -100,7 +109,17 @@
    that a set of tests will be run prior to completing a local commit. For more
    information, see the Python Project Template documentation on 
    [pre-commit](https://lincc-ppt.readthedocs.io/en/latest/practices/precommit.html)
 3. Install `pandoc` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    [Sphinx and Python Notebooks](https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks)
+
+## Citation
+
+If using this code in scientific research please cite the following papers:
+
+
+This project was automatically generated using the LINCC-Frameworks 
+[python-project-template](https://github.com/lincc-frameworks/python-project-template).
+For more information about the project template see the 
+[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.1/README.md` & `lephare-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,33 @@
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/lephare/)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/lephare/smoke-test.yml)](https://github.com/lephare-photoz/lephare/actions/workflows/smoke-test.yml)
 [![Codecov](https://codecov.io/gh/lephare-photoz/lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/lephare-photoz/lephare)
 [![Read The Docs](https://img.shields.io/readthedocs/lephare)](https://lephare.readthedocs.io/)
 
-This project is in an early development stage. If you wish to use and run LePHARE please download it from the [official repository](https://gitlab.lam.fr/Galaxies/LEPHARE/).
+IMPORTANT! This project is in an early development stage. If you wish to use and run LePHARE please download it from the [official repository](https://gitlab.lam.fr/Galaxies/LEPHARE/).
 
-This project was automatically generated using the LINCC-Frameworks 
-[python-project-template](https://github.com/lincc-frameworks/python-project-template).
+LePHARE (PHotometric Analysis for Redshift Estimation) is a Python package built on a complete rewrite in C++ of the [Fortran code](https://www.cfht.hawaii.edu/~arnouts/LEPHARE/acknowledgement.html) LePhare.
+LePHARE computes photometric redshifts and physical parameters by fitting spectral energy distributions (SED) to a dataset of photometric fluxes or apparent magnitudes.
 
-A repository badge was added to show that this project uses the python-project-template, however it's up to
-you whether or not you'd like to display it!
+## Installation
 
-For more information about the project template see the 
-[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
+The simplest way to install lephare is using pip:
+
+```
+pip install lephare
+```
+
+
+If you prefer to use binary executables from the command line you may wish to conduct a [legacy installation](https://gitlab.lam.fr/Galaxies/LEPHARE/).  
+
+## Example usage
+
+We provide a number of [Jupyter notebooks](docs/notebooks/) demonstrating various aspects of the Python code.
 
 ## Dev Guide - Getting Started
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
@@ -45,7 +54,17 @@
    that a set of tests will be run prior to completing a local commit. For more
    information, see the Python Project Template documentation on 
    [pre-commit](https://lincc-ppt.readthedocs.io/en/latest/practices/precommit.html)
 3. Install `pandoc` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    [Sphinx and Python Notebooks](https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks)
+
+## Citation
+
+If using this code in scientific research please cite the following papers:
+
+
+This project was automatically generated using the LINCC-Frameworks 
+[python-project-template](https://github.com/lincc-frameworks/python-project-template).
+For more information about the project template see the 
+[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.1/docs/Makefile` & `lephare-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/docs/conf.py` & `lephare-0.1.2/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 autoapi_member_order = "bysource"
 
 html_theme = "sphinx_rtd_theme"
 
 breathe_projects = {"lephare": "./doxygen_output/xml"}
 breathe_default_project = "lephare"
 
+nbsphinx_kernel_name = "python3"
+
 # Setup the exhale extension
 exhale_args = {
     # These arguments are required
     "containmentFolder": "./doxygen_output/c_lib",
     "rootFileName": "library_root.rst",
     "doxygenStripFromPath": "..",
     "rootFileTitle": "C Library API",
```

### Comparing `lephare-0.1.1/docs/doxygen/Doxyfile` & `lephare-0.1.2/docs/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/docs/index.rst` & `lephare-0.1.2/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,28 @@
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to lephare's documentation!
 ========================================================================================
 **WARNING: This is a work in progress, and should ne be used by anyone at this stage. The current LePHARE code is to be found at https://gitlab.lam.fr/Galaxies/LEPHARE .**
 
+LePHARE (PHotometric Analysis for Redshift Estimation) is a Python package built on a complete rewrite in C++ of the `Fortran code <https://www.cfht.hawaii.edu/~arnouts/LEPHARE/acknowledgement.html>`_ LePhare.
+LePHARE computes photometric redshifts and physical parameters by fitting spectral energy distributions (SED) to a dataset of photometric fluxes or apparent magnitudes.
+
+Installation
+------------
+
+The simplest way to install lephare for most users is with pip:
+
+.. code-block:: console
+
+   >> pip install lephare
+
+If you prefer to use binary executables from the command line you may wish to conduct a `legacy installation <https://gitlab.lam.fr/Galaxies/LEPHARE/>`_.  
+
 Dev Guide - Getting Started
 ---------------------------
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
@@ -43,10 +57,13 @@
    `Sphinx and Python Notebooks <https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks>`_.
 
 
 .. toctree::
    :hidden:
 
    Home page <self>
+   Notebooks <notebooks>
+   Legacy installation <legacy_install>
+   Keywords <keywords>
    C API Reference <doxygen_output/c_lib/library_root>
    Python API Reference <autoapi/index>
-   Notebooks <notebooks>
+
```

### Comparing `lephare-0.1.1/docs/notebooks/Data_retrieval.ipynb` & `lephare-0.1.2/docs/notebooks/Data_retrieval.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9412202380952381%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [5, 4, 3, 2, 1]}}, insert: [(0, OrderedDict([('cell_type', "*

 * *            "'markdown'), ('id', '694d217b-ec1a-42b7-b8e6-dde10c3490b1'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['# Data retrieval example\\n', '\\n', 'In order to run "*

 * *            'lephare we must download some input data. In this short notebook we a simple example '*

 * *            'which uses pooch to check if the required files have already been downloaded and to '*

 * *            "download them i […]*

```diff
@@ -1,24 +1,29 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "694d217b-ec1a-42b7-b8e6-dde10c3490b1",
+            "metadata": {},
+            "source": [
+                "# Data retrieval example\n",
+                "\n",
+                "In order to run lephare we must download some input data. In this short notebook we a simple example which uses pooch to check if the required files have already been downloaded and to download them if not."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "571cf701-c5d0-44b6-b815-2e7bc038016d",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import os\n",
-                "\n",
-                "if \"LEPHAREDIR\" not in os.environ:\n",
-                "    os.environ[\"LEPHAREDIR\"] = \"/pscratch/sd/o/olynn/lephare-dev/\"\n",
-                "if \"LEPHAREWORK\" not in os.environ:\n",
-                "    os.environ[\"LEPHAREWORK\"] = \"/pscratch/sd/o/olynn/lephare-dev/work/\"\n",
                 "import lephare"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "396751cc-c68e-425f-8277-f7ba566a7f8a",
@@ -60,14 +65,24 @@
                 "\n",
                 "partial_print(file_names, 3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "85ab538b-7693-4358-ac36-5e0a42b6a383",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "file_names[0]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "2769d438-03fc-44a1-882a-9d3554dab7b0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Or, alternatively, you can download files by subdirectory\n",
                 "# Here, we specify our desired subdirectories and get a list of the files they contain\n",
                 "\n",
@@ -125,31 +140,58 @@
                 "\n",
                 "retriever = lephare.data_retrieval.make_retriever(\n",
                 "    base_url=base_url, registry_file=registry_file, data_path=data_path\n",
                 ")\n",
                 "\n",
                 "lephare.data_retrieval.download_all_files(retriever, file_names, ignore_registry=False)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8ba1d5c5-09ea-48b8-b9f0-85019728466c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "base_url = lephare.data_retrieval.DEFAULT_BASE_DATA_URL\n",
+                "registry_file = lephare.data_retrieval.DEFAULT_REGISTRY_FILE\n",
+                "data_path = lephare.LEPHAREDIR\n",
+                "base_url, registry_file, data_path"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "fb792b02-ec35-4dbd-b7b5-b8ea74fdd721",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "retriever = lephare.data_retrieval.make_retriever(\n",
+                "    base_url=base_url, registry_file=registry_file, data_path=data_path\n",
+                ")\n",
+                "\n",
+                "lephare.data_retrieval.download_all_files(retriever, file_names, ignore_registry=False)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python (lph)",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "myenv"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.14"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lephare-0.1.1/docs/notebooks/example_full_run.ipynb` & `lephare-0.1.2/docs/notebooks/Example_full_run.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9828272306397307%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Example full run\\n'), (1, '\\n'), (2, 'An example of "*

 * *            "a complete run of the lephare with all stages required to estimate redshift.\\n'), "*

 * *            "(3, '\\n')]}}, 1: {'id': 'dd9c2bb5-89ee-4061-9b19-0833ba449954', 'source': {insert: "*

 * *            "[(0, 'import os\\n'), (1, 'import lephare as lp\\n')], delete: [0]}}, 2: {'source': "*

 * *            "['## Set up the parameters\\n']}, 4: {'source': ['config_file = "*

 * *            '"./data/COSMOS.para"\\n […]*

```diff
@@ -1,52 +1,42 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "3b7a14b6-cef8-48b3-affc-3c021aaa6191",
             "metadata": {},
             "source": [
+                "# Example full run\n",
+                "\n",
+                "An example of a complete run of the lephare with all stages required to estimate redshift.\n",
+                "\n",
                 "Define the two environment variables necessary for Le Phare (directory of LEPHARE package, directory in which to store the libraries) and define the directory in which you run the code. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8fb267ac-fb4e-46b3-bdbb-ea13bf540a1e",
+            "id": "dd9c2bb5-89ee-4061-9b19-0833ba449954",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
-                "\n",
-                "os.environ[\"LEPHAREDIR\"] = os.path.abspath(\"../..\")\n",
-                "os.environ[\"LEPHAREWORK\"] = \"WORK\"\n",
-                "examples_dir = os.path.join(os.environ[\"LEPHAREDIR\"], \"examples\")\n",
-                "%cd $examples_dir"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "be0f7c0f",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from lephare import *\n",
+                "import lephare as lp\n",
                 "import numpy as np\n",
                 "from matplotlib import pylab as plt\n",
                 "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c319f7fb-fd09-4ea4-899a-211e27f95836",
             "metadata": {},
             "source": [
-                "# Set up the parameters\n"
+                "## Set up the parameters\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "48336218-e813-4d76-88d8-6520fa9e1726",
             "metadata": {},
             "source": [
@@ -56,15 +46,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dd703d19-e493-4440-9675-8980a9c9f57f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "keymap = read_config(\"COSMOS.para\")"
+                "config_file = \"./data/COSMOS.para\"\n",
+                "keymap = lp.read_config(config_file)\n",
+                "# Get the auxiliary files required.\n",
+                "lp.data_retrieval.get_auxiliary_data(\n",
+                "    keymap=keymap, additional_files=[\"examples/COSMOS.in\", \"examples/config.yml\", \"examples/output.para\"]\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a853ff51-6c06-46e5-a257-b3470923c932",
             "metadata": {},
             "source": [
@@ -74,18 +69,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1b12b2bc-9e28-4513-b041-9ad44a6ab16e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "keymap[\"ZPHOTLIB\"] = keyword(\"ZPHOTLIB\", \"VISTA_COSMOS_FREE,ALLSTAR_COSMOS,QSO_COSMOS\")\n",
-                "keymap[\"SPEC_OUT\"] = keyword(\"SPEC_OUT\", \"save_spec\")\n",
-                "keymap[\"VERBOSE\"] = keyword(\"VERBOSE\", \"NO\")\n",
-                "keymap[\"AUTO_ADAPT\"] = keyword(\"AUTO_ADAPT\", \"YES\")"
+                "keymap[\"ZPHOTLIB\"] = lp.keyword(\"ZPHOTLIB\", \"VISTA_COSMOS_FREE,ALLSTAR_COSMOS,QSO_COSMOS\")\n",
+                "keymap[\"SPEC_OUT\"] = lp.keyword(\"SPEC_OUT\", \"save_spec\")\n",
+                "keymap[\"VERBOSE\"] = lp.keyword(\"VERBOSE\", \"NO\")\n",
+                "keymap[\"AUTO_ADAPT\"] = lp.keyword(\"AUTO_ADAPT\", \"YES\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "040ab3a2-962b-4584-8834-1d125fe25119",
             "metadata": {},
             "source": [
@@ -104,15 +99,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "572df1dc-cf80-4e38-a0a1-ab4cdf9d5c7a",
             "metadata": {},
             "source": [
-                "# Create filter library\n",
+                "## Create filter library\n",
                 "\n",
                 "Read the filter names to be used in COSMOS.para and generate the filter file"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f39c7b82-e639-4ce3-a009-1b08c474c6b0",
@@ -124,15 +119,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8b303cd5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "filterLib = Filter(config_file=\"COSMOS.para\")\n",
+                "filterLib = lp.Filter(config_file=config_file)\n",
                 "# uncomment to test passing the keymap\n",
                 "# filterLib = Filter(config_keymap=keymap)\n",
                 "filterLib.run()"
             ]
         },
         {
             "cell_type": "markdown",
@@ -145,37 +140,47 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7f1d836f-69ea-4250-8d32-8e31ce60e5aa",
             "metadata": {},
             "outputs": [],
             "source": [
-                "filterLib = FilterSvc.from_config(\"COSMOS.para\")\n",
+                "filterLib = lp.FilterSvc.from_config(config_file)\n",
                 "filter_output = os.path.join(os.environ[\"LEPHAREWORK\"], \"filt\", keymap[\"FILTER_FILE\"].value)\n",
-                "write_output_filter(filter_output + \".dat\", filter_output + \".doc\", filterLib)"
+                "lp.write_output_filter(filter_output + \".dat\", filter_output + \".doc\", filterLib)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3a91c555-5d96-4d98-933f-6cdd03e96285",
             "metadata": {},
             "source": [
                 "It also allows to load the filters from a yaml file, with the possibility to query the SVO service for filters"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "44e6dd2d-83d1-4ead-aee2-f4554f367829",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "!ls $LEPHAREDIR/examples/"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "da762bb3-9a07-4a83-bbe6-4ad5d98c3bf4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "filterLibSVO = FilterSvc.from_yaml(\"config.yml\")\n",
+                "filterLibSVO = lp.FilterSvc.from_yaml(f\"{lp.LEPHAREDIR}/examples/config.yml\")\n",
                 "filter_output = os.path.join(os.environ[\"LEPHAREWORK\"], \"filt\", keymap[\"FILTER_FILE\"].value)\n",
-                "write_output_filter(filter_output + \"_svo.dat\", filter_output + \"_svo.doc\", filterLib)"
+                "lp.write_output_filter(filter_output + \"_svo.dat\", filter_output + \"_svo.doc\", filterLib)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9fd175f2-53b2-4e4c-b13e-db09bbe731af",
             "metadata": {},
             "source": [
@@ -213,37 +218,37 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "412093d4",
             "metadata": {},
             "source": [
-                "# Create SED library\n",
+                "## Create SED library\n",
                 "\n",
                 "SED objects represent SED templates belonging to one of the three possible classes \"STAR\", \"QSO\" (for AGN type of objects), and \"GAL\" for galaxies. SED templates available with LePhare can be found under the `sed` directory. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "23fbfe55",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sedlib = Sedtolib(config_keymap=keymap)"
+                "sedlib = lp.Sedtolib(config_keymap=keymap)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "13b371c4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sedlib.run(typ=\"STAR\", star_sed=\"../examples/STAR_MOD_ALL.list\")"
+                "sedlib.run(typ=\"STAR\", star_sed=\"$LEPHAREDIR/sed/STAR/STAR_MOD_ALL.list\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "da4e53e2-ab9a-4ae6-9d4e-cac0ed610d3a",
             "metadata": {},
@@ -255,35 +260,35 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "99867870-166c-40c4-9aa6-722eab7574a1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sedlib.run(typ=\"GAL\", gal_sed=\"../examples/COSMOS_MOD.list\", gal_lib=\"LIB_GAL\")"
+                "sedlib.run(typ=\"GAL\", gal_sed=\"$LEPHAREDIR/examples/COSMOS_MOD.list\", gal_lib=\"LIB_GAL\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a1418537-a51d-4d7f-9c5b-19820b88aaef",
             "metadata": {},
             "source": [
-                "# Create a magnitude library\n",
+                "## Create a magnitude library\n",
                 "\n",
                 "Use the SED library to create a magnitude library"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1e440962-0d52-4581-ac69-5be8a3c7b985",
             "metadata": {},
             "outputs": [],
             "source": [
-                "maglib = MagGal(config_keymap=keymap)"
+                "maglib = lp.MagGal(config_keymap=keymap)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f76f6cd4",
             "metadata": {},
@@ -329,16 +334,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b653c140-bffd-408d-bbf7-94401460f766",
             "metadata": {},
             "source": [
-                "# Run the photoz\n",
-                "\n"
+                "## Run the photoz"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dbe1ec31-c1fe-49c7-9340-8c36fc220500",
             "metadata": {},
             "source": [
@@ -348,18 +352,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1f97a44a-6c3f-4ca5-a2b7-c3a9d28d33b0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "keymap = read_config(\"COSMOS.para\")\n",
-                "keymap[\"ZPHOTLIB\"] = keyword(\"ZPHOTLIB\", \"VISTA_COSMOS_FREE,ALLSTAR_COSMOS,QSO_COSMOS\")\n",
-                "keymap[\"SPEC_OUT\"] = keyword(\"SPEC_OUT\", \"save_spec\")\n",
-                "keymap[\"VERBOSE\"] = keyword(\"VERBOSE\", \"NO\")"
+                "keymap = lp.read_config(config_file)\n",
+                "keymap[\"ZPHOTLIB\"] = lp.keyword(\"ZPHOTLIB\", \"VISTA_COSMOS_FREE,ALLSTAR_COSMOS,QSO_COSMOS\")\n",
+                "keymap[\"SPEC_OUT\"] = lp.keyword(\"SPEC_OUT\", \"save_spec\")\n",
+                "keymap[\"VERBOSE\"] = lp.keyword(\"VERBOSE\", \"NO\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "72a67aee-128e-48a4-98ec-d8dff7505480",
             "metadata": {},
             "source": [
@@ -369,15 +373,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "83641591-9527-4378-8e9c-2aec34ce8fcb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "photz = PhotoZ(keymap);"
+                "photz = lp.PhotoZ(keymap)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1434ab52-1e7d-4611-8ab6-ac7d3de2f759",
             "metadata": {},
             "source": [
@@ -387,15 +391,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b20bb607-8c6a-4a5a-b93b-ae1e24a03bf3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cat = np.loadtxt(\"COSMOS.in\")\n",
+                "cat = np.loadtxt(f\"{lp.LEPHAREDIR}/examples/COSMOS.in\")\n",
                 "id = cat[:, 0]\n",
                 "fluxes = cat[:, 1:60:2]\n",
                 "efluxes = cat[:, 2:61:2]\n",
                 "context = cat[:, 61]\n",
                 "zspec = cat[:, 62]\n",
                 "print(\"Check format with context and zspec :\", context, zspec)"
             ]
@@ -414,15 +418,15 @@
             "id": "2c4dad65-4e97-43d1-93f2-cd85a2e12a13",
             "metadata": {},
             "outputs": [],
             "source": [
                 "srclist = []\n",
                 "zspec_mask = np.logical_and(zspec > 0.01, zspec < 6)\n",
                 "for i in np.where(zspec_mask)[0]:\n",
-                "    oneObj = onesource(i, photz.gridz)\n",
+                "    oneObj = lp.onesource(i, photz.gridz)\n",
                 "    oneObj.readsource(str(id[i]), fluxes[i, :], efluxes[i, :], int(context[i]), zspec[i], \" \")\n",
                 "    photz.prep_data(oneObj)\n",
                 "    srclist.append(oneObj)\n",
                 "print(\"Sources with a spec-z: \", len(srclist))"
             ]
         },
         {
@@ -459,15 +463,15 @@
             "execution_count": null,
             "id": "23e36e5d-a503-4bc8-bf64-0e808e72d06d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "photozlist = []\n",
                 "for i in range(100):\n",
-                "    oneObj = onesource(i, photz.gridz)\n",
+                "    oneObj = lp.onesource(i, photz.gridz)\n",
                 "    oneObj.readsource(str(id[i]), fluxes[i, :], efluxes[i, :], int(context[i]), zspec[i], \" \")\n",
                 "    photz.prep_data(oneObj)\n",
                 "    photozlist.append(oneObj)\n",
                 "print(\"Number of sources to be analysed: \", len(srclist))"
             ]
         },
         {
@@ -505,14 +509,24 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "t = photz.build_output_tables(photozlist[:100], para_out=None, filename=\"outputpython.fits\")"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6a47dedd-414c-4bfd-ae20-de3b4021badf",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "t[:5]"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "e8969641-6110-4d8a-88cc-72aebf9e6619",
             "metadata": {},
             "source": [
                 "Create one ascii file per object to produce the best-fit template plot"
             ]
         },
@@ -544,32 +558,16 @@
             "outputs": [],
             "source": [
                 "from os import listdir\n",
                 "from os.path import isfile, join\n",
                 "\n",
                 "listname = [f for f in listdir(\"save_spec\") if isfile(join(\"save_spec\", f))]\n",
                 "for namefile in listname:\n",
-                "    plotspec(\"save_spec/\" + str(namefile))"
+                "    lp.plotspec(\"save_spec/\" + str(namefile))"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "64924ccb-c361-4efb-a3f4-81c015e002e1",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "238df684-ea30-4995-9e19-86ce1eb72801",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -580,13 +578,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lephare-0.1.1/docs/notebooks/examples.ipynb` & `lephare-0.1.2/docs/notebooks/Example_SED_manipulation.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9605017971694851%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import os\\n'), (1, 'import lephare as lp\\n'), (4, "*

 * *            "'import struct\\n')], delete: [0]}}, 2: {'id': "*

 * *            "'4d67ed2e-fe2a-4771-a08d-41adf0fc622c', 'source': ['config_file = "*

 * *            '"./data/COSMOS.para"\\n\', \'keymap = lp.read_config(config_file)\\n\', \'# Get the '*

 * *            "auxiliary files required.\\n', 'lp.data_retrieval.get_auxiliary_data(keymap=keymap, "*

 * *            'additional_files=["sed/STAR/PICKLES/f2ii.sed"])\']}, 3: {\'id […]*

```diff
@@ -1,44 +1,69 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "412093d4",
+            "metadata": {},
+            "source": [
+                "# Manipulating a SED object\n",
+                "\n",
+                "SED objects represent SED templates belonging to one of the three possible classes \"STAR\", \"QSO\" (for AGN type of objects), and \"GAL\" for galaxies. SED templates available with LePhare can be found under the `sed` directory. "
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "be0f7c0f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lephare import *\n",
+                "import os\n",
+                "import lephare as lp\n",
                 "import numpy as np\n",
                 "from matplotlib import pylab as plt\n",
+                "import struct\n",
                 "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "4d67ed2e-fe2a-4771-a08d-41adf0fc622c",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "config_file = \"./data/COSMOS.para\"\n",
+                "keymap = lp.read_config(config_file)\n",
+                "# Get the auxiliary files required.\n",
+                "lp.data_retrieval.get_auxiliary_data(keymap=keymap, additional_files=[\"sed/STAR/PICKLES/f2ii.sed\"])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "ca164e65",
             "metadata": {},
             "outputs": [],
             "source": [
                 "filter_name = \"cosmos/u_cfht.lowres\"\n",
-                "f1 = flt(0, filter_name, 1, 0)\n",
-                "f1.read(os.path.join(LEPHAREDIR, \"filt\", filter_name))\n",
+                "f1 = lp.flt(0, filter_name, 1, 0)\n",
+                "f1.read(os.path.join(lp.LEPHAREDIR, \"filt\", filter_name))\n",
                 "f1.plot_filter_curve()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8b303cd5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "filter_driver = Filter(config=\"../test/COSMOS.para\")\n",
+                "filter_driver = lp.Filter(config_file=config_file)\n",
                 "filter_driver.run()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8a765701",
@@ -50,24 +75,14 @@
                 ")\n",
                 "filters = np.loadtxt(filter_output, dtype={\"names\": (\"lamb\", \"val\", \"bid\"), \"formats\": (float, float, int)})\n",
                 "plt.loglog(filters[\"lamb\"], filters[\"val\"])\n",
                 "plt.xlabel(\"wavelength\");"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "412093d4",
-            "metadata": {},
-            "source": [
-                "# Manipulating a SED object\n",
-                "\n",
-                "SED objects represent SED templates belonging to one of the three possible classes \"STAR\", \"QSO\" (for AGN type of objects), and \"GAL\" for galaxies. SED templates available with LePhare can be found under the `sed` directory. "
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "id": "1a5a6be4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "!ls $LEPHAREDIR/sed"
@@ -85,16 +100,16 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "39331577",
             "metadata": {},
             "outputs": [],
             "source": [
                 "star_sed = \"f2ii.sed\"\n",
-                "sed_filename = os.path.join(LEPHAREDIR, \"sed/STAR/PICKLES/\", star_sed)\n",
-                "sed = StarSED(star_sed, 1, \"STAR\")\n",
+                "sed_filename = os.path.join(lp.LEPHAREDIR, \"sed/STAR/PICKLES/\", star_sed)\n",
+                "sed = lp.StarSED(star_sed, 1)\n",
                 "sed.read(sed_filename)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d481fea2",
             "metadata": {},
@@ -144,32 +159,32 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "588241e2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sed2 = StarSED(star_sed, 2, \"DONTKNOW\")\n",
+                "sed2 = lp.StarSED(star_sed, 2)\n",
                 "sed2.readSEDBin(rootname + \".bin\")\n",
                 "x2 = sed.data()[0]\n",
                 "y2 = sed.data()[1]\n",
                 "assert np.all(x == x2)\n",
                 "assert np.all(y == y2)\n",
-                "print(sed.jtype, sed2.jtype)"
+                "print(sed.name, sed2.name)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "23fbfe55",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sed = Sedtolib(\"../test/COSMOS.para\")\n",
-                "sed.run(typ=\"STAR\", star_sed=\"../test/STAR_MOD_ALL.list\", star_fscale=\"1\")"
+                "sed = lp.Sedtolib(config_file)\n",
+                "sed.run(typ=\"STAR\", star_sed=f\"{lp.LEPHAREDIR}/sed/STAR/STAR_MOD_ALL.list\", star_fscale=\"1\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9282090b",
             "metadata": {},
@@ -193,123 +208,58 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d94d211f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import struct\n",
+                "# Code to unpack binary not running\n",
+                "# buf = open(sed_output, \"rb\").read()\n",
+                "# counter = 0\n",
+                "# off = 0\n",
+                "# while counter <= 0:\n",
+                "#     nrec, jtype, nbw = struct.unpack(\"iil\", buf[off : off + 16])\n",
+                "#     wave = struct.unpack(\"d\" * nbw, buf[off + 16 : off + 16 + 8 * nbw])\n",
+                "#     print(nrec, jtype, nbw)\n",
+                "#     off += 16 + 8 * nbw\n",
+                "#     nrec, jtype, nbw = struct.unpack(\"iil\", buf[off : off + 16])\n",
+                "#     spec = struct.unpack(\"d\" * nbw, buf[off + 16 : off + 16 + 8 * nbw])\n",
+                "#     print(nrec, jtype, nbw)\n",
+                "#     off += 16 + 8 * nbw\n",
+                "#     counter += 1\n",
+                "# plt.plot(wave, spec)\n",
+                "# # plt.xlim(1000,1.e4)\n",
+                "# # plt.ylim(1.e-10,1.e-6)\n",
                 "\n",
-                "buf = open(sed_output, \"rb\").read()\n",
-                "counter = 0\n",
-                "off = 0\n",
-                "while counter <= 0:\n",
-                "    nrec, jtype, nbw = struct.unpack(\"iil\", buf[off : off + 16])\n",
-                "    wave = struct.unpack(\"d\" * nbw, buf[off + 16 : off + 16 + 8 * nbw])\n",
-                "    print(nrec, jtype, nbw)\n",
-                "    off += 16 + 8 * nbw\n",
-                "    nrec, jtype, nbw = struct.unpack(\"iil\", buf[off : off + 16])\n",
-                "    spec = struct.unpack(\"d\" * nbw, buf[off + 16 : off + 16 + 8 * nbw])\n",
-                "    print(nrec, jtype, nbw)\n",
-                "    off += 16 + 8 * nbw\n",
-                "    counter += 1\n",
-                "plt.plot(wave, spec)\n",
-                "# plt.xlim(1000,1.e4)\n",
-                "# plt.ylim(1.e-10,1.e-6)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "526460bd",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "n = 6973\n",
-                "struct.unpack(\"d\", buf[off + 16 + 8 * (n - 1) : off + 16 + 8 * n])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e2ed4f27",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "nbw"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "608720be",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "buf[38896 + 16 + 8 : 38896 + 16 + 16]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "06953a40",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "struct.unpack(\"d\", buf[38896 + 16 + 8 : 38896 + 16 + 16])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e639782f",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "4.2399775704000006e-08 / 1.23542470e01"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "6901c062",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "struct.unpack(\"d\" * 1, buf[off + 16 : off + 16 + 8])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f6aaad1e",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "struct.calcsize(\"l\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f4f43f7d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "wave[1], spec[1]"
+                "# n = 6973\n",
+                "# struct.unpack(\"d\", buf[off + 16 + 8 * (n - 1) : off + 16 + 8 * n])\n",
+                "\n",
+                "# nbw\n",
+                "\n",
+                "# buf[38896 + 16 + 8 : 38896 + 16 + 16]\n",
+                "\n",
+                "# struct.unpack(\"d\", buf[38896 + 16 + 8 : 38896 + 16 + 16])\n",
+                "\n",
+                "# print(4.2399775704000006e-08 / 1.23542470e01)\n",
+                "\n",
+                "# struct.unpack(\"d\" * 1, buf[off + 16 : off + 16 + 8])\n",
+                "\n",
+                "# struct.calcsize(\"l\")\n",
+                "\n",
+                "# wave[1], spec[1]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9581fb31",
             "metadata": {},
             "outputs": [],
             "source": [
-                "d = np.loadtxt(\"../sed/STAR/PICKLES/o5v.sed.ext\")\n",
+                "d = np.loadtxt(f\"{lp.LEPHAREDIR}/sed/STAR/PICKLES/o5v.sed.ext\")\n",
                 "plt.plot(d[:, 0], d[:, 1])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2f71a1a5",
@@ -342,60 +292,58 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "51594cd6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lephare import keyword\n",
-                "\n",
-                "k = keyword(\"TEST\", \"0.1,0.1,6\")\n",
+                "k = lp.keyword(\"TEST\", \"0.1,0.1,6\")\n",
                 "print(k.split_double(\"0.03\", 3))\n",
                 "print(k.split_double(\"0.03\", 3))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f76f6cd4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "mag = MagGal(\"../test/COSMOS.para\")\n",
+                "mag = lp.MagGal(config_file)\n",
                 "mag.run(typ=\"STAR\", lib_ascii=\"YES\", star_lib_out=\"ALLSTAR_COSMOS\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e9d3014e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sed.run(typ=\"QSO\", qso_sed=\"$LEPHAREDIR/sed/QSO/SALVATO09/AGN_MOD.list\")"
+                "sed.run(typ=\"QSO\", qso_sed=f\"{lp.LEPHAREDIR}/sed/QSO/SALVATO09/AGN_MOD.list\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ef196d2c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "sed.run(typ=\"GAL\", gal_sed=\"../test/COSMOS_MOD.list\", gal_lib=\"LIB_VISTA\")"
+                "sed.run(typ=\"GAL\", gal_sed=f\"{lp.LEPHAREDIR}/examples/COSMOS_MOD.list\", gal_lib=\"LIB_VISTA\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "055b3728",
             "metadata": {},
             "outputs": [],
             "source": [
-                "mag = MagGal(\"../test/COSMOS.para\")\n",
+                "mag = lp.MagGal(config_file)\n",
                 "mag.run(\n",
                 "    typ=\"QSO\",\n",
                 "    lib_ascii=\"NO\",\n",
                 "    mod_extinc=\"0,1000\",\n",
                 "    eb_v=\"0.,0.1,0.2,0.3\",\n",
                 "    extinc_law=\"SB_calzetti.dat\",\n",
                 "    z_step=\"0.04,0,6\",\n",
@@ -415,13 +363,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.5"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lephare-0.1.1/docs/notebooks/intro.ipynb` & `lephare-0.1.2/docs/notebooks/Example_cosmo.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9685433201058201%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from lephare import zgrid, cosmo\\n')]}}, 6: {'source': "*

 * *            "['len(redshifts2)']}, delete: [4, 2]}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.6'}}"}*

```diff
@@ -11,33 +11,21 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "eaac2d65",
             "metadata": {},
             "outputs": [],
             "source": [
+                "from lephare import zgrid, cosmo\n",
                 "from matplotlib import pylab as plt\n",
                 "\n",
                 "%matplotlib inline"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "eebc75ba",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import os\n",
-                "\n",
-                "os.environ[\"LEPHAREDIR\"] = os.path.abspath(\"../..\")\n",
-                "os.environ[\"LEPHAREWORK\"] = \"WORK\""
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "93246777",
             "metadata": {},
             "source": [
                 "## cosmology module\n",
                 "This module is very limited in scope, as it is used only in computed absolute magnitude when necessary.\n",
                 "The python interface provides access to the `cosmo` class, and \n",
@@ -45,24 +33,14 @@
                 "\n",
                 "The `cosmology.h` also exposes the `zgrid` function that returns a grid of redshift, either linearly binned, or with binning increasing by a factor (1+z) at each step."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "405c4d73",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from lephare._lephare import zgrid, cosmo"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "dd9b19e5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# linear binning\n",
                 "redshifts = zgrid(0, 0.01, 0, 6)\n",
                 "lcdm = cosmo()"
@@ -97,15 +75,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cd6c7698",
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "len(redshifts2)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -116,13 +96,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.11.6"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lephare-0.1.1/examples/color.py` & `lephare-0.1.2/examples/color.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/examples/figuresLPP.py` & `lephare-0.1.2/examples/figuresLPP.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/examples/figuresLPZ.py` & `lephare-0.1.2/examples/figuresLPZ.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/examples/spec.py` & `lephare-0.1.2/examples/spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/pyproject.toml` & `lephare-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/setup.py` & `lephare-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/__init__.py` & `lephare-0.1.2/src/lephare/__init__.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/_flt.py` & `lephare-0.1.2/src/lephare/_flt.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/_pdf.py` & `lephare-0.1.2/src/lephare/_pdf.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/_photoz.py` & `lephare-0.1.2/src/lephare/_photoz.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/_spec.py` & `lephare-0.1.2/src/lephare/_spec.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/_utils.py` & `lephare-0.1.2/src/lephare/_utils.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/data_retrieval.py` & `lephare-0.1.2/src/lephare/data_retrieval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """This module provides functionality for downloading and managing data files using pooch."""
 
 import concurrent.futures
 import os
+import warnings
 from functools import partial
 from urllib.parse import urljoin, urlparse
 
+import numpy as np
 import pooch
 import requests
 
-DEFAULT_BASE_DATA_URL = "https://raw.githubusercontent.com/OliviaLynn/LEPHARE-data/main/"
+from lephare import LEPHAREDIR
+
+DEFAULT_BASE_DATA_URL = "https://raw.githubusercontent.com/lephare-photoz/lephare-data/main/"
 DEFAULT_REGISTRY_FILE = "data_registry.txt"
 
 #! Replace DEFAULT_LOCAL_DATA_PATH with the following:
 # from lephare import data_marshaller
 # DEFAULT_LOCAL_DATA_PATH = data_marshaller.get_data_path()
 #  likely something like: ~/Library/Caches/lephare/data/
 #  Note that we can use pooch.os_cache("lephare") to create a directory in the
@@ -129,15 +133,16 @@
             start_index = list_file.find("filt/")
             end_index = list_file.rfind("/")
             prefix = list_file[start_index:end_index]
 
     # Read in file
     for line in content.splitlines():
         file_name = line.split()[0].strip()
-        file_names.append(os.path.join(prefix, file_name))
+        if file_name[0] != "#":
+            file_names.append(os.path.join(prefix, file_name))
     return file_names
 
 
 def make_default_retriever():
     """Create a retriever with the default settings."""
     return make_retriever(
         base_url=DEFAULT_BASE_DATA_URL, registry_file=DEFAULT_REGISTRY_FILE, data_path=DEFAULT_LOCAL_DATA_PATH
@@ -179,14 +184,16 @@
 
     This function is for thread safety when downloading files in parallel.
 
     Parameters
     ----------
     file_names : list of str
         List of file names with relative paths.
+    base_path : str
+        Path to LEPHAREDIR if not current working directory.
     """
     unique_directories = set(
         os.path.dirname(file_name) for file_name in file_names if os.path.dirname(file_name)
     )
     for directory in unique_directories:
         if not os.path.exists(directory):
             os.makedirs(directory)
@@ -295,7 +302,109 @@
     for file_name in completed_futures:
         if os.path.getsize(file_name) == 0:
             print(f"The file {file_name} is empty.")
             return False
 
     print("All files downloaded successfully and are non-empty.")
     return True
+
+
+def config_to_required_files(keymap, base_url=None):
+    """Take a lephare config and return list of auxiliary files required for run.
+
+    For the sed lists these must be present in the auxiliary files directory. If
+    local full paths set the code will only retrieve opa, vega, and filters.
+
+    In addition to the specified files we also add opa and vega files. These
+    are always required.
+
+    We use the tau opacities by default.
+
+    Parameters
+    ==========
+    keymap : dict of lephare.keyvalue
+        The dictionary of config keys containing filters etc required.
+    base_url : str
+        Url to overwrite default base.
+    """
+    if base_url is None:
+        base_url = DEFAULT_BASE_DATA_URL
+    required_files = []
+    # We always need alloutputkeys.txt
+    # required_files += ["alloutputkeys.txt"]
+    # Opacity always required
+    opa_list = ["opa/OPACITY.dat"] + [f"opa/tau{i:02d}.out" for i in np.arange(81)]
+    required_files += opa_list
+    # vega always required
+    vega_list = [
+        "vega/BD+17.sed",
+        "vega/BD+17o4708.sed",
+        "vega/SunLCB.sed",
+        "vega/VegaLCB.sed",
+        "vega/a0v.sed",
+        "vega/a0v_n.sed",
+    ]
+    required_files += vega_list
+    required_files += [f"filt/{f}" for f in keymap["FILTER_LIST"].value.split(",")]
+    # Get user specified sed lists
+    sed_keys = ["STAR_SED", "GAL_SED", "QSO_SED"]
+    for key in sed_keys:
+        try:
+            list_file = base_url + keymap[key].value
+            required_files += [keymap[key].value]
+            file_names = read_list_file(list_file, prefix=f"sed/{key.split('_')[0]}/")
+            required_files += file_names
+        except KeyError:
+            warnings.warn(f"{key} keyword not set or not present in auxiliary files directory.")
+    # Bethermin12 always required
+    bet_list = "sed/GAL/BETHERMIN12/BETHERMIN12_MOD.list"
+    required_files += [bet_list]
+    required_files += read_list_file(base_url + bet_list, prefix="sed/GAL/")
+    # Get extinction law files
+    ext_list = [f"ext/{f}" for f in keymap["EXTINC_LAW"].value.split(",")]
+    ext_list += ["ext/MW_seaton.dat"]  # Appears to be always required
+    required_files += ext_list
+    return required_files
+
+
+def get_auxiliary_data(lephare_dir=LEPHAREDIR, keymap=None, additional_files=None):
+    """Get all auxiliary data required to run lephare.
+
+    This gets all the filters, seds, and other data files.
+
+    If no keymap is set this will git clone the full repository.
+
+    Parameters
+    ==========
+    lephare_dir : str
+        The path to the lephare directory for auxiliary files.
+    keymap : dict
+        The config dictionary.
+    additional_files : list
+        Any additional files to be downloaded from the auxiliary file repo.
+    """
+    # Get the registry file
+    download_registry_from_github()
+    base_url = DEFAULT_BASE_DATA_URL
+    registry_file = DEFAULT_REGISTRY_FILE
+    data_path = lephare_dir
+    if keymap is None:
+        # Assume if filt is present assume everything is.
+        if os.path.isdir(f"{lephare_dir}/filt"):
+            warnings.warn(
+                "Some data appears present. Not downloading."
+                "Consider setting a keymap to download a subset."
+            )
+        else:
+            # Get the full repository
+            print("Downloading all auxiliary data (~1.5Gb) to {lephare_dir}.")
+            print(f"Getting data from {base_url}.")
+            os.system(f"git clone {base_url}")
+            os.system(f"mv LEPHARE-data/* {lephare_dir}")
+    else:
+        retriever = make_retriever(base_url=base_url, registry_file=registry_file, data_path=data_path)
+        file_list = config_to_required_files(keymap)
+        download_all_files(retriever, file_list, ignore_registry=False)
+        # TODO! This will be deprecated when alloutputkeys.txt is added to the registry:
+        download_file(retriever, "alloutputkeys.txt", ignore_registry=True)
+    if additional_files is not None:
+        download_all_files(retriever, additional_files, ignore_registry=False)
```

### Comparing `lephare-0.1.1/src/lephare/filter.py` & `lephare-0.1.2/src/lephare/filter.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/filterSvc.py` & `lephare-0.1.2/src/lephare/filterSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/magSvc.py` & `lephare-0.1.2/src/lephare/magSvc.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/mag_gal.py` & `lephare-0.1.2/src/lephare/mag_gal.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/runner.py` & `lephare-0.1.2/src/lephare/runner.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/sedtolib.py` & `lephare-0.1.2/src/lephare/sedtolib.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare/zphota.py` & `lephare-0.1.2/src/lephare/zphota.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lephare.egg-info/PKG-INFO` & `lephare-0.1.2/src/lephare.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lephare
-Version: 0.1.1
+Version: 0.1.2
 Summary: LEPHARE photometric redshift estimator
 Home-page: https://gitlab.lam.fr/Galaxies/LEPHARE
 Author: Johann Cohen-Tanugi
 Author-email: Johann Cohen-Tanugi <johann.cohentanugi@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Johann Cohen-Tanugi
@@ -58,24 +58,33 @@
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 
 [![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/lephare/)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/lincc-frameworks/lephare/smoke-test.yml)](https://github.com/lephare-photoz/lephare/actions/workflows/smoke-test.yml)
 [![Codecov](https://codecov.io/gh/lephare-photoz/lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/lephare-photoz/lephare)
 [![Read The Docs](https://img.shields.io/readthedocs/lephare)](https://lephare.readthedocs.io/)
 
-This project is in an early development stage. If you wish to use and run LePHARE please download it from the [official repository](https://gitlab.lam.fr/Galaxies/LEPHARE/).
+IMPORTANT! This project is in an early development stage. If you wish to use and run LePHARE please download it from the [official repository](https://gitlab.lam.fr/Galaxies/LEPHARE/).
 
-This project was automatically generated using the LINCC-Frameworks 
-[python-project-template](https://github.com/lincc-frameworks/python-project-template).
+LePHARE (PHotometric Analysis for Redshift Estimation) is a Python package built on a complete rewrite in C++ of the [Fortran code](https://www.cfht.hawaii.edu/~arnouts/LEPHARE/acknowledgement.html) LePhare.
+LePHARE computes photometric redshifts and physical parameters by fitting spectral energy distributions (SED) to a dataset of photometric fluxes or apparent magnitudes.
 
-A repository badge was added to show that this project uses the python-project-template, however it's up to
-you whether or not you'd like to display it!
+## Installation
 
-For more information about the project template see the 
-[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
+The simplest way to install lephare is using pip:
+
+```
+pip install lephare
+```
+
+
+If you prefer to use binary executables from the command line you may wish to conduct a [legacy installation](https://gitlab.lam.fr/Galaxies/LEPHARE/).  
+
+## Example usage
+
+We provide a number of [Jupyter notebooks](docs/notebooks/) demonstrating various aspects of the Python code.
 
 ## Dev Guide - Getting Started
 
 Before installing any dependencies or writing code, it's a great idea to create a
 virtual environment. LINCC-Frameworks engineers primarily use `conda` to manage virtual
 environments. If you have conda installed locally, you can run the following to
 create and activate a new environment.
@@ -100,7 +109,17 @@
    that a set of tests will be run prior to completing a local commit. For more
    information, see the Python Project Template documentation on 
    [pre-commit](https://lincc-ppt.readthedocs.io/en/latest/practices/precommit.html)
 3. Install `pandoc` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    [Sphinx and Python Notebooks](https://lincc-ppt.readthedocs.io/en/latest/practices/sphinx.html#python-notebooks)
+
+## Citation
+
+If using this code in scientific research please cite the following papers:
+
+
+This project was automatically generated using the LINCC-Frameworks 
+[python-project-template](https://github.com/lincc-frameworks/python-project-template).
+For more information about the project template see the 
+[documentation](https://lincc-ppt.readthedocs.io/en/latest/).
```

### Comparing `lephare-0.1.1/src/lephare.egg-info/SOURCES.txt` & `lephare-0.1.2/src/lephare.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,33 +13,38 @@
 pyproject.toml
 setup.py
 .github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/0-general_issue.md
 .github/ISSUE_TEMPLATE/1-bug_report.md
 .github/ISSUE_TEMPLATE/2-feature_request.md
+.github/workflows/build-documentation.yml
 .github/workflows/compile-cpp.yml
 .github/workflows/pre-commit-ci.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
+docs/keywords.rst
+docs/legacy_install.rst
 docs/notebooks.rst
 docs/requirements.txt
 docs/doxygen/Doxyfile
 docs/notebooks/Building_list_of_onesources.ipynb
 docs/notebooks/Data_retrieval.ipynb
+docs/notebooks/Example_SED_manipulation.ipynb
+docs/notebooks/Example_cosmo.ipynb
+docs/notebooks/Example_full_run.ipynb
 docs/notebooks/Example_of_usage_of_magSvc.ipynb
 docs/notebooks/README.md
 docs/notebooks/Testing_fit_of_one_object_of_the_catalogue.ipynb
-docs/notebooks/example_full_run.ipynb
-docs/notebooks/examples.ipynb
-docs/notebooks/intro.ipynb
+docs/notebooks/data/COSMOS.para
+docs/notebooks/data/output.para
 examples/color.py
 examples/figuresLPP.py
 examples/figuresLPZ.py
 examples/spec.py
 src/lephare/__init__.py
 src/lephare/_flt.py
 src/lephare/_pdf.py
@@ -103,12 +108,13 @@
 tests/data/test_file_names.list
 tests/data/examples/COSMOS.para
 tests/data/filt/subaru/IB527.pb
 tests/data/sed/WDgd71.sed.ext
 tests/data/sed/o5v.sed.ext
 tests/lephare/test_cosmology.py
 tests/lephare/test_dataRetrieval.py
+tests/lephare/test_data_manager.py
 tests/lephare/test_globals.py
 tests/lephare/test_keyword.py
 tests/lephare/test_oneElLambda.py
 tests/lephare/test_onesource.py
 tests/lephare/test_sed.py
```

### Comparing `lephare-0.1.1/src/lib/Makefile` & `lephare-0.1.2/src/lib/Makefile`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/PDF.cpp` & `lephare-0.1.2/src/lib/PDF.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/PDF.h` & `lephare-0.1.2/src/lib/PDF.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/SED.cpp` & `lephare-0.1.2/src/lib/SED.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/SED.h` & `lephare-0.1.2/src/lib/SED.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/SEDLib.cpp` & `lephare-0.1.2/src/lib/SEDLib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/SEDLib.h` & `lephare-0.1.2/src/lib/SEDLib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/_bindings.cc` & `lephare-0.1.2/src/lib/_bindings.cc`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/cosmology.cpp` & `lephare-0.1.2/src/lib/cosmology.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/cosmology.h` & `lephare-0.1.2/src/lib/cosmology.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/ext.cpp` & `lephare-0.1.2/src/lib/ext.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/ext.h` & `lephare-0.1.2/src/lib/ext.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/ext_curv.cpp` & `lephare-0.1.2/src/lib/ext_curv.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/filter.cpp` & `lephare-0.1.2/src/lib/filter.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/filter_extinc.cpp` & `lephare-0.1.2/src/lib/filter_extinc.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/flt.cpp` & `lephare-0.1.2/src/lib/flt.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/flt.h` & `lephare-0.1.2/src/lib/flt.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/globals.cpp` & `lephare-0.1.2/src/lib/globals.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/globals.h` & `lephare-0.1.2/src/lib/globals.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/keyword.cpp` & `lephare-0.1.2/src/lib/keyword.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/keyword.h` & `lephare-0.1.2/src/lib/keyword.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/mag.cpp` & `lephare-0.1.2/src/lib/mag.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/mag.h` & `lephare-0.1.2/src/lib/mag.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/mag_gal.cpp` & `lephare-0.1.2/src/lib/mag_gal.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/oneElLambda.cpp` & `lephare-0.1.2/src/lib/oneElLambda.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/oneElLambda.h` & `lephare-0.1.2/src/lib/oneElLambda.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/onesource.cpp` & `lephare-0.1.2/src/lib/onesource.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/onesource.h` & `lephare-0.1.2/src/lib/onesource.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/opa.cpp` & `lephare-0.1.2/src/lib/opa.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/opa.h` & `lephare-0.1.2/src/lib/opa.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/photoz_lib.cpp` & `lephare-0.1.2/src/lib/photoz_lib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/photoz_lib.h` & `lephare-0.1.2/src/lib/photoz_lib.h`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/sedtolib.cpp` & `lephare-0.1.2/src/lib/sedtolib.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/src/lib/zphota.cpp` & `lephare-0.1.2/src/lib/zphota.cpp`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/conftest.py` & `lephare-0.1.2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,7 +18,13 @@
     test_dir = os.path.abspath(os.path.dirname(__file__))
     return os.path.join(test_dir, "data")
 
 
 @pytest.fixture
 def data_registry_file(test_data_dir):
     return os.path.join(test_data_dir, "test_data_registry.txt")
+
+
+@pytest.fixture
+def unset_env_vars():
+    os.environ.pop("LEPHAREDIR", None)
+    os.environ.pop("LEPHAREWORK", None)
```

### Comparing `lephare-0.1.1/tests/data/calzetti.dat` & `lephare-0.1.2/tests/data/calzetti.dat`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/data/examples/COSMOS.para` & `lephare-0.1.2/tests/data/examples/COSMOS.para`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/data/filt/subaru/IB527.pb` & `lephare-0.1.2/tests/data/filt/subaru/IB527.pb`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/data/sed/WDgd71.sed.ext` & `lephare-0.1.2/tests/data/sed/WDgd71.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/data/sed/o5v.sed.ext` & `lephare-0.1.2/tests/data/sed/o5v.sed.ext`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/data/tau10.out` & `lephare-0.1.2/tests/data/tau10.out`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/lephare/test_cosmology.py` & `lephare-0.1.2/tests/lephare/test_cosmology.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/lephare/test_dataRetrieval.py` & `lephare-0.1.2/tests/lephare/test_dataRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     make_default_retriever,
     make_retriever,
     read_list_file,
 )
 
 # TODO: this will be bundled into a module in the future,
 # so replace the hardcoding when that happens
-DEFAULT_BASE_DATA_URL = "https://raw.githubusercontent.com/OliviaLynn/LEPHARE-data/main/"
+DEFAULT_BASE_DATA_URL = "https://raw.githubusercontent.com/lephare-photoz/lephare-data/main/"
 DEFAULT_REGISTRY_FILE = "data_registry.txt"
 DEFAULT_LOCAL_DATA_PATH = "./data"
 
 
 def test_filter_file_by_prefix(test_data_dir):
     file_path = os.path.join(test_data_dir, "test_file_names.list")
     target_prefixes = ["prefix1", "prefix2"]
```

### Comparing `lephare-0.1.1/tests/lephare/test_keyword.py` & `lephare-0.1.2/tests/lephare/test_keyword.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/lephare/test_oneElLambda.py` & `lephare-0.1.2/tests/lephare/test_oneElLambda.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/lephare/test_onesource.py` & `lephare-0.1.2/tests/lephare/test_onesource.py`

 * *Files identical despite different names*

### Comparing `lephare-0.1.1/tests/lephare/test_sed.py` & `lephare-0.1.2/tests/lephare/test_sed.py`

 * *Files identical despite different names*

