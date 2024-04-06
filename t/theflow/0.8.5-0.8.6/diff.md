# Comparing `tmp/theflow-0.8.5.tar.gz` & `tmp/theflow-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theflow-0.8.5.tar", last modified: Tue Jan 30 16:22:32 2024, max compression
+gzip compressed data, was "theflow-0.8.6.tar", last modified: Sat Apr  6 10:52:23 2024, max compression
```

## Comparing `theflow-0.8.5.tar` & `theflow-0.8.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.032600 theflow-0.8.5/
--rw-rw-r--   0 john      (1000) john      (1000)     1073 2023-06-10 17:42:12.000000 theflow-0.8.5/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     5586 2024-01-30 16:22:32.032600 theflow-0.8.5/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     4478 2023-11-19 02:32:04.000000 theflow-0.8.5/README.md
--rw-rw-r--   0 john      (1000) john      (1000)      893 2024-01-30 16:18:58.000000 theflow-0.8.5/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-01-30 16:22:32.032600 theflow-0.8.5/setup.cfg
--rwxrwxr-x   0 john      (1000) john      (1000)       92 2023-09-04 02:39:08.000000 theflow-0.8.5/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.024600 theflow-0.8.5/tests/
--rw-rw-r--   0 john      (1000) john      (1000)     2030 2024-01-01 04:21:06.000000 theflow-0.8.5/tests/test_backends_http_sync.py
--rw-rw-r--   0 john      (1000) john      (1000)     2633 2023-12-19 19:04:09.000000 theflow-0.8.5/tests/test_config.py
--rw-rw-r--   0 john      (1000) john      (1000)     2148 2023-12-23 16:23:17.000000 theflow-0.8.5/tests/test_context.py
--rw-rw-r--   0 john      (1000) john      (1000)      858 2023-09-09 08:40:04.000000 theflow-0.8.5/tests/test_example_notebooks.py
--rw-rw-r--   0 john      (1000) john      (1000)    10536 2024-01-01 04:21:06.000000 theflow-0.8.5/tests/test_function.py
--rw-rw-r--   0 john      (1000) john      (1000)     8659 2023-12-09 12:39:01.000000 theflow-0.8.5/tests/test_function_declaration.py
--rw-rw-r--   0 john      (1000) john      (1000)     1019 2023-12-19 19:04:09.000000 theflow-0.8.5/tests/test_function_multithread.py
--rw-rw-r--   0 john      (1000) john      (1000)     2057 2023-12-09 12:58:49.000000 theflow-0.8.5/tests/test_middleware.py
--rw-rw-r--   0 john      (1000) john      (1000)      713 2024-01-30 16:18:36.000000 theflow-0.8.5/tests/test_settings.py
--rw-rw-r--   0 john      (1000) john      (1000)    15940 2023-12-06 19:28:05.000000 theflow-0.8.5/tests/test_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     5307 2023-12-19 19:04:09.000000 theflow-0.8.5/tests/test_workflow.py
--rw-rw-r--   0 john      (1000) john      (1000)     1752 2023-11-19 02:32:04.000000 theflow-0.8.5/tests/test_workflow_from.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.024600 theflow-0.8.5/theflow/
--rw-rw-r--   0 john      (1000) john      (1000)      235 2023-12-07 16:49:34.000000 theflow-0.8.5/theflow/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow/backends/
--rw-rw-r--   0 john      (1000) john      (1000)      107 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/backends/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4779 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/backends/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     5709 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/backends/http_sync.py
--rw-rw-r--   0 john      (1000) john      (1000)    60497 2024-01-13 17:20:03.000000 theflow-0.8.5/theflow/base.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow/cache/
--rw-rw-r--   0 john      (1000) john      (1000)      204 2024-01-30 16:18:41.000000 theflow-0.8.5/theflow/cache/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4176 2024-01-30 16:19:45.000000 theflow-0.8.5/theflow/cache/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     2376 2024-01-30 16:18:41.000000 theflow-0.8.5/theflow/cache/filebased.py
--rw-rw-r--   0 john      (1000) john      (1000)     2756 2024-01-30 16:21:16.000000 theflow-0.8.5/theflow/cache/memcached.py
--rw-rw-r--   0 john      (1000) john      (1000)     3349 2023-09-11 15:48:39.000000 theflow-0.8.5/theflow/cache/memory.py
--rw-rw-r--   0 john      (1000) john      (1000)      381 2023-11-19 02:32:04.000000 theflow-0.8.5/theflow/callbacks.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-10 18:21:52.000000 theflow-0.8.5/theflow/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     6365 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/config.py
--rw-rw-r--   0 john      (1000) john      (1000)     5126 2024-01-30 16:18:41.000000 theflow-0.8.5/theflow/context.py
--rw-rw-r--   0 john      (1000) john      (1000)     2925 2024-01-01 04:19:01.000000 theflow-0.8.5/theflow/debug.py
--rw-rw-r--   0 john      (1000) john      (1000)      154 2023-12-08 20:26:15.000000 theflow-0.8.5/theflow/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     7936 2024-01-13 16:37:05.000000 theflow-0.8.5/theflow/middleware.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow/runs/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-10 18:25:36.000000 theflow-0.8.5/theflow/runs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5726 2023-12-19 19:04:09.000000 theflow-0.8.5/theflow/runs/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     1867 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/safe.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow/settings/
--rw-rw-r--   0 john      (1000) john      (1000)     2272 2024-01-30 16:18:36.000000 theflow-0.8.5/theflow/settings/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      663 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/settings/default.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow/storage/
--rw-rw-r--   0 john      (1000) john      (1000)      244 2023-11-30 17:25:13.000000 theflow-0.8.5/theflow/storage/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      744 2023-09-17 16:47:22.000000 theflow-0.8.5/theflow/storage/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      961 2023-09-17 16:47:22.000000 theflow-0.8.5/theflow/storage/local.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow/utils/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-08-27 16:13:23.000000 theflow-0.8.5/theflow/utils/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3630 2023-11-19 02:32:04.000000 theflow-0.8.5/theflow/utils/documentation.py
--rw-rw-r--   0 john      (1000) john      (1000)     2072 2023-10-17 15:01:31.000000 theflow-0.8.5/theflow/utils/hashes.py
--rw-rw-r--   0 john      (1000) john      (1000)     8901 2024-01-01 04:21:06.000000 theflow-0.8.5/theflow/utils/modules.py
--rw-rw-r--   0 john      (1000) john      (1000)     1442 2023-12-01 17:47:02.000000 theflow-0.8.5/theflow/utils/multiprocess.py
--rw-rw-r--   0 john      (1000) john      (1000)     5736 2023-12-06 19:28:05.000000 theflow-0.8.5/theflow/utils/paths.py
--rw-rw-r--   0 john      (1000) john      (1000)     1890 2023-10-17 15:01:31.000000 theflow-0.8.5/theflow/utils/pretties.py
--rw-rw-r--   0 john      (1000) john      (1000)     3266 2024-01-01 04:19:01.000000 theflow-0.8.5/theflow/utils/typings.py
--rw-rw-r--   0 john      (1000) john      (1000)     8044 2023-10-17 15:01:31.000000 theflow-0.8.5/theflow/visualization.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-01-30 16:22:32.028600 theflow-0.8.5/theflow.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     5586 2024-01-30 16:22:32.000000 theflow-0.8.5/theflow.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     1326 2024-01-30 16:22:32.000000 theflow-0.8.5/theflow.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-01-30 16:22:32.000000 theflow-0.8.5/theflow.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)      154 2024-01-30 16:22:32.000000 theflow-0.8.5/theflow.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        8 2024-01-30 16:22:32.000000 theflow-0.8.5/theflow.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.821214 theflow-0.8.6/
+-rw-rw-r--   0 john      (1000) john      (1000)     1073 2023-06-10 17:42:12.000000 theflow-0.8.6/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     5586 2024-04-06 10:52:23.821214 theflow-0.8.6/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     4478 2023-11-19 02:32:04.000000 theflow-0.8.6/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)      893 2024-04-06 10:51:56.000000 theflow-0.8.6/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-06 10:52:23.821214 theflow-0.8.6/setup.cfg
+-rwxrwxr-x   0 john      (1000) john      (1000)       92 2023-09-04 02:39:08.000000 theflow-0.8.6/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.813214 theflow-0.8.6/tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     2030 2024-01-01 04:21:06.000000 theflow-0.8.6/tests/test_backends_http_sync.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2633 2023-12-19 19:04:09.000000 theflow-0.8.6/tests/test_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2148 2023-12-23 16:23:17.000000 theflow-0.8.6/tests/test_context.py
+-rw-rw-r--   0 john      (1000) john      (1000)      858 2023-09-09 08:40:04.000000 theflow-0.8.6/tests/test_example_notebooks.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10536 2024-01-01 04:21:06.000000 theflow-0.8.6/tests/test_function.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8659 2023-12-09 12:39:01.000000 theflow-0.8.6/tests/test_function_declaration.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1019 2023-12-19 19:04:09.000000 theflow-0.8.6/tests/test_function_multithread.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2057 2023-12-09 12:58:49.000000 theflow-0.8.6/tests/test_middleware.py
+-rw-rw-r--   0 john      (1000) john      (1000)      713 2024-01-30 16:18:36.000000 theflow-0.8.6/tests/test_settings.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15940 2023-12-06 19:28:05.000000 theflow-0.8.6/tests/test_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5307 2023-12-19 19:04:09.000000 theflow-0.8.6/tests/test_workflow.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1752 2023-11-19 02:32:04.000000 theflow-0.8.6/tests/test_workflow_from.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.817214 theflow-0.8.6/theflow/
+-rw-rw-r--   0 john      (1000) john      (1000)      235 2023-12-07 16:49:34.000000 theflow-0.8.6/theflow/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.817214 theflow-0.8.6/theflow/backends/
+-rw-rw-r--   0 john      (1000) john      (1000)      107 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/backends/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4779 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/backends/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5709 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/backends/http_sync.py
+-rw-rw-r--   0 john      (1000) john      (1000)    60673 2024-04-06 10:51:22.000000 theflow-0.8.6/theflow/base.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.817214 theflow-0.8.6/theflow/cache/
+-rw-rw-r--   0 john      (1000) john      (1000)      204 2024-01-30 16:18:41.000000 theflow-0.8.6/theflow/cache/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4176 2024-01-30 16:19:45.000000 theflow-0.8.6/theflow/cache/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2376 2024-01-30 16:18:41.000000 theflow-0.8.6/theflow/cache/filebased.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2756 2024-01-30 16:21:16.000000 theflow-0.8.6/theflow/cache/memcached.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3349 2023-09-11 15:48:39.000000 theflow-0.8.6/theflow/cache/memory.py
+-rw-rw-r--   0 john      (1000) john      (1000)      381 2023-11-19 02:32:04.000000 theflow-0.8.6/theflow/callbacks.py
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-10 18:21:52.000000 theflow-0.8.6/theflow/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6365 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5126 2024-01-30 16:18:41.000000 theflow-0.8.6/theflow/context.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2925 2024-01-01 04:19:01.000000 theflow-0.8.6/theflow/debug.py
+-rw-rw-r--   0 john      (1000) john      (1000)      154 2023-12-08 20:26:15.000000 theflow-0.8.6/theflow/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7936 2024-01-13 16:37:05.000000 theflow-0.8.6/theflow/middleware.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.817214 theflow-0.8.6/theflow/runs/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-10 18:25:36.000000 theflow-0.8.6/theflow/runs/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5726 2023-12-19 19:04:09.000000 theflow-0.8.6/theflow/runs/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1867 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/safe.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.817214 theflow-0.8.6/theflow/settings/
+-rw-rw-r--   0 john      (1000) john      (1000)     2272 2024-01-30 16:18:36.000000 theflow-0.8.6/theflow/settings/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      663 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/settings/default.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.817214 theflow-0.8.6/theflow/storage/
+-rw-rw-r--   0 john      (1000) john      (1000)      244 2023-11-30 17:25:13.000000 theflow-0.8.6/theflow/storage/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      744 2023-09-17 16:47:22.000000 theflow-0.8.6/theflow/storage/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      961 2023-09-17 16:47:22.000000 theflow-0.8.6/theflow/storage/local.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.821214 theflow-0.8.6/theflow/utils/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-08-27 16:13:23.000000 theflow-0.8.6/theflow/utils/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3630 2023-11-19 02:32:04.000000 theflow-0.8.6/theflow/utils/documentation.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2072 2023-10-17 15:01:31.000000 theflow-0.8.6/theflow/utils/hashes.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8901 2024-01-01 04:21:06.000000 theflow-0.8.6/theflow/utils/modules.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1442 2023-12-01 17:47:02.000000 theflow-0.8.6/theflow/utils/multiprocess.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5736 2023-12-06 19:28:05.000000 theflow-0.8.6/theflow/utils/paths.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1890 2023-10-17 15:01:31.000000 theflow-0.8.6/theflow/utils/pretties.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3266 2024-01-01 04:19:01.000000 theflow-0.8.6/theflow/utils/typings.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8044 2023-10-17 15:01:31.000000 theflow-0.8.6/theflow/visualization.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-06 10:52:23.821214 theflow-0.8.6/theflow.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     5586 2024-04-06 10:52:23.000000 theflow-0.8.6/theflow.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1326 2024-04-06 10:52:23.000000 theflow-0.8.6/theflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-06 10:52:23.000000 theflow-0.8.6/theflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      154 2024-04-06 10:52:23.000000 theflow-0.8.6/theflow.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        8 2024-04-06 10:52:23.000000 theflow-0.8.6/theflow.egg-info/top_level.txt
```

### Comparing `theflow-0.8.5/LICENSE` & `theflow-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/PKG-INFO` & `theflow-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theflow
-Version: 0.8.5
+Version: 0.8.6
 Summary: A simple framework to build and run flows
 Author-email: trducng <trungduc1992@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/trducng/theflow
 Project-URL: Repository, https://github.com/trducng/theflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `theflow-0.8.5/README.md` & `theflow-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/pyproject.toml` & `theflow-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.8.5"
