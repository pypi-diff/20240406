# Comparing `tmp/pydmt-0.3.5.tar.gz` & `tmp/pydmt-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydmt-0.3.5.tar", last modified: Wed Jan 10 12:09:36 2024, max compression
+gzip compressed data, was "pydmt-0.3.6.tar", last modified: Sat Apr  6 12:25:16 2024, max compression
```

## Comparing `pydmt-0.3.5.tar` & `pydmt-0.3.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.675086 pydmt-0.3.5/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2024-01-10 12:09:20.000000 pydmt-0.3.5/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-01-10 12:09:36.675086 pydmt-0.3.5/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      396 2024-01-10 12:09:20.000000 pydmt-0.3.5/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.671086 pydmt-0.3.5/pydmt/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/__init__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.671086 pydmt-0.3.5/pydmt/api/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/api/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.3.5/pydmt/api/builder.py
--rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.3.5/pydmt/api/copy.py
--rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.3.5/pydmt/api/fail.py
--rw-r--r--   0 mark      (1000) mark      (1000)      613 2023-05-01 12:24:57.000000 pydmt-0.3.5/pydmt/api/feature.py
--rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.3.5/pydmt/api/one_source_one_target.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.672086 pydmt-0.3.5/pydmt/builders/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/builders/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.3.5/pydmt/builders/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      498 2023-11-13 15:29:48.000000 pydmt-0.3.5/pydmt/builders/gem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      396 2023-12-29 14:25:09.000000 pydmt-0.3.5/pydmt/builders/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.3.5/pydmt/builders/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.3.5/pydmt/builders/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1458 2024-01-10 12:08:41.000000 pydmt-0.3.5/pydmt/builders/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.3.5/pydmt/builders/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2328 2024-01-10 12:08:10.000000 pydmt-0.3.5/pydmt/builders/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.3.5/pydmt/builders/yaml.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3284 2024-01-10 12:06:23.000000 pydmt-0.3.5/pydmt/configs.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.673086 pydmt-0.3.5/pydmt/core/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/core/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.3.5/pydmt/core/cache.py
--rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.3.5/pydmt/core/graph.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.3.5/pydmt/core/pydmt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/core/tempdir.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.673086 pydmt-0.3.5/pydmt/features/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/features/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.3.5/pydmt/features/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      370 2023-11-13 08:36:09.000000 pydmt-0.3.5/pydmt/features/gem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.3.5/pydmt/features/make.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1422 2023-05-01 12:22:39.000000 pydmt-0.3.5/pydmt/features/mako.py
--rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.3.5/pydmt/features/npm.py
--rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.3.5/pydmt/features/reqs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.3.5/pydmt/features/sphinx.py
--rw-r--r--   0 mark      (1000) mark      (1000)      455 2023-12-29 15:12:48.000000 pydmt-0.3.5/pydmt/features/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1010 2023-05-01 12:25:10.000000 pydmt-0.3.5/pydmt/features/yaml.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.675086 pydmt-0.3.5/pydmt/helpers/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.3.5/pydmt/helpers/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.3.5/pydmt/helpers/apt.py
--rw-r--r--   0 mark      (1000) mark      (1000)      135 2023-05-02 19:24:19.000000 pydmt-0.3.5/pydmt/helpers/composites.py
--rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.3.5/pydmt/helpers/deb.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.3.5/pydmt/helpers/deb_python_package.py
--rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.3.5/pydmt/helpers/files.py
--rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.3.5/pydmt/helpers/general.py
--rw-r--r--   0 mark      (1000) mark      (1000)      785 2023-05-02 19:24:19.000000 pydmt-0.3.5/pydmt/helpers/git.py
--rw-r--r--   0 mark      (1000) mark      (1000)      212 2023-04-28 19:49:07.000000 pydmt-0.3.5/pydmt/helpers/github.py
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.3.5/pydmt/helpers/messages.py
--rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.3.5/pydmt/helpers/misc.py
--rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.3.5/pydmt/helpers/pkgs.py
--rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-28 04:28:36.000000 pydmt-0.3.5/pydmt/helpers/project.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4782 2023-04-28 19:46:14.000000 pydmt-0.3.5/pydmt/helpers/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)      818 2023-10-10 18:09:54.000000 pydmt-0.3.5/pydmt/helpers/signature.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.3.5/pydmt/helpers/snipplets.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1360 2023-11-16 04:41:39.000000 pydmt-0.3.5/pydmt/helpers/urls.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5395 2024-01-10 12:03:31.000000 pydmt-0.3.5/pydmt/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      174 2024-01-10 12:09:20.000000 pydmt-0.3.5/pydmt/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.675086 pydmt-0.3.5/pydmt/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.5/pydmt/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.3.5/pydmt/utils/digest.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.3.5/pydmt/utils/digester.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.3.5/pydmt/utils/filesystem.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2023-11-16 04:41:08.000000 pydmt-0.3.5/pydmt/utils/importlib.py
--rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.3.5/pydmt/utils/logging.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.3.5/pydmt/utils/php.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2470 2024-01-10 12:08:25.000000 pydmt-0.3.5/pydmt/utils/python.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1339 2023-04-24 05:56:18.000000 pydmt-0.3.5/pydmt/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-10 12:09:36.671086 pydmt-0.3.5/pydmt.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-01-10 12:09:36.000000 pydmt-0.3.5/pydmt.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     1615 2024-01-10 12:09:36.000000 pydmt-0.3.5/pydmt.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-01-10 12:09:36.000000 pydmt-0.3.5/pydmt.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       42 2024-01-10 12:09:36.000000 pydmt-0.3.5/pydmt.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       77 2024-01-10 12:09:36.000000 pydmt-0.3.5/pydmt.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-01-10 12:09:36.000000 pydmt-0.3.5/pydmt.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2024-01-10 12:09:36.676086 pydmt-0.3.5/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1760 2024-01-10 12:09:20.000000 pydmt-0.3.5/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.219427 pydmt-0.3.6/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2024-04-06 12:24:37.000000 pydmt-0.3.6/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-04-06 12:25:16.219427 pydmt-0.3.6/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      396 2024-04-06 12:24:36.000000 pydmt-0.3.6/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.211427 pydmt-0.3.6/pydmt/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/__init__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.215427 pydmt-0.3.6/pydmt/api/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/api/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4112 2022-07-01 10:06:39.000000 pydmt-0.3.6/pydmt/api/builder.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      179 2022-05-04 08:29:53.000000 pydmt-0.3.6/pydmt/api/copy.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      321 2022-05-04 08:30:05.000000 pydmt-0.3.6/pydmt/api/fail.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      613 2023-05-01 12:24:57.000000 pydmt-0.3.6/pydmt/api/feature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      821 2022-07-01 10:05:31.000000 pydmt-0.3.6/pydmt/api/one_source_one_target.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.215427 pydmt-0.3.6/pydmt/builders/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/builders/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1381 2022-10-12 19:15:22.000000 pydmt-0.3.6/pydmt/builders/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      498 2023-11-13 15:29:48.000000 pydmt-0.3.6/pydmt/builders/gem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      396 2023-12-29 14:25:09.000000 pydmt-0.3.6/pydmt/builders/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2978 2022-07-01 10:04:42.000000 pydmt-0.3.6/pydmt/builders/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      493 2022-07-01 09:58:33.000000 pydmt-0.3.6/pydmt/builders/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1885 2024-04-06 12:24:14.000000 pydmt-0.3.6/pydmt/builders/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4170 2022-10-15 12:44:01.000000 pydmt-0.3.6/pydmt/builders/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2328 2024-01-10 12:08:10.000000 pydmt-0.3.6/pydmt/builders/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1276 2022-10-11 06:48:27.000000 pydmt-0.3.6/pydmt/builders/yaml.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3284 2024-01-10 12:06:23.000000 pydmt-0.3.6/pydmt/configs.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.215427 pydmt-0.3.6/pydmt/core/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/core/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2755 2022-05-25 15:17:23.000000 pydmt-0.3.6/pydmt/core/cache.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       50 2020-06-19 19:56:59.000000 pydmt-0.3.6/pydmt/core/graph.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5744 2022-07-01 10:15:48.000000 pydmt-0.3.6/pydmt/core/pydmt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      491 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/core/tempdir.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.215427 pydmt-0.3.6/pydmt/features/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/features/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      518 2022-07-01 09:55:35.000000 pydmt-0.3.6/pydmt/features/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      370 2023-11-13 08:36:09.000000 pydmt-0.3.6/pydmt/features/gem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      374 2022-05-09 23:30:17.000000 pydmt-0.3.6/pydmt/features/make.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1422 2023-05-01 12:22:39.000000 pydmt-0.3.6/pydmt/features/mako.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      380 2022-05-04 08:20:12.000000 pydmt-0.3.6/pydmt/features/npm.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      469 2022-05-05 02:02:20.000000 pydmt-0.3.6/pydmt/features/reqs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      340 2022-05-18 11:32:53.000000 pydmt-0.3.6/pydmt/features/sphinx.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      455 2023-12-29 15:12:48.000000 pydmt-0.3.6/pydmt/features/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1010 2023-05-01 12:25:10.000000 pydmt-0.3.6/pydmt/features/yaml.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.215427 pydmt-0.3.6/pydmt/helpers/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2020-05-31 02:02:11.000000 pydmt-0.3.6/pydmt/helpers/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      823 2022-06-25 06:57:04.000000 pydmt-0.3.6/pydmt/helpers/apt.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      135 2023-05-02 19:24:19.000000 pydmt-0.3.6/pydmt/helpers/composites.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      959 2022-05-18 14:23:43.000000 pydmt-0.3.6/pydmt/helpers/deb.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1022 2022-05-18 18:42:27.000000 pydmt-0.3.6/pydmt/helpers/deb_python_package.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      314 2022-05-29 13:25:55.000000 pydmt-0.3.6/pydmt/helpers/files.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      198 2022-05-16 01:59:39.000000 pydmt-0.3.6/pydmt/helpers/general.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      785 2023-05-02 19:24:19.000000 pydmt-0.3.6/pydmt/helpers/git.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      212 2023-04-28 19:49:07.000000 pydmt-0.3.6/pydmt/helpers/github.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-05-15 16:42:20.000000 pydmt-0.3.6/pydmt/helpers/messages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      165 2022-10-15 00:39:08.000000 pydmt-0.3.6/pydmt/helpers/misc.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      269 2022-05-19 21:19:00.000000 pydmt-0.3.6/pydmt/helpers/pkgs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      187 2023-04-28 04:28:36.000000 pydmt-0.3.6/pydmt/helpers/project.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4782 2023-04-28 19:46:14.000000 pydmt-0.3.6/pydmt/helpers/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      818 2023-10-10 18:09:54.000000 pydmt-0.3.6/pydmt/helpers/signature.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1150 2022-05-16 02:02:20.000000 pydmt-0.3.6/pydmt/helpers/snipplets.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1360 2023-11-16 04:41:39.000000 pydmt-0.3.6/pydmt/helpers/urls.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5395 2024-01-10 12:03:31.000000 pydmt-0.3.6/pydmt/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      174 2024-04-06 12:24:37.000000 pydmt-0.3.6/pydmt/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.219427 pydmt-0.3.6/pydmt/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2017-12-02 11:42:36.000000 pydmt-0.3.6/pydmt/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1174 2022-07-01 10:02:49.000000 pydmt-0.3.6/pydmt/utils/digest.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1044 2021-09-07 01:45:29.000000 pydmt-0.3.6/pydmt/utils/digester.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1244 2021-09-14 23:18:59.000000 pydmt-0.3.6/pydmt/utils/filesystem.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2023-11-16 04:41:08.000000 pydmt-0.3.6/pydmt/utils/importlib.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      178 2022-05-25 15:06:52.000000 pydmt-0.3.6/pydmt/utils/logging.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      265 2021-09-16 23:27:43.000000 pydmt-0.3.6/pydmt/utils/php.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2470 2024-04-06 12:20:29.000000 pydmt-0.3.6/pydmt/utils/python.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1339 2023-04-24 05:56:18.000000 pydmt-0.3.6/pydmt/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 12:25:16.211427 pydmt-0.3.6/pydmt.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1480 2024-04-06 12:25:16.000000 pydmt-0.3.6/pydmt.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     1615 2024-04-06 12:25:16.000000 pydmt-0.3.6/pydmt.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-06 12:25:16.000000 pydmt-0.3.6/pydmt.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       42 2024-04-06 12:25:16.000000 pydmt-0.3.6/pydmt.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       77 2024-04-06 12:25:16.000000 pydmt-0.3.6/pydmt.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-06 12:25:16.000000 pydmt-0.3.6/pydmt.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2024-04-06 12:25:16.219427 pydmt-0.3.6/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1760 2024-04-06 12:24:37.000000 pydmt-0.3.6/setup.py
```

### Comparing `pydmt-0.3.5/LICENSE` & `pydmt-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/PKG-INFO` & `pydmt-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -42,10 +42,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.3.5
+version: 0.3.6
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024
```

### Comparing `pydmt-0.3.5/pydmt/api/builder.py` & `pydmt-0.3.6/pydmt/api/builder.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/api/feature.py` & `pydmt-0.3.6/pydmt/api/feature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/api/one_source_one_target.py` & `pydmt-0.3.6/pydmt/api/one_source_one_target.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/builders/apt.py` & `pydmt-0.3.6/pydmt/builders/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/builders/mako.py` & `pydmt-0.3.6/pydmt/builders/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/builders/reqs.py` & `pydmt-0.3.6/pydmt/builders/reqs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Install requirements
 """
 
-
+import os.path
 from pydmt.api.one_source_one_target import OneSourceOneTarget
 from pydmt.utils.subprocess import check_call
 from pydmt.utils.filesystem import mkdir_touch
 from pydmt.utils.python import collect_reqs, collect_bootstrap_reqs, get_install_args
 from pydmt.configs import ConfigReqs
 
+REQUIREMENTS = "requirements.txt"
+
 
 class BuilderReqs(OneSourceOneTarget):
     """
     This is a review of how to build a python virtual environment:
     # create the virtualenv
     virtualenv [folder]
     # activate it
