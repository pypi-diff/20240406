# Comparing `tmp/octomy-common-1.0.9.tar.gz` & `tmp/octomy-common-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-common-1.0.9.tar", last modified: Sun Jan 17 22:11:21 2021, max compression
+gzip compressed data, was "octomy-common-2.0.0.tar", last modified: Sat Apr  6 10:03:12 2024, max compression
```

## Comparing `octomy-common-1.0.9.tar` & `octomy-common-2.0.0.tar`

### file list

```diff
@@ -1,68 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/
--rw-rw-rw-   0 root         (0) root         (0)      735 2021-01-15 13:54:52.000000 octomy-common-1.0.9/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.437482 octomy-common-1.0.9/.gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      768 2021-01-16 18:41:42.000000 octomy-common-1.0.9/.gitlab/ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)     5904 2021-01-17 22:07:15.000000 octomy-common-1.0.9/Makefile
--rw-r--r--   0 root         (0) root         (0)     7556 2021-01-17 22:11:21.445482 octomy-common-1.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6053 2021-01-15 13:54:52.000000 octomy-common-1.0.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2021-01-17 22:07:15.000000 octomy-common-1.0.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.437482 octomy-common-1.0.9/code_quality/
--rw-rw-rw-   0 root         (0) root         (0)      136 2021-01-15 13:54:52.000000 octomy-common-1.0.9/code_quality/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1919 2021-01-15 13:54:52.000000 octomy-common-1.0.9/code_quality/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      117 2021-01-15 13:54:52.000000 octomy-common-1.0.9/code_quality/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    11867 2021-01-15 13:54:52.000000 octomy-common-1.0.9/code_quality/pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.437482 octomy-common-1.0.9/design/
--rw-rw-rw-   0 root         (0) root         (0)    62298 2021-01-15 13:54:52.000000 octomy-common-1.0.9/design/logo-1024.png
--rw-rw-rw-   0 root         (0) root         (0)     7427 2021-01-15 13:54:52.000000 octomy-common-1.0.9/design/logo-1024.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.433482 octomy-common-1.0.9/fk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.437482 octomy-common-1.0.9/fk/config/
--rw-rw-rw-   0 root         (0) root         (0)    11524 2021-01-17 22:07:15.000000 octomy-common-1.0.9/fk/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.437482 octomy-common-1.0.9/fk/db/
--rw-rw-rw-   0 root         (0) root         (0)    19810 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/db/DatabaseConnection.py
--rw-rw-rw-   0 root         (0) root         (0)     3333 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/db/Influx.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/db/check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.441482 octomy-common-1.0.9/fk/log/
--rw-rw-rw-   0 root         (0) root         (0)     1648 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/log/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.441482 octomy-common-1.0.9/fk/utils/
--rw-rw-rw-   0 root         (0) root         (0)      147 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/Context.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/Profiler.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/Svg.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/Watchdog.py
--rw-rw-rw-   0 root         (0) root         (0)     5884 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/WorkerPool.py
--rw-rw-rw-   0 root         (0) root         (0)     9530 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1766 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/click.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/csv_to_db.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/debug_view.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/excavator.py
--rw-rw-rw-   0 root         (0) root         (0)     2902 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/utils/expiry_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.441482 octomy-common-1.0.9/fk/version/
--rw-rw-rw-   0 root         (0) root         (0)      598 2021-01-15 13:54:52.000000 octomy-common-1.0.9/fk/version/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/octomy_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7556 2021-01-17 22:11:21.000000 octomy-common-1.0.9/octomy_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1157 2021-01-17 22:11:21.000000 octomy-common-1.0.9/octomy_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-17 22:11:21.000000 octomy-common-1.0.9/octomy_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      144 2021-01-17 22:11:21.000000 octomy-common-1.0.9/octomy_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2021-01-17 22:11:21.000000 octomy-common-1.0.9/octomy_common.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-17 22:11:20.000000 octomy-common-1.0.9/octomy_common.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      144 2021-01-15 13:54:52.000000 octomy-common-1.0.9/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      932 2021-01-16 18:28:48.000000 octomy-common-1.0.9/requirements/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      215 2021-01-15 13:54:52.000000 octomy-common-1.0.9/requirements/test_requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     3083 2021-01-16 18:28:48.000000 octomy-common-1.0.9/requirements/test_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2021-01-17 22:11:21.445482 octomy-common-1.0.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     6645 2021-01-17 22:11:15.000000 octomy-common-1.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/Makefile
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/integration/test_true.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/tests/load/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/load/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/load/test_true.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-17 22:11:21.445482 octomy-common-1.0.9/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2021-01-15 13:54:52.000000 octomy-common-1.0.9/tests/unit/test_true.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.0/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.0/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.0/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.0/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 10:03:12.125001 octomy-common-2.0.0/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.0/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-06 08:47:04.000000 octomy-common-2.0.0/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/code_quality/
+-rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.0/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.0/code_quality/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.0/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.0/code_quality/pylintrc
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/design/
+-rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.0/design/logo-1024.png
+-rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.0/design/logo-1024.svg
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.113000 octomy-common-2.0.0/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.117001 octomy-common-2.0.0/octomy/config/
+-rw-r--r--   0 leo       (1000) leo       (1000)    13118 2024-04-06 09:12:51.000000 octomy-common-2.0.0/octomy/config/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.117001 octomy-common-2.0.0/octomy/db/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    12155 2024-04-06 08:50:55.000000 octomy-common-2.0.0/octomy/db/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.117001 octomy-common-2.0.0/octomy/log/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.0/octomy/log/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.117001 octomy-common-2.0.0/octomy/storage/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.0/octomy/storage/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.0/octomy/storage/google_drive.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/octomy/utils/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.0/octomy/utils/Context.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.0/octomy/utils/Profiler.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.0/octomy/utils/Svg.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.0/octomy/utils/Watchdog.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.0/octomy/utils/WorkerPool.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    13880 2024-04-06 09:01:59.000000 octomy-common-2.0.0/octomy/utils/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.0/octomy/utils/click.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.0/octomy/utils/credentials.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.0/octomy/utils/csv_to_db.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.0/octomy/utils/debug_view.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.0/octomy/utils/excavator.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.0/octomy/utils/expiry_cache.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/octomy/version/
+-rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.0/octomy/version/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/octomy/web/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.0/octomy/web/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.0/octomy/web/autoroute.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/octomy/web/context/
+-rw-r--r--   0 leo       (1000) leo       (1000)     2247 2024-03-24 20:06:54.000000 octomy-common-2.0.0/octomy/web/context/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/octomy/web/search/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.0/octomy/web/search/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.121001 octomy-common-2.0.0/octomy_common.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 10:03:11.000000 octomy-common-2.0.0/octomy_common.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1450 2024-04-06 10:03:12.000000 octomy-common-2.0.0/octomy_common.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-06 10:03:11.000000 octomy-common-2.0.0/octomy_common.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 10:03:11.000000 octomy-common-2.0.0/octomy_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      210 2024-04-06 10:03:11.000000 octomy-common-2.0.0/octomy_common.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 10:03:11.000000 octomy-common-2.0.0/octomy_common.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.0/octomy_common.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)      210 2024-04-06 09:42:33.000000 octomy-common-2.0.0/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1282 2024-04-06 09:43:18.000000 octomy-common-2.0.0/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.0/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.0/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-06 10:03:12.129001 octomy-common-2.0.0/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/tests/
+-rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.0/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.0/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.0/tests/integration/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.0/tests/integration/test_true.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.0/tests/load/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.0/tests/load/test_true.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.0/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 10:03:12.125001 octomy-common-2.0.0/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1411 2023-08-28 21:54:48.000000 octomy-common-2.0.0/tests/unit/test_util.py
```

### Comparing `octomy-common-1.0.9/.gitignore` & `octomy-common-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `octomy-common-1.0.9/.gitlab/ci.yaml` & `octomy-common-2.0.0/.gitlab/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 Build:
   stage: build-and-test
   tags:
   - grunner
   script:
   - make pypi-build
   artifacts:
-   paths:
-   - dist
-   expire_in: 2 hours
+    paths:
+    - dist
+    expire_in: 2 hours
 
 Test:
   stage: build-and-test
   tags:
   - grunner
   script:
   - make --version
```