+version = "0.8.6"
 name = "theflow"
 authors = [{ name = "trducng", email = "trungduc1992@gmail.com" }]
 description = "A simple framework to build and run flows"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `theflow-0.8.5/tests/test_backends_http_sync.py` & `theflow-0.8.6/tests/test_backends_http_sync.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_config.py` & `theflow-0.8.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_context.py` & `theflow-0.8.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_example_notebooks.py` & `theflow-0.8.6/tests/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_function.py` & `theflow-0.8.6/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_function_declaration.py` & `theflow-0.8.6/tests/test_function_declaration.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_function_multithread.py` & `theflow-0.8.6/tests/test_function_multithread.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_middleware.py` & `theflow-0.8.6/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_settings.py` & `theflow-0.8.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_utils.py` & `theflow-0.8.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_workflow.py` & `theflow-0.8.6/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/tests/test_workflow_from.py` & `theflow-0.8.6/tests/test_workflow_from.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/backends/base.py` & `theflow-0.8.6/theflow/backends/base.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/backends/http_sync.py` & `theflow-0.8.6/theflow/backends/http_sync.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/base.py` & `theflow-0.8.6/theflow/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1354,15 +1354,19 @@
                     value["default_kwargs"] = {
                         key: value
                         for key, value in attr_value._default._params.items()
                         if not isinstance(value, lazy)
                     }
                 nodes[attr] = value
             elif isinstance(attr_value, ParamAttr):
-                params[attr] = attr_value.__persist_flow__()
+                attr_val = attr_value.__persist_flow__()
+                attr_val["type"] = repr(
+                    attr_value._owner.__annotations__.get(attr_value._name, Any)
+                )
+                params[attr] = attr_val
 
         return {
             "type": f"{cls.__module__}.{cls.__qualname__}",
             "params": params,
             "nodes": nodes,
         }
```