@@ -24,18 +26,27 @@
     # OR if you want to install a list of packages:
     pip install -r [list of packages]
     # OR
     python -m pip install [list of packages]
     """
     def build(self) -> None:
         """
+        If we check if there is a "requirements.txt" file with frozen requirements
+        and install it if there is.
+
+        If we do not have a frozen requirements we install from config/{python|bootstrap}.py
         Why do we do this in two stages? What's wrong with doing this in one stage?
         Because importing python.py may fail because of prereqs that python.py
         needs. In this case the user specifies these prereqs in bootstrap.py
         """
+        if os.path.isfile(REQUIREMENTS):
+            args = get_install_args()
+            args.append(REQUIREMENTS)
+            check_call(args)
+            return
         args = get_install_args()
         packs = collect_bootstrap_reqs()
         if packs:
             args.extend(packs)
             check_call(args)
         args = get_install_args()
         packs = collect_reqs(add_dev=ConfigReqs.reqs_add_dev)
```

### Comparing `pydmt-0.3.5/pydmt/builders/sphinx.py` & `pydmt-0.3.6/pydmt/builders/sphinx.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/builders/venv.py` & `pydmt-0.3.6/pydmt/builders/venv.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/builders/yaml.py` & `pydmt-0.3.6/pydmt/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/configs.py` & `pydmt-0.3.6/pydmt/configs.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/core/cache.py` & `pydmt-0.3.6/pydmt/core/cache.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/core/pydmt.py` & `pydmt-0.3.6/pydmt/core/pydmt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/features/apt.py` & `pydmt-0.3.6/pydmt/features/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/features/mako.py` & `pydmt-0.3.6/pydmt/features/mako.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/features/yaml.py` & `pydmt-0.3.6/pydmt/features/yaml.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/apt.py` & `pydmt-0.3.6/pydmt/helpers/apt.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/deb.py` & `pydmt-0.3.6/pydmt/helpers/deb.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/deb_python_package.py` & `pydmt-0.3.6/pydmt/helpers/deb_python_package.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/git.py` & `pydmt-0.3.6/pydmt/helpers/git.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/python.py` & `pydmt-0.3.6/pydmt/helpers/python.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/signature.py` & `pydmt-0.3.6/pydmt/helpers/signature.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/snipplets.py` & `pydmt-0.3.6/pydmt/helpers/snipplets.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/helpers/urls.py` & `pydmt-0.3.6/pydmt/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/main.py` & `pydmt-0.3.6/pydmt/main.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/utils/digest.py` & `pydmt-0.3.6/pydmt/utils/digest.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/utils/digester.py` & `pydmt-0.3.6/pydmt/utils/digester.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/utils/filesystem.py` & `pydmt-0.3.6/pydmt/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt/utils/python.py` & `pydmt-0.3.6/pydmt/utils/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,26 +67,25 @@
         mod = importlib.import_module("config.python")
         if hasattr(mod, "requires"):
             reqs += getattr(mod, "requires")
         if add_dev and hasattr(mod, "dev_requires"):
             reqs += getattr(mod, "dev_requires")
         return reqs
     except ModuleNotFoundError:
-        pass
-    return []
+        return []
 
 
 def collect_bootstrap_reqs() -> List[str]:
     try:
         mod = importlib.import_module("config.bootstrap")
         if hasattr(mod, "requires"):
             return getattr(mod, "requires")
+        return []
     except ModuleNotFoundError:
-        pass
-    return []
+        return []
 
 
 def get_install_args():
     return [
         "python",
         "-m",
         "pip",
```

### Comparing `pydmt-0.3.5/pydmt/utils/subprocess.py` & `pydmt-0.3.6/pydmt/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/pydmt.egg-info/PKG-INFO` & `pydmt-0.3.6/pydmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydmt
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python dependency management tool
 Home-page: https://veltzer.github.io/pydmt
 Download-URL: https://github.com/veltzer/pydmt
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -42,10 +42,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pydmt
 
 author: Mark Veltzer
 
-version: 0.3.5
+version: 0.3.6
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024
```

### Comparing `pydmt-0.3.5/pydmt.egg-info/SOURCES.txt` & `pydmt-0.3.6/pydmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydmt-0.3.5/setup.py` & `pydmt-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open("README.rst") as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pydmt",
-    version="0.3.5",
+    version="0.3.6",
     packages=[
         "pydmt",
         "pydmt.api",
         "pydmt.builders",
         "pydmt.core",
         "pydmt.features",
         "pydmt.helpers",
```

