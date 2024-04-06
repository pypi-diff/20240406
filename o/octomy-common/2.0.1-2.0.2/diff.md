# Comparing `tmp/octomy-common-2.0.1.tar.gz` & `tmp/octomy-common-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-common-2.0.1.tar", last modified: Sat Apr  6 12:23:02 2024, max compression
+gzip compressed data, was "octomy-common-2.0.2.tar", last modified: Sat Apr  6 12:30:48 2024, max compression
```

## Comparing `octomy-common-2.0.1.tar` & `octomy-common-2.0.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.697925 octomy-common-2.0.1/
--rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.1/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.693925 octomy-common-2.0.1/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.1/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.1/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.1/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 12:23:02.697925 octomy-common-2.0.1/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.1/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-06 10:44:21.000000 octomy-common-2.0.1/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.693925 octomy-common-2.0.1/code_quality/
--rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.1/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.1/code_quality/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.1/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.1/code_quality/pylintrc
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.693925 octomy-common-2.0.1/design/
--rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.1/design/logo-1024.png
--rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.1/design/logo-1024.svg
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.677925 octomy-common-2.0.1/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.681925 octomy-common-2.0.1/octomy/access/
--rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.1/octomy/access/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.681925 octomy-common-2.0.1/octomy/batch/
--rw-r--r--   0 leo       (1000) leo       (1000)    19966 2024-04-01 16:19:39.000000 octomy-common-2.0.1/octomy/batch/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     7061 2024-04-01 16:52:41.000000 octomy-common-2.0.1/octomy/batch/db.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/batch/server/
--rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-common-2.0.1/octomy/batch/server/WebsiteIO.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2205 2023-08-28 22:19:16.000000 octomy-common-2.0.1/octomy/batch/server/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2565 2024-04-01 14:56:50.000000 octomy-common-2.0.1/octomy/batch/types.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/cad/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/cad/generators/
--rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.1/octomy/cad/generators/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.1/octomy/cad/generators/common.py
--rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.1/octomy/cad/generators/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.1/octomy/cad/generators/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    15516 2023-11-26 17:10:20.000000 octomy-common-2.0.1/octomy/cad/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)    28131 2023-12-10 00:24:52.000000 octomy-common-2.0.1/octomy/cad/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.1/octomy/cad/parts.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/cad/types/
--rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.1/octomy/cad/types/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/config/
--rw-r--r--   0 leo       (1000) leo       (1000)    13118 2024-04-06 09:12:51.000000 octomy-common-2.0.1/octomy/config/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/db/
--rw-rw-r--   0 leo       (1000) leo       (1000)    12155 2024-04-06 08:50:55.000000 octomy-common-2.0.1/octomy/db/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/log/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.1/octomy/log/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.685926 octomy-common-2.0.1/octomy/storage/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.1/octomy/storage/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.1/octomy/storage/google_drive.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.689926 octomy-common-2.0.1/octomy/utils/
--rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.1/octomy/utils/Context.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.1/octomy/utils/Profiler.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.1/octomy/utils/Svg.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.1/octomy/utils/Watchdog.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.1/octomy/utils/WorkerPool.py
--rw-r--r--   0 leo       (1000) leo       (1000)    13880 2024-04-06 09:01:59.000000 octomy-common-2.0.1/octomy/utils/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.1/octomy/utils/click.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.1/octomy/utils/credentials.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.1/octomy/utils/csv_to_db.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.1/octomy/utils/debug_view.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.1/octomy/utils/excavator.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.1/octomy/utils/expiry_cache.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.689926 octomy-common-2.0.1/octomy/version/
--rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.1/octomy/version/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.689926 octomy-common-2.0.1/octomy/web/
--rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.1/octomy/web/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.1/octomy/web/autoroute.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.689926 octomy-common-2.0.1/octomy/web/context/
--rw-r--r--   0 leo       (1000) leo       (1000)     2247 2024-03-24 20:06:54.000000 octomy-common-2.0.1/octomy/web/context/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.689926 octomy-common-2.0.1/octomy/web/search/
--rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.1/octomy/web/search/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.693925 octomy-common-2.0.1/octomy_common.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 12:23:02.000000 octomy-common-2.0.1/octomy_common.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1856 2024-04-06 12:23:02.000000 octomy-common-2.0.1/octomy_common.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-06 12:23:02.000000 octomy-common-2.0.1/octomy_common.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 12:23:02.000000 octomy-common-2.0.1/octomy_common.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      210 2024-04-06 12:23:02.000000 octomy-common-2.0.1/octomy_common.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 12:23:02.000000 octomy-common-2.0.1/octomy_common.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.1/octomy_common.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.697925 octomy-common-2.0.1/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)      210 2024-04-06 10:23:12.000000 octomy-common-2.0.1/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1282 2024-04-06 09:43:18.000000 octomy-common-2.0.1/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.1/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.1/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-06 12:23:02.697925 octomy-common-2.0.1/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.1/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.697925 octomy-common-2.0.1/tests/
--rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.1/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.1/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.697925 octomy-common-2.0.1/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.1/tests/integration/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.1/tests/integration/test_true.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.697925 octomy-common-2.0.1/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.1/tests/load/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.1/tests/load/test_true.py
--rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.1/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:23:02.697925 octomy-common-2.0.1/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.1/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1411 2023-08-28 21:54:48.000000 octomy-common-2.0.1/tests/unit/test_util.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.874212 octomy-common-2.0.2/
+-rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.2/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.2/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.2/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.2/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 12:30:48.874212 octomy-common-2.0.2/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.2/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-06 12:30:11.000000 octomy-common-2.0.2/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.870212 octomy-common-2.0.2/code_quality/
+-rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.2/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.2/code_quality/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.2/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.2/code_quality/pylintrc
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.870212 octomy-common-2.0.2/design/
+-rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.2/design/logo-1024.png
+-rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.2/design/logo-1024.svg
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.858212 octomy-common-2.0.2/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.858212 octomy-common-2.0.2/octomy/access/
+-rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.2/octomy/access/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.858212 octomy-common-2.0.2/octomy/batch/
+-rw-r--r--   0 leo       (1000) leo       (1000)    19966 2024-04-01 16:19:39.000000 octomy-common-2.0.2/octomy/batch/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     7061 2024-04-01 16:52:41.000000 octomy-common-2.0.2/octomy/batch/db.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/batch/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-common-2.0.2/octomy/batch/server/WebsiteIO.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2205 2023-08-28 22:19:16.000000 octomy-common-2.0.2/octomy/batch/server/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2565 2024-04-01 14:56:50.000000 octomy-common-2.0.2/octomy/batch/types.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/cad/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/cad/generators/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.2/octomy/cad/generators/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.2/octomy/cad/generators/common.py
+-rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.2/octomy/cad/generators/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.2/octomy/cad/generators/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.2/octomy/cad/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.2/octomy/cad/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.2/octomy/cad/parts.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/cad/types/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.2/octomy/cad/types/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/config/
+-rw-r--r--   0 leo       (1000) leo       (1000)    13118 2024-04-06 09:12:51.000000 octomy-common-2.0.2/octomy/config/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/db/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    12155 2024-04-06 08:50:55.000000 octomy-common-2.0.2/octomy/db/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/log/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.2/octomy/log/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.862212 octomy-common-2.0.2/octomy/storage/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.2/octomy/storage/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.2/octomy/storage/google_drive.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/octomy/utils/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.2/octomy/utils/Context.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.2/octomy/utils/Profiler.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.2/octomy/utils/Svg.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.2/octomy/utils/Watchdog.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.2/octomy/utils/WorkerPool.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    13880 2024-04-06 09:01:59.000000 octomy-common-2.0.2/octomy/utils/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.2/octomy/utils/click.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.2/octomy/utils/credentials.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.2/octomy/utils/csv_to_db.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.2/octomy/utils/debug_view.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.2/octomy/utils/excavator.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.2/octomy/utils/expiry_cache.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/octomy/version/
+-rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.2/octomy/version/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/octomy/web/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.2/octomy/web/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.2/octomy/web/autoroute.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/octomy/web/context/
+-rw-r--r--   0 leo       (1000) leo       (1000)     2247 2024-03-24 20:06:54.000000 octomy-common-2.0.2/octomy/web/context/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/octomy/web/search/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.2/octomy/web/search/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.866212 octomy-common-2.0.2/octomy_common.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 12:30:48.000000 octomy-common-2.0.2/octomy_common.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1856 2024-04-06 12:30:48.000000 octomy-common-2.0.2/octomy_common.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-06 12:30:48.000000 octomy-common-2.0.2/octomy_common.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 12:30:48.000000 octomy-common-2.0.2/octomy_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      210 2024-04-06 12:30:48.000000 octomy-common-2.0.2/octomy_common.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 12:30:48.000000 octomy-common-2.0.2/octomy_common.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.2/octomy_common.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.870212 octomy-common-2.0.2/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)      210 2024-04-06 10:23:12.000000 octomy-common-2.0.2/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1282 2024-04-06 09:43:18.000000 octomy-common-2.0.2/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.2/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.2/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-06 12:30:48.874212 octomy-common-2.0.2/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.2/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.870212 octomy-common-2.0.2/tests/
+-rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.2/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.2/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.870212 octomy-common-2.0.2/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.2/tests/integration/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.2/tests/integration/test_true.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.874212 octomy-common-2.0.2/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.2/tests/load/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.2/tests/load/test_true.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.2/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 12:30:48.874212 octomy-common-2.0.2/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.2/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1411 2023-08-28 21:54:48.000000 octomy-common-2.0.2/tests/unit/test_util.py
```

### Comparing `octomy-common-2.0.1/.gitignore` & `octomy-common-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/.gitlab/ci.yaml` & `octomy-common-2.0.2/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/LICENSE` & `octomy-common-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/PKG-INFO` & `octomy-common-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.1
+Version: 2.0.2
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-common-2.0.1/README.md` & `octomy-common-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/code_quality/Makefile` & `octomy-common-2.0.2/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/code_quality/pylintrc` & `octomy-common-2.0.2/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/design/logo-1024.png` & `octomy-common-2.0.2/design/logo-1024.png`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/design/logo-1024.svg` & `octomy-common-2.0.2/design/logo-1024.svg`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/access/__init__.py` & `octomy-common-2.0.2/octomy/access/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/batch/__init__.py` & `octomy-common-2.0.2/octomy/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/batch/db.py` & `octomy-common-2.0.2/octomy/batch/db.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/batch/server/WebsiteIO.py` & `octomy-common-2.0.2/octomy/batch/server/WebsiteIO.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/batch/server/__init__.py` & `octomy-common-2.0.2/octomy/batch/server/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/batch/types.py` & `octomy-common-2.0.2/octomy/batch/types.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/cad/generators/__init__.py` & `octomy-common-2.0.2/octomy/cad/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/cad/generators/openscad.py` & `octomy-common-2.0.2/octomy/cad/generators/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/cad/ntop.py` & `octomy-common-2.0.2/octomy/cad/ntop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 import asyncio
 import datetime
