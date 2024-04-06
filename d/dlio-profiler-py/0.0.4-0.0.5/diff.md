# Comparing `tmp/dlio_profiler_py-0.0.4.tar.gz` & `tmp/dlio_profiler_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlio_profiler_py-0.0.4.tar", last modified: Wed Feb  7 07:45:30 2024, max compression
+gzip compressed data, was "dist/dlio_profiler_py-0.0.5.tar", last modified: Sat Apr  6 19:21:47 2024, max compression
```

## Comparing `dlio_profiler_py-0.0.4.tar` & `dlio_profiler_py-0.0.5.tar`

### file list

```diff
@@ -1,64 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.419223 dlio_profiler_py-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.411223 dlio_profiler_py-0.0.4/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/CMake/dlio_profiler-config-version.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/CMake/dlio_profiler-config.cmake.build.in
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/CMake/dlio_profiler-config.cmake.install.in
--rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-02-07 07:45:30.419223 dlio_profiler_py-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/dependency/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dependency/cpp.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dependency/install_dependency.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/dlio_profiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dlio_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dlio_profiler/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-02-07 07:45:30.000000 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-07 07:45:30.000000 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 07:45:30.000000 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 07:45:29.000000 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-07 07:45:30.000000 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-07 07:45:30.000000 dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/dlp_analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dlp_analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31030 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dlp_analyzer/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/dlp_analyzer/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.411223 dlio_profiler_py-0.0.4/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/include/dlio_profiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/include/dlio_profiler/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/include/dlio_profiler/core/constants.h
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/include/dlio_profiler/core/typedef.h
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/include/dlio_profiler/dlio_profiler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 07:45:30.419223 dlio_profiler_py-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.411223 dlio_profiler_py-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/src/dlio_profiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.415223 dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/posix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/posix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/stdio.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/stdio.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.419223 dlio_profiler_py-0.0.4/src/dlio_profiler/core/
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/core/dlio_profiler_main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/core/dlio_profiler_main.h
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/core/enumeration.h
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/core/error.h
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/core/macro.h
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/core/singleton.h
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_logger.h
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler_preload.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler_preload.h
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler_py.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.419223 dlio_profiler_py-0.0.4/src/dlio_profiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/utils/configuration_manager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/utils/configuration_manager.h
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/utils/posix_internal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/utils/posix_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/utils/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:45:30.419223 dlio_profiler_py-0.0.4/src/dlio_profiler/writer/
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/writer/chrome_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-07 07:43:52.000000 dlio_profiler_py-0.0.4/src/dlio_profiler/writer/chrome_writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/CMake/dlio_profiler-config-version.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/CMake/dlio_profiler-config.cmake.build.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/CMake/dlio_profiler-config.cmake.install.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18463 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dependency/cpp.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dependency/install_dependency.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dlio_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dlio_profiler/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:21:44.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/dlp_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dlp_analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31030 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dlp_analyzer/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/dlp_analyzer/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/include/dlio_profiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/include/dlio_profiler/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/include/dlio_profiler/core/constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/include/dlio_profiler/core/typedef.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/include/dlio_profiler/dlio_profiler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/posix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/posix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/stdio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/stdio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/dlio_profiler_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/dlio_profiler_main.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/enumeration.h
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/error.h
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/macro.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/core/singleton.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_logger.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler_preload.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler_preload.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler_py.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/utils/configuration_manager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/utils/configuration_manager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/utils/posix_internal.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/utils/posix_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/utils/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:21:47.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/writer/chrome_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-06 19:19:58.000000 dlio_profiler_py-0.0.5/src/dlio_profiler/writer/chrome_writer.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dlio_profiler_py-0.0.4/CMake/dlio_profiler-config.cmake.build.in` & `dlio_profiler_py-0.0.5/CMake/dlio_profiler-config.cmake.build.in`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/CMake/dlio_profiler-config.cmake.install.in` & `dlio_profiler_py-0.0.5/CMake/dlio_profiler-config.cmake.install.in`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/CMakeLists.txt` & `dlio_profiler_py-0.0.5/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #------------------------------------------------------------------------------
 # Build options
 #------------------------------------------------------------------------------
 option(BUILD_PYTHON_BINDINGS "Build python bindings." ON)
 option(DLIO_PROFILER_ENABLE_TESTS "Enable internal tests" Off)
 option(ENABLE_DLIO_BENCHMARK_TESTS "Enable dlio_benchmark tests" Off)
 option(ENABLE_PAPER_TESTS "Enable paper tests" Off)