### Comparing `octomy-common-1.0.9/PKG-INFO` & `octomy-common-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,141 @@
-Metadata-Version: 2.1
-Name: octomy-common
-Version: 1.0.9
-Summary: OctoMY common
-Home-page: https://gitlab.com/octomy/common
-Author: Lennart Rolland
-Author-email: lennart@octomy.org
-Maintainer: Lennart Rolland
-Maintainer-email: lennart@octomy.org
-License: GPL-3 LGPL-3 MIT
-Description: [![pipeline  status](https://gitlab.com/octomy/common/badges/production/pipeline.svg)](https://gitlab.com/octomy/common/-/commits/production)
-        
-        #  About  common
-        <img  src="https://gitlab.com/octomy/common/-/raw/production/design/logo-1024.png"  width="20%"/>
-        
-        This pypi package contains common  files  for  octomy  python  projects
-        
-        -  Common  is  [available  on  gitlab](https://gitlab.com/octomy/common).
-        
-        -  Common  is  [available  in  PyPI](https://pypi.org/project/common/).
-         
-        
-        ```shell
-        
-        #  Clone  git  repository
-        
-        git  clone  git@gitlab.com:octomy/common.git
-        ```
-        
-        ```shell
-        #  Install  package  into  your  current  Python  environment
-        pip  install  octomy-common
-        ```
-        
-        # Versioning
-        
-        In this section the versioning scheme used for all octomy codebases will be explained.
-        
-        First of, we strive to follow [semver](https://semver.org/) as far as possible, so any details pertaining to the actual version numbers themselves is better explained in the semver spec. This documentation refers to how we store, change and update the version number in the project itself, and how that version number is propagated from source to build artifacts such as PyPi packages, Docker images and more.
-        
-        ## Source of version number
-        
-        The source of the version number shall be a one line, plain-text file in the root of the project simply called [VERSION](VERSION)
-        
-        This should contain the full version number on semver format and nothing else. Example versions are:
-        
-        * 0.0.1
-        * 0.1.3
-        * 1.0.0
-        * 2.2.12
-        > NOTE: There should not be any prefixes or postfixes in this version. No "rc", "beta" as this is handled by the logic as described below.
-        
-        ## git branches
-        
-        We will operate with 3 protected git branches. The rules that govern them are as follows:
-        
-        | Branch | Description |
-        | --------------- |--------------------------|
-        | production      | This corresponds to what is in production right now. Using CI/CD, anything merged to this branch will immediately be built and deployed in production, replacing whatever was in production before |
-        | beta      | This corresponds to what is in the beta environment right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the beta environment, replacing whatever was in that environment before. Beta means an almost ready "next version" that is ready to preview for a selection of customers. |
-        | stage-_XXX_      | This corresponds to what is in the stage environment labelled _XXX_ right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the  stage-_XXX_ environment, replacing whatever was in that environment before. Please note that the _XXX_ could be any string, you may have several stage environments labelled as you see fit. Typically you will have a stage set up for a private presentation to a select client, or for internal testing. |
-        | *      | Any other branch is considered unprotected and may be built and tested using CI/CD, but will not be considered for any automatic deployment. When built and deployed manually, these branches will have `test-`prepended to them for easy identification. |
-        
-        
-        ## PyPi packages
-        
-        PyPi package names are on the form `project_name`-`version`-`branch_name`. The branch name is omitted for "production" giving simply `project_name`-`version` in that case. Further, any branch name starting with `stage-` will have the `stage-` part removed. And finally, any branch that is not production, beta or stage-X will have `test-`prepended to the branch name itself, so it becomes  `project_name`-`version`-test-`branch_name`.
-        
-        ## Docker images
-        
-        Docker images are named `project_name` and tagged with `branch_name`-`version`. The branch name is omitted for "production" giving simply `version` in that case. Further, any branch name starting with `stage-` will have the `stage-` part removed. And finally, any branch that is not production, beta or stage-X will have `test-`prepended to the branch name itself, so it becomes  `version`-test-`branch_name`.
-        
-        ## Examples
-        
-        * Example project name: __my_project__
-        * Example version: __1.2.3__
-        * Example stage name: __my_presentation__
-        
-        | git branch name | Docker image             | PyPi package             |
-        | --------------- |--------------------------| -------------------------|
-        | `production`      | my_project:_1.2.3_         | my_project-_1.2.3_         |
-        | `beta`            | my_project:_1.2.3_-`beta`    | my_project-_1.2.3_-`beta`    |
-        | `stage-my_presentation` | my_project:_1.2.3_-`my_presentation` | my_project-_1.2.3_-`my_presentation` |
-        | `silly_branch` | my_project:_1.2.3_-__test__-`silly_branch` | my_project-_1.2.3_-__test__-`silly_branch` |
-        
-        ## Implementation
-        
-        To maintain this versioning, we depend on a few tools for the logic:
-        
-        1. bash
-        2. make
-        3. setup.py (Python)
-        
-        Each octomy project will have a [Makefile](Makefile) in the root of the project that has targets for building and pushing pypi and/or Docker images. It [specifies bash as the shell](https://www.gnu.org/software/make/manual/html_node/Choosing-the-Shell.html) to use, and use [bash string manipulation and conditions](https://www.gnu.org/software/bash/manual/bash.html) to generate the correct version string following the rules above for Docker tags. Further, the rules are implemented as a function in setup.py to satisfy the rules when building pypi package.
-        
-        The Makefile targets are named as follows:
-        
-        | make target     | Description                                                    |
-        | --------------- |----------------------------------------------------------------|
-        | docker-build    | Build the docker image with correct version tags               |
-        | docker-push     | Push the docker image with correct version tags to registry    |
-        | pypi-build      | Build the pypi package with correct version                    |
-        | pypi-push       | Push the pypi package with correct version to PyPi repository  |
-        
-        ## Example implementation
-        
-        This project will follow the rules above and will contain the Makefile targets that can be used as a reference for other projects.
-Keywords: octomy common
-Platform: Linux
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: Topic :: Utilities
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.7.4
-Description-Content-Type: text/markdown
+[![pipeline  status](https://gitlab.com/octomy/common/badges/production/pipeline.svg)](https://gitlab.com/octomy/common/-/commits/production)
+
+<!---
+                                                         
+                                                         
+     ## ## ## ## ## ## ## ## ## ## ##                    
+        ## ## ## ## ## ## ## ## ##                       
+           ## ## ## ## ## ## ##                          
+              ## ## ## ## ##                             
+                 ## ## ##                                
+                    ##                                   
+                                                         
+                                                         
+WARNING: This file is AUTO GENERATED from "resources/templates/README.md".
+         Any changes you make will be OVERWRITTEN at the 
+         next invocation of `make readme`                
+                                                         
+                                                         
+                    ##                                   
+                 ## ## ##                                
+              ## ## ## ## ##                             
+           ## ## ## ## ## ## ##                          
+        ## ## ## ## ## ## ## ## ##                       
+     ## ## ## ## ## ## ## ## ## ## ##                    
+                                                         
+                                                         
+-->
+
+#  Practical details
+<img  src="https://gitlab.com/octomy/common/-/raw/production/resources/iamges/logos/1024.svg"  width="20%"/>
+
+This is the common project version 1.0.47
+
+- common is [available  on  gitlab](https://gitlab.com/octomy/common).
+- common is [available as private Docker image](https://gitlab.com/octomy/common/container_registry).
+
+
+```shell
+#  Clone  git  repository
+git  clone  git@gitlab.com:octomy/common.git
+```
+
+```shell
+# Pull image from Docker registry
+docker pull registry.gitlab.com/octomy/common
+
+```
+
+
+# What is common?
+
+common is a pypi package that contains common  files  for  OctoMY™ Python projects.
+
+
+```shell
+
+#  Clone  git  repository
+
+git  clone  git@gitlab.com:octomy/common.git
+```
+
+```shell
+#  Install  package  into  your  current  Python  environment
+pip  install  octomy-common
+```
+
+# Versioning
+
+In this section the versioning scheme used for all octomy codebases will be explained.
+
+First of, we strive to follow [semver](https://semver.org/) as far as possible, so any details pertaining to the actual version numbers themselves is better explained in the semver spec. This documentation refers to how we store, change and update the version number in the project itself, and how that version number is propagated from source to build artifacts such as PyPi packages, Docker images and more.
+
+## Source of version number
+
+The source of the version number shall be a one line, plain-text file in the root of the project simply called [VERSION](VERSION)
+
+This should contain the full version number on semver format and nothing else. Example versions are:
+
+* 0.0.1
+* 0.1.3
+* 1.0.0
+* 2.2.12
+> NOTE: There should not be any prefixes or postfixes in this version. No "rc", "beta" as this is handled by the logic as described below.
+
+## git branches
+
+We will operate with 3 protected git branches. The rules that govern them are as follows:
+
+| Branch | Description |
+| --------------- |--------------------------|
+| production      | This corresponds to what is in production right now. Using CI/CD, anything merged to this branch will immediately be built and deployed in production, replacing whatever was in production before |
+| beta      | This corresponds to what is in the beta environment right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the beta environment, replacing whatever was in that environment before. Beta means an almost ready "next version" that is ready to preview for a selection of customers. |
+| stage-_XXX_      | This corresponds to what is in the stage environment labelled _XXX_ right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the  stage-_XXX_ environment, replacing whatever was in that environment before. Please note that the _XXX_ could be any string, you may have several stage environments labelled as you see fit. Typically you will have a stage set up for a private presentation to a select client, or for internal testing. |
+| *      | Any other branch is considered unprotected and may be built and tested using CI/CD, but will not be considered for any automatic deployment. When built and deployed manually, these branches will have `test-`prepended to them for easy identification. |
+
+
+## PyPi packages
+
+PyPi package names are on the form `project_name`-`version` The branch name is omitted entirely and it is expected that PyPi packages are deployed only for the production branch.
+
+## Docker images
+
+Docker images are named `project_name` and tagged with `branch_name`-`version`. The branch name is omitted for "production" giving simply `version` in that case. Further, any branch name starting with `stage-` will have the `stage-` part removed. And finally, any branch that is not production, beta or stage-X will have `test-`prepended to the branch name itself, so it becomes  `version`-test-`branch_name`.
+
+## Examples
+
+* Example project name: __my_project__
+* Example version: __1.2.3__
+* Example stage name: __my_presentation__
+
+| git branch name         | Docker image                               | PyPi package             |
+| ----------------------- |--------------------------------------------| -------------------------|
+| `production`            | my_project:_1.2.3_                         | my_project-_1.2.3_       |
+| `beta`                  | my_project:_1.2.3_-`beta`                  | N/A                      |
+| `stage-my_presentation` | my_project:_1.2.3_-`my_presentation`       | N/A                      |
+| `silly_branch`          | my_project:_1.2.3_-__test__-`silly_branch` | N/A                      |
+
+## Implementation
+
+To maintain this versioning, we depend on a few tools for the logic:
+
+1. bash
+2. make
+3. setup.py (Python)
+
+Each octomy project will have a [Makefile](Makefile) in the root of the project that has targets for building and pushing pypi and/or Docker images. It [specifies bash as the shell](https://www.gnu.org/software/make/manual/html_node/Choosing-the-Shell.html) to use, and use [bash string manipulation and conditions](https://www.gnu.org/software/bash/manual/bash.html) to generate the correct version string following the rules above for Docker tags. Further, the rules are implemented as a function in setup.py to satisfy the rules when building pypi package.
+
+The Makefile targets are named as follows:
+
+| make target     | Description                                                    |
+| --------------- |----------------------------------------------------------------|
+| docker-build    | Build the docker image with correct version tags               |
+| docker-push     | Push the docker image with correct version tags to registry    |
+| pypi-build      | Build the pypi package with correct version                    |
+| pypi-push       | Push the pypi package with correct version to PyPi repository. NOTE: Should only be called for production branch  |
+
+## Example implementation
+
+This octomy-common project will follow the rules above and will contain the Makefile targets that can be used as a reference for other projects.
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `octomy-common-1.0.9/code_quality/Makefile` & `octomy-common-2.0.0/code_quality/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -36,22 +36,35 @@
 	flake8 --select=F403 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
 	flake8 --select=F821 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
 	flake8 --select=F841 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
 	flake8 --select=W0107 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
 	flake8 --select=W0706 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
 	flake8 --select=W0105 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
 
+unused:
+	flake8 --select=F401 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
+
+undefined:
+	flake8 --select=F821 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
+
+space:
+	flake8 --select=E101 --max-complexity 10 --exclude build,junk --exit-zero "${APP_DIR}"
+
 ############### Help ####################
 
 help:
 	@echo ""
 	@echo " Available targets:"
 	@echo ""
 	@echo " + make help          Show this help"
 	@echo " + make all           Run all targets"
+	@echo " + make black         Run black"
 	@echo " + make flake         Run flake"
 	@echo " + make mypy          Run mypy"
 	@echo " + make pylint        Run pylint"
 	@echo " + make coverage      Run coverage"
-	@echo " + make black         Run black"
+	@echo " + make low-hanging   Run flake with most low-hanging warnings only"
+	@echo " + make unused        Run flake with unused warnings only"
+	@echo " + make undefined     Run flake with undefined warnings only"
+	@echo " + make space         Run flake with space warnings only"
 	@echo ""
```

### Comparing `octomy-common-1.0.9/code_quality/pylintrc` & `octomy-common-2.0.0/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-common-1.0.9/design/logo-1024.png` & `octomy-common-2.0.0/design/logo-1024.png`

 * *Files identical despite different names*

### Comparing `octomy-common-1.0.9/design/logo-1024.svg` & `octomy-common-2.0.0/design/logo-1024.svg`

 * *Files identical despite different names*

### Comparing `octomy-common-1.0.9/fk/log/__init__.py` & `octomy-common-2.0.0/octomy/log/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 import inspect
 import warnings
 
 log_setup_once = False
 
 
 def setup_logging(name=None, log_level=logging.INFO):
-    """Set up logging."""
-    global log_setup_once
-    if not log_setup_once:
-        log_setup_once = True
-        logging.basicConfig(level=log_level)
-        fmt = "%(asctime)s %(levelname)s (%(threadName)s) [%(name)s:%(lineno)s::%(funcName)s()] - %(message)s"
-        colorfmt = "%(log_color)s{}%(reset)s".format(fmt)
-        datefmt = "%Y-%m-%d %H:%M:%S"
-
-        # Suppress overly verbose output that isn't helpful from some libraries we depend on
-        for key in ["requests", "tensorboard", "urllib3", "aiohttp.access", "uamqp", "sqlalchemy", "sqlalchemy.engine.base", "matplotlib.font_manager"]:
-            logging.getLogger(key).setLevel(logging.WARNING)
-
-        # Enable debug logging for some insteresting libraries (for development)
-        logging.getLogger("fk").setLevel(logging.DEBUG)
-
-        try:
-            from colorlog import ColoredFormatter
-
-            logging.getLogger().handlers[0].setFormatter(ColoredFormatter(colorfmt, datefmt=datefmt, reset=True, log_colors={"DEBUG": "cyan", "INFO": "green", "WARNING": "yellow", "ERROR": "red", "CRITICAL": "red"}))
-        except ImportError:
-            # Ignore failures in loading color coded logs
-            pass
-
-        # Set this log level as default
-        logger = logging.getLogger("")
-        logger.setLevel(log_level)
-    if not name:
-        name = inspect.stack()[1][1]
-    logger = logging.getLogger(name)
-    try:
-        import colored_traceback.auto
-    except ImportError:
-        pass
+	"""Set up logging."""
+	global log_setup_once
+	if not log_setup_once:
+		log_setup_once = True
+		logging.basicConfig(level=log_level)
+		fmt = "%(asctime)s %(levelname)s (%(threadName)s) [%(name)s:%(lineno)s::%(funcName)s()] - %(message)s"
+		colorfmt = "%(log_color)s{}%(reset)s".format(fmt)
+		datefmt = "%Y-%m-%d %H:%M:%S"
+
+		# Suppress overly verbose output that isn't helpful from some libraries we depend on
+		for key in ["requests", "tensorboard", "urllib3", "aiohttp.access", "uamqp", "sqlalchemy", "sqlalchemy.engine.base", "matplotlib.font_manager"]:
+			logging.getLogger(key).setLevel(logging.WARNING)
+
+		# Enable debug logging for some insteresting libraries (for development)
+		logging.getLogger("fk").setLevel(logging.DEBUG)
+
+		try:
+			from colorlog import ColoredFormatter
+
+			logging.getLogger().handlers[0].setFormatter(ColoredFormatter(colorfmt, datefmt=datefmt, reset=True, log_colors={"DEBUG": "cyan", "INFO": "green", "WARNING": "yellow", "ERROR": "red", "CRITICAL": "red"}))
+		except ImportError:
+			# Ignore failures in loading color coded logs
+			pass
+
+		# Set this log level as default
+		logger = logging.getLogger("")
+		logger.setLevel(log_level)
+	if not name:
+		name = inspect.stack()[1][1]
+	logger = logging.getLogger(name)
+	try:
+		import colored_traceback.auto
+	except ImportError:
+		pass
 
-    return logger
+	return logger
```

### Comparing `octomy-common-1.0.9/fk/utils/Watchdog.py` & `octomy-common-2.0.0/octomy/utils/Watchdog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from threading import Timer
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class Watchdog(BaseException):
-    def __init__(self, timeout, userHandler=None):  # timeout in seconds
-        self.timeout = timeout
-        # logger.info(f"WATCHDOG SET WITH TIME {self.timeout}")
-        self.handler = userHandler if userHandler is not None else self.defaultHandler
-        self.timer = Timer(self.timeout, self.handler)
-        self.timer.start()
-
-    def reset(self):
-        self.timer.cancel()
-        self.timer = Timer(self.timeout, self.handler)
-        self.timer.start()
-
-    def stop(self):
-        # logger.info(f"WATCHDOG STOPPED")
-        self.timer.cancel()
-
-    def defaultHandler(self):
-        logger.info("WATCHDOG TIMED OUT")
-        raise self
+	def __init__(self, timeout, userHandler=None):  # timeout in seconds
+		self.timeout = timeout
+		# logger.info(f"WATCHDOG SET WITH TIME {self.timeout}")
+		self.handler = userHandler if userHandler is not None else self.defaultHandler
+		self.timer = Timer(self.timeout, self.handler)
+		self.timer.start()
+
+	def reset(self):
+		self.timer.cancel()
+		self.timer = Timer(self.timeout, self.handler)
+		self.timer.start()
+
+	def stop(self):
+		# logger.info(f"WATCHDOG STOPPED")
+		self.timer.cancel()
+
+	def defaultHandler(self):
+		logger.info("WATCHDOG TIMED OUT")
+		raise self
```

### Comparing `octomy-common-1.0.9/fk/utils/click.py` & `octomy-common-2.0.0/octomy/utils/click.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import datetime
 import math
 from time import sleep
 
-from fk.utils import human_delta
+from octomy.utils import human_delta
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class OnTheClockTimer:
-    """
-    Class to provide a schedule from time of day + recurring interval as starting point
-    Also provides convenience methods to make it easy to keep track of this schedule
-    """
-
-    def __init__(self, start_time: datetime.time, interval: datetime.timedelta):
-        self.start_time = start_time
-        self.interval = interval
-
-    def closest_start_time(self, now: datetime.datetime = datetime.datetime.now()) -> datetime.datetime:
-        time_of_day = now.time()
-        common_date = datetime.date(2019, 1, 1)
-        p1 = datetime.datetime.combine(common_date, time_of_day)
-        p2 = datetime.datetime.combine(common_date, self.start_time)
-        from_start = p1 - p2
-        interval_count = from_start / self.interval
-        next_time = (math.floor(interval_count) + 1) * self.interval
-        # logger.info(f"DATE: {now.date()}, TIME:{now.time()}, from_start:{from_start}, interval_count:{interval_count}, last_time={last_time}, next_time={next_time}")
-        return datetime.datetime.combine(now.date(), self.start_time) + next_time
-
-    def time_left(self, now: datetime.datetime = datetime.datetime.now()) -> datetime.timedelta:
-        return self.closest_start_time(now=now) - now
-
-    def wait_for_trigger(self, now: datetime.datetime = datetime.datetime.now()):
-        iv = self.time_left(now=now)
-        sec = iv.total_seconds()
-        if sec > 0:
-            logger.info(f"Waiting for {human_delta(iv)}")
-            sleep(sec)
-        return True
+	"""
+	Class to provide a schedule from time of day + recurring interval as starting point
+	Also provides convenience methods to make it easy to keep track of this schedule
+	"""
+
+	def __init__(self, start_time: datetime.time, interval: datetime.timedelta):
+		self.start_time = start_time
+		self.interval = interval
+
+	def closest_start_time(self, now: datetime.datetime = datetime.datetime.now()) -> datetime.datetime:
+		time_of_day = now.time()
+		common_date = datetime.date(2019, 1, 1)
+		p1 = datetime.datetime.combine(common_date, time_of_day)
+		p2 = datetime.datetime.combine(common_date, self.start_time)
+		from_start = p1 - p2
+		interval_count = from_start / self.interval
+		next_time = (math.floor(interval_count) + 1) * self.interval
+		# logger.info(f"DATE: {now.date()}, TIME:{now.time()}, from_start:{from_start}, interval_count:{interval_count}, last_time={last_time}, next_time={next_time}")
+		return datetime.datetime.combine(now.date(), self.start_time) + next_time
+
+	def time_left(self, now: datetime.datetime = datetime.datetime.now()) -> datetime.timedelta:
+		return self.closest_start_time(now=now) - now
+
+	def wait_for_trigger(self, now: datetime.datetime = datetime.datetime.now()):
+		iv = self.time_left(now=now)
+		sec = iv.total_seconds()
+		if sec > 0:
+			logger.info(f"Waiting for {human_delta(iv)}")
+			sleep(sec)
+		return True
 
-    def __str__(self):
-        return f"OnTheClockTimer(start_time={self.start_time}, interval={self.interval})"
+	def __str__(self):
+		return f"OnTheClockTimer(start_time={self.start_time}, interval={self.interval})"
```

### Comparing `octomy-common-1.0.9/fk/utils/csv_to_db.py` & `octomy-common-2.0.0/octomy/utils/csv_to_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,57 +19,57 @@
 # 	csv_reader = csv.reader(utf8_data, dialect=dialect, **kwargs)
 # 	for row in csv_reader:
 # 		yield [unicode(cell, 'ISO-8859-1') for cell in row]
 
 
 # Main entrypoint of script
 if __name__ == "__main__":
-    # Change current working dir to that of this script's location
-    cwd = os.path.dirname(os.path.realpath(__file__))
-    os.chdir(cwd)
-    print("Set working dir to " + cwd)
-
-    # Load credentials
-    credentials = credentials.load_credentials()
-    if not credentials:
-        sys.exit(1)
-
-    print("#############################################################################")
-
-    db = Database(credentials)
-
-    # File containting one shop name per line
-    oh_no_fn = "oh_no.csv"
-
-    # reader = unicode_csv_reader(open(oh_no_fn))
-
-    # for site_id in reader:		print(site_id)
-
-    map = {"Comment": "comment", "Api Key": "api_key", "Created At": "created_at", "Fetched At": "fetched_at", "Fetched Count": "fetched_count", "Link": "link", "Sale Date First": "sale_date_first", "Sale Date First Ever": "sale_date_first_ever", "Sale Date Last": "sale_date_last", "Site Id": "site_id", "Spread": "spread"}
-
-    # sys.exit(1)
-    with open(oh_no_fn) as csv_file:
-        csv_reader = csv.reader(csv_file, delimiter="\t")
-        line_count = 0
-        headers = []
-        for row in csv_reader:
-            if line_count == 10:
-                # break
-                pass
-            if line_count == 0:
-                print(f'Column names are {", ".join(row)}')
-                headers = row
-                line_count += 1
-            else:
-                spop = {}
-                for index, header in enumerate(headers):
-                    h = map.get(header, header)
-                    v = row[index]
-                    if v == "":
-                        v = None
-                    elif h.startswith("sale_date_"):
-                        v = datetime.datetime(v)
-                    spop[h] = v
-                i = db.upsert_spop_id(spop)
-                # print(f"LINE:{spop} ---> {i}")
-                line_count += 1
-        print(f"Processed {line_count} lines.")
+	# Change current working dir to that of this script's location
+	cwd = os.path.dirname(os.path.realpath(__file__))
+	os.chdir(cwd)
+	print("Set working dir to " + cwd)
+
+	# Load credentials
+	credentials = credentials.load_credentials()
+	if not credentials:
+		sys.exit(1)
+
+	print("#############################################################################")
+
+	db = Database(credentials)
+
+	# File containting one shop name per line
+	oh_no_fn = "oh_no.csv"
+
+	# reader = unicode_csv_reader(open(oh_no_fn))
+
+	# for site_id in reader:		print(site_id)
+
+	map = {"Comment": "comment", "Api Key": "api_key", "Created At": "created_at", "Fetched At": "fetched_at", "Fetched Count": "fetched_count", "Link": "link", "Sale Date First": "sale_date_first", "Sale Date First Ever": "sale_date_first_ever", "Sale Date Last": "sale_date_last", "Site Id": "site_id", "Spread": "spread"}
+
+	# sys.exit(1)
+	with open(oh_no_fn) as csv_file:
+		csv_reader = csv.reader(csv_file, delimiter="\t")
+		line_count = 0
+		headers = []
+		for row in csv_reader:
+			if line_count == 10:
+				# break
+				pass
+			if line_count == 0:
+				print(f'Column names are {", ".join(row)}')
+				headers = row
+				line_count += 1
+			else:
+				spop = {}
+				for index, header in enumerate(headers):
+					h = map.get(header, header)
+					v = row[index]
+					if v == "":
+						v = None
+					elif h.startswith("sale_date_"):
+						v = datetime.datetime(v)
+					spop[h] = v
+				i = db.upsert_spop_id(spop)
+				# print(f"LINE:{spop} ---> {i}")
+				line_count += 1
+		print(f"Processed {line_count} lines.")
```

### Comparing `octomy-common-1.0.9/fk/utils/debug_view.py` & `octomy-common-2.0.0/octomy/utils/debug_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 
 # return debugger(request, session, "Install page", permission_url)
 # return debugger(request, session, pprint.pformat(shop), redirect_url)
 # return debugger(request, session, "Main page", redirect_url)
 
 
 def debugger(request, session, message, link):
-    return render_template("shopify_bp/debugger.html", request=pprint.pformat(request.__dict__, 1, 2400), session=pprint.pformat(dict(session)), message=message, link=link)
+	return render_template("shopify_bp/debugger.html", request=pprint.pformat(request.__dict__, 1, 2400), session=pprint.pformat(dict(session)), message=message, link=link)
```

### Comparing `octomy-common-1.0.9/octomy_common.egg-info/PKG-INFO` & `octomy-common-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,119 +1,166 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 1.0.9
-Summary: OctoMY common
+Version: 2.0.0
+Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
-Author: Lennart Rolland
-Author-email: lennart@octomy.org
-Maintainer: Lennart Rolland
-Maintainer-email: lennart@octomy.org
-License: GPL-3 LGPL-3 MIT
-Description: [![pipeline  status](https://gitlab.com/octomy/common/badges/production/pipeline.svg)](https://gitlab.com/octomy/common/-/commits/production)
-        
-        #  About  common
-        <img  src="https://gitlab.com/octomy/common/-/raw/production/design/logo-1024.png"  width="20%"/>
-        
-        This pypi package contains common  files  for  octomy  python  projects
-        
-        -  Common  is  [available  on  gitlab](https://gitlab.com/octomy/common).
-        
-        -  Common  is  [available  in  PyPI](https://pypi.org/project/common/).
-         
-        
-        ```shell
-        
-        #  Clone  git  repository
-        
-        git  clone  git@gitlab.com:octomy/common.git
-        ```
-        
-        ```shell
-        #  Install  package  into  your  current  Python  environment
-        pip  install  octomy-common
-        ```
-        
-        # Versioning
-        
-        In this section the versioning scheme used for all octomy codebases will be explained.
-        
-        First of, we strive to follow [semver](https://semver.org/) as far as possible, so any details pertaining to the actual version numbers themselves is better explained in the semver spec. This documentation refers to how we store, change and update the version number in the project itself, and how that version number is propagated from source to build artifacts such as PyPi packages, Docker images and more.
-        
-        ## Source of version number
-        
-        The source of the version number shall be a one line, plain-text file in the root of the project simply called [VERSION](VERSION)
-        
-        This should contain the full version number on semver format and nothing else. Example versions are:
-        
-        * 0.0.1
-        * 0.1.3
-        * 1.0.0
-        * 2.2.12
-        > NOTE: There should not be any prefixes or postfixes in this version. No "rc", "beta" as this is handled by the logic as described below.
-        
-        ## git branches
-        
-        We will operate with 3 protected git branches. The rules that govern them are as follows:
-        
-        | Branch | Description |
-        | --------------- |--------------------------|
-        | production      | This corresponds to what is in production right now. Using CI/CD, anything merged to this branch will immediately be built and deployed in production, replacing whatever was in production before |
-        | beta      | This corresponds to what is in the beta environment right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the beta environment, replacing whatever was in that environment before. Beta means an almost ready "next version" that is ready to preview for a selection of customers. |
-        | stage-_XXX_      | This corresponds to what is in the stage environment labelled _XXX_ right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the  stage-_XXX_ environment, replacing whatever was in that environment before. Please note that the _XXX_ could be any string, you may have several stage environments labelled as you see fit. Typically you will have a stage set up for a private presentation to a select client, or for internal testing. |
-        | *      | Any other branch is considered unprotected and may be built and tested using CI/CD, but will not be considered for any automatic deployment. When built and deployed manually, these branches will have `test-`prepended to them for easy identification. |
-        
-        
-        ## PyPi packages
-        
-        PyPi package names are on the form `project_name`-`version`-`branch_name`. The branch name is omitted for "production" giving simply `project_name`-`version` in that case. Further, any branch name starting with `stage-` will have the `stage-` part removed. And finally, any branch that is not production, beta or stage-X will have `test-`prepended to the branch name itself, so it becomes  `project_name`-`version`-test-`branch_name`.
-        
-        ## Docker images
-        
-        Docker images are named `project_name` and tagged with `branch_name`-`version`. The branch name is omitted for "production" giving simply `version` in that case. Further, any branch name starting with `stage-` will have the `stage-` part removed. And finally, any branch that is not production, beta or stage-X will have `test-`prepended to the branch name itself, so it becomes  `version`-test-`branch_name`.
-        
-        ## Examples
-        
-        * Example project name: __my_project__
-        * Example version: __1.2.3__
-        * Example stage name: __my_presentation__
-        
-        | git branch name | Docker image             | PyPi package             |
-        | --------------- |--------------------------| -------------------------|
-        | `production`      | my_project:_1.2.3_         | my_project-_1.2.3_         |
-        | `beta`            | my_project:_1.2.3_-`beta`    | my_project-_1.2.3_-`beta`    |
-        | `stage-my_presentation` | my_project:_1.2.3_-`my_presentation` | my_project-_1.2.3_-`my_presentation` |
-        | `silly_branch` | my_project:_1.2.3_-__test__-`silly_branch` | my_project-_1.2.3_-__test__-`silly_branch` |
-        
-        ## Implementation
-        
-        To maintain this versioning, we depend on a few tools for the logic:
-        
-        1. bash
-        2. make
-        3. setup.py (Python)
-        
-        Each octomy project will have a [Makefile](Makefile) in the root of the project that has targets for building and pushing pypi and/or Docker images. It [specifies bash as the shell](https://www.gnu.org/software/make/manual/html_node/Choosing-the-Shell.html) to use, and use [bash string manipulation and conditions](https://www.gnu.org/software/bash/manual/bash.html) to generate the correct version string following the rules above for Docker tags. Further, the rules are implemented as a function in setup.py to satisfy the rules when building pypi package.
-        
-        The Makefile targets are named as follows:
-        
-        | make target     | Description                                                    |
-        | --------------- |----------------------------------------------------------------|
-        | docker-build    | Build the docker image with correct version tags               |
-        | docker-push     | Push the docker image with correct version tags to registry    |
-        | pypi-build      | Build the pypi package with correct version                    |
-        | pypi-push       | Push the pypi package with correct version to PyPi repository  |
-        
-        ## Example implementation
-        
-        This project will follow the rules above and will contain the Makefile targets that can be used as a reference for other projects.
-Keywords: octomy common
+Author: OctoMY
+Author-email: pypi@octomy.org
+Maintainer: OctoMY
+Maintainer-email: pypi@octomy.org
+License: Proprietary Software License
+Keywords: software
 Platform: Linux
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.7.4
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![pipeline  status](https://gitlab.com/octomy/common/badges/production/pipeline.svg)](https://gitlab.com/octomy/common/-/commits/production)
+
+<!---
+                                                         
+                                                         
+     ## ## ## ## ## ## ## ## ## ## ##                    
+        ## ## ## ## ## ## ## ## ##                       
+           ## ## ## ## ## ## ##                          
+              ## ## ## ## ##                             
+                 ## ## ##                                
+                    ##                                   
+                                                         
+                                                         
+WARNING: This file is AUTO GENERATED from "resources/templates/README.md".
+         Any changes you make will be OVERWRITTEN at the 
+         next invocation of `make readme`                
+                                                         
+                                                         
+                    ##                                   
+                 ## ## ##                                
+              ## ## ## ## ##                             
+           ## ## ## ## ## ## ##                          
+        ## ## ## ## ## ## ## ## ##                       
+     ## ## ## ## ## ## ## ## ## ## ##                    
+                                                         
+                                                         
+-->
+
+#  Practical details
+<img  src="https://gitlab.com/octomy/common/-/raw/production/resources/iamges/logos/1024.svg"  width="20%"/>
+
+This is the common project version 1.0.47
+
+- common is [available  on  gitlab](https://gitlab.com/octomy/common).
+- common is [available as private Docker image](https://gitlab.com/octomy/common/container_registry).
+
+
+```shell
+#  Clone  git  repository
+git  clone  git@gitlab.com:octomy/common.git
+```
+
+```shell
+# Pull image from Docker registry
+docker pull registry.gitlab.com/octomy/common
+
+```
+
+
+# What is common?
+
+common is a pypi package that contains common  files  for  OctoMY™ Python projects.
+
+
+```shell
+
+#  Clone  git  repository
+
+git  clone  git@gitlab.com:octomy/common.git
+```
+
+```shell
+#  Install  package  into  your  current  Python  environment
+pip  install  octomy-common
+```
+
+# Versioning
+
+In this section the versioning scheme used for all octomy codebases will be explained.
+
+First of, we strive to follow [semver](https://semver.org/) as far as possible, so any details pertaining to the actual version numbers themselves is better explained in the semver spec. This documentation refers to how we store, change and update the version number in the project itself, and how that version number is propagated from source to build artifacts such as PyPi packages, Docker images and more.
+
+## Source of version number
+
+The source of the version number shall be a one line, plain-text file in the root of the project simply called [VERSION](VERSION)
+
+This should contain the full version number on semver format and nothing else. Example versions are:
+
+* 0.0.1
+* 0.1.3
+* 1.0.0
+* 2.2.12
+> NOTE: There should not be any prefixes or postfixes in this version. No "rc", "beta" as this is handled by the logic as described below.
+
+## git branches
+
+We will operate with 3 protected git branches. The rules that govern them are as follows:
+
+| Branch | Description |
+| --------------- |--------------------------|
+| production      | This corresponds to what is in production right now. Using CI/CD, anything merged to this branch will immediately be built and deployed in production, replacing whatever was in production before |
+| beta      | This corresponds to what is in the beta environment right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the beta environment, replacing whatever was in that environment before. Beta means an almost ready "next version" that is ready to preview for a selection of customers. |
+| stage-_XXX_      | This corresponds to what is in the stage environment labelled _XXX_ right now. Using CI/CD, anything merged to this branch will immediately be built and deployed into the  stage-_XXX_ environment, replacing whatever was in that environment before. Please note that the _XXX_ could be any string, you may have several stage environments labelled as you see fit. Typically you will have a stage set up for a private presentation to a select client, or for internal testing. |
+| *      | Any other branch is considered unprotected and may be built and tested using CI/CD, but will not be considered for any automatic deployment. When built and deployed manually, these branches will have `test-`prepended to them for easy identification. |
+
+
+## PyPi packages
+
+PyPi package names are on the form `project_name`-`version` The branch name is omitted entirely and it is expected that PyPi packages are deployed only for the production branch.
+
+## Docker images
+
+Docker images are named `project_name` and tagged with `branch_name`-`version`. The branch name is omitted for "production" giving simply `version` in that case. Further, any branch name starting with `stage-` will have the `stage-` part removed. And finally, any branch that is not production, beta or stage-X will have `test-`prepended to the branch name itself, so it becomes  `version`-test-`branch_name`.
+
+## Examples
+
+* Example project name: __my_project__
+* Example version: __1.2.3__
+* Example stage name: __my_presentation__
+
+| git branch name         | Docker image                               | PyPi package             |
+| ----------------------- |--------------------------------------------| -------------------------|
+| `production`            | my_project:_1.2.3_                         | my_project-_1.2.3_       |
+| `beta`                  | my_project:_1.2.3_-`beta`                  | N/A                      |
+| `stage-my_presentation` | my_project:_1.2.3_-`my_presentation`       | N/A                      |
+| `silly_branch`          | my_project:_1.2.3_-__test__-`silly_branch` | N/A                      |
+
+## Implementation
+
+To maintain this versioning, we depend on a few tools for the logic:
+
+1. bash
+2. make
+3. setup.py (Python)
+
+Each octomy project will have a [Makefile](Makefile) in the root of the project that has targets for building and pushing pypi and/or Docker images. It [specifies bash as the shell](https://www.gnu.org/software/make/manual/html_node/Choosing-the-Shell.html) to use, and use [bash string manipulation and conditions](https://www.gnu.org/software/bash/manual/bash.html) to generate the correct version string following the rules above for Docker tags. Further, the rules are implemented as a function in setup.py to satisfy the rules when building pypi package.
+
+The Makefile targets are named as follows:
+
+| make target     | Description                                                    |
+| --------------- |----------------------------------------------------------------|
+| docker-build    | Build the docker image with correct version tags               |
+| docker-push     | Push the docker image with correct version tags to registry    |
+| pypi-build      | Build the pypi package with correct version                    |
+| pypi-push       | Push the pypi package with correct version to PyPi repository. NOTE: Should only be called for production branch  |
+
+## Example implementation
+
+This octomy-common project will follow the rules above and will contain the Makefile targets that can be used as a reference for other projects.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `octomy-common-1.0.9/requirements/test_requirements.txt` & `octomy-common-2.0.0/requirements/test_requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,146 +1,168 @@
-#
-# This file is autogenerated by pip-compile
-# To update, run:
-#
-#    pip-compile --output-file=test_requirements.txt temporary_requirements.in
-#
---extra-index-url https://__token__:eyXpjbSx_ySDvQLayXGz@gitlab.com/api/v4/projects/23170380/packages/pypi/simple
-
-appdirs==1.4.3
+appdirs==1.4.4
     # via black
 astroid==2.3.3
     # via pylint
-atomicwrites==1.3.0
-    # via pytest
-attrs==19.3.0
+attrs==20.3.0
     # via
-    #   black
     #   pytest
-black==19.3b0
-    # via -r temporary_requirements.in
-certifi==2020.11.8
+    #   pytest-mypy
+black==20.8b1
+    # via -r test_requirements.in
+certifi==2020.12.5
     # via requests
-chardet==3.0.4
+charset-normalizer==3.2.0
     # via requests
-click==7.1.1
+click==7.1.2
     # via
     #   black
     #   pip-tools
 colored-traceback==0.3.0
-    # via -r temporary_requirements.in
-colorlog==4.1.0
-    # via -r temporary_requirements.in
-coverage==5.0.4
-    # via pytest-cov
-entrypoints==0.3
-    # via flake8
+    # via -r requirements.in
+colorlog==6.7.0
+    # via -r requirements.in
+commonmark==0.9.1
+    # via rich
+coverage[toml]==5.3.1
+    # via
+    #   coverage
+    #   pytest-cov
 filelock==3.0.12
     # via pytest-mypy
-flake8==3.7.9
-    # via -r temporary_requirements.in
+flake8==3.8.4
+    # via -r test_requirements.in
+furl==2.0.0
+    # via -r requirements.in
 idna==2.10
     # via requests
-importlib-metadata==1.5.0
-    # via
-    #   pluggy
-    #   pytest
+importlib-metadata==4.11.3
+    # via pytest-randomly
+iniconfig==1.1.1
+    # via pytest
 isort==4.3.21
     # via pylint
 lazy-object-proxy==1.4.3
     # via astroid
 mccabe==0.6.1
     # via
     #   flake8
     #   pylint
-mock==3.0.5
-    # via -r temporary_requirements.in
-more-itertools==8.2.0
-    # via pytest
-mypy-extensions==0.4.3
-    # via mypy
-mypy==0.770
+mock==4.0.3
+    # via -r test_requirements.in
+mypy==0.790
     # via
-    #   -r temporary_requirements.in
+    #   -r test_requirements.in
     #   pytest-mypy
     #   sqlalchemy-stubs
-packaging==20.3
+mypy-extensions==0.4.3
+    # via
+    #   black
+    #   mypy
+orderedmultidict==1.0.1
+    # via furl
+packaging==20.8
     # via pytest
-pip-tools==4.5.1
-    # via -r temporary_requirements.in
+pathspec==0.8.1
+    # via black
+pip-tools==5.5.0
+    # via -r test_requirements.in
 pluggy==0.13.1
     # via pytest
-psycopg2==2.8.6
-    # via -r temporary_requirements.in
-py3dns==3.2.1
-    # via -r temporary_requirements.in
-py==1.8.1
-    # via pytest
-pycodestyle==2.5.0
+pprintpp==0.4.0
+    # via pytest-clarity
+psycopg[binary,pool]==3.0.18
+    # via
+    #   -r requirements.in
+    #   psycopg
+psycopg-binary==3.0.18
+    # via psycopg
+psycopg-pool==3.1.1
+    # via psycopg
+py==1.10.0
+    # via pytest
+py3dns==4.0.0
+    # via -r requirements.in
+pycodestyle==2.6.0
     # via flake8
-pyflakes==2.1.1
+pyflakes==2.2.0
     # via
     #   flake8
     #   pytest-flakes
 pygments==2.7.4
-    # via colored-traceback
+    # via
+    #   colored-traceback
+    #   rich
 pylint==2.4.2
-    # via -r temporary_requirements.in
-pyparsing==2.4.6
+    # via -r test_requirements.in
+pyparsing==2.4.7
     # via packaging
-pytest-asyncio==0.10.0
-    # via -r temporary_requirements.in
-pytest-cov==2.8.1
-    # via -r temporary_requirements.in
-pytest-flakes==4.0.0
-    # via -r temporary_requirements.in
-pytest-mock==1.13.0
-    # via -r temporary_requirements.in
-pytest-mypy==0.6.0
-    # via -r temporary_requirements.in
-pytest-timeout==1.3.4
-    # via -r temporary_requirements.in
-pytest==4.6.9
+pytest==7.1.0
     # via
-    #   -r temporary_requirements.in
+    #   -r test_requirements.in
     #   pytest-asyncio
+    #   pytest-clarity
     #   pytest-cov
     #   pytest-flakes
     #   pytest-mock
     #   pytest-mypy
+    #   pytest-randomly
     #   pytest-timeout
-python-dateutil==2.8.1
-    # via -r temporary_requirements.in
-pytz==2020.4
-    # via -r temporary_requirements.in
-requests==2.25.0
-    # via -r temporary_requirements.in
-six==1.14.0
+pytest-asyncio==0.18.2
+    # via -r test_requirements.in
+pytest-clarity==1.0.1
+    # via -r test_requirements.in
+pytest-cov==3.0.0
+    # via -r test_requirements.in
+pytest-flakes==4.0.3
+    # via -r test_requirements.in
+pytest-mock==3.7.0
+    # via -r test_requirements.in
+pytest-mypy==0.9.1
+    # via -r test_requirements.in
+pytest-randomly==3.11.0
+    # via -r test_requirements.in
+pytest-timeout==1.4.2
+    # via -r test_requirements.in
+python-dateutil==2.8.2
+    # via -r requirements.in
+pytz==2023.3
+    # via -r requirements.in
+regex==2020.11.13
+    # via black
+requests==2.31.0
+    # via -r requirements.in
+rich==12.0.0
+    # via pytest-clarity
+six==1.15.0
     # via
     #   astroid
-    #   mock
-    #   packaging
-    #   pip-tools
-    #   pytest
+    #   furl
+    #   orderedmultidict
     #   python-dateutil
-sqlalchemy-stubs==0.3
-    # via -r temporary_requirements.in
-toml==0.10.0
-    # via black
-typed-ast==1.4.1
+sqlalchemy-stubs==0.4
+    # via -r test_requirements.in
+toml==0.10.2
     # via
-    #   astroid
+    #   black
+    #   coverage
+tomli==2.0.1
+    # via pytest
+typed-ast==1.4.2
+    # via
+    #   black
     #   mypy
-typing-extensions==3.7.4.1
+typing-extensions==4.7.1
     # via
+    #   black
     #   mypy
     #   sqlalchemy-stubs
 urllib3==1.26.2
     # via requests
 validate-email==1.3
-    # via -r temporary_requirements.in
-wcwidth==0.1.8
-    # via pytest
+    # via -r requirements.in
 wrapt==1.11.2
     # via astroid
-zipp==3.1.0
+zipp==3.4.0
     # via importlib-metadata
+
+# The following packages are considered to be unsafe in a requirements file:
+# pip
```