-import fk.utils
+import octomy.utils
 import logging
 import os
 import pprint
 import re
 import subprocess
 import sys
 import shlex
@@ -443,14 +443,14 @@
 					if float(self.antialias) != 1.0:
 						for outfile in self.outfiles:
 							self._process_frame(outfile)
 				else:
 					self.process_animation(basename)
 			self.complete = True
 			took = now() - start
-			logger.info(f"Rendering took {fk.utils.human_delta(took)}")
+			logger.info(f"Rendering took {octomy.utils.human_delta(took)}")
 			return self.success, self.success and None or self.error_string()
 		except Exception as e:
 			logger.exception("Error occurred while running OpenScad")
 			return self.success, f"Exception: '{pprint.pformat(e)}'"
 		# Whatever happened here, tell the system
 		return self.success, "Unexpected end of run()"
```

### Comparing `octomy-common-2.0.1/octomy/cad/openscad.py` & `octomy-common-2.0.2/octomy/cad/openscad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 import asyncio
 import datetime
-import fk.utils
+import octomy.utils
 import logging
 import os
 import pprint
 import re
 import subprocess
 import sys
 import shlex
@@ -414,16 +414,16 @@
 		if "?" == t:
 			# End of initial variable section
 			break;
 	took = now() - start
 	if do_debug:
 		logger.info("#"*240)
 		logger.info("\n"*2)