+option(DISABLE_HWLOC "Disable HWLOC" On)
 #------------------------------------------------------------------------------
 # Setup install and output Directories
 #------------------------------------------------------------------------------
 if(DEFINED ENV{DLIO_PYTHON_EXECUTABLE})
     set(PYTHON_EXECUTABLE  $ENV{DLIO_PYTHON_EXECUTABLE})
 elseif(DEFINED DLIO_PYTHON_EXECUTABLE)
     set(PYTHON_EXECUTABLE  $ENV{DLIO_PYTHON_EXECUTABLE})
@@ -96,16 +97,24 @@
             ${CMAKE_BINARY_DIR}/lib CACHE PATH "Single Directory for all Libraries"
             )
     set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY
             ${CMAKE_BINARY_DIR}/lib CACHE PATH "Single Directory for all static libraries."
             )
 endif ()
 
-
-
+#------------------------------------------------------------------------------
+# Set CXX FLAGS
+#------------------------------------------------------------------------------
+if (DISABLE_HWLOC)
+    message(STATUS "[DLIO_PROFILER] disabling HWLOC")
+    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -DDISABLE_HWLOC=0")
+else()
+    message(STATUS "[DLIO_PROFILER] enabling HWLOC")
+    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -DDISABLE_HWLOC=1")
+endif()
 
 
 if (BUILD_PYTHON_BINDINGS)
     find_package(pybind11 REQUIRED)
     #add_subdirectory(dependency/py11bind)
 endif()
 #add_subdirectory(external/cpp-logger)
@@ -123,15 +132,18 @@
 export(EXPORT gotcha-targets
         FILE "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/cmake/gotcha/gotchaTargets.cmake")]]
 #include_directories(external/GOTCHA/include)
 #add_subdirectory(external/brahma)
 #add_dependencies(brahma gotcha)
 link_directories(${CMAKE_BINARY_DIR}/lib)
 link_directories(${CMAKE_BINARY_DIR})
-set(DEPENDENCY_LIB stdc++fs -lhwloc)
+set(DEPENDENCY_LIB stdc++fs)
+if (NOT DISABLE_HWLOC)
+    set(DEPENDENCY_LIB ${DEPENDENCY_LIB} -lhwloc)
+endif()
 
 if (${CPP_LOGGER_FOUND})
     include_directories(${CPP_LOGGER_INCLUDE_DIRS})
     set(DEPENDENCY_LIB ${DEPENDENCY_LIB} ${CPP_LOGGER_LIBRARIES})
     message(STATUS "[DLIO_PROFILER] found cpp-logger at ${CPP_LOGGER_INCLUDE_DIRS}")
 else ()
     message(FATAL_ERROR "-- [DLIO_PROFILER] cpp-logger is needed for ${PROJECT_NAME} build")
```

### Comparing `dlio_profiler_py-0.0.4/PKG-INFO` & `dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,141 @@
 Metadata-Version: 2.1
-Name: dlio_profiler_py
-Version: 0.0.4
+Name: dlio-profiler-py
+Version: 0.0.5
 Summary: I/O profiler for deep learning python apps. Specifically for dlio_benchmark.
 Home-page: https://github.com/hariharan-devarajan/dlio-profiler
 Author: Hariharan Devarajan (Hari)
+License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/hariharan-devarajan/dlio-profiler/issues
 Project-URL: Source, https://github.com/hariharan-devarajan/dlio-profiler