### Comparing `theflow-0.8.5/theflow/cache/base.py` & `theflow-0.8.6/theflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/cache/filebased.py` & `theflow-0.8.6/theflow/cache/filebased.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/cache/memcached.py` & `theflow-0.8.6/theflow/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/cache/memory.py` & `theflow-0.8.6/theflow/cache/memory.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/config.py` & `theflow-0.8.6/theflow/config.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/context.py` & `theflow-0.8.6/theflow/context.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/debug.py` & `theflow-0.8.6/theflow/debug.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/middleware.py` & `theflow-0.8.6/theflow/middleware.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/runs/base.py` & `theflow-0.8.6/theflow/runs/base.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/safe.py` & `theflow-0.8.6/theflow/safe.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/settings/__init__.py` & `theflow-0.8.6/theflow/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/settings/default.py` & `theflow-0.8.6/theflow/settings/default.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/storage/base.py` & `theflow-0.8.6/theflow/storage/base.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/storage/local.py` & `theflow-0.8.6/theflow/storage/local.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/documentation.py` & `theflow-0.8.6/theflow/utils/documentation.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/hashes.py` & `theflow-0.8.6/theflow/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/modules.py` & `theflow-0.8.6/theflow/utils/modules.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/multiprocess.py` & `theflow-0.8.6/theflow/utils/multiprocess.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/paths.py` & `theflow-0.8.6/theflow/utils/paths.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/pretties.py` & `theflow-0.8.6/theflow/utils/pretties.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/utils/typings.py` & `theflow-0.8.6/theflow/utils/typings.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow/visualization.py` & `theflow-0.8.6/theflow/visualization.py`

 * *Files identical despite different names*

### Comparing `theflow-0.8.5/theflow.egg-info/PKG-INFO` & `theflow-0.8.6/theflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theflow
-Version: 0.8.5
+Version: 0.8.6
 Summary: A simple framework to build and run flows
 Author-email: trducng <trungduc1992@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/trducng/theflow
 Project-URL: Repository, https://github.com/trducng/theflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `theflow-0.8.5/theflow.egg-info/SOURCES.txt` & `theflow-0.8.6/theflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