-	#logger.info(f"Parsing took {fk.utils.human_delta(took)}")
-	#logger.info(f"Final parsed parameters for source {fk.utils.human_bytesize(len(source))} ({len(lines)} lines):")
+	#logger.info(f"Parsing took {octomy.utils.human_delta(took)}")
+	#logger.info(f"Final parsed parameters for source {octomy.utils.human_bytesize(len(source))} ({len(lines)} lines):")
 	#logger.info(f"parameters:{len(parameters_list)}")
 	#logger.info(f"D:{pprint.pformat(parameters_list)}")
 	#logger.info("...")
 	return parameters_list
 
 
 class RenderMode(Enum):
@@ -846,14 +846,14 @@
 					if float(self.antialias) != 1.0:
 						for outfile in self.outfiles:
 							self._process_frame(outfile)
 				else:
 					self.process_animation(basename)
 			self.complete = True
 			took = now() - start
-			logger.info(f"Rendering took {fk.utils.human_delta(took)}")
+			logger.info(f"Rendering took {octomy.utils.human_delta(took)}")
 			return self.success, self.success and None or self.error_string()
 		except Exception as e:
 			logger.exception("Error occurred while running OpenScad")
 			return self.success, f"Exception: '{pprint.pformat(e)}'"
 		# Whatever happened here, tell the system
 		return self.success, "Unexpected end of run()"