+Description: [![DLIO Profiler Build and Test](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml/badge.svg)](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml)
+        [![Coverage Status](https://coveralls.io/repos/github/hariharan-devarajan/dlio-profiler/badge.svg?branch=feature/apis)](https://coveralls.io/github/hariharan-devarajan/dlio-profiler?branch=dev)
+        [![Documentation Status](https://readthedocs.org/projects/dlio-profiler/badge/?version=latest)](https://dlio-profiler.readthedocs.io/en/latest/?badge=latest)
+        
+        # DLIO Profiler v0.0.5
+        A multi-level profiler for capturing application functions and low-level system I/O calls from deep learning workloads.
+        
+        Requirements for profiler
+        1. Python > 3.7
+        2. pybind11
+        
+        
+        Requirements for analyzer
+        1. bokeh>=2.4.2
+        2. pybind11
+        3. [zindex_py](https://github.com/hariharan-devarajan/zindex.git)
+        4. pandas>=2.0.3
+        5. dask>=2023.5.0
+        6. distributed
+        7. numpy>=1.24.3
+        8. pyarrow>=12.0.1
+        9. rich>=13.6.0
+        10. python-intervals>=1.10.0.post1
+        11. matplotlib>=3.7.3
+        
+        ## Build DLIO Profiler with pip
+        
+        Users can easily install DLIO profiler using pip. This is the way most python packages are installed.
+        This method would work for both native python environments and conda environments.
+        
+        ### From source
+        
+        ```bash
+            git clone git@github.com:hariharan-devarajan/dlio-profiler.git
+            cd dlio-profiler
+            # You can skip this for installing the dev branch.
+            # for latest stable version use master branch.
+            git checkout tags/<Release> -b <Release>
+            pip install .
+        ```
+        
+        ### From Github
+        
+        ```bash
+        DLP_VERSION=dev
+        pip install git+https://github.com/hariharan-devarajan/dlio-profiler.git@${DLP_VERSION}
+        ```
+        
+        For more build instructions check [here](https://dlio-profiler.readthedocs.io/en/latest/build.html)
+        
+        Usage
+        
+        ```
+            from dlio_profiler.logger import dlio_logger, fn_interceptor
+            log_inst = dlio_logger.initialize_log(logfile=None, data_dir=None, process_id=-1)
+            dlio_log = fn_interceptor("COMPUTE")
+        
+            # Example of using function decorators
+            @dlio_log.log
+            def log_events(index):
+                sleep(1)
+        
+            # Example of function spawning and implicit I/O calls
+            def posix_calls(val):
+                index, is_spawn = val
+                path = f"{cwd}/data/demofile{index}.txt"
+                f = open(path, "w+")
+                f.write("Now the file has more content!")
+                f.close()
+                if is_spawn:
+                    print(f"Calling spawn on {index} with pid {os.getpid()}")
+                    log_inst.finalize() # This need to be called to correctly finalize DLIO Profiler.
+                else:
+                    print(f"Not calling spawn on {index} with pid {os.getpid()}")
+        
+            # NPZ calls internally calls POSIX calls.
+            def npz_calls(index):
+                # print(f"{cwd}/data/demofile2.npz")
+                path = f"{cwd}/data/demofile{index}.npz"
+                if os.path.exists(path):
+                    os.remove(path)
+                records = np.random.randint(255, size=(8, 8, 1024), dtype=np.uint8)
+                record_labels = [0] * 1024
+                np.savez(path, x=records, y=record_labels)
+        
+            def main():
+                log_events(0)
+                npz_calls(1)
+                with get_context('spawn').Pool(1, initializer=init) as pool:
+                    pool.map(posix_calls, ((2, True),))
+                log_inst.finalize()
+        
+        
+            if __name__ == "__main__":
+                main()
+        
+        ```
+        
+        For this example, as the DLIO_PROFILER_CPP_INIT do not pass log file or data dir, we need to set ``DLIO_PROFILER_LOG_FILE`` and ``DLIO_PROFILER_DATA_DIR``.
+        By default the DLIO Profiler mode is set to FUNCTION.
+        Example of running this configurations are:
+        
+        ```
+        
+            # the process id, app_name and .pfw will be appended by the profiler for each app and process.
+            # name of final log file is ~/log_file-<APP_NAME>-<PID>.pfw
+            DLIO_PROFILER_LOG_FILE=~/log_file
+            # Colon separated paths for including for profiler
+            DLIO_PROFILER_DATA_DIR=/dev/shm/:/p/gpfs1/$USER/dataset:$PWD/data
+            # Enable profiler
+            DLIO_PROFILER_ENABLE=1
+        ```
+        
+        For more example check [Examples](https://dlio-profiler.readthedocs.io/en/latest/examples.html).
+        
+        
 Keywords: profiler,deep learning,I/O,benchmark,NPZ,pytorch benchmark,tensorflow benchmark
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: pybind11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dlp_analyzer
-License-File: LICENSE
-
-[![DLIO Profiler Build and Test](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml/badge.svg)](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/hariharan-devarajan/dlio-profiler/badge.svg?branch=feature/apis)](https://coveralls.io/github/hariharan-devarajan/dlio-profiler?branch=dev)
-[![Documentation Status](https://readthedocs.org/projects/dlio-profiler/badge/?version=latest)](https://dlio-profiler.readthedocs.io/en/latest/?badge=latest)
-
-# DLIO Profiler v0.0.4
-A multi-level profiler for capturing application functions and low-level system I/O calls from deep learning workloads.
-
-Requirements for profiler
-1. Python > 3.7
-2. pybind11
-
-
-Requirements for analyzer
-1. bokeh>=2.4.2
-2. pybind11
-3. [zindex_py](https://github.com/hariharan-devarajan/zindex.git)
-4. pandas>=2.0.3
-5. dask>=2023.5.0
-6. distributed
-7. numpy>=1.24.3
-8. pyarrow>=12.0.1
-9. rich>=13.6.0
-10. python-intervals>=1.10.0.post1
-11. matplotlib>=3.7.3
-
-## Build DLIO Profiler with pip
-
-Users can easily install DLIO profiler using pip. This is the way most python packages are installed.
-This method would work for both native python environments and conda environments.
-
-### From source
-
-```bash
-    git clone git@github.com:hariharan-devarajan/dlio-profiler.git
-    cd dlio-profiler
-    # You can skip this for installing the dev branch.
-    # for latest stable version use master branch.
-    git checkout tags/<Release> -b <Release>
-    pip install .
-```
-
-### From Github
-
-```bash
-DLP_VERSION=dev
-pip install git+https://github.com/hariharan-devarajan/dlio-profiler.git@${DLP_VERSION}
-```
-
-For more build instructions check [here](https://dlio-profiler.readthedocs.io/en/latest/build.html)
-
-Usage
-
-```
-    from dlio_profiler.logger import dlio_logger, fn_interceptor
-    log_inst = dlio_logger.initialize_log(logfile=None, data_dir=None, process_id=-1)
-    dlio_log = fn_interceptor("COMPUTE")
-
-    # Example of using function decorators
-    @dlio_log.log
-    def log_events(index):
-        sleep(1)
-
-    # Example of function spawning and implicit I/O calls
-    def posix_calls(val):
-        index, is_spawn = val
-        path = f"{cwd}/data/demofile{index}.txt"
-        f = open(path, "w+")
-        f.write("Now the file has more content!")
-        f.close()
-        if is_spawn:
-            print(f"Calling spawn on {index} with pid {os.getpid()}")
-            log_inst.finalize() # This need to be called to correctly finalize DLIO Profiler.
-        else:
-            print(f"Not calling spawn on {index} with pid {os.getpid()}")
-
-    # NPZ calls internally calls POSIX calls.
-    def npz_calls(index):
-        # print(f"{cwd}/data/demofile2.npz")
-        path = f"{cwd}/data/demofile{index}.npz"
-        if os.path.exists(path):
-            os.remove(path)
-        records = np.random.randint(255, size=(8, 8, 1024), dtype=np.uint8)
-        record_labels = [0] * 1024
-        np.savez(path, x=records, y=record_labels)
-
-    def main():
-        log_events(0)
-        npz_calls(1)
-        with get_context('spawn').Pool(1, initializer=init) as pool:
-            pool.map(posix_calls, ((2, True),))
-        log_inst.finalize()
-
-
-    if __name__ == "__main__":
-        main()
-
-```
-
-For this example, as the DLIO_PROFILER_CPP_INIT do not pass log file or data dir, we need to set ``DLIO_PROFILER_LOG_FILE`` and ``DLIO_PROFILER_DATA_DIR``.
-By default the DLIO Profiler mode is set to FUNCTION.
-Example of running this configurations are:
-
-```
-
-    # the process id, app_name and .pfw will be appended by the profiler for each app and process.
-    # name of final log file is ~/log_file-<APP_NAME>-<PID>.pfw
-    DLIO_PROFILER_LOG_FILE=~/log_file
-    # Colon separated paths for including for profiler
-    DLIO_PROFILER_DATA_DIR=/dev/shm/:/p/gpfs1/$USER/dataset:$PWD/data
-    # Enable profiler
-    DLIO_PROFILER_ENABLE=1
-```
-
-For more example check [Examples](https://dlio-profiler.readthedocs.io/en/latest/examples.html).
-
```

### Comparing `dlio_profiler_py-0.0.4/README.md` & `dlio_profiler_py-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![DLIO Profiler Build and Test](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml/badge.svg)](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/hariharan-devarajan/dlio-profiler/badge.svg?branch=feature/apis)](https://coveralls.io/github/hariharan-devarajan/dlio-profiler?branch=dev)
 [![Documentation Status](https://readthedocs.org/projects/dlio-profiler/badge/?version=latest)](https://dlio-profiler.readthedocs.io/en/latest/?badge=latest)
 
-# DLIO Profiler v0.0.4
+# DLIO Profiler v0.0.5
 A multi-level profiler for capturing application functions and low-level system I/O calls from deep learning workloads.
 
 Requirements for profiler
 1. Python > 3.7
 2. pybind11
```

### Comparing `dlio_profiler_py-0.0.4/dependency/install_dependency.sh` & `dlio_profiler_py-0.0.5/dependency/install_dependency.sh`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/dlio_profiler/logger.py` & `dlio_profiler_py-0.0.5/dlio_profiler/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -245,7 +245,27 @@
                                                          duration=end - start,
                                                          string_args=self._arguments)
                 else:
                     dlio_logger.get_instance().log_event(name=init.__qualname__, cat=self._cat, start_time=start,
                                                          duration=end - start)
 
         return new_init
+
+    def log_static(self, func):
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if DLIO_PROFILER_ENABLE:
+                start = dlio_logger.get_instance().get_time()
+            x = func(*args, **kwargs)
+            if DLIO_PROFILER_ENABLE:
+                end = dlio_logger.get_instance().get_time()
+                if len(self._arguments) > 0:
+                    dlio_logger.get_instance().log_event(name=func.__qualname__, cat=self._cat, start_time=start,
+                                                         duration=end - start,
+                                                         string_args=self._arguments)
+                else:
+                    dlio_logger.get_instance().log_event(name=func.__qualname__, cat=self._cat, start_time=start,
+                                                         duration=end - start)
+            return x
+
+        return wrapper
```

### Comparing `dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/PKG-INFO` & `dlio_profiler_py-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,141 @@
 Metadata-Version: 2.1
-Name: dlio-profiler-py
-Version: 0.0.4
+Name: dlio_profiler_py
+Version: 0.0.5
 Summary: I/O profiler for deep learning python apps. Specifically for dlio_benchmark.
 Home-page: https://github.com/hariharan-devarajan/dlio-profiler
 Author: Hariharan Devarajan (Hari)
+License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/hariharan-devarajan/dlio-profiler/issues
 Project-URL: Source, https://github.com/hariharan-devarajan/dlio-profiler
+Description: [![DLIO Profiler Build and Test](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml/badge.svg)](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml)
+        [![Coverage Status](https://coveralls.io/repos/github/hariharan-devarajan/dlio-profiler/badge.svg?branch=feature/apis)](https://coveralls.io/github/hariharan-devarajan/dlio-profiler?branch=dev)
+        [![Documentation Status](https://readthedocs.org/projects/dlio-profiler/badge/?version=latest)](https://dlio-profiler.readthedocs.io/en/latest/?badge=latest)
+        
+        # DLIO Profiler v0.0.5
+        A multi-level profiler for capturing application functions and low-level system I/O calls from deep learning workloads.
+        
+        Requirements for profiler
+        1. Python > 3.7
+        2. pybind11
+        
+        
+        Requirements for analyzer
+        1. bokeh>=2.4.2
+        2. pybind11
+        3. [zindex_py](https://github.com/hariharan-devarajan/zindex.git)
+        4. pandas>=2.0.3
+        5. dask>=2023.5.0
+        6. distributed
+        7. numpy>=1.24.3
+        8. pyarrow>=12.0.1
+        9. rich>=13.6.0
+        10. python-intervals>=1.10.0.post1
+        11. matplotlib>=3.7.3
+        
+        ## Build DLIO Profiler with pip
+        
+        Users can easily install DLIO profiler using pip. This is the way most python packages are installed.
+        This method would work for both native python environments and conda environments.
+        
+        ### From source
+        
+        ```bash
+            git clone git@github.com:hariharan-devarajan/dlio-profiler.git
+            cd dlio-profiler
+            # You can skip this for installing the dev branch.
+            # for latest stable version use master branch.
+            git checkout tags/<Release> -b <Release>
+            pip install .
+        ```
+        
+        ### From Github
+        
+        ```bash
+        DLP_VERSION=dev
+        pip install git+https://github.com/hariharan-devarajan/dlio-profiler.git@${DLP_VERSION}
+        ```
+        
+        For more build instructions check [here](https://dlio-profiler.readthedocs.io/en/latest/build.html)
+        
+        Usage
+        
+        ```
+            from dlio_profiler.logger import dlio_logger, fn_interceptor
+            log_inst = dlio_logger.initialize_log(logfile=None, data_dir=None, process_id=-1)
+            dlio_log = fn_interceptor("COMPUTE")
+        
+            # Example of using function decorators
+            @dlio_log.log
+            def log_events(index):
+                sleep(1)
+        
+            # Example of function spawning and implicit I/O calls
+            def posix_calls(val):
+                index, is_spawn = val
+                path = f"{cwd}/data/demofile{index}.txt"
+                f = open(path, "w+")
+                f.write("Now the file has more content!")
+                f.close()
+                if is_spawn:
+                    print(f"Calling spawn on {index} with pid {os.getpid()}")
+                    log_inst.finalize() # This need to be called to correctly finalize DLIO Profiler.
+                else:
+                    print(f"Not calling spawn on {index} with pid {os.getpid()}")
+        
+            # NPZ calls internally calls POSIX calls.
+            def npz_calls(index):
+                # print(f"{cwd}/data/demofile2.npz")
+                path = f"{cwd}/data/demofile{index}.npz"
+                if os.path.exists(path):
+                    os.remove(path)
+                records = np.random.randint(255, size=(8, 8, 1024), dtype=np.uint8)
+                record_labels = [0] * 1024
+                np.savez(path, x=records, y=record_labels)
+        
+            def main():
+                log_events(0)
+                npz_calls(1)
+                with get_context('spawn').Pool(1, initializer=init) as pool:
+                    pool.map(posix_calls, ((2, True),))
+                log_inst.finalize()
+        
+        
+            if __name__ == "__main__":
+                main()
+        
+        ```
+        
+        For this example, as the DLIO_PROFILER_CPP_INIT do not pass log file or data dir, we need to set ``DLIO_PROFILER_LOG_FILE`` and ``DLIO_PROFILER_DATA_DIR``.
+        By default the DLIO Profiler mode is set to FUNCTION.
+        Example of running this configurations are:
+        
+        ```
+        
+            # the process id, app_name and .pfw will be appended by the profiler for each app and process.
+            # name of final log file is ~/log_file-<APP_NAME>-<PID>.pfw
+            DLIO_PROFILER_LOG_FILE=~/log_file
+            # Colon separated paths for including for profiler
+            DLIO_PROFILER_DATA_DIR=/dev/shm/:/p/gpfs1/$USER/dataset:$PWD/data
+            # Enable profiler
+            DLIO_PROFILER_ENABLE=1
+        ```
+        
+        For more example check [Examples](https://dlio-profiler.readthedocs.io/en/latest/examples.html).
+        
+        
 Keywords: profiler,deep learning,I/O,benchmark,NPZ,pytorch benchmark,tensorflow benchmark
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: pybind11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dlp_analyzer
-License-File: LICENSE
-
-[![DLIO Profiler Build and Test](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml/badge.svg)](https://github.com/hariharan-devarajan/dlio-profiler/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/hariharan-devarajan/dlio-profiler/badge.svg?branch=feature/apis)](https://coveralls.io/github/hariharan-devarajan/dlio-profiler?branch=dev)
-[![Documentation Status](https://readthedocs.org/projects/dlio-profiler/badge/?version=latest)](https://dlio-profiler.readthedocs.io/en/latest/?badge=latest)
-
-# DLIO Profiler v0.0.4
-A multi-level profiler for capturing application functions and low-level system I/O calls from deep learning workloads.
-
-Requirements for profiler
-1. Python > 3.7
-2. pybind11
-
-
-Requirements for analyzer
-1. bokeh>=2.4.2
-2. pybind11
-3. [zindex_py](https://github.com/hariharan-devarajan/zindex.git)
-4. pandas>=2.0.3
-5. dask>=2023.5.0
-6. distributed
-7. numpy>=1.24.3
-8. pyarrow>=12.0.1
-9. rich>=13.6.0
-10. python-intervals>=1.10.0.post1
-11. matplotlib>=3.7.3
-
-## Build DLIO Profiler with pip
-
-Users can easily install DLIO profiler using pip. This is the way most python packages are installed.
-This method would work for both native python environments and conda environments.
-
-### From source
-
-```bash
-    git clone git@github.com:hariharan-devarajan/dlio-profiler.git
-    cd dlio-profiler
-    # You can skip this for installing the dev branch.
-    # for latest stable version use master branch.
-    git checkout tags/<Release> -b <Release>
-    pip install .
-```
-
-### From Github
-
-```bash
-DLP_VERSION=dev
-pip install git+https://github.com/hariharan-devarajan/dlio-profiler.git@${DLP_VERSION}
-```
-
-For more build instructions check [here](https://dlio-profiler.readthedocs.io/en/latest/build.html)
-
-Usage
-
-```
-    from dlio_profiler.logger import dlio_logger, fn_interceptor
-    log_inst = dlio_logger.initialize_log(logfile=None, data_dir=None, process_id=-1)
-    dlio_log = fn_interceptor("COMPUTE")
-
-    # Example of using function decorators
-    @dlio_log.log
-    def log_events(index):
-        sleep(1)
-
-    # Example of function spawning and implicit I/O calls
-    def posix_calls(val):
-        index, is_spawn = val
-        path = f"{cwd}/data/demofile{index}.txt"
-        f = open(path, "w+")
-        f.write("Now the file has more content!")
-        f.close()
-        if is_spawn:
-            print(f"Calling spawn on {index} with pid {os.getpid()}")
-            log_inst.finalize() # This need to be called to correctly finalize DLIO Profiler.
-        else:
-            print(f"Not calling spawn on {index} with pid {os.getpid()}")
-
-    # NPZ calls internally calls POSIX calls.
-    def npz_calls(index):
-        # print(f"{cwd}/data/demofile2.npz")
-        path = f"{cwd}/data/demofile{index}.npz"
-        if os.path.exists(path):
-            os.remove(path)
-        records = np.random.randint(255, size=(8, 8, 1024), dtype=np.uint8)
-        record_labels = [0] * 1024
-        np.savez(path, x=records, y=record_labels)
-
-    def main():
-        log_events(0)
-        npz_calls(1)
-        with get_context('spawn').Pool(1, initializer=init) as pool:
-            pool.map(posix_calls, ((2, True),))
-        log_inst.finalize()
-
-
-    if __name__ == "__main__":
-        main()
-
-```
-
-For this example, as the DLIO_PROFILER_CPP_INIT do not pass log file or data dir, we need to set ``DLIO_PROFILER_LOG_FILE`` and ``DLIO_PROFILER_DATA_DIR``.
-By default the DLIO Profiler mode is set to FUNCTION.
-Example of running this configurations are:
-
-```
-
-    # the process id, app_name and .pfw will be appended by the profiler for each app and process.
-    # name of final log file is ~/log_file-<APP_NAME>-<PID>.pfw
-    DLIO_PROFILER_LOG_FILE=~/log_file
-    # Colon separated paths for including for profiler
-    DLIO_PROFILER_DATA_DIR=/dev/shm/:/p/gpfs1/$USER/dataset:$PWD/data
-    # Enable profiler
-    DLIO_PROFILER_ENABLE=1
-```
-
-For more example check [Examples](https://dlio-profiler.readthedocs.io/en/latest/examples.html).
-
```

### Comparing `dlio_profiler_py-0.0.4/dlio_profiler_py.egg-info/SOURCES.txt` & `dlio_profiler_py-0.0.5/dlio_profiler_py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 CMakeLists.txt
-LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 CMake/dlio_profiler-config-version.cmake.in
 CMake/dlio_profiler-config.cmake.build.in
 CMake/dlio_profiler-config.cmake.install.in
```

### Comparing `dlio_profiler_py-0.0.4/dlp_analyzer/main.py` & `dlio_profiler_py-0.0.5/dlp_analyzer/main.py`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/dlp_analyzer/plots.py` & `dlio_profiler_py-0.0.5/dlp_analyzer/plots.py`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/include/dlio_profiler/core/constants.h` & `dlio_profiler_py-0.0.5/include/dlio_profiler/core/constants.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/include/dlio_profiler/dlio_profiler.h` & `dlio_profiler_py-0.0.5/include/dlio_profiler/dlio_profiler.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/pyproject.toml` & `dlio_profiler_py-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/setup.py` & `dlio_profiler_py-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         cmake_args += [f"-DCMAKE_PREFIX_PATH={install_prefix}", f"-Dpybind11_DIR={py_cmake_dir}"]
         print(cmake_args)
 
         # Using this requires trailing slash for auto-detection & inclusion of
         # auxiliary "native" libs
         build_type = os.environ.get("CMAKE_BUILD_TYPE", "Release")
         cmake_args += [f"-DCMAKE_BUILD_TYPE={build_type}"]
+        enable_hwloc = os.environ.get("DLIO_PROFILER_DISABLE_HWLOC", "On")
+        cmake_args += [f"-DDISABLE_HWLOC={enable_hwloc}"]
         enable_tests = os.environ.get("DLIO_PROFILER_ENABLE_TESTS", "Off")
         cmake_args += [f"-DDLIO_PROFILER_ENABLE_TESTS={enable_tests}"]
         enable_dlio_tests = os.environ.get("ENABLE_DLIO_BENCHMARK_TESTS", "Off")
         cmake_args += [f"-DENABLE_DLIO_BENCHMARK_TESTS={enable_dlio_tests}"]
         enable_dlio_tests = os.environ.get("ENABLE_PAPER_TESTS", "Off")
         cmake_args += [f"-DENABLE_PAPER_TESTS={enable_dlio_tests}"]
         cmake_args += [f"-DPYTHON_EXECUTABLE={sys.executable}"]
@@ -123,15 +125,15 @@
 import pathlib
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="dlio_profiler_py",
-    version="0.0.4",
+    version="0.0.5",
     description="I/O profiler for deep learning python apps. Specifically for dlio_benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hariharan-devarajan/dlio-profiler",
     author="Hariharan Devarajan (Hari)",
     classifiers=[  # Optional
         # How mature is this project? Common values are
```

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/posix.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/posix.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/posix.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/posix.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/stdio.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/stdio.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/brahma/stdio.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/brahma/stdio.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/core/dlio_profiler_main.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/core/dlio_profiler_main.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/core/dlio_profiler_main.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/core/dlio_profiler_main.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/core/enumeration.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/core/enumeration.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/core/error.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/core/error.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/core/macro.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/core/macro.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/core/singleton.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/core/singleton.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_logger.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_logger.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler_preload.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler_preload.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/dlio_profiler_py.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/dlio_profiler_py.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/utils/configuration_manager.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/utils/configuration_manager.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/utils/configuration_manager.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/utils/configuration_manager.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/utils/posix_internal.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/utils/posix_internal.cpp`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/utils/posix_internal.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/utils/posix_internal.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/utils/utils.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/utils/utils.h`

 * *Files identical despite different names*

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/writer/chrome_writer.cpp` & `dlio_profiler_py-0.0.5/src/dlio_profiler/writer/chrome_writer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,17 @@
                                    filename.c_str());
           }
         }
       }
     }
   }
   if (enable_core_affinity) {
+#if DISABLE_HWLOC == 1
     hwloc_topology_destroy(topology);
+#endif
   }
   DLIO_PROFILER_LOGDEBUG("Finished writer finalization", "");
 }
 
 
 void
 dlio_profiler::ChromeWriter::convert_json(ConstEventType event_name, ConstEventType category, TimeResolution start_time,
```

### Comparing `dlio_profiler_py-0.0.4/src/dlio_profiler/writer/chrome_writer.h` & `dlio_profiler_py-0.0.5/src/dlio_profiler/writer/chrome_writer.h`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 #define DLIO_PROFILER_CHROME_WRITER_H
 
 #include <dlio_profiler/core/constants.h>
 #include <dlio_profiler/core/typedef.h>
 #include <dlio_profiler/utils/configuration_manager.h>
 #include <dlio_profiler/utils/posix_internal.h>
 #include <dlio_profiler/utils/utils.h>
+#if DISABLE_HWLOC == 1
 #include <hwloc.h>
+#endif
+#include <assert.h>
 #include <unistd.h>
 
 #include <any>
 #include <atomic>
 #include <mutex>
 #include <shared_mutex>
 #include <string>
@@ -27,16 +30,20 @@
     class ChromeWriter {
     private:
         std::unordered_map<char *, std::any> metadata;
     protected:
         bool throw_error;
         std::string filename;
     private:
-        bool enable_core_affinity, include_metadata, enable_compression;
+        bool include_metadata, enable_compression;
+
+        bool enable_core_affinity;
+#if DISABLE_HWLOC == 1
         hwloc_topology_t topology;
+#endif
         FILE* fh;
         std::atomic_int index;
         char hostname[256];
         static const int MAX_LINE_SIZE=4096;
         static const int MAX_META_LINE_SIZE=3000;
         void convert_json(ConstEventType event_name, ConstEventType category, TimeResolution start_time,
                                                   TimeResolution duration, std::unordered_map<std::string, std::any> *metadata,
@@ -53,22 +60,24 @@
                   filename.c_str(), written_elements, write_size, strerror(errno));
           }  // GCOVR_EXCL_STOP
           return written_elements;
         }
         std::vector<unsigned> core_affinity() {
           DLIO_PROFILER_LOGDEBUG("ChromeWriter.core_affinity","");
           auto cores = std::vector<unsigned>();
+#if DISABLE_HWLOC == 1
           if (enable_core_affinity) {
             hwloc_cpuset_t set = hwloc_bitmap_alloc();
             hwloc_get_cpubind(topology, set, HWLOC_CPUBIND_PROCESS);
             for (unsigned id = hwloc_bitmap_first(set); id != -1; id = hwloc_bitmap_next(set, id)) {
               cores.push_back(id);
             }
             hwloc_bitmap_free(set);
           }
+#endif
           return cores;
         }
 
         void get_hostname(char* hostname) {
           DLIO_PROFILER_LOGDEBUG("ChromeWriter.get_hostname","");
           gethostname(hostname, 256);
         }
@@ -79,16 +88,18 @@
           DLIO_PROFILER_LOGDEBUG("ChromeWriter.ChromeWriter","");
           auto conf = dlio_profiler::Singleton<dlio_profiler::ConfigurationManager>::get_instance();
           get_hostname(hostname);
           include_metadata = conf->metadata;
           enable_core_affinity = conf->core_affinity;
           enable_compression = conf->compression;
           if (enable_core_affinity) {
+#if DISABLE_HWLOC == 1
             hwloc_topology_init(&topology);  // initialization
             hwloc_topology_load(topology);   // actual detection
+#endif
           }
         }
         ~ChromeWriter(){DLIO_PROFILER_LOGDEBUG("Destructing ChromeWriter","");}
         void initialize(char *filename, bool throw_error);
 
         void log(ConstEventType event_name, ConstEventType category, TimeResolution &start_time, TimeResolution &duration,
                  std::unordered_map<std::string, std::any> *metadata, ProcessID process_id, ThreadID tid);
```