```

### Comparing `octomy-common-2.0.1/octomy/cad/parts.py` & `octomy-common-2.0.2/octomy/cad/parts.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/cad/types/__init__.py` & `octomy-common-2.0.2/octomy/cad/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/config/__init__.py` & `octomy-common-2.0.2/octomy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/db/__init__.py` & `octomy-common-2.0.2/octomy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/log/__init__.py` & `octomy-common-2.0.2/octomy/log/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/storage/google_drive.py` & `octomy-common-2.0.2/octomy/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/Profiler.py` & `octomy-common-2.0.2/octomy/utils/Profiler.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/Svg.py` & `octomy-common-2.0.2/octomy/utils/Svg.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/Watchdog.py` & `octomy-common-2.0.2/octomy/utils/Watchdog.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/WorkerPool.py` & `octomy-common-2.0.2/octomy/utils/WorkerPool.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/__init__.py` & `octomy-common-2.0.2/octomy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/click.py` & `octomy-common-2.0.2/octomy/utils/click.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/credentials.py` & `octomy-common-2.0.2/octomy/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/csv_to_db.py` & `octomy-common-2.0.2/octomy/utils/csv_to_db.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/debug_view.py` & `octomy-common-2.0.2/octomy/utils/debug_view.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/excavator.py` & `octomy-common-2.0.2/octomy/utils/excavator.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/utils/expiry_cache.py` & `octomy-common-2.0.2/octomy/utils/expiry_cache.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/web/__init__.py` & `octomy-common-2.0.2/octomy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/web/autoroute.py` & `octomy-common-2.0.2/octomy/web/autoroute.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/web/context/__init__.py` & `octomy-common-2.0.2/octomy/web/context/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy/web/search/__init__.py` & `octomy-common-2.0.2/octomy/web/search/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/octomy_common.egg-info/PKG-INFO` & `octomy-common-2.0.2/octomy_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.1
+Version: 2.0.2
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-common-2.0.1/octomy_common.egg-info/SOURCES.txt` & `octomy-common-2.0.2/octomy_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/requirements/requirements.txt` & `octomy-common-2.0.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/requirements/test_requirements.txt` & `octomy-common-2.0.2/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/setup.py` & `octomy-common-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/tests/Makefile` & `octomy-common-2.0.2/tests/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.1/tests/unit/test_util.py` & `octomy-common-2.0.2/tests/unit/test_util.py`

 * *Files identical despite different names*

